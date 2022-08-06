<template>
    <div>
        <h1>salam</h1>
        <button @click="buttonClicked(1)">{{ button1_text }}</button>
        <button @click="buttonClicked(2)">{{ button2_text }}</button>
    </div>
</template>

<script>
export default {
    name: 'Connection_test',
    data() {
        return {
            button1_text: 'Click me (1)',
            button2_text: 'Click me (2)',
        }
    },
    methods: {
        buttonClicked(ID) {
            console.log(ID)
            if ("alt" in window) {
                console.log('inash')
                // alt.emit('TestConnection_to_ALTV')
            }
        }
    }

}
</script>

<style>
</style>