<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppUtilityLink from './components/AppUtilityLink.vue'

export default {
    components: { AppHeader, AppMain, AppUtilityLink },
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
</template>

<style lang="scss">
@use './assets/scss/style.scss'
</style>
