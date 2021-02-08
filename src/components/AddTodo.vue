<template>
    <div>
        <form @submit="addTodo">
            <input type="text" v-model="title" name="title" class="btn_input" 
            placeholder="Add stuff..">
            <input type="submit" value="Submit" class="btn">
        </form>
    </div>
</template>

<script>
// import {v4} from "uuid";

export default {
    name: "AddTodo",
    data(){
        return {
            title:''
        }
    },
    methods: {
        addTodo(e){
            e.preventDefault();
            const newTodo = {
                // id: v4(),
                title: this.title,
                completed: false
            }
            this.$emit('add-todo', newTodo);

            this.title = '';
        }
    }
}
</script>

<style scoped>

</style>