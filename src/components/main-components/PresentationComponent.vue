<script setup>
  import data from '@/assets/data.json';
</script>

<template>
    <div>
      <h2>{{ data.name }}</h2>
      <p>
        Atualmente, estudante do curso técnico integrado de Informática para Internet no Instituto Federal de Acre.
      </p>
    </div>

    <div>
        <a :href=data.social_medias.github>Email</a>
        <a :href=data.social_medias.github>Github</a>
        <a :href=data.social_medias.linkedin>Linkedin</a>
        <a :href=data.social_medias.instagram>Instagram</a>
    </div>

    <div>
      <img :src="data.profile_photo" alt="Foto de perfil" width="150">
    </div>
</template>