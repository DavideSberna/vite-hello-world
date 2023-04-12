<template>
    <div>
        <div v-for="(img, index) in imgArr">
            <!-- <img src="../assets/img/item1.svg" alt=""> -->
            <img :src="img" :alt="'immagine' + ' ' + (index + 1)">
            
        </div>
    </div>
</template>


<script>
export default{
    name: 'AppMain',
    data(){
        return{
            imgArr:[
                '../assets/img/item1.svg',
                '../assets/img/item2.svg',
                '../assets/img/item3.svg',
            ]
            
        }
    }
}
</script>