<script setup>
import { onMounted, ref } from 'vue'

const burger = ref(null)
const html = document.querySelector('html')

onMounted(() => {
  burger.value.addEventListener('click', () => {
    document.querySelector('.header').classList.toggle('open')
    html.classList.toggle('overflow-hidden')
  })
})
</script>

<template>
  <header class="header">
    <div class="navigation">
      <div class="container">
        <div class="navigation_wrap">
          <img class="navigation_logo-img" src="/logo.svg" alt="">

          <button class="navigation-button" ref="burger">
            <span></span><span></span><span></span>
          </button>

          <div class="navigation_menu-wrap">
            <div class="navigation_menu">
              <ul>
                <li class="navigation_menu-list">
                  <a href="#" class="navigation_menu_list-link">Возможности</a>

                  <a href="#" class="navigation_menu_list-link">Как это работает?</a>
                </li>
              </ul>

              <div class="navigation_menu-text">
                <p>
                  г Сургут, ул Базовая, д. 34, офис 10<br>
                  ОГРН 1238600001200ИНН<br>
                  8602309464
                </p>

                <p>
                  ООО Дотсолюшн © 2023
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>


<style scoped>

</style>