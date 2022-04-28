<template>
<!-- components -> subFolder -> subMainFolder -> subSectionCc -> PartBbcc.vue -->
    <div class="part_bbcc_1st_div">
        <div class="w_40">
            <h2>
                OOOOOOOO
            </h2>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Error odit, sit praesentium labore culpa sapiente molestias expedita? Non, delectus ullam ducimus at blanditiis maxime molestias in quasi. Porro, repellendus quia?
            </p>
            <hr>
        </div>

        <div class="part_bbcc_1st_div__container2">
            <div class="part_bbcc_1st_div__container2__row">
                <div v-for="div in 3" :key="div" class="w_25 p_20">
                    <img src="" alt="img">
                    <span>
                        comacose
                    </span>
                    <h3>
                        next investment
                    </h3>
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolor dolore deserunt, quam officiis blanditiis maiores soluta illum error earum accusantium inventore magnam quia nemo perspiciatis veritatis aut dolorum quidem eius.
                    </p>
                    <h6>
                        read more
                    </h6>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PartBbcc',
}
</script>

<style scoped lang="scss">
@import '../../../cssComp/mixin.scss';
@import '../../../cssComp/style.scss';

.part_bbcc_1st_div {
    @include displayFlexBasic(flex, column, center, center);
}

.part_bbcc_1st_div__container2__row {
    @include displayFlexBasic(flex, row, center, center);
}
</style>