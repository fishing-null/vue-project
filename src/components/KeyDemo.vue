<template>
    <h3>列表渲染</h3>
    <p v-for="name of names">{{ name }}</p>
    <div>
        <p v-for="object in result" v-bind:key="object.id">{{object}}</p>
    </div>
</template>
<script>
    export default{
        data(){
            return {
                names: ["1","2","3"],
                result:[
                    {
                        id:2405,
                        title: 'How to do lists in Vue',
                        author: 'Jane Doe',
                        publishedAt: '2016-04-10'
                    },
                    {
                        id:2406,
                        title: 'How to do lists in Vue',
                        author: 'Jane Doe',
                        publishedAt: '2016-04-10'
                    }

                ]

        }
    }
}
</script>