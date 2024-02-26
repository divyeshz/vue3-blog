<template>
    <div>
        <h1>{{ childUser }}</h1>
        <User :getName="getUserName" />
    </div>
</template>

<script>
import User from './User.vue';

export default {
    name: 'Home',
    data() {
        return {
            childUser: "Neel"
        }
    },
    components: {
        User,
    },
    methods: {
        getUserName(name) {
            this.childUser = name
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