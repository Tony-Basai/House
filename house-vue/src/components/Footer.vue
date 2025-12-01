<script setup>
</script>
 
<template>
    <footer class="footer">
        <div class="footer__container">
            <div class="footer-container__contact">
                <div class="contact__logo">
                    <img class="contact-logo__img" src="../assets/FooterStar.svg" alt="">
                    <h5 class="contact__logo__title">
                        Ink. House
                    </h5>
                </div>
                <div class="contact__items">
                    <p class="contact-items__numbers">
                        +7 (999) 543-54-54
                    </p>
                    <p class="contact-items__text">
                        Мастерская
                    </p>
                </div>
            </div>
            <div class="footer-container__boxes">
                <div class="container-boxes__about-us">
                    <div class="about-us__box">
                        <h5 class="about-us-box__title">Репродукции</h5>
                        <p class="about-us-box__item">Франция</p>
                        <p class="about-us-box__item">Германия</p>
                        <p class="about-us-box__item">Англия</p>
                    </div>
                    <div class="about-us__box">
                        <h5 class="about-us-box__title">Новинки</h5>
                        <p class="about-us-box__item">2021</p>
                        <p class="about-us-box__item">2020</p>
                    </div>
                    <div class="about-us__box">
                        <h5 class="about-us-box__title">О нас</h5>
                        <p class="about-us-box__item">Художники</p>
                        <p class="about-us-box__item">Менеджеры</p>
                    </div>
                </div>
                <div class="container-info__about-us">
                    <div class="about-us__social-media">
                        <button class="social-media__button"><img src="../assets/Facebook.svg" alt=""></button>
                        <button class="social-media__button"><img src="../assets/Instagram.svg" alt=""></button>
                        <button class="social-media__button"><img src="../assets/YouTube.svg" alt=""></button>
                    </div>
                    <p class="about-us__info">Ink. House ®</p>
                    <p class="about-us__info">All rights reserved</p>
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped>
.footer{
    max-width: 90rem;
    width: 100%;
    margin: 0 auto;
    padding: 1.4375rem 8rem;
    font-family: 'Raleway' sans-serif;
    background-color: #E1EDE6;
}

.footer__container{
    display: flex;
    justify-content: space-between;
}

.footer-container__contact{
    display: flex;
    flex-direction: column;
    gap: 2.1875rem;
}

.contact__logo{
    display: flex;
    gap: 0.5rem;
}

.contact-logo__img{
    max-width: 2.1575rem;
    width: 100%;
}

.contact__logo__title{
    font-weight: 700;
    font-size: 1.25rem;
    color: #598D66;
}

.contact__items{
    display: flex;
    flex-direction: column;
    grid-area: 0.5rem;
}

.contact-items__numbers{
    font-weight: 500;
    font-size: 1.25rem;
    color: #2C2D35;
}

.contact-items__text{
    font-weight: 500;
    font-size: 1.125rem;
    color: #86928B;
}

.footer-container__boxes{
    display: flex;
    gap: 15.5rem;
}

.container-boxes__about-us{
    display: flex;
    gap: 3.75rem;
}

.about-us__box{
    display: flex;
    flex-direction: column;
    gap: 0.375rem;
}

.about-us-box__title{
    font-weight: 500;
    font-size: 1.25rem;
    color: #2C2D35;
}

.about-us-box__item{
    font-weight: 500;
    font-size: 1.125rem;
    line-height: 150%;
    color: #86928B;
}

.container-info__about-us{
    display: flex;
    flex-direction: column;
    gap: 0.625rem;
}

.about-us__social-media{
    display: flex;
    gap: 1.875rem;
}

.social-media__button{
    background: none;
    border: none;
    cursor: pointer;
}

.about-us__info{
    font-weight: 500;
    font-size: 0.75rem;
    line-height: 120%;
    color: #86928B;
}
</style>