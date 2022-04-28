<template>
    <div class="section_two_1st_div">
        <div class="section_two_2nd_div w_50 p_20">
            <div class="section_two_3rd_div bg_white w_50">

                <div class="section_two_3rd_div__container1">
                    <h2 class="text_capitalize">
                        upcoming events
                    </h2>
                </div>

                <div v-for="div in 3" :key="div" class="section_two_3rd_div__container2">
                    <div class="p_20 bg_orange">
                        data
                    </div>

                    <div class="px_20">
                        <h5>
                            melburne coaching
                        </h5>
                        <span>
                            ora
                        </span>
                        <span>
                            luogo
                        </span>
                        <h6>
                            read more
                        </h6>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionBb',
    components: {
    }
}
</script>

<style scoped lang="scss">
@import '../../cssComp/mixin.scss';
@import '../../cssComp/style.scss';

.section_two_1st_div {
    @include backgroundBasic(no-repeat, cover, center);
    background-image: url('../../../assets/img/h1-img-09.jpg')
}

.section_two_2nd_div, .section_two_3rd_div {
    @include displayFlexBasic(flex, column, center, center);
}

.section_two_3rd_div__container2 {
    @include displayFlexBasic(flex, row, center, start);
    h5, h6 {
        margin: 0;
    }
    padding: 20px;
}

.o {
    @include displayFlexBasic(flex, column, center, center);
}
</style>