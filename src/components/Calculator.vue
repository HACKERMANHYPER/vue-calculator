<template>
    <div class="calculator">
        <div class="display">0</div>
        <div>CE</div>
        <div>C</div>
        <div><BackIcon /></div>
        <div>/</div>
        <div>7</div>
        <div>8</div>
        <div>9</div>
        <div>*</div>
        <div>4</div>
        <div>5</div>
        <div>6</div>
        <div>-</div>
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>+</div>
        <div>0</div>
        <div>.</div>
        <div class="equal">=</div>
    </div>
</template>

<script setup>
import BackIcon from './BackIcon.vue';
</script>

<style>
:root {
    --grey: #212832;
    --orange: #fb7845;
}

.calculator {
    display: grid;
    grid-template-columns: repeat(4, 5rem);
    justify-content: center;
    row-gap: 10px;
    column-gap: 10px;
    text-align: center;
    background-color: black;
    padding: 2rem;
}
.calculator .display {
    grid-column: 1 / 5;
    grid-row: 1;
    text-align: right;
    font-size: 2rem;
    font-weight: 500;
}
.calculator .equal {
    grid-column: 3 / 5;
    grid-row: 6;
    background-color: var(--orange);
    font-weight: 800;
}
.calculator div {
    background-color: var(--grey);
    border-radius: 2px;
    padding: 15px;
    font-weight: 500;
}
</style>
