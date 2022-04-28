<template>
    <div class="main_comp_1st_div">
        <SectionOne/>
    </div>
</template>

<script>
import SectionOne from './subFolder/subMainFolder/SectionOne.vue';

export default {
    name: 'MainComp',
    components: {
        SectionOne,
    }
}
</script>

<style scoped lang="scss">
@import './cssComp/mixin.scss';
@import './cssComp/style.scss';

.main_comp_1st_div {
    @include displayFlexBasic(flex, row, center, center)
}
</style>