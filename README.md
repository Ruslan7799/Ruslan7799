<template>
     <div>
       <span v-text="msg"> </span> <br/>
       <span v-html ="title"> </span>     
    </div>

    <div v-if ="isAdmin">
      <h1>Assalomu alaykum, Hurmatli Admistrator</h1>
    </div>
     
     <div v-else>
      <h1>Assalomu alaykum, Hurmatli Foydalanuvchi</h1>
    </div>


    <div>
      <p v-if="word === 'car' "> Mashina </p>
      <p v-else-if="word === 'Book' "> Kitob </p>
      <p v-else-if="word === 'animal' "> Hayvon </p>
      <p v-else> Bunday soz mavjud emas </p>
      <p v-show = "isBool">Men Ko'rinyabman</p>
    </div>

    <div>
      <p v-for ="i in 10">Salom</p>
    </div>
</template>

<script>
   export default {
     name :'App' ,
     data() {
         return {
           msg : "Tezkor Xabar" ,
           title : "<h1>Salom Dunyo</h1>",
           isAdmin :true ,
           word : "" ,
           isBool : false,
         }
      }
    }
  
</script>

<style>

</style>

