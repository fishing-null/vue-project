<template>
    <div>
        
        <button @click="incrementCount" v-if="ifPrint === 1">点击按钮+1</button>
        <p v-show = "flag">你点击了{{count}}次按钮</p>
        <button @click="printMessage">点击控制台打印消息</button>
    </div>

</template>
    
    
<script>
export default{
    data(){
        return{
            count:0,
            ifPrint: 1,
            flag: true,
        }
    },
    //通过方法事件处理器打印语句
    methods:{
        incrementCount(){
            //判断是否为偶数,只在偶数时打印文本
            if(this.count % 2 == 0){
                this.flag = false;
            }else{
                this.flag = true;
            }
            this.count++;
        },
        printMessage(){
            console.log("打印一条消息")
            console.log(this.flag)
        },
    }
}
    
</script>