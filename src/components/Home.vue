<template>
    <div>
        <h1>Email {{ email }}</h1>
        <h1>Name {{ getName('Neel Joshi') }}</h1>
    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            email: 'test@gmail.com',
            getName: function (name) {
                return name
            }
        }
    },
}
</script>

<style scoped></style>