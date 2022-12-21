<template>
<div>
<title> Pour une vraie intégration du vélo à Cherbourg-en-Cotentin</title>
    <NavBar/>
    <HeroHeader/>
    <PartenaireSection/>
    <ThreeBar/>
    <FooterBar/>
</div>

</template>

<script>
import PartenaireSection from '../components/PartenaireSection.vue';
import ThreeBar from '../components/ThreeBar.vue';
import NavBar from '~/components/NavBar.vue';
import HeroHeader from '~/components/HeroHeader.vue';
import FooterBar from '~/components/FooterBar.vue';


export default {
    name: "IndexPage",
    components: { NavBar, HeroHeader, PartenaireSection, ThreeBar, FooterBar }
}
</script>
