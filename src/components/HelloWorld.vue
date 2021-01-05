<template>
    <div>
        {{a}}
        <button @click="setmsg">a</button>
    </div>
</template>

<script>
    export default {
        name: 'HelloWorld',
        data(){
            return{
                a:1
            }
        },
        methods:{
           async setmsg(){
                this.a++;
              await  this.$nextTick()
            }
        }
    }
</script>

<style scoped lang="less">

</style>
