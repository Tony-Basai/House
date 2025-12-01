<script setup>
</script>

<template>
    <section class="new-collection">
        <div class="new-collection__container">
            <div class="collection-cont__header">
                <img class="cont-header__img" src="../assets/ImageStar.svg" alt="">
                <h3 class="cont-header__title">
                    Новая коллекция французских авторов
                </h3>
            </div>
            <p class="collection-cont__info">
                Сложно сказать, почему акционеры крупнейших компаний призывают нас к новым свершениям, которые, в свою очередь, должны быть заблокированы в рамках своих собственных рациональных ограничений.
                <br>
                <br>Принимая во внимание показатели успешности, граница обучения кадров предопределяет высокую востребованность направлений прогрессивного развития.
            </p>
            <button class="collection-cont__button">
                Ознакомиться
            </button>
        </div>
    </section>
</template>

<style scoped>
.new-collection {
    position: relative;
    max-width: 90rem;
    width: 100%;
    height: 35.875rem;
    background-image: url('@/assets/NewCollection.svg');
    background-size: cover;
    background-position: center;
    overflow: hidden;
    box-shadow: 100px 100px 100px 66px rgba(21, 22, 22, 0.65) inset;
}

.new-collection__container {
    max-width: 33rem;
    width: 100%;
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
    position: absolute;
    top: 4.375rem;
    left: 8rem;
}

.collection-cont__header{
    display: flex;
    align-items: center;
    gap: 1.25rem;
}

.cont-header__title{
    font-weight: 500;
    font-size: 2.5rem;
    color: #F4F6F5;
}

.collection-cont__info{
    font-weight: 500;
    font-size: 1.125rem;
    line-height: 150%;
    color: #FFFFFF;
}

.collection-cont__button{
    max-width: 14rem;
    width: 100%;
    font-weight: 500;
    font-size: 1.25rem;
    padding: 1.3125rem 0;
    margin-top: 2.5rem;
    color: #2C2D35;
    background: #EEDB6D;
    border: none;
    cursor: pointer;
}

.collection-cont__button:hover{
    background: #FAEB97;
}
</style>