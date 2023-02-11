<template>
    <div class="w-[95%] mb-3 mx-3">
    <div class="card w-full bg-base-100 shadow-xl   ">
        <figure><img :src="'/'+id+'/'+'1.png'" alt="Shoes" /></figure>
        <div class="w-full h-full absolute bg-gradient-to-br from-black  to-transparent mix-blend-darken "></div>
        <div class="w-full h-full absolute flex flex-col ">
            <h2 class="flex-1 items-start text-2xl font-bold text-white mt-10 ml-10">{{ title }}</h2>
            <div class="flex-end flex justify-end">
                <NuxtLink to="/contact" class="btn btn-primary  mr-2 mb-5">Contact</NuxtLink>
                <NuxtLink :to="'/'+id" class="btn btn-primary  mr-5 mb-5">Info</NuxtLink>
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