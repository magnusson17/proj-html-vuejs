<template>
    <div class="section_dd_1st_div bg_black p_20">
        <div class="section_dd_1st_div__row">
            <div class="section_dd_1st_div__row__col w_50">
                <img src="" alt="img">
                <h4>
                    cynthia clark
                </h4>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ratione necessitatibus tempore fugit deleniti nostrum, reprehenderit, voluptas exercitationem aliquid at consequuntur dolorem. Veniam similique necessitatibus iste? Officia mollitia quae consequuntur deserunt.
                </p>
                <hr>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionDd',
    components: {
    }
}
</script>

<style scoped lang="scss">
@import '../../cssComp/mixin.scss';
@import '../../cssComp/style.scss';

.section_dd_1st_div__row {
    @include displayFlexBasic(flex, row, center, center);
}

.section_dd_1st_div__row__col {
    @include displayFlexBasic(flex, column, center, center);
}
</style>