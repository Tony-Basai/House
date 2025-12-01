<script setup>
</script>

<template>
    <section class="team">
        <div class="team__container">
            <img class="team-container__img" src="../assets/Group.svg" alt="">
            <div class="team-container__info">
                <h3 class="container-info__title">
                    Наша команда
                </h3>
                <p class="container-info__description">
                    Значимость этих проблем настолько очевидна, что базовый вектор развития позволяет оценить значение экспериментов, поражающих по своей масштабности и грандиозности. Мы вынуждены отталкиваться от того, что консультация с широким активом.
                </p>
                <div class="container-info__person">
                    <img class="info-person__img" src="../assets/Ellipse1.svg" alt="">
                    <img class="info-person__img" src="../assets/Ellipse2.svg" alt="">
                    <img class="info-person__img" src="../assets/Ellipse3.svg" alt="">
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.team{
    max-width: 90rem;
    width: 100%;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    padding-bottom: 4.375rem;
}

.team__container{
    max-width: 69.375rem;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 1.875rem;
}

.team-container__info{
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
}

.container-info__title{
    font-weight: 500;
    font-size: 2.5rem;
    line-height: 110%;
    color: #2C2D35;
}

.container-info__description{
    font-weight: 500;
    font-size: 1.125rem;
    line-height: 150%;
    color: #2C2D35;
}

.container-info__person{
    display: flex;
    gap: 1.875rem;
}
</style>