<template>
    <div>
        <h2>
            User Component
        </h2>

        <button @click="getName(userName)">Send User Name </button>
    </div>
</template>

<script>
export default {
    name: 'User',
    data() {
        return {
            userName: 'Divyesh'
        }
    },
    props: {
        getName: Function
    }
}
</script>

<style scoped></style>