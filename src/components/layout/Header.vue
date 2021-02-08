<template>
    <header class="header">
        <h1>TodoList</h1>
        <div id="nav">
            <router-link to="/">Home</router-link> |
            <router-link to="/about">About</router-link>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header"
}

</script>

<style scoped>
    .header{
        background: lightblue;
        color: black;
        text-align: center;
    }

    .header a {
        color: brown;
        padding-right: 10px;
        padding-left: 10px;
        text-decoration: none;
    }


</style>