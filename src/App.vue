<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
import AppUtilityLink from './components/AppUtilityLink.vue'

export default {
    components: { AppHeader, AppMain, AppUtilityLink, AppFooter },
    data() {
        return {

        }
    },
}
</script>

<template>
    <AppHeader />
    <AppMain />
    <AppUtilityLink />
    <AppFooter />
</template>

<style lang="scss">
@use './assets/scss/style.scss'
</style>
