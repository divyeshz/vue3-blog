<template>
    <div>
        <h1>Dynamic components</h1>

        <button @click="tab = 'Java'">Load Java</button>
        <button @click="tab = 'Node'">Load Node</button>
        <button @click="tab = 'Php'">Load Php</button>

        <component :is="tab" />
    </div>
</template>

<script>
import Php from './Php.vue';
import Node from './Node.vue';
import Java from './Java.vue';

export default {
    name: 'Home',
    data() {
        return {
            tab: 'Java'
        }
    },
    components: {
        Php,
        Node,
        Java
    },
    watch: {
        count(newValue, oldValue) {
            if (newValue > 5 && newValue > oldValue) {
                alert('Value is grater than 5');
            }
            // alert('Value Change');
        }
    },
    methods: {
        getMethodResult() {
            console.log('getMethodResult');
            return (this.dollars * this.rupeeValue) - this.discount
        }
    },
    computed: {
        getComputedResult() {
            console.log('getComputedResult');
            return (this.dollars * this.rupeeValue) - this.discount
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>