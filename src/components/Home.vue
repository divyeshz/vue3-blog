<template>
    <div>
        <input type="text" v-model="text" />
        <h2>{{ text }}</h2>
    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            text: null,
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