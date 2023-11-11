<template>
  <div class="event-calendar">
    <table>
      <thead>
      <tr>
        <th>Fecha</th>
        <th>Título</th>
        <th>Descripción</th>
      </tr>
      </thead>
      <tbody>
      <tr v-for="(event, index) in events" :key="index">
        <td>{{ event.date }}</td>
        <td>{{ event.title }}</td>
        <td>{{ event.description }}</td>
      </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  props: {
    events: {
      type: Array,
      required: true,
    },
  },
};
</script>

<style scoped>
.event-calendar {
  max-width: 600px;
  margin: 0 auto;
}

table {
  width: 100%;
  border-collapse: collapse;
}

th, td {
  border: 1px solid #ccc;
  padding: 8px;
}

th {
  background-color: #f0f0f0;
  font-weight: bold;
}
</style>
