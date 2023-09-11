<template>
    <div 
     class="entry-container mb-3 pointer p-2"
     @click="$router.push({ name:'entry', params: { id: 10 }})"
    >
    <div class="entry-container mb-3 pointer p-2">
        <div class="entry-title d-flex">
            <span class="text-success fs-5">15</span>
            <span class="mx-1 fs-5">Julio</span>
            <span class="mx-2 fw-ligth">2021, Jueves</span>
        </div>
        <div class="entry-description">
            Commodo mollit minim proident proident laboris esse dolor. Ea tempor excepteur in sint dolor et enim. Ex dolor irure aute anim nulla ad ut anim ea aliquip do. Cillum magna proident reprehenderit dolor ullamco ullamco. Eu enim nisi aliquip ullamco cupidatat nisi aliqua qui culpa reprehenderit. Esse eu occaecat ullamco sunt eiusmod non. Voluptate sunt occaecat Lorem eu sit ea consequat magna incididunt Lorem aliqua.
        </div>
    </div>
   </div>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
.entry-container{
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;
    &:hover{
        background-color: lighten($color: grey, $amount: 45);
        
    }
    .entry-description{
        font-size: 12px;
    }
}
</style>