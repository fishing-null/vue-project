<template>
<p>你要打印的消息是: {{message}} </p>
<input v-model="message" placeholder="在这里编辑"> </input>
</template>


<script>
export default{
    data(){
        return{
            message:"",
        }
    }
}

</script>