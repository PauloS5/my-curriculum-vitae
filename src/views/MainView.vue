<script setup>
  import PresentationComponent from '@/components/main-components/PresentationComponent.vue';
  import HabilitiesComponent from '@/components/main-components/HabilitiesComponent.vue';
  import ExperienceComponent from '@/components/main-components/ExperienceComponent.vue';
  import PersonalProjects from '@/components/main-components/PersonalProjects.vue';
  import EducationComponent from '@/components/main-components/EducationComponent.vue';
</script>

<template>
  <section>
    <PresentationComponent />
  </section>

  <section>
    <HabilitiesComponent />
  </section>

  <section>
    <ExperienceComponent />
  </section>

  <section>
    <PersonalProjects />
  </section>
  
  <section>
    <EducationComponent />
  </section>
</template>
