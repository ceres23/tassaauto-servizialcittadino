<template>
  <div>
    <TitoloServizio :servizio="servizio" />
    <div class="app-container" ref="formContainer">
      <v-card class="card-view-page">
      <div class="app-row inner-cont-alert">
        <div class="text-intro col-lg-8 offset-lg-2 col-12">
          <v-alert color="danger" show>
            <strong>Questo può dipendere:</strong>
            <ul>
              <li>da un link esterno non aggiornato</li>
              <li>da un cambio d'indirizzo della pagina</li>
              <li>da un indirizzo scritto in maniera errata </li>
            </ul>
          </v-alert>
        </div>
      </div>
      </v-card>
    </div>
  </div>
</template>

<script>
import TitoloServizio from '@/components/layout/TitoloServizio'
export default {
  components: { TitoloServizio },
  data () {
    return {
      servizio: 'not_found'
    }
  }
}
</script>
