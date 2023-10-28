<template>
    <div class="body">
        <header-component></header-component>
        <home-section></home-section>
        <holiday-section></holiday-section>
        <culture-section></culture-section>
        <!--<culture-section2></culture-section2>-->
        <tour-section2></tour-section2>
        <tour-section></tour-section>
        <holiday-section2></holiday-section2>
<!--        <newsletter-section></newsletter-section>-->
        <footer-section></footer-section>
        <copyright-section></copyright-section>
        <popup-section>
        </popup-section>
    </div>
</template>

<script>
import HeaderComponent from "@/components/HeaderComponent.vue";
import HomeSection from "@/components/HomeSection.vue";
import FeatureSection from "@/components/FeatureSection.vue";
import HolidaySection from "@/components/HolidaySection.vue";
import HolidaySection2 from "@/components/HolidaySection2.vue";
import TourSection from "@/components/TourSection.vue";
import CultureSection from "@/components/CultureSection.vue";
import CultureSection2 from "@/components/CultureSection2.vue";
import NewsletterSection from "@/components/NewsletterSection.vue";
import FooterSection from "@/components/FooterSection.vue";
import CopyrightSection from "@/components/CopyrightSection.vue";
import TourSection2 from "@/components/TourSection2.vue";
import PopupSection from "@/components/PopupSection.vue";

    export default {
        components: {
            HomeSection,
            HeaderComponent,
            FeatureSection,
            HolidaySection,
            TourSection,
            CultureSection,
            NewsletterSection,
            FooterSection,
            CopyrightSection,
            HolidaySection2,
            CultureSection2,
            TourSection2,
            PopupSection,
        },
        mounted() {
            console.log('Component mounted.')
        }
    }
</script>

<style scoped>
@import "../../taproom/assets/sass/style.css";
</style>

<script></script>
