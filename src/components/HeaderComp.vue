<template>
    <div class="header_comp_1st_div">
        <NavBar/>
        <div class="w_50">
            <h2>
                prova
            </h2>
            <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Labore praesentium deserunt architecto harum dolore suscipit, cumque, ab veniam ducimus sapiente magni expedita consectetur quis facilis perspiciatis quibusdam at doloribus. Excepturi.
            </p>
            <button>
                click
            </button>
        </div>
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
@import './cssComp/mixin.scss';
@import './cssComp/style.scss';

.header_comp_1st_div {
    @include backgroundBasic(no-repeat, cover, center);
    background-image: url('../assets/img/rev-slider-main-home-img-03.jpg');
}
</style>