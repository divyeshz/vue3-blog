<template>
    <div>
        <h1 v-if="show">If Else Condition</h1>
        <h1 v-else>Else Condition</h1>

        <button @click="hideAndShow">Show Else Condition</button>
    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            show: true
        }
    },
    methods: {
        test() {
            alert('Function Called')
        },
        hideAndShow() {
            this.show = !this.show
        },
        countClick() {
            this.count++;
        },
        getValues() {

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