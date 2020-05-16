<template>
    <!-- <task-form outside="Добавление задачи"></task-form> -->
    <!--<p>Добавление задачи</p> -->
    <task-form v-bind:outside="someString"></task-form>
</template>
<script>
    import TaskForm from "@/components/TaskForm.vue";
	export default {
        name: "AddTask",
        components: {
            TaskForm
        },
        data: function () {
            return {
                someString: "Добавление задачи"
            }
        }
	}
</script>
<style lang="scss">
</style>
