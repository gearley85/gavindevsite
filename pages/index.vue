<template>
    
    <div class="main-container">

        <HeaderBlack @togglenav="navOpen = !navOpen" @toggleSearch="searchOpen = !searchOpen" />

        <OffCanvasMobileMenu :class="{'show-mobile-menu' : navOpen}" @togglenav="navOpen = !navOpen" />

        

        <div class="freelancer-wrapper bg_image--27" :style="{ backgroundImage: `url('/img/bg/bg-image-27.jpg')` }">
            <div class="row">
                <div class="col-lg-6">
                    <div class="freelancer-left">
                        <!-- Start About Area -->
                        <div class="freelancer-about-area pb--130">
                            <div class="inner wow move-up">
                                <h2 class="heading heading-h2 font-50 font-400 line-height-1-62">
                                    <span class="theme-color">Hello.</span> My name is Gavin Earley.
                                </h2>
                                <div class="thumb mt--55">
                                    <img class="w-100" src="/img/about/about-7.jpg" alt="about image">
                                </div>
                                <div class="bkseparator--40"></div>
                                <h4 class="heading heading-h4">About me</h4>
                                <div class="bkseparator--30"></div>
                                <p class="bk_pra">I am a software engineer, husband, father, amateur photographer and licensed drone pilot.</p>
                                <div class="bkseparator--40"></div>
                                <div class="signeture">
                                    <img src="/img/icons/singneture2.png" alt="about image">
                                </div>
                            </div>
                        </div>
                        <!-- End About Area -->

  

                        <!-- Start Contact Area -->
                        <div class="freelancer-contact-area pb--100 pt--150">
                            <div class="contact-inner">
                                <div class="brook-section-title wow move-up">
                                    <h2 class="heading heading-h2 font-50 font-400 line-height-1-62">Message me.</h2>
                                </div>
                                <div class="content">
                                    <div class="bkseparator--25"></div>
                                    <p class="bk_pra pr--40 wow move-up">Contact me below </p>
                                    <div class="freelancer-contact mt--40">
                                        <h5 class="heading bk-hover heading-h5 font-400 line-height-1-39 wow move-up">
                                            <a href="mailto:info@yourdomain.com">gavinearley@gmail.com</a>
                                        </h5>
                                        <div class="bkseparator--20"></div>
           
                                        <div class="view-more-btn heding-color font-600 mt--55 wow move-up">
                                            <nuxt-link to="/contact-us-modern">
                                                <span>More details</span> 
                                                <span class="btn-arrow"></span>
                                            </nuxt-link>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <!-- End Contact Area -->

                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="freelancer-right pb--100">
                        <!-- Start Portfolio Area -->
                        <div class="freelancer-portfolio">
                            <div class="brook-section-title text-start text-lg-end mb--55">
                                <h2 class="heading heading-h2 font-50 font-400 line-height-1-62 wow move-up">Some of my work.</h2>
                            </div>

                            <div class="portfolio portfolio_style--1 mt--30 wow move-up" v-for="portfolio in portfolioData.portfolioItems.slice(0, 7)" :key="portfolio.id">
                                <div class="thumb">
                                    <img :src="portfolio.image" alt="Portfolio Images">
                                </div>
                                <div class="port-overlay-info">
                                    <div class="hover-action">
                                        <h3 class="post-overlay-title">
                                            <nuxt-link :to="`/portfolio/${portfolio.slug}`">
                                                {{ portfolio.heading }}
                                            </nuxt-link>
                                        </h3>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <!-- End Portfolio Area -->
                    </div>
                </div>
            </div>
        </div>

        <footer id="page-footer-wrapper" class="page-footer bg_color--4">
            <div class="copyright">
                <div class="container ptb--40">
                    <div class="row align-items-center">
                        <div class="col-md-6">
                            <div class="copyright-left text-md-start text-center">
                                <ul class="bk-copyright-menu d-flex bk-hover justify-content-center justify-content-md-start flex-wrap flex-sm-nowrap">
                                
                                    <li>
                                        <nuxt-link to="/portfolio/portfolio-grid-boxed">Latest Projects</nuxt-link>
                                    </li>
                                    <li>
                                        <nuxt-link to="/contact-us-modern">Contact Me</nuxt-link>
                                    </li>
                                </ul>
                            </div>
                        </div>
                        <div class="col-md-6">
                            <div class="copyright-right text-md-end text-center">
                                <p>&copy; 2023 <b>Gavin Earley</b> </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </footer>

    </div>

</template>

<script>

    import portfolioData from '../data/portfolio.json'

    export default {
        components: {
            HeaderBlack: () => import('@/components/HeaderBlack'),
            OffCanvasMobileMenu: () => import('@/components/OffCanvasMobileMenu'),
            SearchPopup: () => import('@/components/SearchPopup'),
        },

        data () {
            return {
                portfolioData,
                navOpen: false,
                searchOpen: false
            }
        },

        mounted () {
            document.body.classList.add('template-color-4', 'template-font-1')
        },

        head() {
            return {
                title: 'Gavin Earley'
            }
        },
    };
</script>