<script setup>
const products = [
  {
    id: 1,
    name: 'Funko Dwight Schrute',
    href: 'https://shope.ee/8zgalsZ8Mc',
    source: 'Shopee - BR',
    imageSrc: new URL('/public/images/link1.jpg', import.meta.url).href
  },
  {
    id: 2,
    name: 'Pocket Pop The Office',
    href: 'https://s.click.aliexpress.com/e/_DFLC953',
    source: 'Aliexpress - China',
    imageSrc: new URL('/public/images/link7.jpg', import.meta.url).href
  },
  {
    id: 3,
    name: 'Caneca Dwight Schrute',
    href: 'https://shope.ee/7pUdNml1dY',
    source: 'shopee - BR',
    imageSrc: new URL('/public/images/link3.jpg', import.meta.url).href
  },
  {
    id: 4,
    name: 'Funko Dwight Schrute ',
    href: 'https://shope.ee/7pUjntg1eC',
    source: 'Shopee - China',
    imageSrc: new URL('/public/images/link4.jpg', import.meta.url).href
  },
  {
    id: 5,
    name: 'Posters The Office',
    href: 'https://s.click.aliexpress.com/e/_DEPOzpT',
    source: 'Aliexpress - China',
    imageSrc: new URL('/public/images/link5.jpg', import.meta.url).href
  },
  {
    id: 6,
    name: 'Camisa Dwight Schrute',
    href: 'https://s.click.aliexpress.com/e/_DE14plL',
    source: 'Aliexpress - China',
    imageSrc: new URL('/public/images/link6.jpg', import.meta.url).href
  },
  {
    id: 7,
    name: 'Caneca Gerente Assistente',
    href: 'https://shope.ee/3VLeDqezTs',
    source: 'Shopee - BR',
    imageSrc: new URL('/public/images/link2.jpg', import.meta.url).href 
  },
  {
    id: 8,
    name: 'Chaveiros The Office',
    href: 'https://s.click.aliexpress.com/e/_DkR1TEl',
    source: 'Aliexpress - China',
    imageSrc: new URL('/public/images/link8.jpg', import.meta.url).href
  },
  // More products...
]
</script>
<template>
  <div class="body">
    <div id="apoie">
      <div class="relative overflow-hidden bg-white">
        <div class="pb-80 pt-16 sm:pb-40 sm:pt-24 lg:pb-48 lg:pt-40">
          <div class="relative mx-auto max-w-7xl px-4 sm:static sm:px-6 lg:px-8">
            <div class="sm:max-w-lg"
            >
              <h1 class="text-4xl font-bold tracking-tight text-gray-900 sm:text-6xl">Todo dia Dwight</h1>
              <p class="mt-2 text-xl text-gray-500">Apoie este perfil através de uma doação ou adquirindo os itens colecionáveis. O seu incentivo é importante!</p>
              <p class="mt-4 text-xl text-gray-500">Plataforma de apoio <u> <a target="_blank"  href="https://livepix.gg/tododiadwight" class="text-xl text-blue-500">Livepix →</a></u></p>
                
            </div>
            
            <div>
              <div class="mt-10">
                <!-- Decorative image grid -->
                <div aria-hidden="true" class="pointer-events-none lg:absolute lg:inset-y-0 lg:mx-auto lg:w-full lg:max-w-7xl">
                  <div class="absolute transform sm:left-1/2 sm:top-0 sm:translate-x-8 lg:left-1/2 lg:top-1/2 lg:-translate-y-1/2 lg:translate-x-8">
                    <div class="flex items-center justify-center space-x-6 lg:space-x-8">
                    
                        <div class="h-4/5 w-4/5  overflow-hidden rounded-lg">
                          <img src="/public/images/colagem.jpeg" class="h-full w-full object-cover object-center" />
                        </div>
              
                  

                    </div>
                  </div>
                </div>

              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div id="item" class="p-2 product">

        <!-- <div class="flex justify-center">
            <img class="title-img" src="/public/logo.png">
        </div> -->
        <hr class="mt-5">
        <div class="flex justify-center mt-5">
          <h1 class="text-4xl font-bold tracking-tight text-gray-900 ">Colecionáveis</h1>

        </div>

        <div class="mx-auto mt-3 max-w-2xl px-4 py-8 lg:max-w-7xl">

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
  </div>

</template>

<style scoped>

.body{
  margin-top:48px
}
.product{
  height: auto;
}

.support{
  height: auto;
}

.title-img{
    width: 45%;
    height: 45%;
}
.mt-4 {
  white-space: nowrap;
}


</style>

