<script setup>
const route = useRoute();
const dir = route.params.id;
let cnt=0;
switch(dir[0]){
    case "ldpb52":
        cnt=3;
        break;
    case "nefil":
        cnt=3;
        break;
    case "pb40":
        cnt=1;
        break;
    case "tocator":
        cnt=5;
        break;
}

</script>

<template>
    <div class="w-screen pt-20 prose mx-auto mb-2">
        <ContentDoc />
        <div class="flex justify-center items-center">
        <NuxtLink to="/contact"> <button class="btn">Contact</button></NuxtLink>
        </div>
    </div>

  
    
    <h1 class="text-5xl text-center font-bold mb-5 mt-10">
        Galerie
    </h1>
    <div class="divider w-screen"></div>

    <div class="w-screen grid grid-flow-row grid-cols-1 sm:grid-cols-1 grid-rows-1 place-items-center place-content-center">
       <div v-for="i in cnt">
            <Cardspec :src="'/'+dir[0]+'/'+i+'.png'"/>
        </div>
    </div>
 
</template>




