<template>
    <div class="backdrop">
        <div class="modal">
            <h1>Modal Title </h1>
            <p>This is my modal</p>
        </div>
    </div>
</template>

<script>
export default {
    props: ['header']
}
</script>

<style scoped>
.modal {
    width: 400px;
    padding: 20px;
    margin: 100px auto;
    background:white;
    border-radius: 10px;
}

.backdrop{
    top: 0;
    position: fixed;
    background: rgba(0, 0, 0, 0.575);
    width: 100%;
    height: 100%;
}

h1 {
    color: green;
    font-style: normal;
}
</style>