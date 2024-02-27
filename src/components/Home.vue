<template>
    <div>
        <h1>Non-Props Data</h1>
        <User data="Some Data" id="user-cmp" />
    </div>
</template>

<script>
import User from './User.vue';

export default {
    name: 'Home',
    data() {
        return {
            formData: {
                email: '',
                password: '',
                country: '',
                technology: [],
                gender: '',
            },
            errors: [],
        }
    },
    components: {
        User
    },
    methods: {

    },
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>