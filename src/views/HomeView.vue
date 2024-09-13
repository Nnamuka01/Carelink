<script setup>
import AppFeatures from '@/components/AppFeatures.vue';
import AppHeader from '../components/AppHeader.vue';
import Company from '../components/Company.vue';
import Faq from '@/components/AppFaq.vue';
import AppFooter from '@/components/AppFooter.vue';
</script>

<template>
  <main>
    <AppHeader />
    <Company />
    <AppFeatures />
    <Faq />
    <AppFooter />
  </main>
</template>
