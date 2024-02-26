<template>
    <div>
        <h1>Get Checkbox & Radio Button Value</h1>
        <h3>Technology</h3>
        <label for="java">Java</label>
        <input type="checkbox" name="" id="java" v-model="technology" value="Java">
        <br />
        <br />
        <label for="php">PHP</label>
        <input type="checkbox" name="" v-model="technology" id="php" value="PHP">
        <br />
        <br />
        <label for="vue">Vue</label>
        <input type="checkbox" name="" v-model="technology" id="vue" value="Vue">
        <br />
        <h4>selected Technology :- {{ technology }}</h4>

        <h3>Gender</h3>
        <label for="male">Male</label>
        <input type="radio" value="Male" name="gender" id="male" v-model="gender">
        <br />
        <br />
        <label for="female">Female</label>
        <input type="radio" value="Female" name="gender" id="female" v-model="gender">
        <br />
        <h4>selected Gender :- {{ gender }}</h4>

    </div>
</template>

<script>

export default {
    name: 'Home',
    data() {
        return {
            technology: [],
            gender: null
        }
    },
    methods: {
        test() {
            alert('Function Called')
        },
        countClick() {
            this.count++;
        },
        getValues() {

        },
        getData() {
            return {
                name: 'Divyesh',
                email: this.email
            }
        }
    },
}
</script>

<style scoped></style>