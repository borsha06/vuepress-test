<template>
    <div class="modal">
        <q-btn @click="modal">Do something</q-btn>
    </div>

</template>
<script>
    import Vue from 'vue';
    import Quasar from "quasar-framework/dist/quasar.mat.esm";
    import "quasar-framework/dist/umd/quasar.mat.css";
    import Swal from 'sweetalert2';
    import { QBtn } from "quasar-framework/dist/quasar.mat.esm";

    Vue.use(Quasar);

    export default{
        name: "App",
        components: {
            QBtn,
        },

        data(){
            return {
                opened: false
            }
        },
        methods: {


            modal: function () {
                Swal('Hello world!')
            }
        }
    }

</script>