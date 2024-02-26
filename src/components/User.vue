<template>
    <div>
        <h3>
            Name Is {{ user.name }} And Email Is {{ user.email }}
        </h3>
        <button @click.prevent="getData(user.name)"> Get Name</button>
    </div>
</template>

<script>
export default {
    name: 'User',
    data() {
        return {

        }
    },
    props: {
        user: Object,
        getData: Function,
    }
}
</script>

<style scoped></style>