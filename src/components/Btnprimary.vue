<template>
    <button class="find-out" href="">{{ text }}</button>
</template>

<script setup lang="ts">
interface Props {
    text: string
}

const props = defineProps<Props>()
const { text } = props
</script>

<style>
.find-out {
    appearance: none;
    border: 0;
    padding: clamp(10px, 1.6vw, 14px) clamp(26px, 3.8vw, 42px);
    border-radius: 30px;
    background: linear-gradient(135deg, #0465B1 0%, #0A7AD8 100%);
    color: #fff;
    font-weight: 700;
    letter-spacing: 0.02rem;
    cursor: pointer;
    font-size: clamp(14px, 1.8vw, 16px);
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(4, 101, 177, 0.25);
}

.find-out:hover {
    background: linear-gradient(135deg, #035492 0%, #0866BF 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(4, 101, 177, 0.35);
}
</style>
