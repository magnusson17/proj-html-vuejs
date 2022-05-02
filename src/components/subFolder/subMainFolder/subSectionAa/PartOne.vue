<template>
<!-- components -> subFolder -> subMainFolder -> subSectionAacc -> PartOne.vue -->
    <div class="part_one_1st_div bg_white py_50">
        <div class="part_one_1st_div__container1">
            <h2 class="text_capitalize">
                our specialities<span class="text_ff4612">.</span>
            </h2>
            <p class="text_a6a6a6 w_50">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab labore, neque id sunt rerum at voluptates qui dolor vel, ratione, quisquam placeat nostrum officiis suscipit! Vel eos ex quam amet.
            </p>
            <hr class="w_5 little_hr">
        </div>

        <div class="part_one_1st_div__container2">
            <div 
            v-for="(element, index) in ourSpecialitiesArray" 
            :key="index"
            class="p_20">
                <img :src="require(`../../../../assets/img/${element.img}`)" alt="img">
                <h4 class="text_capitalize">
                    {{element.name}}
                </h4>
                <span class="text_a6a6a6">
                    {{element.content}}
                </span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PartOne',
    data() {
        return {
            ourSpecialitiesArray: [
                {
                    name: 'knowing',
                    content: 'lorem ipsum knowing',
                    img: 'svg-0.svg'
                },
                {
                    name: 'selling',
                    content: 'lorem ipsum selling',
                    img: 'svg-1.svg'
                },
                {
                    name: 'learning',
                    content: 'lorem ipsum learning',
                    img: 'svg-2.svg'
                },
                {
                    name: 'contact',
                    content: 'lorem ipsum contact',
                    img: 'svg-3.svg'
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../../../cssComp/mixin.scss';
@import '../../../cssComp/style.scss';

.part_one_1st_div, .part_one_1st_div__container1 {
    @include displayFlexBasic(flex, column, center, center);
}

.part_one_1st_div {
    margin-top: -50px;
}

.part_one_1st_div__container2 {
    @include displayFlexBasic(flex, row, center, center);
    div {
        @include displayFlexBasic(flex, column, center, center);
        text-align: center;
    }
}
</style>