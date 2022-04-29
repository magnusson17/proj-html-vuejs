<template>
    <div class="section_two_1st_div">
        <div class="section_two_2nd_div w_50">
            <div class="section_two_3rd_div bg_white w_50 my_60">

                <div class="section_two_3rd_div__container1 w_100 text_center bg_f9f9f9">
                    <h2 class="text_capitalize">
                        upcoming events
                    </h2>
                </div>

                <div 
                v-for="(element, index) in upcomingEvents" 
                :key="index" 
                class="section_two_3rd_div__container2 w_100 py_20 bg_f9f9f9">
                    <div class="p_10 bg_ff4612 text_white text_center">
                        <div class="fs_1_2em">
                            {{element.date.number}}
                        </div>
                        <div class="fs_0_6em">
                            <span>{{element.date.month}},{{element.date.year}}</span>
                        </div>
                    </div>

                    <div class="px_20">
                        <h4 class="text_capitalize">
                            {{element.title}}
                        </h4>
                        <p class="fs_0_6em text_a6a6a6">
                            <span>
                                <i class="fa-regular fa-clock text_ff4612"></i>
                            </span>
                            {{element.date.timeStart}} - {{element.date.timeEnd}}, {{element.date.number}}, {{element.date.month}}, {{element.date.year}}
                        </p>
                        <p class="text_capitalize fs_0_6em text_a6a6a6">
                            <span>
                                <i class="fa-solid fa-location-dot text_ff4612"></i>
                            </span>
                            cambridge
                        </p>
                        <h6 class="text_uppercase">
                            read more
                        </h6>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionBb',
    components: {
    },

    data() {
        return {
            upcomingEvents: [
                {
                    title: 'melburne coaching',
                    date: {
                        number: 7,
                        month: 'jan',
                        year: 2022,
                        timeStart: '9:00 am',
                        timeEnd: '5:00 pm'
                    }
                },
                {
                    title: 'new york coaching',
                    date: {
                        number: 11,
                        month: 'jan',
                        year: 2022,
                        timeStart: '9:00 am',
                        timeEnd: '5:00 pm'
                    }
                },
                {
                    title: 'london coaching',
                    date: {
                        number: 21,
                        month: 'jan',
                        year: 2022,
                        timeStart: '9:00 am',
                        timeEnd: '5:00 pm'
                    }
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../../cssComp/mixin.scss';
@import '../../cssComp/style.scss';

.section_two_1st_div {
    @include backgroundBasic(no-repeat, cover, center);
    background-image: url('../../../assets/img/h1-img-09.jpg')
}

.section_two_2nd_div, .section_two_3rd_div {
    @include displayFlexBasic(flex, column, center, center);
}

.section_two_3rd_div__container2 {
    @include displayFlexBasic(flex, row, center, start);
    h4, h6 {
        margin: 0;
    }
    border-top: 1px solid #e1e1e1;
    cursor: pointer;
    &:hover {
        h4 {
            color: #ff4612;
        }
        background-color: white;
    }
}
</style>