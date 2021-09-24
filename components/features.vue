<template>
  <div>
    <h1>Creative approach to Solving Problems</h1>
    <p>
      We only hire great people who strive to push their<br />
      ideas into fruition by outmuscling.
    </p>
    <br />
    <br />

    <v-row>
      <v-col v-for="card in cards" :key="card" cols="6" sm="4" align="center">
           <v-hover v-slot="{ hover }" >
        <v-card flat class="pa-6" :elevation="hover ? 12 : 0">
         <v-icon x-large >{{
              card.icon
            }}</v-icon>
          <h1>{{ card.title }}</h1>

          <p>
            {{ card.subtitle }}
          </p>
        </v-card>
        </v-hover>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cards: [
        {
          icon: 'mdi-monitor',
          title: 'Results oriented',
          subtitle:
            'With our powerful network of personalities dedicated to inspiration and creativity.',
        },
        {
          icon: ' mdi-application-edit-outline',
          title: 'Visual Composer',
          subtitle:
            'We work with good people that share in the belief that design makes a difference.',
        },
        {
          icon: 'mdi-account',
          title: 'Free Support',
          subtitle:
            'We’re honest folk that believe in hard work and building lasting relationships.',
        },
      ],
    }
  },
}
</script>

<style scoped>
h1 {
  margin-top: 10%;
  text-align: center;
}
p {
  margin-top: 5%;
  text-align: center;
  font-size: 20px;
}
</style>
