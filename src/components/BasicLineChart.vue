<template>
<!-- 基础折线图 -->
    <div class="basic-line-echarts common-echarts">
        <div class="basic_echart" style="width: 300px; height: 300px"></div>
    </div>
</template>

<script>
export default {
    name: 'BasicLine',
    components: {},
    filters: {},
    mixins: [],
    model: {},
    props: {},
    data() {
        return {
            basicChartInstance: null
        }
    },
    computed:{},
    watch: {},
    created() {},
    mounted() {
        this.initChart();
    },
    updated() {},
    activated() {},
    deactiveated() {},
    beforeDestroy() {},
    destroyed() {},
    methods: {
        initChart() {
            this.basicChartInstance = this.$echarts.init(document.getElementById('basic_echart'));

            let options = {

            };

            this.$echarts.setOption(options);
        }
    }
}
</script>

<style scoped lang="scss">
</style>
