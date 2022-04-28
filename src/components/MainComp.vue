<template>
    <div>
        <div>
            <SectionAa/>
        </div>

        <div>
            <SectionBb/>
        </div>

        <div>
            <SectionCc/>
        </div>

        <div>
            <SectionDd/>
        </div>
    </div>
</template>

<script>
import SectionAa from './subFolder/subMainFolder/SectionAa.vue';
import SectionBb from './subFolder/subMainFolder/SectionBb.vue';
import SectionCc from './subFolder/subMainFolder/SectionCc.vue';
import SectionDd from './subFolder/subMainFolder/SectionDd.vue';

export default {
    name: 'MainComp',
    components: {
        SectionAa,
        SectionBb,
        SectionCc,
        SectionDd,
    }
}
</script>

<style scoped lang="scss">
@import './cssComp/mixin.scss';
@import './cssComp/style.scss';
</style>