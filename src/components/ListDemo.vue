<template>
    <h3>列表渲染</h3>
    <p v-for="name of names">{{ name }}</p>
    <div>

        <p v-for="(value,key,index) of result">{{ value }}-{{ key }}-{{ index }}</p>
    </div>
</template>
<script>
    export default{
        data(){
            return {
                names: ["1","2","3"],
                result:
                    {
                        title: 'How to do lists in Vue',
                        author: 'Jane Doe',
                        publishedAt: '2016-04-10'
                    },
        }
    }
}
</script>