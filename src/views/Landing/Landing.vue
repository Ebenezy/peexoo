<template>
    <div class="peexoo-landing">
        <HeaderNav/>
        <div class="peexoo-header">

        </div>
        <div class="nav-below">
            <div class="container">
                <div class="nav-below2">
                    <img src="../../assets/images/photographer.jpg" alt="photographer" class="hidden-xs hidden-sm">
                    <div></div>
                    <div class="navbar-below">
                        <router-link to="">Details</router-link>
                        <router-link to="">Portfolio</router-link>
                        <router-link to="" active class="active">Availability</router-link>
                        <router-link to="">Pricing Package</router-link>
                        <router-link to="">Reviews</router-link>
                    </div>
                </div>
            </div>
        </div>

        <div class="afroshot-section">
            <div class="container">
                <div class="afroshots">
                    <div class="afroshots-v">
                        <h1>Afroshots</h1>
                        <img src="../../assets/images/verified.svg" alt="Verified">
                    </div>
                    <div class="afro_buttons">
                        <button class="btn-message-photo">Message Photographer</button>
                        <button class="btn-book-now">Book Now</button>
                    </div>
                </div>

                <div class="calender-section">
                    <vue-cal selected-date="2020-01-01"
                            xsmall
                            default-view="month"
                            class="calendar-single vuecal--rounded-theme vuecal--green-theme"
                            hide-view-selector
                            :time="false"
                            :disable-views="['week']"
                            :time-from="10 * 60"
                            :on-event-click="onEventClick"
                            :events="events">
                        <template v-slot:events-count="{ events, view }">
                        <span v-if="customEventsCount(events)">
                            {{ customEventsCount(events) }}
                        </span>
                        </template>
                    </vue-cal>

                    <vue-cal selected-date="2020-02-01"
                            xsmall
                            default-view="month"
                            class="calendar-single vuecal--rounded-theme vuecal--green-theme"
                            hide-view-selector
                            :time="false"
                            :disable-views="['week']"
                            :events="events">
                        <template v-slot:events-count="{ events, view }">
                        <span v-if="customEventsCount(events)">
                            {{ customEventsCount(events) }}
                        </span>
                        </template>
                    </vue-cal>

                    <vue-cal selected-date="2020-03-01"
                            xsmall
                            default-view="month"
                            class="calendar-single vuecal--rounded-theme vuecal--green-theme"
                            hide-view-selector
                            :time="false"
                            :disable-views="['week']"
                            :events="events">
                        <template v-slot:events-count="{ events, view }">
                        <span v-if="customEventsCount(events)">
                            {{ customEventsCount(events) }}
                        </span>
                        </template>
                    </vue-cal>
                </div>
            </div>
        </div>
        <Footer/>
        <CC/>
    </div>
</template>

<script>
    import HeaderNav from "../../components/HeaderNav/HeaderNav";
    import VueCal from 'vue-cal'
    import Footer from "../../components/Footer/Footer";
    import CC from "../../components/Footer/CC";

    export default {
        name: "Landing.vue",
        components: {
            HeaderNav,
            VueCal,
            Footer,
            CC
        },
        computed: {
    layout() {
      return this.$screens(
        {
          // Default layout for mobile
          default: {
            columns: 1,
            rows: 1,
            isExpanded: true,
          },
          // Override for large screens
          lg: {
            columns: 2,
            rows: 2,
            isExpanded: false,
          },
        },
      );
    }
  }
    }
</script>

<style scoped>

</style>