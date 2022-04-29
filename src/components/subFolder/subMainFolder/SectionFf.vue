<template>
    <div class="section_ff_1st_div my_60">
        <div class="section_ff_1st_div__row1">
            <div class="section_ff_1st_div__row1__col1 w_40 p_60">
                <img class="w_100" src="../../../assets/img/h1-contact-rev-01.png" alt="">
            </div>

            <div class="section_ff_1st_div__row1__col2 w_40">
                <h2 class="text_capitalize">
                    contact us<span class="text_ff4612">.</span>
                </h2>
                <div class="w_10">
                    <hr class="little_hr w_100">
                </div>
                <p class="text_a6a6a6">
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quas impedit cupiditate quisquam possimus, error praesentium qui labore ipsum? Numquam eveniet ipsa debitis perferendis quae corrupti eligendi quasi facilis harum eos.
                </p>
                <form class="w_100 py_20" action="">
                    <div class="w_100 mb_20 o">
                        <input class="d_inline_block w_48" type="text" placeholder="Your name">
                        <input class="d_inline_block w_48" type="mail" placeholder="Your e-mail">
                    </div>
                    <input class="d_block w_100 h_60px" type="text" placeholder="Write a message">
                </form>
                <button class="btn_basic btn_orange text_uppercase">
                    send <i class="fa-solid fa-arrow-right-long"></i>
                </button>
            </div>
        </div>

        <div class="section_ff_1st_div__row2 mt_60">
            <div class="p_20">
                <img src="../../../assets/img/h4-clients-img-01.png" alt="">
            </div>
            <div class="p_20">
                <img src="../../../assets/img/h4-clients-img-03.png" alt="">
            </div>
            <div class="p_20">
                <img src="../../../assets/img/h4-clients-img-05.png" alt="">
            </div>
            <div class="p_20">
                <img src="../../../assets/img/h4-clients-img-07.png" alt="">
            </div>
            <div class="p_20">
                <img src="../../../assets/img/h4-clients-img-09.png" alt="">
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

// .section_ff_1st_div__row1__col1 {
//     @include backgroundBasic(no-repeat, cover, center);
//     background-image: url('../../../assets/img/h1-contact-rev-01.png')
// }

.section_ff_1st_div__row1__col2 {
    @include displayFlexBasic(flex, column, center, start);
}

form {
    input {
        border: none;
        border-bottom: 1px solid black;
    }
}

.o {
    @include displayFlexBasic(flex, row, space-between, center);
}
</style>