<template>
  <div>
    <h1>Calendario de Eventos</h1>
    <event-calendar :events="eventList" />
  </div>
</template>

<script>
import EventCalendar from './EventCalendar.vue';

export default {
  data() {
    return {
      eventList: [
        {
          date: '2023-11-15 16:00',
          title: 'Agenda ocupada',
          description: 'Sumergirme en mi propia miseria',
        },
        {
          date: '2023-11-15 16:30',
          title: 'Agenda ocupada',
          description: 'Contemplar el abismo',
        },
        {
          date: '2023-11-15 17:00',
          title: 'Agenda ocupada',
          description: 'Solucionar la hambruna mundial sin decirselo a nadie',
        },
        {
          date: '2023-11-15 17:30',
          title: 'Agenda ocupada',
          description: 'Danza y ejercicio',
        },
        {
          date: '2023-11-15 18:30',
          title: 'Agenda ocupada',
          description: 'Cena conmigo mismo; NOTA: esa no se cancela',
        },
        {
          date: '2023-11-15 19:00',
          title: 'Agenda ocupada',
          description: 'Luchar con el odio que me tengo ',
        }
      ],
    };
  },
  components: {
    EventCalendar,
  },
};
</script>

<style>
h1 {
  text-align: center;
  margin-top: 20px;
}

</style>
