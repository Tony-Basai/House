<script setup>
import { ref, computed } from 'vue';

import ReproductionsCard from './ReproductionsCard.vue';
import Image1 from '../assets/Image1.svg'
import Image2 from '../assets/Image2.svg'
import Image3 from '../assets/Image3.svg'
import Image4 from '../assets/Image4.svg'
import Image5 from '../assets/Image5.svg'
import Image6 from '../assets/Image6.svg'
import Image7 from '../assets/Image7.svg'
import Image8 from '../assets/Image8.svg'
import Image9 from '../assets/Image9.svg'
import Image10 from '../assets/Image10.svg'
import Image11 from '../assets/Image11.svg'
import Image12 from '../assets/Image12.svg'
import Image13 from '../assets/Image13.svg'
import Image14 from '../assets/Image14.svg'
import Image15 from '../assets/Image15.svg'
import Image16 from '../assets/Image16.svg'
import Image17 from '../assets/Image17.svg'
import Image18 from '../assets/Image18.svg'

const cards = ref([
    {
        id: 1,
        country: "Франция",
        image: Image1,
        autor: "Марсель Руссо",
        name: "Охота Амура",
        description: "Холст, масло (50х80)",
        price: 14500
    },
    {
        id: 2,
        country: "Франция",
        image: Image2,
        autor: "Анри Селин",
        name: "Дама с собачкой",
        description: "Акрил, бумага (50х80)",
        price: 16500
    },
    {
        id: 3,
        country: "Франция",
        image: Image3,
        autor: "Франсуа Дюпон",
        name: "Процедура",
        description: "Цветная литография (40х60)",
        price: 20000
    },
    {
        id: 4,
        country: "Франция",
        image: Image4,
        autor: "Луи Детуш",
        name: "Роза",
        description: "Бумага, акрил (50х80)",
        price: 12000
    },
    {
        id: 5,
        country: "Франция",
        image: Image5,
        autor: "Франсуа Дюпон",
        name: "Птичья трапеза",
        description: "Цветная литография (40х60)",
        price: 22500
    },
    {
        id: 6,
        country: "Франция",
        image: Image6,
        autor: "Пьер Моранж",
        name: "Пейзаж с рыбой",
        description: "Цветная литография (40х60)",
        price: 20000
    },
    {
        id: 7,
        country: "Германия",
        image: Image7,
        autor: "Курт Вернер",
        name: "Над городом",
        description: "Цветная литография (40х60)",
        price: 16000
    },
    {
        id: 8,
        country: "Германия",
        image: Image8,
        autor: "Макс Рихтер",
        name: "Птенцы",
        description: "Холст, масло (50х80)",
        price: 14500
    },
    {
        id: 9,
        country: "Германия",
        image: Image9,
        autor: "Мартин Майер",
        name: "Среди листьев",
        description: "Цветная литография (40х60)",
        price: 20000
    },
    {
        id: 10,
        country: "Германия",
        image: Image10,
        autor: "Герман Беккер",
        name: "Яркая птица",
        description: "Цветная литография (40х60)",
        price: 13000
    },
    {
        id: 11,
        country: "Германия",
        image: Image11,
        autor: "Вульф Бауэр",
        name: "Дятлы",
        description: "Бумага, акрил (50х80)",
        price: 20000
    },
    {
        id: 12,
        country: "Германия",
        image: Image12,
        autor: "Вальтер Хартманн",
        name: "Большие воды",
        description: "Бумага, акрил (50х80)",
        price: 23000
    },
    {
        id: 13,
        country: "Англия",
        image: Image13,
        autor: "Пол Смит",
        name: "Дикий зверь",
        description: "Акварель, бумага (50х80)",
        price: 19500
    },
    {
        id: 14,
        country: "Англия",
        image: Image14,
        autor: "Джон Уайт",
        name: "Скалистый берег",
        description: "Цветная литография (40х60)",
        price: 17500
    },
    {
        id: 15,
        country: "Англия",
        image: Image15,
        autor: "Джим Уотсон",
        name: "Река и горы",
        description: "Акварель, бумага (50х80)",
        price: 20500
    },
    {
        id: 16,
        country: "Англия",
        image: Image16,
        autor: "Юджин Зиллион",
        name: "Белый попугай",
        description: "Цветная литография (40х60)",
        price: 15500
    },
    {
        id: 17,
        country: "Англия",
        image: Image17,
        autor: "Эрик Гиллман",
        name: "Ночная рыба",
        description: "Бумага, акрил (50х80)",
        price: 12500
    },
    {
        id: 18,
        country: "Англия",
        image: Image18,
        autor: "Альфред Барр",
        name: "Рыжий кот",
        description: "Цветная литография (40х60)",
        price: 21000
    }
])

const selectedCountry = ref('Франция')

const filteredCards = computed(() =>{
    if (!selectedCountry.value) return cards.value;
    return cards.value.filter(
        item => item.country === selectedCountry.value
    )
})

function filterByCountry(country) {
    selectedCountry.value = country
}
</script>

<template>
    <section class="reproductions">
        <div class="reproductions__items">
            <h3 class="reprod-items__title">Репродукции</h3>
            <div class="reprod-items__buttons">
                <button class="reprod-buttons__button" @click="filterByCountry('Франция')">Франция</button>
                <button class="reprod-buttons__button" @click="filterByCountry('Германия')">Германия</button>
                <button class="reprod-buttons__button" @click="filterByCountry('Англия')">Англия</button>
            </div>
        </div>

        <div class="reprod-container__cards">
            <ReproductionsCard
                v-for="card in filteredCards" :key="card.id"
                :image ="card.image" 
                :autor ="card.autor" 
                :name ="card.name" 
                :description ="card.description" 
                :price ="card.price"                   
            />
        </div>

    </section>
</template>

<style scoped>
.reproductions{
    max-width: 90rem;
    width: 100%;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1.875rem;
}

.reproductions__items{
    max-width: 69.375rem;
    width: 100%;
    display: flex;
    justify-content: space-between;
    gap: 26.6875rem;
}

.reprod-items__title{
    font-weight: 500;
    font-size: 2.5rem;
    line-height: 110%;
    color: #2C2D35;

}

.reprod-items__buttons{
    display: flex;
    gap: 1.875rem;
}

.reprod-buttons__button{
    font-weight: 500;
    font-size: 1.25rem;
    background-color: #D4E8D9;
    color: #2C2D35;
    border-radius: 1.25rem;
    padding: 0.625rem 1.25rem;
    border: none;
    cursor: pointer;
}

.reprod-buttons__button:hover{
    background-color: #376B44;
    color: #F4F6F5;
}

.reprod-container__cards{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(3, auto);
    gap: 1.875rem;
}
</style>