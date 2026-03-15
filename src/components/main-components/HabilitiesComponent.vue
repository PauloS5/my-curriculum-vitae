<script setup>
  import data from '@/assets/data.json';
</script>

<template>
    <div>
        <h2>Habilidades</h2>
        <p>
            Tecnologias que utilizo diariamente e domino.
        </p>
    </div>
    
    <div>
        <ul v-for="tech in data.technologies">
            <li>{{ tech }}</li>
        </ul>
    </div>
</template>