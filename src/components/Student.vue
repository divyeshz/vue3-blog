<template>
    <div>
        <h2>Student Name is {{ name }}</h2>
    </div>
</template>

<script>
export default {
    name: 'Student',
    props: {
        name: String
    }
}
</script>

<style scoped></style>