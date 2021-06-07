<template>

    <div class="text-center bg-secondary px-5 py-5 mt-5 rounded">
        
        <h2><Hijo @evento="nombre=$event"></Hijo> 
        {{nombre}}</h2>

        <Hijo :msg="message"></Hijo>

    </div>

</template>

<script>

import Hijo from "./Hijo.vue";

export default {
    name:'Padre',
    components:{
        Hijo
    },

    data(){
        return{
            message:"Soc el pare",
            nombre:''
        }
    },

}
</script>

