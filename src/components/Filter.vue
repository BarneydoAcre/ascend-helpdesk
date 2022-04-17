
<template>
    <div id="Filter">
        <form id="Filter_options">
            <div id="Filter_options_cliente" class="input-field">
                <h6 for="Filter_options_cliente_input">Cliente</h6>
                <input type="text" name="cliente" id="Filter_options_cliente_input" list="clientes" />
                <datalist id="clientes">
                    <option>Luan Gabriel</option>
                    <option>Lucas Sarri</option>
                    <option>William Ruiz</option>
                    <option>Gustavo Saratti</option>
                </datalist>
            </div>
            <div id="Filter_options_status" class="input-field">
                <h6>Status</h6>
                <input type="text" name="status" id="Filter_options_status_select" list="status" />
                <datalist id="status">
                    <option disabled selected>Status</option>
                    <option value="Em atendimento">Em atendimento</option>
                    <option value="Com terceiro">Com terceiro</option>
                    <option value="Com cliente">Com cliente</option>
                    <option value="Finalizado">Finalizado</option>
                </datalist>
            </div>
            <div id="Filter_options_prioridade" class="input-field">
                <h6>Prioridade</h6>
                <input type="text" name="prioridade" id="Filter_options_prioridade_select" list="prioridade" />
                <datalist id="prioridade">
                    <option disabled selected>prioridade</option>
                    <option value="Baixa">Baixa</option>
                    <option value="Media">Media</option>
                    <option value="Alta">Alta</option>
                    <option value="Urgente">Urgente</option>
                </datalist>
            </div>
            <div id="Filter_options_analista" class="input-field">
                <h6>Analista</h6>
                <input type="text" name="analista" id="Filter_options_analista_select" list="analista" />
                <datalist id="analista">
                    <option disabled selected>analista</option>
                    <option value="Luan">Luan</option>
                    <option value="Lucas">Lucas</option>
                </datalist>
            </div>
            <div id="Filter_options_data" class="input-field">
                <h6>De:</h6>
                <input name="data_inicial" type="date" id="Filter_options_data_input">
            </div>
            <div id="Filter_options_data" class="input-field">
                <h6>Até:</h6>
                <input name="data_final" type="date" id="Filter_options_data_input">
            </div>
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
    background-color: rgb(216,216,216);
    border-radius: 5px;
    margin: 16px 16px 16px 0;
}
#Filter_options {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    align-items: center;
    align-content: center;

    border-radius: 4px;
    width: 100%;
    height: 100%;
}
#Filter_options div {
    margin-left: 8px;
    margin-right: 8px;
}
#Filter_options div input {
    border: unset;
    border-bottom: 1px solid #999;
    width: 140px;
    height: 30px;
    background: rgb(255, 255, 255,0)
}
#Filter_options div input:focus-visible {
    outline: unset;
}
h6 {
    margin: unset;
    padding: unset;
    font-size: 10px;
    color: #9e9e9e;
    transform: translateY(4px);
}
</style>