<template>
    <div class="b-nav">
        <div class="b-nav__box">
            <a href class="b-nav__link">Home</a>
        </div>
        <div class="b-nav__box">
            <a href class="b-nav__link">About</a>
        </div>
        <div class="b-nav__box">
            <a href class="b-nav__link">Services</a>
        </div>
        <div class="b-nav__box">
            <a href class="b-nav__link">Blog</a>
        </div>
    </div>
</template>
<script></script>
<style lang="scss">
.b-nav {
    display: flex;
    position: relative;
    z-index: 1;

    &__link {
        text-decoration: none;
        color: black;
    }
    &__box:not(:last-child) {
        margin-right: 15px;
    }
    &__box:hover &__link {
        border-bottom: 1px solid black;
        padding-bottom: 5px;
    }
}
</style>