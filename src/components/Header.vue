<template>
    <header>
    <h1>
{{title}}
    </h1>
    <Button text="Add Task" color="green" />
    
    </header>
</template>

<script>
import Button from "./Button.vue";
export default {
    name: 'Header',
    props: {
        title: {
            type: String,
            default: 'Task Tracker',
            required: true
        }
    },
    components: {
        Button
    }
}
</script>
<style scoped>
header{
    /*background-color: #333;
    color: #fff;
    text-align: center;
    padding: 15px;*/
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;

}
</style>