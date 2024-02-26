<template>
    <div>
        <h1>Ref</h1>
        <input type="text" ref="text">

        <button @click="getText"> click me </button>
    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            childUser: "Neel"
        }
    },
    components: {

    },
    methods: {
        getText() {
            this.$refs.text.focus()
            let value = this.$refs.text.value
            console.log(value);
        }
    },
}
</script>

<style scoped>
h1 {
    color: orange;
}

.green {
    background-color: green;
    width: 500px;
    padding: 10px;
}

.err {
    color: red;
}

.other {
    font-size: 50px;
}
</style>