<template>
    <div>
        <div>
            <SectionOne/>
        </div>

        <div>
            <SectionTwo/>
        </div>
    </div>
</template>

<script>
import SectionOne from './subFolder/subMainFolder/SectionOne.vue';
import SectionTwo from './subFolder/subMainFolder/SectionTwo.vue';

export default {
    name: 'MainComp',
    components: {
        SectionOne,
        SectionTwo,
    }
}
</script>

<style scoped lang="scss">
@import './cssComp/mixin.scss';
@import './cssComp/style.scss';
</style>