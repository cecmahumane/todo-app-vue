<script>
export default {
    data() {
        return {
            todoText: ""
        }
    },

    methods: {
        onSubmit() {
            if (this.todoText === "") {
                alert("Please enter a todo")
            } else {
                alert(this.todoText);
                this.todoText = ""
            }
        }
    }
}
</script>

<template>
    <form @submit.prevent="onSubmit">
        <input v-model="todoText" type="text" placeholder="Add Todo..." />
        <input type="submit" value="Add Todo" />
    </form>
    <p>{{ todoText }}</p>
</template>

<style scoped>
.read-the-docs {
    color: #888;
}
</style>
