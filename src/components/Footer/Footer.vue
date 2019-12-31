<template>
    <footer class="footer">
        <div class="container">
            <div class="row">
                <div class="col-md-4">
                    <div class="quick_links">
                        <p>Quick Links</p>
                        <ul>
                            <li><router-link to="">Explore photos</router-link></li>
                            <li><router-link to="">Find my photos</router-link></li>
                            <li><router-link to="">Peexoomemories</router-link></li>
                            <li><router-link to="">Become a photographer</router-link></li>
                        </ul>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="company">
                        <p>Company</p>
                        <ul>
                            <li><router-link to="">About Us</router-link></li>
                            <li><router-link to="">FAQs</router-link></li>
                            <li><router-link to="">Pricing</router-link></li>
                            <li><router-link to="">Careers</router-link></li>
                            <li><router-link to="">Help &amp; Support</router-link></li>
                            <li><router-link to="">Terms of Service</router-link></li>
                            <li><router-link to="">Privacy Policy</router-link></li>
                        </ul>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="connect_us">
                        <p>Connect with Us</p>
                        <ul>
                            <li>5A, Awudu Egheda,<br>Lekki, Lagos</li>
                            <li><a href="tel:+234 8003229932">+234 8003229932</a></li>
                            <li><a href="mailto:customer.service@peexo.ai">customer.service@peexo.ai</a></li>
                        </ul>
                        <ul class="social">
                            <li><a href="https://www.whatsapp.com" target="_blank"><img src="../../assets/images/social/whatsapp.svg" alt="whatsapp" class=""></a></li>
                            <li><a href="https://www.facebook.com" target="_blank"><img src="../../assets/images/social/facebook.svg" alt="facebook" class=""></a></li>
                            <li><a href="https://www.twitter.com" target="_blank"><img src="../../assets/images/social/twitter.svg" alt="twitter" class=""></a></li>
                            <li><a href="https://www.instagram.com" target="_blank"><img src="../../assets/images/social/instagram.svg" alt="instagram" class=""></a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer.vue",
    components: {

    }
}
</script>

<style scoped>
    a{
        text-decoration: none;
    }
    a:hover, a:focus, a:active{
        text-decoration: none;
        /*color: #FECB32;*/
    }
    

</style>