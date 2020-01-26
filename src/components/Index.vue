<template>
  <div class="index px-4 flex mb-4">
   <div class="max-w-sm rounded overflow-hidden shadow-lg m-4 p-4 bg-white" v-for="note in notes" :key="note.id">
  <img class="w-full" src="../assets/logo.png" alt="Sunset in the mountains">
  <div class="px-6 py-4">
    <div class="font-bold text-xl mb-2">{{note.title}}</div>
    <p class="text-white bg-gray-600 text-base p-4">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et perferendis eaque, exercitationem praesentium nihil.
    </p>
  </div>
  <div class="px-6 py-4">
    <span class="inline-block bg-red-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 " v-for="(learn,index) in note.learns" :key="index">{{learn}}</span>
    
  </div>
</div>
  </div>
</template>


<script>
export default {
  name:"Index",
  data(){
    return {

      notes:[
        {id:1,title:"How Learn Node",url:'node-js',learns:["js","html","css","vue"]},
        {id:1,title:"How Learn DotNetCore",url:'net-c#',learns:["c#","html","css","vue","dotNet"]},
        {id:1,title:"How Learn DotNetCore",url:'net-c#',learns:["c#","html","css","vue","dotNet"]},
      ]

    }
  }
}
</script>


<style scoped>


</style>