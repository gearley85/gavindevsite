<template>
    <footer class="page-footer bg_color--3 pl--150 pr--150 pl_lp--70 pr_lp--70 pl_lg--70 pr_lg--70 pl_md--50 pr_md--50 pl_sm--30 pr_sm--30">
        <div class="bk-footer-inner pt--150 pb--60 pt_md--90 pt_sm--90 pb_md--30 pb_sm--20">
            <div class="row">
                <div class="col-lg-5 col-xl-7 col-sm-6">
                    <div class="footer-widget">
                        <div class="logo">
                            <nuxt-link to="/">
                                <img src="/img/logo/brook.png" alt="Brand Logo">
                            </nuxt-link>
                        </div>
                    </div>
                </div>
                <div class="col-lg-3 col-xl-2 col-sm-6 mt_mobile--40">
                    <div class="footer-widget menu--about">
                        <h2 class="widgettitle">About us</h2>
                        <div class="footer-menu">
                            <ul class="ft-menu-list bk-hover">
   
                                <li>
                                    <nuxt-link to="/contact-us-modern">Contact</nuxt-link>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4 col-xl-3 col-sm-6 mt_md--40 mt_sm--40">
                    <div class="footer-widget menu--contact">
                        <h2 class="widgettitle">Contact</h2>
                        <div class="footer-address bk-hover mb--20">
                           
                            <p>
                                <a href="mailto:info@yourdomain.com">gavinearley@gmail.com</a>
                            </p>
                        </div>
                        <div class="social-share social--transparent text-white">
                            <a href="https://www.linkedin.com/in/earleygavin/" target="_blank">
                                <i class="fab fa-linkedin"></i>
                            </a>

                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Start Copyright Area -->
        <div class="copyright ptb--50">
            <div class="row align-items-center">
                <div class="col-md-6">
                    <div class="copyright-left text-start">
                        <ul class="bk-copyright-menu d-flex justify-content-center justify-content-md-start bk-hover">

                            <li>
                                <nuxt-link to="/portfolio/portfolio-grid-boxed">Latest Projects</nuxt-link>
                            </li>
                            <li>
                                <nuxt-link to="/contact-us-modern">Contact Us</nuxt-link>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-md-6">
                    <div class="copyright-right text-center text-md-end">
                        <p>&copy; 2023 </p>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>