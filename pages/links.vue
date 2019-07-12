<template>
  <slide class="bg-gray-200 px-8 py-4" prev="/fin">
    <h1 class="text-100"><span class="underline">Links</span> and <span class="line-through">shit</span></h1>
    <ul class="text-4xl">
      <li 
        v-for="(link, index) in links"
        :key="index"
      >
        <a :href="link" target="_blank" class="hover:underline">{{ link }}</a>
      </li>
      
    </ul>
  </slide>
</template>

<script>
export default {
  computed: {
    links () {
      return [
        'https://upload.wikimedia.org/wikipedia/commons/9/95/Vue.js_Logo_2.svg',
        'https://angular.io/assets/images/logos/angular/angular.svg',
        'https://nodejs.org/static/images/logo.svg',
        'https://www.apachefriends.org//images/xampp-logo-ac950edf.svg',
        'https://jamstack.org/',
        'https://jamstack.wtf/',
        'https://snipcart.com/blog/jamstack',
        'https://alternativeto.net/software/netlify/',
        'https://laravel.com/docs/5.8/valet',
        'https://laravel.com/docs/5.8/homestead',
        'https://www.rapidtables.com/web/html/html-codes.html',
        'https://tailwindcss.com/'
      ]
    }
  }
}
</script>

