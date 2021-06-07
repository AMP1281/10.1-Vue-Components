<template>

    <div class= "text-center bg-info rounded-pill">

        <h2>{{msg}}</h2>

    </div>

</template>

<script>
export default {
  name: 'Hijo',
  props:['msg'],

  data(){
      return{
          msgh:"Soc el fill"
      }
  },
  mounted(){
      this.$emit("evento",this.msgh);
  },
}
</script>