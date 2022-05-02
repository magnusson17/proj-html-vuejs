<template>
    <div class="section_ff_1st_div py_60 bg_f9f9f9">
        <div class="section_ff_1st_div__row1">
            <div class="section_ff_1st_div__row1__col1 w_40 p_60">
                <div class="p_relative row">
                    <img class="w_100" src="../../../assets/img/h1-contact-rev-01.png" alt="world">
                    <div class="pos_absolute p_20 bg_white">
                        <h4 class="text_capitalize">
                            new york coaching
                        </h4>
                        <h6 class="text_uppercase">
                            read more
                        </h6>
                    </div>
                </div>
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
                    <div class="w_100 mb_20 row_between">
                        <input class="d_inline_block w_45" type="text" placeholder="Your name">
                        <input class="d_inline_block w_45" type="mail" placeholder="Your e-mail">
                    </div>
                    <input class="w_100 h_60px" type="textarea" placeholder="Write a message">
                    <button class="btn_basic btn_orange text_uppercase mt_20">
                        send <i class="fa-solid fa-arrow-right-long"></i>
                    </button>
                </form>
            </div>
        </div>

        <div class="section_ff_1st_div__row2 mt_60">
            <div class="p_20 hover">
                <img src="../../../assets/img/h4-clients-img-01.png" alt="img" class="hover_none">
                <img src="../../../assets/img/h4-clients-img-02.png" alt="img" class="hover_block d_none">
            </div>
            <div class="p_20 hover">
                <img src="../../../assets/img/h4-clients-img-03.png" alt="img" class="hover_none">
                <img src="../../../assets/img/h4-clients-img-04-1.png" alt="img" class="hover_block d_none">
            </div>
            <div class="p_20 hover">
                <img src="../../../assets/img/h4-clients-img-05.png" alt="img" class="hover_none">
                <img src="../../../assets/img/h4-clients-img-06-1.png" alt="img" class="hover_block d_none">
            </div>
            <div class="p_20 hover">
                <img src="../../../assets/img/h4-clients-img-07.png" alt="img" class="hover_none">
                <img src="../../../assets/img/h4-clients-img-08-1.png" alt="img" class="hover_block d_none">
            </div>
            <div class="p_20 hover">
                <img src="../../../assets/img/h4-clients-img-09.png" alt="img" class="hover_none">
                <img src="../../../assets/img/h4-clients-img-10-1.png" alt="img" class="hover_block d_none">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionFf',
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
    div {
        @include displayFlexBasic(flex, row, space-between, center);
    }
}

.hover:hover .hover_none {
    display: none;
}

.hover:hover .hover_block {
    display: block;
}

.row {
    @include displayFlexBasic(flex, row, center, center);
}

.row_between {
    @include displayFlexBasic(flex, row, space-between, center);
}

.pos_absolute {
    position: absolute;
    h4, h6 {
        margin: 0;
    }
}

form {
    input {
        background-color: transparent;
        padding: 5px;
    }
}
</style>