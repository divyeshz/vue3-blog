<template>
    <div>
        <h1>Simple Form</h1>
        <ul>
            <li v-for="error in errors" :key="error">
                {{ error }} is not valid
            </li>
        </ul>
        <form action="">
            <label for="email">Email</label>
            <input type="text" id="email" placeholder="email" ref="text" v-model="formData.email">
            <br />
            <br />
            <label for="pass">Password</label>
            <input type="password" id="pass" placeholder="email" ref="text" v-model="formData.password">
            <br />
            <br />
            <label for="country">Country</label>
            <select name="country" id="country" v-model="formData.country">
                <option value="India">India</option>
                <option value="China">China</option>
                <option value="Japan">Japan</option>
            </select>
            <br />
            <h3>Technology</h3>
            <input type="checkbox" name="" value="php" id="php" v-model="formData.technology">
            <label for="php">PHP</label>
            <br />
            <input type="checkbox" name="" value="css" id="css" v-model="formData.technology">
            <label for="css">CSS</label>
            <br />
            <input type="checkbox" name="" value="html" id="html" v-model="formData.technology">
            <label for="html">HTML</label>
            <br />
            <h3>Gender</h3>
            <input type="radio" name="" value="male" id="male" v-model="formData.gender">
            <label for="male">Male</label>
            <br />
            <input type="radio" name="" value="female" id="female" v-model="formData.gender">
            <label for="female">Female</label>
            <br />
            <br />
            <button @click.prevent="login">Login</button>
        </form>
    </div>
</template>

<script>

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
    methods: {
        login() {
            this.errors = [];
            for (const item in this.formData) {
                if (this.formData[item] === "" || this.formData[item].length === 0) {
                    this.errors.push(item)
                }

            }

            if (this.errors.length === 0) {
                alert("Data has been submitted");
            }

            console.log('Login Data', this.formData);
            console.log('Error Item', this.errors);
        }
    },
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>