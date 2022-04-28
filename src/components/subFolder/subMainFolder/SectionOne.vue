<template>
    <div class="section_one_1st_div">
        <div class="w_50">
            <PartOne/>
        </div>
    </div>
</template>

<script>
import PartOne from './subSectionOne/PartOne.vue';

export default {
    name: 'SectionOne',
    components: {
        PartOne,
    }
}
</script>

<style scoped lang="scss">
@import '../../cssComp/mixin.scss';
@import '../../cssComp/style.scss';

.section_one_1st_div {
    @include displayFlexBasic(flex, row, center, center);
}
</style>