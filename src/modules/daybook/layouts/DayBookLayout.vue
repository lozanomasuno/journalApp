<template>
    <Navbar></Navbar>
    <div class="d-flex">
        <div class="col-4">
            <EntryList></EntryList>
        </div>
        <div class="col">
            <router-view></router-view>
        </div>
    </div>
</template>
<script>
import { defineAsyncComponent } from 'vue';
export default {
    components: {
        Navbar: defineAsyncComponent( ()=> import('../components/app-navbar.vue')),
        EntryList: defineAsyncComponent(()=> import ('../components/app-entrylist.vue'))
    }
}
</script>