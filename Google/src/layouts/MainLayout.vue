<template>
  <q-layout view="lHh Lpr lFf">
    <q-header >
      <q-toolbar 
          style="background-color:white; color:black">
        

        <q-toolbar-title>
  
        </q-toolbar-title>
          <div><a href="#">Gmail</a></div>
          <div style="flex:0.03"></div>
          <div><a href="#">Images</a></div>
          <div style="flex:0.03"></div>
          <div style="flex: 0.02;">
            <img class="icone" src="./grid.png" alt="">
          </div>
          <div style="flex:0.03"></div>
          <div>
            <q-btn style="text-transform: none !important;" align="right" class="btn-fixed-width" color="primary" label="Connexion" />
          </div>

        <div>
        </div>
      </q-toolbar>
    </q-header>

   

    <q-page-container >
      
      
      <router-view />
    </q-page-container>
    <div style="background-color:#F2F2F2;color: #6F6F6F;"  class="q-pa-sm footer">
      <div>France</div>
      <hr>
      <div style="padding-top: 10px;" class="row">
        <div style="flex:0.35;" class="row">
          <div class="esp"></div>
          <div style="flex: 0.22;"><a href="#">À propos</a> </div>
          <div class="esp"></div>
          <div style="flex: 0.22;"><a href="#">Publicité</a> </div>
          <div class="esp"></div>
          <div style="flex: 0.22;"><a href="#">Entreprise</a> </div>
          <div class="esp"></div>
          <div style="flex: 1;"><a href="#">Comment fonctionne la recherche Google ?</a> </div>
        </div>
        <div style="flex: 0.35;" class="row">
          <!-- <div style="flex:0.02">
            <img src="./feuille.jpg" alt="">
          </div> -->
          <div style="flex:1;text-align: center;"><a href="#">Neutre en carbone depuis 2007</a> </div>      
        </div>
       
        <div style=" flex: 0.3;" class="row">
          <div><a href="#">Info consammateurs</a> </div>
          <div class="esp"></div>
          <div><a href="#">Confidentialité</a> </div>
          <div class="esp"></div>
          <div><a href="#">Conditions</a> </div>
          <div class="esp"></div>
          <div><a href="#">Paramètres</a> </div>
        </div>
      </div>
    </div>
  </q-layout>
</template>

<script lang="ts">
// import EssentialLink from 'components/EssentialLink.vue'

const linksData = [
  {
    title: 'Docs',
    caption: 'quasar.dev',
    icon: 'school',
    link: 'https://quasar.dev'
  },
  {
    title: 'Github',
    caption: 'github.com/quasarframework',
    icon: 'code',
    link: 'https://github.com/quasarframework'
  },
  {
    title: 'Discord Chat Channel',
    caption: 'chat.quasar.dev',
    icon: 'chat',
    link: 'https://chat.quasar.dev'
  },
  {
    title: 'Forum',
    caption: 'forum.quasar.dev',
    icon: 'record_voice_over',
    link: 'https://forum.quasar.dev'
  },
  {
    title: 'Twitter',
    caption: '@quasarframework',
    icon: 'rss_feed',
    link: 'https://twitter.quasar.dev'
  },
  {
    title: 'Facebook',
    caption: '@QuasarFramework',
    icon: 'public',
    link: 'https://facebook.quasar.dev'
  },
  {
    title: 'Quasar Awesome',
    caption: 'Community Quasar projects',
    icon: 'favorite',
    link: 'https://awesome.quasar.dev'
  }
]

import { defineComponent, ref } from '@vue/composition-api'

export default defineComponent({
  name: 'MainLayout',
  // components: { EssentialLink },
  setup () {
    const leftDrawerOpen = ref(false)
    const essentialLinks = ref(linksData)

    return { leftDrawerOpen, essentialLinks }
  }
})
</script>
<style lang="scss">
img{
  width: 100%;
}
.icone{
  margin-top: 5px;
}
.imgg{
  flex: 0.2;
  height:20px;
}
// .espb{
//   justify-content: space-around;
//   text-align: center;
//   padding: 10px 200px;
//   align-items: center;
// }
.esp{
  display:flex;
  flex:0.18;
  }
  hr{
    color: #F2F2F2
    
  }
  a{
    text-decoration:none;
    color: unset;
  }
  a:hover{
    text-decoration: black  underline !important;
    // border: solid 1px red;

  }

</style>