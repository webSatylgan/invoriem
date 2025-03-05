<script setup>
    import {onMounted, ref} from "vue";

    // vars ---------
    let slideWidth;

    // Mounted events
    onMounted(() => {
        slideWidth = document.querySelector(".studies_slide").offsetWidth;
    });


</script>

<template>
<div class="studies">
    <div class="container">
        <h2>Case Studies</h2>
        <p>We deliver a unique and truly bespoke approach to delivering international <br> developments to market, with over 10 years success around the world.</p>
        <div class="slider_traker">
            <div class="studies_slider">
                <div class="studies_slide">
                    <h3>France</h3>
                    <div class="studies_slide-text">
                        <h3>France</h3>
                        <img src="@assets/imgs/slider-01.jpg" alt="">
                    </div>
                </div>
                <div class="studies_slide">
                    <h3>Moroco</h3>
                    <div class="studies_slide-text">
                        <h3>Moroco</h3>
                        <img src="@assets/imgs/slider-02.jpg" alt="">
                    </div>
                </div>
                <div class="studies_slide">
                    <h3>London</h3>
                    <div class="studies_slide-text">
                        <h3>London</h3>
                        <img src="@assets/imgs/slider-03.jpg" alt="">
                    </div>
                </div>
            </div>
            <div class="studies_slider" aria-hidden="true">
                <div class="studies_slide">
                    <h3>France</h3>
                    <div class="studies_slide-text">
                        <h3>France</h3>
                        <img src="@assets/imgs/slider-01.jpg" alt="">
                    </div>
                </div>
                <div class="studies_slide">
                    <h3>Moroco</h3>
                    <div class="studies_slide-text">
                        <h3>Moroco</h3>
                        <img src="@assets/imgs/slider-02.jpg" alt="">
                    </div>
                </div>
                <div class="studies_slide">
                    <h3>London</h3>
                    <div class="studies_slide-text">
                        <h3>London</h3>
                        <img src="@assets/imgs/slider-03.jpg" alt="">
                    </div>
                </div>
            </div>
        </div>
    </div>
</div> <!-- studies -->
</template>

<style scoped>
    .studies {
        width: 100%;
        margin-top: 185px;
    }

    .studies .container p {
        margin-top: 50px;
    }

    .slider_traker {
        display: flex;
        margin-top: 150px;

        overflow: hidden;
    }

    .studies_slider {
        display: flex;
        gap: 50px;
        padding-right: 50px;

        position: relative;

        animation: scroll 15s linear infinite;
    }

    @keyframes scroll {
        from {
            transform: translateX(0);
        }
        to {
            transform: translateX(calc(-100%));
        }
    }

    .studies_slide {
        min-width: 720px;
        width: 100%;
        padding-left: 50px;

        position: relative;
    }

    .studies_slide h3 {
        font-family: var(--font-family);
        font-weight: 600;
        font-size: 120px;
        color: var(--teal);

        position: absolute;
        bottom: 120px;
        left: 0;

    }

    .studies_slide-text {
        width: 100%;
        overflow: hidden;

        position: relative;
    }
    
    .studies_slide-text h3 {
        color: #fff;
        left: -50px;
    }

    .studies_slide-text img {
        max-width: 645px;
        width: 100%;

        overflow: hidden;
    }

    @media (max-width: 1000px) {
        .studies .container p {
            font-size: 20px;
        }
    }

    @media (max-width: 600px) {
        .studies_slide {
            min-width: 500px;
        }
    }


</style>