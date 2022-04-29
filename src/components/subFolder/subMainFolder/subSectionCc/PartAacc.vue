<template>
<!-- components -> subFolder -> subMainFolder -> subSectionCc -> PartAacc.vue -->
    <div class="part_aacc_1st_div">
        <div class="w_40 p_60">
            <h2 class="text_capitalize">
                creative leader<span class="text_ff4612">.</span>
            </h2>
            <div class="w_10">
                <hr class="little_hr w_100">
            </div>
            <p class="text_a6a6a6">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, natus! Quasi voluptatum repellat, debitis quam impedit fugiat neque, adipisci voluptatibus provident consectetur dolorem recusandae. Porro laborum quaerat cupiditate. Quibusdam, quos?
            </p>
            <h6 class="text_uppercase">
                read more
            </h6>
        </div>

        <div class="w_40 p_60">
            <div class="py_10">
                <div class="row">
                    <h4 class="text_capitalize">
                        mentorship
                    </h4>
                    <span class="fw_bold ">
                        78%
                    </span>
                </div>

                <div class="row w_100">
                    <div class="w_78">
                        <hr class="little_hr">
                    </div>
                    <div  class="w_22">
                        <hr class="">
                    </div>
                </div>
            </div>

            <div class="py_10">
                <div class="row">
                    <h4 class="text_capitalize">
                        education
                    </h4>
                    <span class="fw_bold ">
                        95%
                    </span>
                </div>

                <div class="row w_100">
                    <div class="w_95">
                        <hr class="little_hr">
                    </div>
                    <div  class="w_5">
                        <hr class="">
                    </div>
                </div>
            </div>

            <div class="py_10">
                <div class="row">
                    <h4 class="text_capitalize">
                        learning
                    </h4>
                    <span class="fw_bold ">
                        65%
                    </span>
                </div>

                <div class="row w_100">
                    <div class="w_65">
                        <hr class="little_hr">
                    </div>
                    <div  class="w_35">
                        <hr class="">
                    </div>
                </div>
            </div>

            <div class="py_10">
                <div class="row">
                    <h4 class="text_capitalize">
                        motivation
                    </h4>
                    <span class="fw_bold ">
                        83%
                    </span>
                </div>

                <div class="row w_100">
                    <div class="w_83">
                        <hr class="little_hr">
                    </div>
                    <div  class="w_17">
                        <hr class="">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PartAacc',
}
</script>

<style scoped lang="scss">
@import '../../../cssComp/mixin.scss';
@import '../../../cssComp/style.scss';

.part_aacc_1st_div {
    @include displayFlexBasic(flex, row, center, center);
}

.row {
    @include displayFlexBasic(flex, row, space-between, center);
}

h4 {
    margin: 0;
}
</style>