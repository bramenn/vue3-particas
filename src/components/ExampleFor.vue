<!-- <template>
<ul>
    <li v-for="country in countries" v-bind:key="country">
    <li v-for="country in countries" :key="country">
        {{ country }}
    </li>
</ul>
</template>

<script lang="ts" setup>
import {Ref, ref} from "vue";
let countries:Ref<Array<string>> = ref([
    "Colombia", "Alemania", "Chile", "China"
])

</script>

<script scoped>
</script> -->


<!-- ------------------------- -->
<!-- ------------------------- -->

<template>
<ul>
    <!-- <li v-for="country in countries" v-bind:key="country"> -->
    <li v-for="country in countries" :key="country.code">
        {{ country.name }}
    </li>
</ul>
</template>

<script lang="ts" setup>
import {Ref, ref} from "vue";

interface ICountry {
    code: string,
    name: string,
}

let countries:Ref<Array<ICountry>> = ref ([
    {
        code: "co",
        name: "Colombia"
    },
    {
        code: "de",
        name: "Alemania"
    },
    {
        code: "ch",
        name: "Chile"
    },
    {
        code: "xi",
        name: "China"
    },
])

</script>

<script scoped>
</script>


