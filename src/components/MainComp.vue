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
    </div>
</template>

<script>
import SectionAa from './subFolder/subMainFolder/SectionAa.vue';
import SectionBb from './subFolder/subMainFolder/SectionBb.vue';
import SectionCc from './subFolder/subMainFolder/SectionCc.vue';

export default {
    name: 'MainComp',
    components: {
        SectionAa,
        SectionBb,
        SectionCc,
    }
}
</script>

<style scoped lang="scss">
@import './cssComp/mixin.scss';
@import './cssComp/style.scss';
</style>