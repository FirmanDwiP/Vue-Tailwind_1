<template>
  <div class="">
  
  <button class= "text-white rounded bg-red-500 px-6 py-4 font-sans font-semibold shadow-lg hover:bg-black fokus:outline-none" @click="ubahmodal = !ubahmodal">Modal</button>
  <div class="fixed overflow-x-hidden overflow-y-auto inset-0 flex justify-center item-center z-50" v-if="ubahmodal">
    <div class="relative mx-auto w-auto max-w-2xl">
      <div class="bg-white w-full rounded max-w-2xl flex flex-col">
      <div class="text-2xl font-bold">Text Header</div>
      <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere iusto quis rem, ullam veniam deleniti nesciunt quasi earum quam sequi aut ut officiis quia odio voluptatem reiciendis sint? Exercitationem, dolor?</span>
      <button class="bg-green-500 text-white px-6 mt-1 py-2 w-3/12 m-auto mb-3" @click="ubahmodal = false">Tutup</button>
      </div>
    </div>
  </div>
  <div v-if="ubahmodal" class="absolute inset-0 z-40 opacity-25 bg-black"></div>
  </div>
  
</template>

<script>
export default {
  name: 'modal',
  data() {
    return {
      ubahmodal: false
    }
  },
  methods: {
    
  },
  
}
</script>
