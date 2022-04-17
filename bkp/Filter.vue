
<template>
    <div id="Filter">
        <form id="Filter_options">
            <div id="Filter_options_cliente" class="input-field">
                <label for="Filter_options_cliente_input">Cliente</label>
                <input type="text" name="cliente" id="Filter_options_cliente_input">
            </div>
            <select name="analists" id="Filter_options_status">
                <option value="Luan Gabriel">Luan Gabriel</option>
                <option value="Lucas Sarri">Lucas Sarri</option>
            </select>
            <select name="analists" id="Filter_options_prioridade">
                <option value="Luan Gabriel">Luan Gabriel</option>
                <option value="Lucas Sarri">Lucas Sarri</option>
            </select>
            <select name="analists" id="Filter_options_select Filter_select_analist">
                <option value="Luan Gabriel">Luan Gabriel</option>
                <option value="Lucas Sarri">Lucas Sarri</option>
            </select>
            <select name="analists" id="Filter_options_select Filter_select_analist">
                <option value="Luan Gabriel">Luan Gabriel</option>
                <option value="Lucas Sarri">Lucas Sarri</option>
            </select>
            <select name="analists" id="Filter_options_select Filter_select_analist">
                <option value="Luan Gabriel">Luan Gabriel</option>
                <option value="Lucas Sarri">Lucas Sarri</option>
            </select>
        </form>
    </div>
</template>

<script>
export default {
    name: 'Filter',
    props: {},
    data () {
        return {

        }
    }
}
</script>

<style scoped>
#Filter {
    grid-area: filter;
    
    background-color: rgb(214, 214, 214);
    margin: 16px 16px 16px 32px;
    border-radius: 4px;
    height: inherit;
}
#Filter_options {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    align-content: center;

    width: 100%;
    height: 100%;
}
#Filter_options_cliente {
    grid-area: dl;
    margin-top: unset;
    margin-bottom: unset;
    margin: 4px;
}
#Filter_options_cliente label:not(.label-icon).active {
    transform: translateY(-4px) scale(0.8);
}
#Filter_options_cliente_input {
    height: 30px;
    font-size: 12px;
}
#Filter_options_status {
}
#Filter select {
    display: block;
    width: 100px;
    height: 30px;
    margin: 4px;
    background-color: white;
}
</style>