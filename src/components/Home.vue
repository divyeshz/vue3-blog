<template>
    <div>
        <h1>Home component</h1>
        <Child name="Divyesh" :user="user" :getData="getData" />
    </div>
</template>

<script>
import Child from './Child.vue'

export default {
    name: 'Home',
    data() {
        return {
            user: {
                name: 'Divyesh', email: 'd@gmail.com'
            }
        }
    },
    methods: {
        getData(){
            console.log('Call');
        }
    },
    components: {
        Child
    }
}
</script>

<style scoped></style>