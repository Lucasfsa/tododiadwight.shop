<script setup>
const products = [
  {
    id: 1,
    name: 'Funko Dwight Schrute',
    href: 'https://shope.ee/8zgalsZ8Mc',
    source: 'Shopee - BR',
    imageSrc: '/src/img/shopee/link1.jpg',
  },
  {
    id: 2,
    name: 'Pocket Pop The Office',
    href: 'https://s.click.aliexpress.com/e/_DFLC953',
    source: 'Aliexpress - China',
    imageSrc:  '/src/img/aliexpress/link7.jpg',
  },
  {
    id: 3,
    name: 'Caneca Dwight Schrute',
    href: 'https://shope.ee/7pUdNml1dY',
    source: 'shopee - BR',
    imageSrc:  '/src/img/shopee/link3.jpg',
  },
  {
    id: 4,
    name: 'Funko Dwight Schrute ',
    href: 'https://shope.ee/7pUjntg1eC',
    source: 'Shopee - China',
    imageSrc:  '/src/img/shopee/link4.jpg',
  },
  {
    id: 5,
    name: 'Posters The Office',
    href: 'https://s.click.aliexpress.com/e/_DEPOzpT',
    source: 'Aliexpress - China',
    imageSrc:  '/src/img/aliexpress/link5.jpg',
  },
  {
    id: 6,
    name: 'Camisa Dwight Schrute',
    href: 'https://s.click.aliexpress.com/e/_DE14plL',
    source: 'Aliexpress - China',
    imageSrc:  '/src/img/aliexpress/link6.jpg',
  },
  {
    id: 7,
    name: 'Caneca Gerente Assistente',
    href: 'https://shope.ee/3VLeDqezTs',
    source: 'Shopee - BR',
    imageSrc:  '/src/img/shopee/link2.jpg',
  },
  {
    id: 8,
    name: 'Chaveiros The Office',
    href: 'https://s.click.aliexpress.com/e/_DkR1TEl',
    source: 'Aliexpress - China',
    imageSrc:  '/src/img/aliexpress/link8.jpg',
  },
  // More products...
]
</script>
<template>
    <div class="bg-white p-2 shadow-lg body">

        <!-- <div class="flex justify-center">
            <img class="title-img" src="/public/logo.png">
        </div> -->

        <div class="mx-auto max-w-2xl px-4 py-8 lg:max-w-7xl">

            <div class="grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 xl:gap-x-8">
                <a v-for="product in products" :key="product.id" :href="product.href" target="_blank" class="group">
                <div class="aspect-h-1 aspect-w-1 w-full overflow-hidden rounded-lg bg-gray-200 xl:aspect-h-8 xl:aspect-w-7">
                    <img :src="product.imageSrc" :alt="product.imageAlt" class="h-full w-full object-cover object-center group-hover:opacity-75" />
                </div>
                <h3 class="mt-4 text-lg font-medium text-gray-900">{{ product.name }}</h3>
                <p class="mt-1 text-sm text-gray-700">{{ product.source }}</p>
                </a>
            </div>
        </div>
        
    </div>
</template>

<style scoped>
.body{
    height: auto;
    border-radius: 3px;
}

.title-img{
    width: 45%;
    height: 45%;
}

</style>

