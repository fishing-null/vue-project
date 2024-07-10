<template>
    <div>
        <button @click="count++">点击按钮+1</button>
        <p >你点击了{{count}}次按钮</p>
        <button @click="printMessage">点击控制台打印消息</button>
    </div>

</template>
    
    
<script>
export default{
    data(){
        return{
            count:0,
        }
    },
    methods:{
        printMessage(){
            console.log("打印一条消息")
        }
    }
}
    
</script>