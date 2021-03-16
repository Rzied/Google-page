<template>
  <!-- <q-page class="row items-center justify-evenly">
    <example-component
      title="Example component"
      active
      :todos="todos"
      :meta="meta"
    ></example-component>
  </q-page> -->
  
  <div class="">
    <div class="row">
      <div style="flex: 2;"></div>
      <div style="flex: 2.3;">
        <img src="./imgg.png" alt="">
      </div>
      <div style="flex: 2;"></div>
    </div>
    <div style="justify-content: center;" class="row">

      <q-input style="flex:0.35;" rounded outlined v-model="text" >
        <template v-slot:prepend>
          <q-icon name="search" />
        </template>
      </q-input>    
    </div>
    <div style="justify-content: center;margin-top: 35px;" class="row">
      <div><q-btn flat class="btng" label="Recherche Google" /></div>
      <div class="mini"></div>
      <div><q-btn flat class="btng" label="J'ai de la chance" /></div>
    </div>
       <div class="vide"></div>
  </div>
  
  
</template>

<script lang="ts">

// import { Todo, Meta } from 'components/models'
// import ExampleComponent from 'components/CompositionComponent.vue'
// import { defineComponent, ref } from '@vue/composition-api'

// export default defineComponent({
//   name: 'PageIndex',
//   components: { ExampleComponent },
//   setup () {
//     const todos = ref<Todo[]>([
//       {
//         id: 1,
//         content: 'ct1'
//       },
//       {
//         id: 2,
//         content: 'ct2'
//       },
//       {
//         id: 3,
//         content: 'ct3'
//       },
//       {
//         id: 4,
//         content: 'ct4'
//       },
//       {
//         id: 5,
//         content: 'ct5'
//       }
//     ])
//     const meta = ref<Meta>({
//       totalCount: 1200
//     })
//     return { todos, meta }
//   }
// })
</script>
<style lang="scss">
.vide{
  height: 332px;
}
.mini{
  flex:0.01;
}
.btng{
  text-transform: none !important;
  font-weight: 300;
  color: black;
  background-color: #F8F9FA;
}

</style>
