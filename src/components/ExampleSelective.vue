<template>

<h1 v-if="age < 18">Eres menor de edad</h1>
<!-- <h1 v-else-if="age >= 18">Eres mayor de edad</h1> -->
<h1 v-else>Eres mayor de edad</h1>

<!-- DIRECTIVA V-SHOW: Basicamente oculta el componente pero no lo desaperece del HTML -->
<!-- Esto no es muy util si quiero ocultar datos al usuario -->
<!-- <h1 v-show="age < 18">Eres menor de edad</h1>
<h1 v-show="age >= 18">Eres menor de edad</h1> -->
</template>

<script lang="ts" setup>
    let age = 18
</script>

<script scoped>
</script>