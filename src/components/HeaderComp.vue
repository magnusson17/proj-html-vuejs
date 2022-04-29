<template>
    <div class="header_comp_1st_div">
        <NavBar/>
        <div class="w_50">
            <div class="header_comp_1st_div__row">
                <div class="w_50 mb_150">
                    <h2 class="text_capitalize fs_3em">
                        our team<span class="text_ff4612">.</span>
                    </h2>
                    <p class="text_a6a6a6">
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Labore praesentium deserunt architecto harum dolore suscipit, cumque, ab veniam ducimus sapiente magni expedita consectetur quis facilis perspiciatis quibusdam at doloribus. Excepturi.
                    </p>
                    <div>
                        <button class="btn_basic btn_white">
                            read more <i class="fa-solid fa-arrow-right-long"></i>
                        </button>

                        <button class="btn_basic btn_orange">
                            purchase <i class="fa-solid fa-arrow-right-long"></i>
                        </button>
                    </div>
                </div>
            </div>
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

.header_comp_1st_div__row {
    @include displayFlexBasic(flex, row, center, center);
}
</style>