<template>
    <div class="backdrop">
        <div class="modal" :class="{sale: theme =='sale'}">
            <h1>{{header}} </h1>
            <p>{{ text }}</p>
        </div>
    </div>
</template>

<script>
export default {
    props: ['header','text','theme']
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
    color: white;
    font-style: normal;
}
.modal.sale {
    background-color: rgb(201, 43, 43);
    color: white;
}

</style>