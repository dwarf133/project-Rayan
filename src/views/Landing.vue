<template>
  <div>
    <header-component></header-component>
    <home-section></home-section>
    <possibilities-section></possibilities-section>
    <tour-section></tour-section>
    <holiday-section></holiday-section>
    <culture-section></culture-section>
    <!--<culture-section2></culture-section2>-->
    <tour-section2></tour-section2>
    <holiday-section2></holiday-section2>
    <lead-form-section></lead-form-section>
    <!--        <newsletter-section></newsletter-section>-->
    <footer-section></footer-section>
    <copyright-section></copyright-section>
  </div>
</template>
<script>


import HeaderComponent from "@/components/Taproom/HeaderComponent.vue";
import HomeSection from "@/components/Taproom/HomeSection.vue";
import FeatureSection from "@/components/Taproom/FeatureSection.vue";
import PossibilitiesSection from "@/components/Taproom/PossibilitiesSection.vue";
import HolidaySection from "@/components/Taproom/HolidaySection.vue";
import HolidaySection2 from "@/components/Taproom/HolidaySection2.vue";
import TourSection from "@/components/Taproom/TourSection.vue";
import CultureSection from "@/components/Taproom/CultureSection.vue";
import CultureSection2 from "@/components/Taproom/CultureSection2.vue";
import NewsletterSection from "@/components/Taproom/NewsletterSection.vue";
import FooterSection from "@/components/Taproom/FooterSection.vue";
import CopyrightSection from "@/components/Taproom/CopyrightSection.vue";
import TourSection2 from "@/components/Taproom/TourSection2.vue";
import LeadFormSection from "@/components/Taproom/LeadFormSection.vue";

  export default {
    components: {
      HomeSection,
      PossibilitiesSection,
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
      LeadFormSection,
    },
    data() {
      return {
      };
    },
    methods: {

    },
    mounted() {

    }
  };
</script>
<style>

</style>
