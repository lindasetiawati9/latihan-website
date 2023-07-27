<script setup>
import { TheCard } from 'flowbite-vue'
import { Rating } from 'flowbite-vue'
import { ref } from 'vue'
import { Tabs, Tab } from 'flowbite-vue'
import { Button } from 'flowbite-vue'
const activeTab = ref('first')
</script>
<template>
    <center>
        <h1 style="color: rgb(243, 93, 118);" class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Menu</h1>
    </center><br>
    <center>
      <tabs variant="underline" v-model="activeTab" class="p-5"> <!-- class appends to content DIV for all tabs -->
    <tab name="MoodBoster" title="MoodBoster">
      <div class="flex flex-row">
    <div class="basis-1/3">
    <the-card variant="image" img-src="https://theheirloompantry.co/wp-content/uploads/2023/04/fruit-sando-japanese-fruit-sandwich-the-heirloom-pantry-04.jpg" img-alt="1">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Sandwich Fruit</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
        Fruit sando atau fruit sandwich adalah makanan dari Jepang yang bentuknya seperti sandwich atau roti tangkup.
    </p><br>
    <Rating :rating="4">
      <template #besideText>
          <p class="ml-2 text-sm font-medium text-gray-500 dark:text-gray-400">4.95 out of 5</p>
        </template>
    </Rating><br>
    <Button color="default">
    <template #prefix>
      <svg class="mr-2 -ml-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M3 1a1 1 0 000 2h1.22l.305 1.222a.997.997 0 00.01.042l1.358 5.43-.893.892C3.74 11.846 4.632 14 6.414 14H15a1 1 0 000-2H6.414l1-1H14a1 1 0 00.894-.553l3-6A1 1 0 0017 3H6.28l-.31-1.243A1 1 0 005 1H3zM16 16.5a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM6.5 18a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path></svg>
    </template>
    Beli Rp.14000,-
  </Button>
    </the-card>
    </div>

    <div class="basis-1/3">
    <the-card variant="image" img-src="https://lovefoodfeed.com/wp-content/uploads/2023/01/Macarons-px-1200-01-1.jpg" img-alt="2">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Macaron</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Macaron adalah sejenis kue yang berasal dari Italia dengan bahan utama tepung almond, putih telur dan gula pasir biskuit berbentuk bulat kecil, aneka warna, renyah di luar, namun bagian tengahnya terdapat krim lembut yang lumer di mulut. 
    </p><br>
    <Rating :rating="4">
      <template #besideText>
          <p class="ml-2 text-sm font-medium text-gray-500 dark:text-gray-400">4.95 out of 5</p>
        </template>
    </Rating>
    <br>
    <Button color="default">
    <template #prefix>
      <svg class="mr-2 -ml-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M3 1a1 1 0 000 2h1.22l.305 1.222a.997.997 0 00.01.042l1.358 5.43-.893.892C3.74 11.846 4.632 14 6.414 14H15a1 1 0 000-2H6.414l1-1H14a1 1 0 00.894-.553l3-6A1 1 0 0017 3H6.28l-.31-1.243A1 1 0 005 1H3zM16 16.5a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM6.5 18a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path></svg>
    </template>
    Beli Rp.12000,-
  </Button>
    </the-card>
    </div>

    <div class="basis-1/3">
    <the-card variant="image" img-src="https://media.istockphoto.com/id/1271274108/photo/dessert-of-belgian-waffle-and-fresh-berries-isolated-on-white.jpg?s=612x612&w=0&k=20&c=dr1KZtRU4A7ekn5b250Zr5b_T08vm_Iv0mHOwQihCuU=" img-alt="3">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">waffle ice cream</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
        Waffle selama ini dikenal sebagai dessert yang dihidangkan saat sarapan dengan sirup maple, madu, atau pasta coklat sebagai topping-nya.
    </p><br>
    <Rating :rating="4">
      <template #besideText>
          <p class="ml-2 text-sm font-medium text-gray-500 dark:text-gray-400">4.95 out of 5</p>
        </template>
    </Rating>
    <br>
    <Button color="default">
    <template #prefix>
      <svg class="mr-2 -ml-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M3 1a1 1 0 000 2h1.22l.305 1.222a.997.997 0 00.01.042l1.358 5.43-.893.892C3.74 11.846 4.632 14 6.414 14H15a1 1 0 000-2H6.414l1-1H14a1 1 0 00.894-.553l3-6A1 1 0 0017 3H6.28l-.31-1.243A1 1 0 005 1H3zM16 16.5a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM6.5 18a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path></svg>
    </template>
    Beli Rp.22000,-
  </Button>
    </the-card>
    </div>
  </div>
    </tab>

    <tab name="Party" title="Party">
      <div class="flex flex-row">
    <div class="basis-1/3">
    <the-card variant="image" img-src="https://down-id.img.susercontent.com/file/f4910f49bf6c810836d024a9e2ce8625" img-alt="1">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Minimalis Cake</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
        Minimalis Cake atau Kue Minimalis adalah Kue Hidangan ala korea yang teksturnya lembut. Minimalis cake ini dihias dengan olesan buttercream berwarna menarik.
    </p><br>
    <Rating :rating="4">
      <template #besideText>
          <p class="ml-2 text-sm font-medium text-gray-500 dark:text-gray-400">4.95 out of 5</p>
        </template>
    </Rating>
    <br>
    <Button color="default">
    <template #prefix>
      <svg class="mr-2 -ml-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M3 1a1 1 0 000 2h1.22l.305 1.222a.997.997 0 00.01.042l1.358 5.43-.893.892C3.74 11.846 4.632 14 6.414 14H15a1 1 0 000-2H6.414l1-1H14a1 1 0 00.894-.553l3-6A1 1 0 0017 3H6.28l-.31-1.243A1 1 0 005 1H3zM16 16.5a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM6.5 18a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path></svg>
    </template>
    Beli Rp.83000,-
  </Button>
    </the-card>
    </div>

    <div class="basis-1/3">
    <the-card variant="image" img-src="https://s0.bukalapak.com/img/50237437792/s-463-463/0b692ff99408c5dfc32b22dd73487169.jpg.webp" img-alt="2">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Cup Cake</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
        Cup Cake merupakan makanan berupa cake lembut dengan beraneka topping yang disajikan dalam sebuah cup kecil. Biasanya disajikan di acara Ulang Tahun anak-anak.
    </p><br>
    <Rating :rating="4">
      <template #besideText>
          <p class="ml-2 text-sm font-medium text-gray-500 dark:text-gray-400">4.95 out of 5</p>
        </template>
    </Rating><br>
    <Button color="default">
    <template #prefix>
      <svg class="mr-2 -ml-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M3 1a1 1 0 000 2h1.22l.305 1.222a.997.997 0 00.01.042l1.358 5.43-.893.892C3.74 11.846 4.632 14 6.414 14H15a1 1 0 000-2H6.414l1-1H14a1 1 0 00.894-.553l3-6A1 1 0 0017 3H6.28l-.31-1.243A1 1 0 005 1H3zM16 16.5a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM6.5 18a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path></svg>
    </template>
    Beli(1) Rp.5500,-
  </Button>
    </the-card>
    </div>

    <div class="basis-1/3">
    <the-card variant="image" img-src="https://goukm.id/wp-content/uploads/2020/12/dessert-kekinian.jpeg" img-alt="3">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Dessert Box</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Dessert box merupakan makanan berupa cake dengan beraneka topping yang disajikan dalam sebuah kotak plastik.
    </p><br>
    <Rating :rating="4">
      <template #besideText>
          <p class="ml-2 text-sm font-medium text-gray-500 dark:text-gray-400">4.95 out of 5</p>
        </template>
    </Rating>
    <br>
    <Button color="default">
    <template #prefix>
      <svg class="mr-2 -ml-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M3 1a1 1 0 000 2h1.22l.305 1.222a.997.997 0 00.01.042l1.358 5.43-.893.892C3.74 11.846 4.632 14 6.414 14H15a1 1 0 000-2H6.414l1-1H14a1 1 0 00.894-.553l3-6A1 1 0 0017 3H6.28l-.31-1.243A1 1 0 005 1H3zM16 16.5a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM6.5 18a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path></svg>
    </template>
    Beli Rp.25000,-
  </Button>
    </the-card>
    </div>
  </div>
    </tab>

    <tab name="SweetDrinks" title="SweetDrinks">
      <div class="flex flex-row">
    <div class="basis-1/3">
    <the-card variant="image" img-src="https://www.theepicureanmouse.com/wp-content/uploads/2022/05/strawberry-banana-milkshake-featured-pic.jpg" img-alt="1">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Milkshake</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
        Milkshake adalah minuman dingin dari campuran susu, es krim, dan sirop berperasa yang dikocok hingga berbusa.
    </p><br>
    <Rating :rating="4">
      <template #besideText>
          <p class="ml-2 text-sm font-medium text-gray-500 dark:text-gray-400">4.95 out of 5</p>
        </template>
    </Rating>
    <br>
    <Button color="default">
    <template #prefix>
      <svg class="mr-2 -ml-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M3 1a1 1 0 000 2h1.22l.305 1.222a.997.997 0 00.01.042l1.358 5.43-.893.892C3.74 11.846 4.632 14 6.414 14H15a1 1 0 000-2H6.414l1-1H14a1 1 0 00.894-.553l3-6A1 1 0 0017 3H6.28l-.31-1.243A1 1 0 005 1H3zM16 16.5a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM6.5 18a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path></svg>
    </template>
    Beli Rp.12000,-
  </Button>
    </the-card>
    </div>

    <div class="basis-1/3">
    <the-card variant="image" img-src="https://www.anediblemosaic.com/wp-content/uploads//2022/03/boba-milk-tea-featured-image.jpg" img-alt="2">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Boba Drink</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
        Boba Drink adalah minuman sejenis bubble tea yang terdiri dari racikan susu, teh, gula, dengan topping pearls yang terbuat dari tepung tapioka dan gula. Menariknya, boba drink bukanlah minuman yang baru diluncurkan karena sudah ada di Taiwan sejak tahun 1987!
    </p><br>
    <Rating :rating="4">
      <template #besideText>
          <p class="ml-2 text-sm font-medium text-gray-500 dark:text-gray-400">4.95 out of 5</p>
        </template>
    </Rating>
    <br>
    <Button color="default">
    <template #prefix>
      <svg class="mr-2 -ml-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M3 1a1 1 0 000 2h1.22l.305 1.222a.997.997 0 00.01.042l1.358 5.43-.893.892C3.74 11.846 4.632 14 6.414 14H15a1 1 0 000-2H6.414l1-1H14a1 1 0 00.894-.553l3-6A1 1 0 0017 3H6.28l-.31-1.243A1 1 0 005 1H3zM16 16.5a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM6.5 18a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path></svg>
    </template>
    Beli Rp.10000,-
  </Button>
    </the-card>
    </div>

    <div class="basis-1/3">
    <the-card variant="image" img-src="https://www.bellieinsalute.it/wp-content/uploads/2020/04/cocktail.jpg" img-alt="3">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Fruit Drink</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Fruit Drink adalah minuman sehat yang dibuat dari potongan buah dan sirup, dan disajikan dingin.
    </p><br>
    <Rating :rating="4">
      <template #besideText>
          <p class="ml-2 text-sm font-medium text-gray-500 dark:text-gray-400">4.95 out of 5</p>
        </template>
    </Rating>
    <br>
    <Button color="default">
    <template #prefix>
      <svg class="mr-2 -ml-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M3 1a1 1 0 000 2h1.22l.305 1.222a.997.997 0 00.01.042l1.358 5.43-.893.892C3.74 11.846 4.632 14 6.414 14H15a1 1 0 000-2H6.414l1-1H14a1 1 0 00.894-.553l3-6A1 1 0 0017 3H6.28l-.31-1.243A1 1 0 005 1H3zM16 16.5a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM6.5 18a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path></svg>
    </template>
    Beli Rp.13000,-
  </Button>
    </the-card>
    </div>
  </div>
    </tab>
    
    <tab name="❀❀❀" title="❀❀❀" :disabled="true"></tab>
  </tabs>
</center>
</template>
