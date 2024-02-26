<template>
    <div>
        <HelloWorld msg="You did it!" />
        <Home />
    </div>
</template>

<script>
import HelloWorld from '@/components/HelloWorld.vue';
import Home from '@/components/Home.vue';

export default {
    name: 'HomeView',
    components: {
        HelloWorld,
        Home,
    }
}
</script>

<style scoped></style>