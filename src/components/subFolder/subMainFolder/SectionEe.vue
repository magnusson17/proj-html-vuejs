<template>
    <div class="section_ee_1st_div">
        <div class="h_70vh">

        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionEe',
    components: {
    }
}
</script>

<style scoped lang="scss">
@import '../../cssComp/mixin.scss';
@import '../../cssComp/style.scss';

.section_ee_1st_div {
    div {
        @include backgroundBasic(no-repeat, cover, center);
        background-image: url('../../../assets/img/h1-img-04.jpg');
    }
}
</style>