<template>
    <nav class="page_nav">
        <ul class="mainmenu">


            <li class="lavel-1 with--drop slide--megamenu">
                <nuxt-link to="/portfolio/portfolio-grid-boxed">
                    <span>Portfolio</span>
                </nuxt-link>
                <ul class="mega__width--fullscreen">
                    <div class="container">
                        <div class="mega__list">
                            <li class="mega--title">
                                PORTFOLIO SAMPLES 01
                                <ul>
                                    <li>
                                        <nuxt-link to="/portfolio/portfolio-grid-boxed"><span>Portfolio Grid Boxed</span></nuxt-link>
                                    </li>
                                    <li>
                                        <nuxt-link to="/portfolio/portfolio-grid-wide"><span>Portfolio Grid Wide</span></nuxt-link>
                                    </li>
                                    <li>
                                        <nuxt-link to="/portfolio/portfolio-with-caption"><span>Portfolio With Caption</span></nuxt-link>
                                    </li>
                                </ul>
                            </li>
  
                        </div>
                    </div>
                </ul>
            </li>

       

           
        </ul>
    </nav>
</template>

<style lang="scss">
    .mega__list {
        display: flex;
        li {
            flex-basis: 25%;
        }
    }
</style>