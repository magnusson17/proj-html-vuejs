<template>
    <div>
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

.section_one_1st_div {
    @include displayFlexBasic(flex, column, center, center);
}
</style>