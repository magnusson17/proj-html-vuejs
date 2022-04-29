<template>
    <div class="section_dd_1st_div bg_gray p_20">
        <div class="section_dd_1st_div__row">

            <div @click="lessIndexBe()">
                <i class="fa-solid fa-arrow-left-long"></i>
            </div>

            <div class="section_dd_1st_div__row__col w_50">
                <img :src="`../../../assets/img/${this.testimonials[this.indexBe].img}`" alt="img">
                <h4 class="text_white text_capitalize">
                    {{this.testimonials[this.indexBe].name}}
                </h4>
                <p class="text_white">
                    {{this.testimonials[this.indexBe].quote}}
                </p>
                <div class="w_100">
                    <div
                    v-for="(element, index) in testimonials" 
                    :key="index" 
                    class="w_33 d_inline_block"
                    >
                    <!-- :class="(index = this.indexBe) ? 'little_hr' : '' " -->
                        <hr class="w_100">
                    </div>
                </div>
            </div>

            <div @click="plusIndexBe()">
                <i class="fa-solid fa-arrow-right-long"></i>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionDd',
    components: {
    },

    data() {
        return {
            testimonials: [
                {
                    name: 'cynthia clark',
                    img: 'h3-img-04.png',
                    quote: 'lorem cynthia ipsum'
                },
                {
                    name: 'yan min son',
                    img: 'h3-img-07.png',
                    quote: 'lorem yan ipsum'
                },
                {
                    name: 'anna panna',
                    img: 'h3-img-08.png',
                    quote: 'lorem anna ipsum'
                },
            ],

            indexBe: 0,
        }
    },

    methods: {
        plusIndexBe() {
            this.indexBe++
            if (this.indexBe == this.testimonials.length) {
                this.indexBe = 0
            }
        },

        lessIndexBe() {
            this.indexBe--
            if (this.indexBe < 0) {
                this.indexBe = (this.testimonials.length - 1)
            }
        }
    }
}
</script>

<style scoped lang="scss">
@import '../../cssComp/mixin.scss';
@import '../../cssComp/style.scss';

.section_dd_1st_div__row {
    @include displayFlexBasic(flex, row, space-between, center);
}

.section_dd_1st_div__row__col {
    @include displayFlexBasic(flex, column, center, center);
}
</style>