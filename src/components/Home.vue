<template>
    <div>
        <h1>Watchers</h1>
        {{ count }}
        <br>
        <button @click="count++">+</button>
        <button @click="count--">-</button>
    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            count: 0
        }
    },
    watch: {
        count(newValue, oldValue) {
            if (newValue > 5 && newValue > oldValue) {
                alert('Value is grater than 5');
            }
            // alert('Value Change');
        }
    },
    methods: {
        getMethodResult() {
            console.log('getMethodResult');
            return (this.dollars * this.rupeeValue) - this.discount
        }
    },
    computed: {
        getComputedResult() {
            console.log('getComputedResult');
            return (this.dollars * this.rupeeValue) - this.discount
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>