<template>
    <div v-bind:class="{'is-complete': todo.completed}">
        <p>{{ todo.title }}</p>
    </div>
</template>

<script>
export default {
    name: 'TodoItem',
    props: ["todo"],

}
</script>

<style scoped>
    .is-complete {
        text-decoration: line-through;
    }
</style>