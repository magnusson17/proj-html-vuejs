<template>
<!-- components -> subFolder -> subMainFolder -> subSectionAa -> PartTwo.vue -->
    <div class="part_two_1st_div m_60">
        <div class="w_40 part_two_1st_div__container1">
            <img class="w_100" src="../../../../assets/img/h1-img-01.jpg" alt="">
        </div>

        <div class="part_two_1st_div__container2 w_25 p_20 bg_white">
            <h3 class="text_capitalize">
                jason pickford
            </h3>
            <p class="text_a6a6a6">
                founder and executive director
            </p>
            <div class="w_10">
                <hr class="w_100 little_hr">
            </div>
            <p class="text_a6a6a6">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Earum, illo ipsum perspiciatis fugiat incidunt, qui est natus, doloremque alias aspernatur eum omnis nisi expedita hic. Rem culpa at velit alias?
            </p>
            <div class="part_two_1st_div__container2__link_and_signiature">
                <div>
                    1
                </div>
                <div>
                    2
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PartTwo',
}
</script>

<style scoped lang="scss">
@import '../../../cssComp/mixin.scss';
@import '../../../cssComp/style.scss';

.part_two_1st_div {
    @include displayFlexBasic(flex, row, center, center);
    background-image: url('../../../../assets/img/svg-4.svg');
    background-repeat: no-repeat;
    background-position: right;
}

.part_two_1st_div__container2__link_and_signiature {
    @include displayFlexBasic(flex, row, space-between, center)
}

.part_two_1st_div__container1 {
    margin-right: -50px;
}
</style>