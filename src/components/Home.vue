<template>
    <div>
        <h1>Props</h1>
        <Student :name="name" />
        <Teacher name="Divyesh" />
    </div>
</template>

<script>
import Student from './Student.vue';
import Teacher from './Teacher.vue';

export default {
    name: 'Home',
    data() {
        return {
            name: "Neel"
        }
    },
    computed: {
        applyStyle() {
            return {
                green: this.colorFull, err: true, other: false
            }
        }
    },
    components: {
        Student,
        Teacher
    }
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