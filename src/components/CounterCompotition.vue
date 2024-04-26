<!-- Este ejemplo explica como tranferir datos el template usando el compotition API en sus dos formas -->

<template>
<h3>{{ counter }}</h3>
<button @click="addCounter">Incrementar</button>
</template>

<!-- ASÍ SE DESCRIBE UN COMPONENTE DE MANERA MAS EXPLICITA -->
<!-- <script lang="ts">
import { defineComponent, Ref, ref } from "vue"
export default defineComponent({
    name: 'CounterComposition',
    setup(){
        let counter:Ref = ref(0);
        const addCounter = ():void => {
            counter.value++
        }
        return {counter, addCounter}
    }
})
</script> -->


<!-- "setup" ayuda a no definir todo lo anterior -->
<script lang="ts" setup>
import { Ref, ref } from "vue"
let counter:Ref = ref(0);
const addCounter = ():void => {
    counter.value++
}
</script>

