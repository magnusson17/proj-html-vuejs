<template>
    <div class="nav_bar_1st_div">
        <div>
            <span>
                Nevermind
            </span>
        </div>

        <div>
            <ul>
                <li>1</li>
                <li>2</li>
                <li>3</li>
                <li>4</li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'NavBar'
}
</script>

<style scoped lang="scss">
@import '../cssComp/mixin.scss';

.nav_bar_1st_div {
    @include displayFlexBasic(flex, row, space-between, center);
    div {
        ul {
            @include displayFlexBasic(flex, row, space-between, center);
            list-style: none;
        }
    }
}
</style>