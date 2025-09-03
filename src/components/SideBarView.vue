<script setup lang="ts"></script>

<!-- //////////////////////////////////////////////////////////////////////// -->

<template>
    <ul>
        <li>
            <router-link to="/">Inicio </router-link>
        </li>
        <li>
            <router-link to="/about">About </router-link>
        </li>
    </ul>

    <div class="row" id="main">
        <div class="col">
            <h6>Hola, soy un sidebar</h6>
        </div>
    </div>
</template>

<!-- //////////////////////////////////////////////////////////////////////// -->

<style lang="css">
    #main{
        background-color: antiquewhite;
        height: 100vh;
    }
</style>
