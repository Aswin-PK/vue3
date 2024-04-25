<template>
    <div>
        <StudentList :students="students" />
    </div>
</template>

<script>
import { ref } from 'vue';
import StudentList from '../components/StudentList.vue';

export default {
    name: 'HomePage',
    components: { StudentList },
        setup() {
        const students = ref([
            { name: 'ABC', age: 20, course: 'MCA' },
            { name: 'BCD', age: 24, course: 'M.Com' },
            { name: 'EFG', age: 23, course: 'MBA' },
            { name: 'LMN', age: 21, course: 'BCA' },
        ]);

        return { students }
    }
}
</script>

<style>
    
</style>