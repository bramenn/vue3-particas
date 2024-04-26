<!-- Este ejemplo es usando Compotition API y bindeo de estilos css -->

<template>
<!-- <p v-bind:class="{ 'danger': hasError }"> -->
<p :class="{ 'danger': hasError }">
    El mensaje se ha enviado satisfactoriamente.
</p>

<p v-bind:style="{ backgroundColor: '#ccc', color: new_color }">
    El mensaje se ha enviado satisfactoriamente 2.
</p>
<!-- <button v-on:click="handleClick">Cambiar color</button> -->
<button @click="handleClick">Cambiar color</button>

<!-- ------------------------- -->


</template>




<!-- <script lang="ts">
    import { defineComponent } from "vue";
    export default defineComponent({
        name: "ClassBind",
        data() {
            return {
                hasError: true
            }
        }
    })

</script> -->

<!-- ------------------------- -->
<!-- ------------------------- -->

<!-- <script lang="ts">
    import { defineComponent } from "vue";
    export default defineComponent({
        name: "ClassBind",
        setup() {
            let hasError = false;
            return {hasError}
        }
    })

</script> -->


<!-- ------------------------- -->
<!-- ------------------------- -->


<!-- <script lang="ts" setup>
    import {ref} from "vue"
    let hasError = true;
    let new_color = ref("green");

    const handleClick = () => {new_color.value = "yellow"}

</script> -->


<!-- <script lang="ts">
    import { defineComponent} from "vue"
    export default defineComponent({
        name: "ClassBind",
        data() {
            return {
                new_color: 'blue',
                hasError: true
            }
        },
        methods: {
            handleClick() {
                this.new_color = "brown"
            }
        }
    })
</script> -->

<script lang="ts">
    import { defineComponent, ref } from "vue"
    export default defineComponent({
        name: "ClassBind",
        setup() {
            let new_color = ref('blue');
            let hasError = ref(true);

            const handleClick = () => {
                new_color.value = "brown"
            }

            return {new_color, hasError, handleClick}
        },
    })
</script>


<style>
.danger {
    color: red;
}

</style>
