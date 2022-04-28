<template>
<!-- components -> subFolder -> subMainFolder -> subSectionCc -> PartAacc.vue -->
    <div class="part_aacc_1st_div">
        <div class="w_50 p_60">
            <h2 class="text_capitalize">
                creative leader
            </h2>
            <hr>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, natus! Quasi voluptatum repellat, debitis quam impedit fugiat neque, adipisci voluptatibus provident consectetur dolorem recusandae. Porro laborum quaerat cupiditate. Quibusdam, quos?
            </p>
            <h6>
                read more
            </h6>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PartAacc',
}
</script>

<style scoped lang="scss">
@import '../../../cssComp/mixin.scss';
@import '../../../cssComp/style.scss';

.part_aacc_1st_div {
    @include displayFlexBasic(flex, row, center, center);
}
</style>