<template>
    <div class="modal">
        <vk-button @click="modal">My Button</vk-button>
    </div>

</template>
<script>
    import Vue from 'vue';

    import Vuikit from 'vuikit'
    import Swal from 'sweetalert2'

    Vue.use(Vuikit)

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