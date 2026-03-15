<script setup>
  import data from '@/assets/data.json';
</script>


<template>
    <h2>Formação</h2>

    <ul v-for="course in data.education">
        <li>
            <h3>{{ course.title }}</h3>
            <p>{{ course.institution }}</p>
            <p>{{ course.description }}</p>
            <p v-if="course.start_year && course.end_year">{{ course.start_year }} - {{ course.end_year }}</p>
            <p>{{ course.duration }}</p>
            <ul v-for="hab in course.habilities">
                <li>{{ hab }}</li>
            </ul>
        </li>
    </ul>
</template>