<template>
    <div id="Action">
        <button><b>+</b> Ticket</button>
        <button><b>+</b> Cliente</button>
        <button><b>+</b> Teste</button>
        <button>Aplicar Filtro</button>
    </div>
</template>

<script>
export default {
    name: 'Action',
    methods: {
    }
}
</script>

<style scoped>
#Action {
    background-color: rgb(216,216,216);
    border-radius: 5px;
    margin: 16px 16px 16px 0;

    display: flex;
    justify-content: space-evenly;
    align-items: center;
}
#Action button {
    width: 100px;
    height: 30px;
    border: unset
}
#Action button:hover {
    background-color: #666;
}
</style>