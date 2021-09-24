<template>
<v-row>
<v-col
v-for="card2 in cards" :key="card2"
      cols="6"
      sm="4"
      
    >
     <v-hover v-slot="{ hover }" >
    <v-card flat
    class="pa-6"
   
    :elevation="hover ? 12 : 0"
  >
 
   <h1><v-icon x-large >{{card2.icon}}</v-icon>&nbsp; &nbsp;{{card2.title}}</h1>
    <p>{{card2.subtitle}}</p>
  </v-card>
     </v-hover>
</v-col>
</v-row>
</template>


<script>
export default {
  data() {
    return {
      cards: [
        {
          icon:'mdi-clock-outline',
          title: 'Unlimited Colors',
          subtitle:
            'Our energy is focus in inspiring projects, activation campaigns and influence strategies',
        },
        {
          icon:'mdi-earth',
          title: 'High Quality Design',
          subtitle:
            'We believe in a collaborative partnership where we work with you to create the perfect solution.',
        },
        {
          icon:'mdi-clock-outline',
          title: 'Luxurious Layouts',
          subtitle:
            'We help our clients in developing systems of digital products and services over time.',
        },
      ],
    }
  },
}
</script>

<style scoped>
h1{
    font-size: 15px;
}
</style>