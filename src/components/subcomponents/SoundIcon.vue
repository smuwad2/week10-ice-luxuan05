<script>
    export default { 
        data() {
            return {
                soundEmojis: ['🔇', '🔈', '🔉', '🔊']
            }
        },
        // TODO: add code to define a necessary prop
        props:{
            soundLevel: {
                type: Number,
                required: true, 
                validator: (value) => value >= 0 && value <= 3
            }
        },
        methods:{

        }
    }
</script>

<template>
    <!-- TODO: add your template code here. Use span element. --> 
    <span>{{ soundEmojis[soundLevel] }}</span>
</template>