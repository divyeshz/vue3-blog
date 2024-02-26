<template>
    <div>
        <h2>Teacher Name is {{ name }}</h2>
    </div>
</template>

<script>
export default {
    name: 'Teacher',
    props:{
        name: String
    }
}
</script>

<style scoped></style>