<template>
  <slide class="bg-gray-200 px-8 py-4">
    <h1 class="text-5xl">Links and shit</h1>
    <ul>
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
        'https://snipcart.com/blog/jamstack'
      ]
    }
  }
}
</script>

