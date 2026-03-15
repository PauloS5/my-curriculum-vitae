<script setup>
  import data from '@/assets/data.json';
</script>

<template>
    <h2>Projetos Pessoais</h2>

    <ul v-for="project in data.personal_projects">
        <li>
            <h3>{{ project.title }}</h3>
            <a :href="project.git_repository">Github</a>
            <a v-if="project.deploy" :href="project.deploy">Deploy</a>
            <p>{{ project.description }}</p>
            <ul v-for="hab in project.habilities">
                <li>{{ hab }}</li>
            </ul>
        </li>
    </ul>
</template>