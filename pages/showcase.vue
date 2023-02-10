<template>
    <div  class="pt-20 w-screen grid grid-flow-row grid-cols-1 sm:grid-cols-3 place-items-center place-content-start gap-3">
        <div v-for="id in ids">
    <Card :title="id.title" :id="id.id"/>
</div>
    </div>
</template>

<script>


export default{
    data(){
        return{
            ids: [{ title: "Presa PB-40", id: "pb40" }, { title: "Linia LDPB-52",id:"ldpb52"}, {title:"Linie cu tocator",id:"tocator"}, {title:"Presa Nefil",id:"nefil"}]
        }
    }
}
</script>