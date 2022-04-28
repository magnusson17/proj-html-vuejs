<template>
    <div class="section_one_1st_div w_50">
        <div class="section_one_1st_div__container1">
            <h2 class="text_capitalize">
                our specialities.
            </h2>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab labore, neque id sunt rerum at voluptates qui dolor vel, ratione, quisquam placeat nostrum officiis suscipit! Vel eos ex quam amet.
            </p>
            <div>
                <hr>
            </div>
        </div>

        <div class="section_one_1st_div__container2">
            <div>
                <img src="" alt="img">
                <h6>knowing</h6>
                <span>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</span>
            </div>
            <div>
                <img src="" alt="img">
                <h6>knowing</h6>
                <span>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</span>
            </div>
            <div>
                <img src="" alt="img">
                <h6>knowing</h6>
                <span>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</span>
            </div>
            <div>
                <img src="" alt="img">
                <h6>knowing</h6>
                <span>Lorem ispansum dolor, sit amet consectetur adipisicing elit.</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionOne',
}
</script>

<style scoped lang="scss">
@import '../../cssComp/mixin.scss';
@import '../../cssComp/style.scss';

.section_one_1st_div, .section_one_1st_div__container1 {
    @include displayFlexBasic(flex, column, center, center);
}

.section_one_1st_div__container2 {
    @include displayFlexBasic(flex, row, center, center);
    div {
        @include displayFlexBasic(flex, column, center, center);
        text-align: center;
        h6 {
            text-transform: capitalize;
        }
    }
}
</style>