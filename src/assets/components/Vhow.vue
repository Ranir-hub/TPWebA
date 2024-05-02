<script setup>
const projects = [
    {
        img: {
            src: "/schedule.png"
        },
        text: {
            title: "Составьте расписание"
        },
        description: "Выберите время, предмет и класс. Ученики получат уведомление о предстоящем уроке."
    },

    {
        img: {
            src: "/office.png"
        },
        text: {
            title: "Подготовьте материал"
        },
        description: "Загружайте необходимые материалы к уроку."
    },

    {
        img: {
            src: "/study.png"
        },
        text: {
            title: "Начните урок с учениками"
        },
        description: "Задавайте вопросы и вызывайте «к доске» детей с поднятой рукой."
    }
]
</script>

<template>
    <section class="how">
        <div class="container">
            <h2>
                Как это работает?
            </h2>
            <div class="row">

                <div class="col-lg-4"
                        v-for="(item, index) in projects"
                        :key="index">
                    <div class="how_card">
                        <img :src="item.img.src" class="how_card-img">
                        <h3>{{item.text.title}}</h3>
                        <p>{{item.description}}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped></style>
