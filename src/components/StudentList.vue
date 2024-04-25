<template>
  <div v-for="student in students" :key="student" class="student-list">
    <span>{{ student.name }}</span> - <span>{{ student.age }}</span><span></span>
  </div>
</template>


<script>
import { computed, ref } from 'vue';

export default {
  name: 'StudentList',
  props: ['students'],
}
</script>


<style scoped>
</style>
