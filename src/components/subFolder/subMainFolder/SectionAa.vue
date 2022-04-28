<template>
    <div class="section_one_1st_div">
        <div class="w_90">
            <PartOne/>
        </div>

        <div>
            <PartTwo/>
        </div>
    </div>
</template>

<script>
import PartOne from './subSectionAa/PartOne.vue';
import PartTwo from './subSectionAa/PartTwo.vue';

export default {
    name: 'SectionAa',
    components: {
        PartOne,
        PartTwo,
    }
}
</script>

<style scoped lang="scss">
@import '../../cssComp/mixin.scss';
@import '../../cssComp/style.scss';

.section_one_1st_div {
    @include displayFlexBasic(flex, column, center, center);
}
</style>