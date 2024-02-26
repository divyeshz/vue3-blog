<template>
    <div>
        <h1>Email {{ email }}</h1>
        <h1>Name {{ getName('Neel Joshi') }}</h1>
        <h1>Get Data :- {{ getData().email }}</h1>
    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            email: 'test@gmail.com',
        }
    },
    methods: {
        getName(name) {
            return name
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