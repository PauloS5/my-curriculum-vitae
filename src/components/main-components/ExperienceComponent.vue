<script setup>
  import data from '@/assets/data.json';
</script>

<template>
    <h2>Experiências</h2>

    <ul v-for="exp in data.experiences">
        <li>
            <h3>{{ exp.title }}</h3>
            <p>{{ exp.stack_holder }}</p>
            <p>{{ exp.description }}</p>
            <ul v-for="hab in exp.habilities">
                <li>{{ hab }}</li>
            </ul>
        </li>
    </ul>
</template>