<template>
    <div class="section_one_1st_div">
        <div class="w_50">
            <PartOne/>
        </div>

        <div>
            <PartTwo/>
        </div>
    </div>
</template>

<script>
import PartOne from './subSectionOne/PartOne.vue';
import PartTwo from './subSectionOne/PartTwo.vue';

export default {
    name: 'SectionCc',
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