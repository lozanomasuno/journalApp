<template>
    <div class="entry-title d-flex justify-content-between p-2">
        <div>
            <span class="text-success f3 fw-bold">15</span>
            <span class="mx-1 fs-3">Julio</span>
            <span class="mx-2 fs-4 fw-light">2021, Jueves</span>
        </div>
        <div>
            <button class="btn btn-danger mx-2">
                Borrar
                <i class="fa fa-trash-alt"></i>
            </button>
            <button class="btn btn-primary">
                Subir foto
                <i class="fa fa-upload"></i>
            </button>
        </div>
    </div>

    <hr>
    <div class="d-flex flex-column px-3 h-75">
        <textarea name="" id="" cols="30" rows="10" placeholder="What Happens today?">

        </textarea>
        
    </div>
    <Fab 
        icon = "fa-save"
    />
    <img src="http://t0.gstatic.com/licensed-image?q=tbn:ANd9GcR4KP0sEPRfzdEXr8GXecgOu6QrPYLO0N_jz2Lyd6Ng-dsY3yWuRdwEyle5QobuLsQHzNEkfd7CCswpRUxLtO0" alt="entry-picture" class="thumbnail">
</template>

<script>
import { defineAsyncComponent } from 'vue';

export default {
    components:{
        Fab: defineAsyncComponent(()=> import ('../components/app-fab.vue'))
    }
}
</script>
<style scoped lang="scss">
    textarea {
        font-size: 20px;
        border: none;
        height: 100%;
        
        &:focus {
            outline: none;
        }
    }
    img {
        width: 200px;
        position: fixed;
        bottom: 150px;
        right: 20px;
        box-shadow: 0px 5px 10px rgba($color: #000000, $alpha:0.2);
    }
</style>