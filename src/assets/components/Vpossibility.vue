<script setup>
import {Swiper} from "swiper";
import { onMounted } from 'vue'
import {Pagination} from "swiper/modules";

let swiper;

onMounted(() => {
  swiper = new Swiper(".thisSwiper", {
    modules: [Pagination],
    spaceBetween: 30,
  pagination: {
      el: ".swiper-pagination",
  },
  mousewhell: true,
  keyboard: true, 
  slidesPerView: 'auto',
  breakpoints: {
      576: {
        slidesPerView: 2,
        spaceBetween: 20,
      },
      768: {
        slidesPerView: 3,
        spaceBetween: 20,
      },
      1200: {
          slidesPerView: 4,
          spaceBetween: 20,
        },
    }
  });
});
</script>

<template>
    <section class="possibility">
        <div class="container">
            <h2>
                Возможности
            </h2>
            <div class="swiper thisSwiper">
                <div class="swiper-wrapper">

                    <div class="swiper-slide">
                        <div class="possibility_card_bl">
                            <div class="possibility_card_bl-rectangle">
                                <img src="/chat.png">
                            </div>
                            <h3>Общение с классом</h3>
                            <div class="possibility_card-text">
                                <p>Видеосвязь</p>
                                <p>Чат с классом</p>
                            </div>
                        </div>
                    </div>

                    <div class="swiper-slide">
                        <div class="possibility_card_or">
                            <div class="possibility_card_or-rectangle">
                                <img src="/view.png">
                            </div>
                            <h3>
                                Проведение занятий
                            </h3>
                            <div class="possibility_card-text">
                                <p>Презентация файлов</p>
                                <p>Демонстрация экрана</p>
                            </div>
                        </div>
                    </div>

                    <div class="swiper-slide">
                        <div class="possibility_card_bl">
                            <div class="possibility_card_bl-rectangle">
                                <img src="/traffic.png">
                            </div>
                            <h3>
                                Посещаемость
                            </h3>
                            <div class="possibility_card-text">
                                <p>Автоматическое отслеживание присутствующих</p>
                            </div>
                        </div>
                    </div>

                    <div class="swiper-slide">
                        <div class="possibility_card_or">
                            <div class="possibility_card_or-rectangle">
                                <img src="/history.png">
                            </div>
                            <h3>
                                История занятий
                            </h3>
                            <div class="possibility_card-text">
                                <p>Материалы урока</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="swiper-pagination"></div>
            </div>
        </div>
    </section>
</template>

<style scoped></style>
