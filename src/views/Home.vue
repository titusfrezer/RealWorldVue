<template>
  <div class="events">
    <img alt="Vue logo" src="../assets/logo.png" />
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "Home",
  components: {
    EventCard
  },
  data(){
    return{
      events:[
        {
          id:1244,
          title:'animal welfare',
          description:'find your feline friend',
          time:'12 pm',
          organizer:'mike d'
        },
        {
          id:3555,
          title:'London has fallen',
          description:'find your feline friend',
          time:'12 pm',
          organizer:'titus d'
        },
        {
          id:645454,
          title:'Tuer welfare',
          description:'find your feline friend',
          time:'12 am',
          organizer:'bisre d'
        }
      ]
    }
  }
};
</script>

<style scoped>
.events{
  display:flex;
  flex-direction: column;
  align-items:center
}
</style>
