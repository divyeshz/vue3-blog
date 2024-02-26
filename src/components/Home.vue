<template>
    <div>
        <button @dblclick="test()">Double Click Me</button>
        <button @click="test()">Click Me</button>

        <button @click="countClick()">Count Click</button>
        <h2>Button Clicked {{ count }} times</h2>
    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            count: 0,
            email: 'test@gmail.com',
        }
    },
    methods: {
        test() {
            alert('Function Called')
        },
        countClick() {
            this.count++;
        },
        getData() {
            return {
                name: 'Divyesh',
                email: this.email
            }
        }
    },
}
</script>

<style scoped></style>