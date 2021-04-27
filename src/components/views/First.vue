<template>
    <div class="first-app">
        {{msg}}
        <confirm text="注册" @message="getMessage"></confirm>
    </div>
</template>
<script>
import Confirm from '../sub/Confirm'
export default {
    name: "First",
    Components: {
        Confirm
    },
    data() {
        return {
            msg: "Welcome to FirstApp"
        };
    },
    methods: {
        getMessage(val){
            alert(val);
        }
    }
};
</script>

<style>

</style>