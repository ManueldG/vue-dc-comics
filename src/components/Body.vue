<template>
  <div id="Body">
      <img src="@/assets/img/dc-logo.png" alt="logo">
      <ul>
          <Covers v-for="( cover , index ) in covers" :key="index" :detail="cover" />
      </ul>
  </div>
</template>

<script>
import Covers from '@/components/Covers.vue';
import covers from '@/components/covers.js'
export default {
    name : "Body",
    components: {
        Covers
        },
    data: function(){
        return {
            covers
        }

    }
}
</script>

<style scoped lang="scss">

#Body{
    background-color: rgb(43, 105, 221);
        ul{
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            list-style: none;
            }
        
    }
    
</style>