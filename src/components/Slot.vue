<template>
    <div>
        <slot></slot>
    </div>
</template>

<script>
export default {
    name: 'SlotCompo',
    props: {
        msg: String
    }
}
</script>

<style scoped></style>