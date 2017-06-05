<template>
<div class="wrapper">
<am-head></am-head>
<am-sidebar></am-sidebar>
<div>
<transition name="move" mode="out-in"><router-view></router-view></transition>
</div>
</div>
</template>
<script>
import amHead from './common/Head.vue';
import amSidebar from './common/Sidebar.vue';
export default {
    components:{
        amHead, amSidebar
    }
}
</script>

<style scoped="">

</style>
