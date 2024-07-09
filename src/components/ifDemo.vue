<template>
    <div v-if="flag">flag标签为true且则显示，否则不显示</div>
    <div v-else-if="type === 'C'">flag为flase且标签为D则显示</div>
    <div v-else-if="type === 'D'">flag为flase且标签为D则显示</div>
</template>

<script>
    export default{
        data(){
            return{
                flag:false,
                type:"D"
            }
        }
    }
</script>