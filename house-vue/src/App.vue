<script setup>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import Reproductions from './components/Reproductions.vue';
import NewCollection from './components/NewCollection.vue';
import Team from './components/Team.vue';
import Footer from './components/Footer.vue';
</script>

<template>
    <Header/>
    <main class="main">
        <Hero/>
        <Reproductions/>
        <NewCollection/>
        <Team/>
    </main>
    <Footer/>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Raleway:ital,wght@0,100..900;1,100..900&display=swap');

.main{
    max-width: 90rem;
    width: 100%;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 4.375rem;
}
</style>