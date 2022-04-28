<template>
<!-- components -> subFolder -> subMainFolder -> subSectionOne -> PartTwo.vue -->
    <div class="part_two_1st_div">
        <div>
            <img src="../../../../assets/img/h1-img-01.jpg" alt="">
        </div>

        <div class="part_two_1st_div__container2">
            <h3>
                jason pickford
            </h3>
            <p>
                founder and executive director
            </p>
            <hr>
            <p>
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
    @include displayFlexBasic(flex, row, center, center)
}

.part_two_1st_div__container2__link_and_signiature {
    @include displayFlexBasic(flex, row, space-between, center)
}
</style>