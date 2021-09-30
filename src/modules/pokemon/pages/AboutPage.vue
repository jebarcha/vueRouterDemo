<template>
    <h1>About Page</h1>
    <hr>
    <h2>{{ name }}</h2>
    <button @click="onChangeName">
        Change Name
    </button>
</template>

<script>
export default {

    data() {
        return {
            name: 'Jose'
        }
    },
    
    methods: {
        onChangeName() {
            console.log('name will be changed to Juan');
            this.name = 'Juan'
        }
    },

    beforeCreate() {
        console.log('beforeCreate');
    },
    created() {
        this.name = 'John Lennon'
        console.log('created');
        
        // HTTP calls here

    },
    beforeMount() {
        console.log('beforeMount');
    },
    mounted() {
        console.log('mounted');
    },
    beforeUpdate() {
        console.log('beforeUpdate');
    },
    updated() {
        console.log('updated');
    },
    activated() {
        console.log('activated');
    },
    deactivated() {
        console.log('deactivated');
    },
    beforeUnmount() {
        console.log('beforeUnmount');
    },
    unmounted() {
        console.log('unmounted');
    },
    errorCaptured() {
        console.log('errorCaptured');
    },
    renderTracked() {
        console.log('renderTracked');
    },
    renderTriggered() {
        console.log('renderTriggered');
    }
}
</script>

<style>

</style>