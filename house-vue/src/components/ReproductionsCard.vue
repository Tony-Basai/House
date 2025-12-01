<script setup>
const props = defineProps({
    id: Number,
    image: String,
    autor: String,
    name: String,
    description: String,
    price: Number,
    country: String
})
</script>

<template>
                <div class="reprod-cards__card">
                    <img class="reprod-card__img" :src=" props.image " alt="">
                    <div class="reprod-card__info">
                        <h6 class="card-items__author">
                            {{ props.autor }}
                        </h6>
                        <h4 class="card-items__name">
                            {{ props.name }}
                        </h4>
                        <h6 class="card-items__description">
                            {{ props.description }}
                        </h6>
                    </div>
                    <div class="reprod-card__items-price">
                        <p class="reprod-card__price">
                            {{ props.price }} руб
                        </p>
                        <button class="reprod-card__button">
                            В корзину
                        </button>
                    </div>
                </div>
</template>

<style scoped>
.reprod-cards__card{
    max-width: 21.875rem;
    width: 100%;
    background-color: #E1EDE6;
    padding: 1.25rem;
}

.reprod-card__img{
    max-width: 19.375rem;
    width: 100%;
}

.reprod-card__info{
    display: flex;
    flex-direction: column;
    gap: 0.5625rem;
    margin-top: 1.25rem;
}

.card-items__author{
    font-weight: 500;
    font-size: 1.125rem;
    color: #86928B;
}

.card-items__name{
    font-weight: 500;
    font-size: 1.875rem;
    color: #2C2D35;
}

.card-items__description{
    font-weight: 500;
    font-size: 1.125rem;
    color: #2C2D35;
}

.reprod-card__items-price{
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
    margin-top: 1.875rem;
}

.reprod-card__price{
    font-weight: 500;
    font-size: 1.5rem;
    color: #598D66;
}

.reprod-card__button{
    font-weight: 500;
    font-size: 1.25rem;
    padding: 1.3125rem 0;
    color: #598D66;
    background: none;
    border: 0.0625rem solid #598D66;
    cursor: pointer;
}

.reprod-card__button:hover{
    background-color: #598D66;
    color: #E1EDE6;
}
</style>