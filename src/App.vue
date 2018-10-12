<template>
    <div id="app">
        <TodoHeader></TodoHeader>
        <TodoInput></TodoInput>
        <TodoList></TodoList>
        <TodoFooter></TodoFooter>
    </div>
</template>

<script>
    import TodoHeader from './components/TodoHeader'
    import TodoList from './components/TodoList'
    import TodoInput from './components/TodoInput'
    import TodoFooter from './components/TodoFooter'

    export default {
        data() {
            return {
                todoItems: []
            }
        },
        methods: {
            // removeOneItem(todoItem, index) {
            //     localStorage.removeItem(todoItem.item);
            //     this.todoItems.splice(index, 1);
            // },
            // toggleOneItem(todoItem, index) {
            //     this.todoItems[index].completed = !this.todoItems[index].completed;
            //     localStorage.removeItem(todoItem.item);
            //     localStorage.setItem(todoItem.item, JSON.stringify(todoItem));
            // },
            // clearAllItem() {
            //     localStorage.clear();
            //     this.todoItems = [];
            // }
        },
        name: 'app',
        components: {
            TodoHeader,
            TodoInput,
            TodoList,
            TodoFooter
        }
    }
</script>

<style>
    body {
        text-align: center;
        background-color: #F6f6f6;
    }

    input {
        border-style: groove;
        width: 200px;
    }

    button {
        border-style: groove;
    }

    .shadow {
        box-shadow: 5px 10px 10px rgba(0, 0, 0, 0.03);
    }

</style>
