<template>
    <div class="section_ff_1st_div">
        <div class="section_ff_1st_div__row1">
            <div class="section_ff_1st_div__row1__col1 w_40">
                <h4>
                    new york
                </h4>
            </div>

            <div class="section_ff_1st_div__row1__col2 w_40">
                <h2>
                    contact us.
                </h2>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quas impedit cupiditate quisquam possimus, error praesentium qui labore ipsum? Numquam eveniet ipsa debitis perferendis quae corrupti eligendi quasi facilis harum eos.
                </p>
                <p>
                    qui va il form
                </p>
                <button>
                    click
                </button>
            </div>
        </div>

        <div class="section_ff_1st_div__row2">
            <div v-for="div in 5" :key="div" class="p_20">
                img
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionFf',
    components: {
    }
}
</script>

<style scoped lang="scss">
@import '../../cssComp/mixin.scss';
@import '../../cssComp/style.scss';

.section_ff_1st_div__row1, .section_ff_1st_div__row2 {
    @include displayFlexBasic(flex, row, center, center);
}

.section_ff_1st_div__row1__col2 {
    @include displayFlexBasic(flex, column, center, start);
}
</style>