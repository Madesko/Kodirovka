<template>
    <div>
        <div>
            <p>����� �����: {{tasks.length}}</p>
            <nav>
                <router-link to="/add/task">������� ������</router-link>
                <router-link to="/all/tasks">�������� �����</router-link>
            </nav>
        </div>
        <div>
            <router-view></router-view>
        </div>
    </div>
</template>
<script>
    import { allTasks } from "./tmp/taskArr";
    export default {
        name: "App",
        data: function () {
            return {
                tasks: allTasks
            }
        }
    }
</script>
<style lang="scss">
</style>
