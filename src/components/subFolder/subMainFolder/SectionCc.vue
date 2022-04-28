<template>
    <div class="section_cc_1st_div">
        <div>
            <PartAacc/>
        </div>

        <div>
            <PartBbcc/>
        </div>
    </div>
</template>

<script>
import PartAacc from './subSectionCc/PartAacc.vue'
import PartBbcc from './subSectionCc/PartBbcc.vue'

export default {
    name: 'SectionCc',
    components: {
        PartAacc,
        PartBbcc,
    }
}
</script>

<style scoped lang="scss">
@import '../../cssComp/mixin.scss';
@import '../../cssComp/style.scss';

.section_cc_1st_div {
    @include displayFlexBasic(flex, row, center, center);
}
</style>