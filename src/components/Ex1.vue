<script>
    //import component
    import soundIcon from './subcomponents/SoundIcon.vue'
    
    export default { 
        components:{
            soundIcon
        },
        data() {
            return {
                soundLevel: 0
            }
        }
    }
</script>

<template>

   Sound level
    <input type="number" min="0" max="3" v-model="soundLevel"> 
    <!-- TODO: Add Code Here to make use of the component -->
    <soundIcon :soundLevel="soundLevel" />

</template>

