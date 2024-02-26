<template>
    <div>
        <h1>Class Binding</h1>
        <h3 class="otherClass" :class="applyStyle">Green Class text</h3>
        <button @click="colorFull = !colorFull">Apply Style</button>
    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            colorFull: false
        }
    },
    computed: {
        applyStyle() {
            return {
                green: this.colorFull, err: true, other: false
            }
        }
    },
}
</script>

<style scoped>
h1 {
    color: orange;
}

.green {
    background-color: green;
    width: 500px;
    padding: 10px;
}

.err {
    color: red;
}

.other {
    font-size: 50px;
}
</style>