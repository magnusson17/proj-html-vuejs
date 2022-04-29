<template>
    <div class="footer_comp_1st_div bg_black">
        <div class="row text_white">
            <div class="w_20 m_20">
                <h3 class="text_capitalize">
                    about
                </h3>
                <div class="w_10">
                    <hr class="little_hr w_100">
                </div>
                <p>
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Qui, dolorum doloremque recusandae ab aperiam accusantium repellendus veritatis, nam impedit molestias maxime tenetur iure debitis deserunt, eum voluptatibus nesciunt aliquid porro?
                </p>
                <div>
                    img
                </div>
            </div>

            <div class="w_20 m_20">
                <h3 class="text_capitalize">
                    twitter
                </h3>
                <div class="w_10">
                    <hr class="little_hr w_100">
                </div>
                <ul>
                    <!-- <i class="fa-brands fa-twitter"></i> -->
                    <li>
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eum perspiciatis delectus omnis doloribus nemo libero non minima! Magnam magni, sunt ratione minus hic officia provident. Illo sunt adipisci iste esse.
                    </li>
                    <li>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas neque id tempore perferendis facere vitae temporibus autem quo magnam. Porro aliquid neque maiores eius tempore similique omnis ab recusandae ipsa?
                    </li>
                </ul>
            </div>

            <div class="w_20 m_20">
                <h3 class="text_capitalize">
                    important links
                </h3>
                <div class="w_10">
                    <hr class="little_hr w_100">
                </div>
                <ul>
                    <li>
                        About me
                    </li>
                    <li>
                        About us
                    </li>
                    <li>
                        Lenguage packs
                    </li>
                    <li>
                        Become a coach
                    </li>
                    <li>
                        Monthly events
                    </li>
                </ul>
            </div>

            <div class="w_20 m_20">
                <h3 class="text_capitalize">
                    contact me
                </h3>
                <div class="w_10">
                    <hr class="little_hr w_100">
                </div>
                <span>1</span>
            </div>
        </div>

        <div class="row bg_ff4612 p_10">
            <div>
                <span>hoooooooooooooooooooooooo</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterComp',
    components: {
    }
}
</script>

<style scoped lang="scss">
@import '../components/cssComp/mixin.scss';
@import '../components/cssComp/style.scss';

.row {
    @include displayFlexBasic(flex, row, center, start)
}

// li::marker {
//     font-family: "Font Awesome 5 Free";
//     font-weight: 400;
//     content: "\f099";
// }
</style>