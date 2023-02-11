<template>
    <div class="w-full mb-3 flex justify-center items-center">
        <img class="w-[95%]" :src="src" alt="Shoes" />
    </div>
</template>
<script>
export default{
    props:["src"]
}
</script>