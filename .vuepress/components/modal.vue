<template>
    <div class="modal">
        <b-button @click="modal">I am a Button</b-button>
    </div>

</template>
<script>

    import Vue from 'vue'
    import BootstrapVue from 'bootstrap-vue'
    import 'bootstrap/dist/css/bootstrap.css'
    import 'bootstrap-vue/dist/bootstrap-vue.css'

    Vue.use(BootstrapVue);

    export default{


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