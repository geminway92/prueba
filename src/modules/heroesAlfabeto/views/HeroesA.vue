<template>
    <div  class="ul-characters">
            <ul>

                <li v-for="item in heroesA" :key="item" class="li-characters"
                >
                {{item.name}} <img :src="item.image.url"  alt="">
                
                </li>  

            </ul>
                
        </div>
</template>

<script>
import useHeroes from '../../heroesAlfabeto/composables/useHeroes'


export default {
    name: 'letter-a',

    setup() {

        const { heroesA} = useHeroes()

        return{
            heroesA,

        }
    }
   
}


</script>
