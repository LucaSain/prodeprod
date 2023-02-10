<template>
    <div class="w-[98%] mb-3">
    <div class="card w-full bg-base-100 shadow-xl image-full">
        <figure><img :src="'/'+id+'/'+'1.png'" alt="Shoes" /></figure>
        <div class="card-body">
            <h2 class="card-title flex-1 items-start">{{ title }}</h2>
            <div class="flex-end card-actions justify-end">
                <NuxtLink :to="'/'+id" class="btn btn-primary border-white">Info</NuxtLink>
            </div>
        </div>
    </div>
    </div>
</template>

<script>


export default{
    props:["id","title"]
}
</script>