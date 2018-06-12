<template>
<div class="modal">

    <md-button class="md-primary md-raised" @click="modal">Primary</md-button>
</div>
</template>
<script>

    import Swal from 'sweetalert2';

    import Vue from 'vue';
    import VueMaterial from 'vue-material'
    import 'vue-material/dist/vue-material.css'
    Vue.use(VueMaterial);



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

    <style scoped>
    @import "~material-design-icons/iconfont/material-icons.css";
</style>
