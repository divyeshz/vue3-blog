<template>
    <div>
        <h2>
            User Component
        </h2>
        <ul>
            <li>Divyesh</li>
            <li>Neel</li>
            <li>Dhruv</li>
        </ul>
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
        data: String
    }
}
</script>

<style scoped></style>