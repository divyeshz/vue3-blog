<template>
    <div>
        <h1>Computed Property</h1>

        <h2>Inline Result :- {{ (dollars * rupeeValue) - discount }}</h2>
        <h2>Method Result :- {{ getMethodResult() }}</h2>
        <h2>Computed Result :- {{ getComputedResult }}</h2>
    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            dollars: 100,
            rupeeValue: 90,
            discount: 10,
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