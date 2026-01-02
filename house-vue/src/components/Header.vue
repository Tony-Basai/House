<script setup>
</script>

<template>
    <nav class="nav">
        <a class="nav__logo" href="#hero">
            <img class="nav__logo-img" src="../assets/Star-logo.svg" alt="">
            <h5 class="nav__logo-title">Ink. House</h5>
        </a>
        <div class="nav__items">
            <ul class="nav__list">
                <li class="nav__list-item">
                    <a class="nav__list-item__link" href="#reproductions">Репродукции</a>
                </li>
                <li class="nav__list-item">
                    <a class="nav__list-item__link" href="#new-collection">Новинки</a>
                </li>
                <li class="nav__list-item">
                    <a class="nav__list-item__link" href="#team">О нас</a>
                </li>
            </ul>
            <button class="nav__button-basket"></button>
        </div>
    </nav>
</template>

<style scoped>
.nav{
    max-width: 90rem;
    width: 100%;
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    padding: 2.375rem 10.3125rem;
    font-family: 'Raleway' sans-serif;
    background-color: #E1EDE6;
}

@media (max-width: 768px) {
    .nav{
        max-width: 48rem;
        width: 100%;
        padding: 2.0625rem 2.4375rem;
    }

    .nav__items{
        display: flex;
        gap: 3rem;
    }

    .nav__list-item{
        font-size: 1.125rem;
    }
}

.nav__logo{
    display: flex;
    align-items: center;
    gap: 0.5rem;
    text-decoration: none;
}

.nav__logo-title{
    font-weight: 700;
    font-size: 1.25rem;
    color: #598D66;
}

.nav__items{
    display: flex;
    gap: 3.75rem;
}

.nav__list{
    display: flex;
    gap: 3.75rem;
    list-style: none;
}

.nav__list-item__link{
    font-weight: 500;
    font-size: 1.25rem;
    cursor: pointer;
    color: #2C2D35;
    text-decoration: none;
}

.nav__list-item__link:hover{
    color: #598D66;
}

.nav__button-basket {
  width: 1.5rem;
  height: 1.5rem;
  background-color: #000;
  -webkit-mask-image: url("../assets/cart.svg");
  -webkit-mask-repeat: no-repeat;
  -webkit-mask-position: center;
  -webkit-mask-size: contain;

  mask-image: url("../assets/cart.svg");
  mask-repeat: no-repeat;
  mask-position: center;
  mask-size: contain;

  transition: background-color 0.3s ease;
  cursor: pointer;
}

.nav__button-basket:hover {
  background-color: #598D66;
}
</style>