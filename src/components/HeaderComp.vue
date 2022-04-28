<template>
    <div>
        <NavBar/>
    </div>
</template>

<script>
import NavBar from './subFolder/NavBar.vue';

export default {
    name: 'HeaderComp',
    components: {
        NavBar,
    }
}
</script>

<style scoped lang="scss">

</style>