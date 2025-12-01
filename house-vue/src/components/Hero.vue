<script setup>
</script>

<template>
    <search class="hero">
        <div class="hero__container">
            <img class="hero__img" src="../assets/ImageHero.svg" alt="">
            <div class="hero__info">
                <h1 class="hero-info__title">
                    Реплики картин от <span class="hero-title__span">Ink. House</span>
                </h1>
                <p class="hero-info__description">
                    Высокое качество отрисовки на плотной бумаге или льняном холсте. Редкие произведения, доступные цены.
                </p>
                <button class="hero-info__button">Продукция</button>
            </div>
        </div>
    </search>
</template>

<style scoped>
.hero{
    max-width: 90rem;
    width: 100%;
    margin: 0 auto;
}

@media (max-width: 768px) {
    .hero{
        max-width: 25rem;
        width: 100%; 
    }

    .hero__container{
        display: flex;
        align-items: center;
    }

    .hero__img{
        max-width: 5rem;
        width: 100%;
    }

    .hero__info{
        max-width: 10rem;
        width: 100%;
    }

    .hero-info__title{
        font-size: 1rem;
    }

    .hero-info__description{
        max-width: 10rem;
        width: 100%;
    }

    .hero-info__button{
        max-width: 10rem;
        width: 100%;
    }
}

.hero__container{
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1.875rem;
}

.hero__img{
    max-width: 33.75rem;
    width: 100%;
}

.hero__info{
    max-width: 30rem;
    width: 100%;
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
}

.hero-info__title{
    font-weight: 500;
    font-size: 3.75rem;
    line-height: 110%;
    color: #2C2D35;
}

.hero-title__span{
    color: #598D66;
}

.hero-info__description{
    max-width: 33.75rem;
    width: 100%;
    font-weight: 500;
    font-size: 1rem;
    line-height: 150%;
    color: #86928B;
}

.hero-info__button{
    max-width: 14rem;
    width: 100%;
    font-weight: 500;
    font-size: 1.25rem;
    padding: 1.3125rem 0;
    margin-top: 2.5rem;
    color: #598D66;
    border: 0.0625rem solid #598D66;
    background: none;
    cursor: pointer;
}

.hero-info__button:hover{
    background-color: #598D66;
    color: #E1EDE6;
}
</style>