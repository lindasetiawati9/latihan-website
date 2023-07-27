<script setup>
import { Carousel } from 'flowbite-vue'

const props = defineProps({
    pictures: {
        type: Array,
        default() {
            return [
                {
                    'src': 'https://caliclecups.com/cdn/shop/articles/melting_ice_cream.jpg?v=1647644764',
                    'alt': 'Picture 1',
                },
                {
                    'src': 'https://www.savour-magazine.co.uk/wp-content/uploads/2019/04/Apple-waffles-landscape.jpg',
                    'alt': 'Picture 2',
                },
                {
                    'src': 'https://nibble-images.b-cdn.net/nibble/original_images/dessert_bittersweet_f7c1994792.jpg',
                    'alt': 'Picture 3',
                }
            ]
        },
    },
})

</script>
<template>
    <Carousel :pictures="pictures" :slide="true" :slide-interval="1000" ></Carousel>
  </template>