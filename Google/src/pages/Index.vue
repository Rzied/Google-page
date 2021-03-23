<template>
  <q-layout class="column q-pa-md">
    <q-toolbar>
      <q-toolbar-title></q-toolbar-title>
      <div><a href="" class="">Gmail </a></div>
      <div class="mini"></div>
      <div><a href="#">Images</a></div>
      <q-btn flat round dense icon="apps" class="appsIcon" />
      <div>
        <q-btn
          style="text-transform: none !important"
          align="right"
          class="btn-fixed-width"
          color="primary"
          label="Connexion"
        />
      </div>
    </q-toolbar>
    <q-page
      style="min-height: 580px"
      class="flex justify-center column q-pa-md"
    >
      <div class="q-pa-md">
        <div class="flex flex-center">
          <q-img style="max-width: 350px" src="./google.png" />
        </div>
        <div class="flex justify-center row">
          <div style="max-width: 750px" class="col-12 col-sm-10 q-pa-md">
            <q-input rounded outlined v-model="text">
              <template v-slot:prepend>
                <q-icon name="search" />
              </template>
            </q-input>
          </div>
        </div>

        <div class="row justify-center">
          <div class="bbtn">
            <q-btn no-caps flat class="btng" label="Recherche Google" />
          </div>

          <div class="mini"></div>
          <div class="bbtn">
            <q-btn no-caps flat class="btng" label="J'ai de la chance" />
          </div>
        </div>
      </div>
    </q-page>

    <q-footer class="color">
      <q-toolbar class="column bg-accent q-pa-md">
        <div style="width: 100%" class="flex justify-start">
          <div>France</div>
          <q-separator style="width: 100%" color="dark" />
        </div>
        <div
          style="width: 100%; text-align: center"
          class="row justify-between"
        >
          <div class="col-12 col-md-5 justify-between" style="">
            <div class="row justify-between">
              <div><a href="">À propos</a></div>
              <div><a href="">Publicité</a></div>
              <div><a href="">Entreprise</a></div>
              <div><a href="">Comment fonctionne la recherche Google ?</a></div>
            </div>
          </div>
          <div style="" class="col-12 col-md-3 justify-center">
            Neutre en carbone depuis 2007
          </div>
          <div class="col-12 col-md-4 justify-between" style="">
            <div class="row justify-between">
              <div class="">Info consommateurs</div>
              <div class="">Confidentialité</div>
              <div class="">Conditions</div>
              <div class="">Paramètres</div>
            </div>
          </div>
        </div>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script>
export default {
  name: "PageIndex",
};
</script>

<style lang="scss">
.mini {
  flex: 0.02;
}
.appsIcon {
  margin: 2px 15px;
}
.bbtn {
  text-transform: none !important;
  font-weight: 300;
  color: black;
  background-color: #f8f9fa;
}
a {
  text-decoration: none;
  color: unset;
}
a:hover {
  text-decoration: black underline !important;
}
q-toolbar {
  background-color: #fefefe !important;
}
.color {
  color: #a8a8a8;
}
</style>