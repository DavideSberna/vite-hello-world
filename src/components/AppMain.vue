<template>
    <div class="container">
        <div v-for="(item, index) in imgArr">
            <div class="d-flex align-center j-content-center">
                <div class="left" :class="{'orderEven': (index + 1) % 2 === 0}">
                    <img :src="item.image" :alt="'immagine' + ' ' + (index + 1)">
                </div>
                <div class="right">
                    <h3>{{ item.title }}</h3>
                    <p>{{ item.description }}</p>
                </div>
            </div>
        </div>
    </div>
</template>


<script>
import item1 from '../assets/img/item1.svg';
import item2 from '../assets/img/item2.svg';
import item3 from '../assets/img/item3.svg';
export default{
    name: 'AppMain',
    data(){
        return{
            imgArr:[
                {
                    image: item1,
                    title: 'Titolo articolo',
                    description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit quibusdam.',
                },
                {
                    image: item2,
                    title: 'Titolo articolo',
                    description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit quibusdam.',
                },
                {
                    image: item3,
                    title: 'Titolo articolo',
                    description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit quibusdam.',
                }
            ]
            
            
        }
    },
    methods: {
    getImageUrl(imageFilename) {
      return new URL("../assets/" + imageFilename, import.meta.url).href;
    },
  },
}
</script>

