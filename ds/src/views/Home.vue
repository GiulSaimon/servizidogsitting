<template>
  <v-container class="fill-height d-flex align-center justify-center">
    <v-row justify="center">
      <v-col cols="12" md="12" lg="10">
        <v-card elevation="0" style="background-color: transparent;" class="pa-0 text-center">

          <div class="pa-6">
            <h1 class="text-h4 font-weight-bold pb-5" :style="{ color: primaryColor }">
              Trasformate la vostra vita insieme
            </h1>

            <h2 class="text-h6 pb-2" :style="{ color: primaryColor }">
              Educazione e Benessere<br />
              per il tuo cucciolo
            </h2>

            <v-divider class="mb-6"></v-divider>

            <p class="mb-4 text-body-1">
              Mi chiamo Giulia, ho 23 anni e ho la passione per i cani.
            </p>

            <p class="mb-4 text-body-1">
              Sono un’addestratrice cinofila certificata ENCI.
            </p>

            <p class="mb-6 text-body-1">
              Se il tuo obiettivo è trasformare la convivenza quotidiana in un percorso sereno,
              rendendo ogni momento insieme un piacere condiviso, contattami e ti aiuterò a realizzarlo.
            </p>

            <v-divider class="mb-6"></v-divider>

            <h2 class="text-h6 font-weight-bold mb-4" :style="{ color: primaryColor }">Disponibile per</h2>

            <v-list density="comfortable" bg-color="transparent">
                <v-list-item v-for="(item, i) in servizi" :key="i">
                  <v-list-item-title>
                      <v-icon class="mr-2" icon="mdi-paw"></v-icon>
                      <span v-html="item"></span>
                  </v-list-item-title>
                </v-list-item>
              </v-list>
          </div>
          <v-row class="d-flex justify-center align-center">
            <v-col cols="4">
              <v-img src="/servizidogsitting/img1.webp" width="100%" />
            </v-col>

            <v-col cols="4">
              <v-img src="/servizidogsitting/img2.webp" width="100%" />
            </v-col>

            <v-col cols="4">
              <v-img src="/servizidogsitting/img3.webp" width="100%" />
            </v-col>
          </v-row>
          <v-row class="d-flex justify-center align-center">
            <v-col cols="8" md="6" lg="6">
              <v-img
                src="/servizidogsitting/dog.webp"
                width="100%"
              />
            </v-col>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
const primaryColor = '#ff54b0'

const servizi = [
  'Sessione educativa a partire da 30 €',
  'Percorsi educativi base a partire da 130 € (pacchetto da 5 lezioni)',
  'Passeggiate pomeridiane/serali o weekend a partire da 10 €/h',
  'Dog Sitter tutto il giorno o mezze giornate: prezzo da concordare'
]
</script>

<style scoped>
h1, h2, h3 {
  line-height: 1.3;
  margin:0;
  text-wrap: wrap;
}
span {
  text-wrap: wrap;
}
</style>