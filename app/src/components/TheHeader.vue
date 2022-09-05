<template>
    

    <div v-for-key="obj in todos"></div>


</template>

<script>

    export default {
        name: 'App',
        data(){
            return{
                todos: [{

                }]
            }
        }
            
    }
</script>

<style>
    .header{
        background: #000;
        color: #fff;
    }
</style>