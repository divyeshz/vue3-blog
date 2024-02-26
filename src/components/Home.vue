<template>
    <div>
        <h1>For loop</h1>
        <ul v-for="tech in technology" :key="tech">
            <li> {{ tech }}</li>
        </ul>

        <br />
        <br />
        <ul>
            <li v-for="user in users" :key="user.name">
                Name is : {{ user.name }} and
                Email is : {{ user.email }}
            </li>
        </ul>
    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            technology: ['Java', 'PHP', 'Vue', 'Node', 'Html'],
            users: [
                {
                    name: "Divyesh",
                    email: "test@gmail.com"
                },
                {
                    name: "Neel",
                    email: "test1@gmail.com"
                },
                {
                    name: "Ravi",
                    email: "test3@gmail.com"
                },
                {
                    name: "Yash",
                    email: "test4@gmail.com"
                },
            ]
        }
    },
    methods: {

    },
}
</script>

<style scoped></style>