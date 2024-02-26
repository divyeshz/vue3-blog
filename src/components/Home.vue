<template>
    <div>
        <h1>Html Binding</h1>
        <h3>{{ text }}</h3>
        <span v-html="tag"></span>

    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            text: 'Divyesh',
            tag: ' <h3>Divyesh Mepal</h3>'
        }
    },
    methods: {

    },
}
</script>

<style scoped></style>