<template>
  <div id="Body">
      <div class="blue">
          
      </div>
      <ul>
          <Covers v-for="( cover , index ) in covers" :key="index" :detail="cover" /> <!-- passo l'oggetto cover al props detail del componente Covers -->
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