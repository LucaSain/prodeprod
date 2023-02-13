
<style scoped src="@/assets/leaflet.css">

</style>
<template>
  
    <div class="w-screen h-screen flex flex-col sm:flex-row justify-center items-center bg-base-200">
       
    <div class="flex flex-col justify-center items-center">
        <div class="text-5xl font-bold mt-20 sm:mt-0">Despre</div>
        <h1 class="text-xl prose ml-4 mt-4 sm:mt-10">
        S. C. Prodeprod si Interprinderea Individiuala Sainenco Igor activeaza in domeniul dezvoltarii utilajelor industriale de
        peste 30 de ani vechime avand un portofoliu extins de clienti multumiti care folosesc utilajele noastre in Republica
        Moldova.</h1>
        <div class="w-full flex justify-center items-center "><NuxtLink to="/contact"><div class="btn mt-4">Contact</div></NuxtLink></div>   

    </div>
    <div class="basis-1/2 h-full w-full flex justify-center items-center">
    <div class=" h-[72%] sm:h-1/2 w-[90%] rounded-lg" id="map"></div>
    </div>

    </div>
</template>
<script>
export default {
    
    methods: {
initcarte(){
            var map = L.map('map').setView([47.19988358683537, 28.48168251554165], 7);

    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
    }).addTo(map);

            L.marker([47.78413698304982,27.922484703507877]).addTo(map)
        .bindPopup('<div class="text-xl font-bold">Prodeprod</div>')
       
 
}
    },
  
    mounted() {
// Patch for Vectorgrid with Leaflet >= 1.8
L.DomEvent.fakeStop = function () {
    return true;
}
this.$nextTick(function () {
    this.initcarte();
})
    },
};
</script>
