<template>
    <nav class="d-flex justify-content-between p-3 height-header" :style="backgroundColor">
        <img src="@/assets/logo.png" alt="" height="50" class="img-fluid h-100" />
        <div class="input-group filtro-ajuste">
            <input type="text" class="form-control" id="username" placeholder="Username" />
            <div class="input-group-prepend">
                <span class="input-group-text h-100 border-none">@</span>
            </div>
        </div>
        <div class="mt-3 nivel-total">
            <input type="text" class="nivel text-center" placeholder="70%" />
        </div>
        <img src="@/assets/avatar.png" class="avatar" height="50" />
    </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "HeaderComponent",
    components: {},
    props: {},
    data() {
        return {
            backgroundColor: {
                background: "#7f93a3",
            },
        };
    },
    computed: {},
    watch: {},

    methods: {},
});
</script>

<style scoped>
.corHeader {
    background-color: #7f93a3;
}
.height-header {
    height: 92px;
    border-bottom: 1px solid black;
}
.filtro-ajuste {
    width: 544px;
    height: 40px;
    margin-top: 10px;
}
.border-none {
    border-radius: 0px;
}
.nivel-total {
    width: 200px;
    background-color: #cd6759;
    height: 20px;
    display: flex;
    border-radius: 10px;
    border: 1px solid black;
}
.nivel {
    width: 160px;
    height: 18px;
    border-radius: 10px;
    border: 1px solid black;
    background-color: #06fc1f;
}
.avatar {
    border: 2px solid black;
    border-radius: 50%;
    padding: 2px;
}
</style>
