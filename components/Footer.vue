<template>
  <v-card height="400px">
    <v-footer v-bind="localAttrs" :padless="padless">
      <v-card flat tile width="100%" class="red lighten-1 text-center">
        <v-card-text>
          <v-btn v-for="icon in icons" :key="icon" class="mx-4" icon>
            <v-icon size="24px">
              {{ icon.iconname }}
            </v-icon>
          </v-btn>
        </v-card-text>

        <v-divider></v-divider>

        <v-card-text class="white--text">
          {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-card>
</template>

<script>
export default {
   data: () => ({
     icons: [
         {
               iconname:'mdi-facebook',
               href:'www.facebook.com'
       },
       {
               iconname:'mdi-twitter',
               href:'www.facebook.com'
       },
       {
               iconname:'mdi-instagram ',
               href:'www.facebook.com'
       },
       {
                iconname:'mdi-play-network-outline',
                href:'www.facebook.com'
       },
     ],
     items: [
       'default',
       'absolute',
       'fixed',
     ],
     padless: false,
     variant: 'default',
   }),

 }
</script>

<style></style>
