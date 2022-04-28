<template>
    <div class="nav_bar_1st_div p_20">
        <div>
            <h2 class="text_capitalize">
               everlead<span class="text_ff4612">.</span>
            </h2>
        </div>

        <div>
            <ul>
                <li 
                v-for="(element, index) in linkNavBar" 
                :key="index"
                class="text_uppercase">
                    {{element}}
                </li>
                <li>
                    <i class="fa-solid fa-magnifying-glass"></i>
                </li>
                <li>
                    <i class="fa-solid fa-list"></i>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'NavBar',
    data() {
        return {
            linkNavBar: [
                'homes',
                'pages',
                'blog',
                'shop',
                'events',
                'elements'
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../cssComp/mixin.scss';
@import '../cssComp/style.scss';

.nav_bar_1st_div {
    @include displayFlexBasic(flex, row, space-between, center);
    div {
        ul {
            @include displayFlexBasic(flex, row, space-between, center);
            list-style: none;
            li {
                padding: 0 10px 0 10px;
                cursor: pointer;
                transition: 0.2s;
                &:hover {
                    color: #ff4612;
                }
            }
        }
    }
}
</style>