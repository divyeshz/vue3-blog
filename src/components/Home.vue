<template>
    <div>
        <h1>Home component</h1>

        <ul>
            <li v-for="user in users" :key="user.name">
                <User :user="user" :getData="getData" />
            </li>
        </ul>

    </div>
</template>

<script>
import User from './User.vue';

export default {
    name: 'Home',
    data() {
        return {
            users: [
                {
                    name: 'Divyesh', email: 'd@gmail.com'
                },
                {
                    name: 'Neel', email: 'n@gmail.com'
                },
                {
                    name: 'Yash', email: 'y@gmail.com'
                },
                {
                    name: 'Ravi', email: 'r@gmail.com'
                },
            ]
        }
    },
    methods: {
        getData(name) {
            alert(name);
        }
    },
    components: {
        User
    }
}
</script>

<style scoped></style>