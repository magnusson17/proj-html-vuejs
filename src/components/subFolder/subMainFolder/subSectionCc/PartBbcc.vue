<template>
<!-- components -> subFolder -> subMainFolder -> subSectionCc -> PartBbcc.vue -->
    <div class="part_bbcc_1st_div">
        <div class="row w_40">
            <h2 class="text_capitalize">
                latest news<span class="text_ff4612">.</span>
            </h2>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Error odit, sit praesentium labore culpa sapiente molestias expedita?
            </p>
            <div class="w_10">
                <hr class="little_hr">
            </div>
        </div>

        <div class="part_bbcc_1st_div__container2">
            <div class="part_bbcc_1st_div__container2__row">
                <div v-for="(element, index) in latestNewsArray" :key="index" class="w_25 p_20">
                    <img src="../../../../assets/img/h1-blog-img-01.jpg" alt="img" class="w_100">
                    <p class="fs_0_6em text_a6a6a6 text_capitalize">
                        <i class="fa-regular fa-clock text_ff4612"></i>
                        {{element.date.number}},{{element.date.month}},{{element.date.year}},
                        <i class="fa-regular fa-user text_ff4612"></i>
                        {{element.reporter}}
                    </p>
                    <h3 class="text_capitalize">
                        {{element.text}}
                    </h3>
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolor dolore deserunt, quam officiis blanditiis maiores soluta illum error earum accusantium inventore magnam quia nemo perspiciatis veritatis aut dolorum quidem eius.
                    </p>
                    <h6 class="text_uppercase">
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

    data() {
        return {
            latestNewsArray: [
                {
                    text: 'next investment',
                    img: 'h1-blog-img-01.jpg',
                    date: {
                        number: 5,
                        month: 'may',
                        year: 2022,
                    },
                    reporter: 'amanda joa'
                },
                {
                    text: 'team building',
                    img: 'h1-blog-img-02.jpg',
                    date: {
                        number: 5,
                        month: 'may',
                        year: 2022,
                    },
                    reporter: 'pinco pallino'
                },
                {
                    text: 'new busisness day',
                    img: 'h1-blog-img-03.jpg',
                    date: {
                        number: 5,
                        month: 'may',
                        year: 2022,
                    },
                    reporter: 'papu gomez'
                },
            ]
        }
    }
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

.row {
    @include displayFlexBasic(flex, column, center, center);
}
</style>