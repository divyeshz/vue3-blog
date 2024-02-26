<template>
    <div>
        <h2>Child Component Name is {{ name }}</h2>
        <h3>User : {{ user }}</h3>
        <h3>User name : {{ user.name }}</h3>
        <h3>User email : {{ user.email }}</h3>
        <button @click="getData()"> Call Parent component Function</button>
    </div>
</template>

<script>
export default {
    name: 'Child',
    props: {
        name: String,
        user: Object,
        getData: Function
    }
}
</script>