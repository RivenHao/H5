<template>
    <div>
        <ul>
            <!-- <li v-for="data in datalist" :key="data">
                {{ data }}
            </li> -->
            <TabbarItem v-for="data in datalist" :key="data" :item="data"></TabbarItem>
        </ul>
    </div>
</template>

<script>
import TabbarItem from './TabbarItem.vue'

export default {
    data() {
        return {
            datalist:["首页","列表","我的"]
        }
    },
    components:{
        TabbarItem
    },
    methods:{
        
    }
}
</script>

<style scoped>
    ul{
        display: flex;
        position: fixed;
        bottom: 0;
        width: 100%;
        height: 50px;
        line-height: 50px;
    }
    li{
        text-align: center;
        flex: 1;
    }
</style>