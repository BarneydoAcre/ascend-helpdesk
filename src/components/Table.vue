<template>
    <div id="Table">
        <table id="Table_t">
            <thead id="Table_header">
                <tr id="Table_header_row">
                    <th id="Table_header_id">id</th>
                    <th id="Table_header_assunto">Assunto</th>
                    <th id="Table_header_status">Status</th>
                    <th id="Table_header_tempo">Tempo</th>
                </tr>
            </thead>
            <tbody id="Table_header">
                <tr id="Table_data_row">
                    <td id="Table_data_id">#00001</td>
                    <td id="Table_data_assunto">Ajuda com emissão de nota fiscal</td>
                    <td id="Table_data_status">Em Atendimento</td>
                    <td id="Table_data_tempo">1 hora e 30 minutos</td>
                </tr>
                <tr id="Table_row">
                    <td id="Table_data_id">#00002</td>
                    <td id="Table_data_assunto">Problema com impressora</td>
                    <td id="Table_data_status">Finalizado</td>
                    <td id="Table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Table_row">
                    <td id="Table_data_id">#00002</td>
                    <td id="Table_data_assunto">Problema com impressora</td>
                    <td id="Table_data_status">Finalizado</td>
                    <td id="Table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Table_row">
                    <td id="Table_data_id">#00002</td>
                    <td id="Table_data_assunto">Problema com impressora</td>
                    <td id="Table_data_status">Finalizado</td>
                    <td id="Table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Table_row">
                    <td id="Table_data_id">#00002</td>
                    <td id="Table_data_assunto">Problema com impressora</td>
                    <td id="Table_data_status">Finalizado</td>
                    <td id="Table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Table_row">
                    <td id="Table_data_id">#00002</td>
                    <td id="Table_data_assunto">Problema com impressora</td>
                    <td id="Table_data_status">Finalizado</td>
                    <td id="Table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Table_row">
                    <td id="Table_data_id">#00002</td>
                    <td id="Table_data_assunto">Problema com impressora</td>
                    <td id="Table_data_status">Finalizado</td>
                    <td id="Table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Table_row">
                    <td id="Table_data_id">#00002</td>
                    <td id="Table_data_assunto">Problema com impressora</td>
                    <td id="Table_data_status">Finalizado</td>
                    <td id="Table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Table_row">
                    <td id="Table_data_id">#00002</td>
                    <td id="Table_data_assunto">Problema com impressora</td>
                    <td id="Table_data_status">Finalizado</td>
                    <td id="Table_data_tempo">27 minutos</td>
                </tr>
            </tbody>
        </table>
        </div>
</template>

<script>
export default {
    name: 'Table',
}
</script>

<style scoped>
#Table {
    background-color: rgb(216,216,216);
    border-radius: 5px 5px 5px 5px;
    overflow-y: scroll;
}
#Table_t {
}

th, td {
    border-collapse: collapse;
    border: 1px solid rgb(216,216,216);
    
}
#Table thead th{
    background-color: rgb(146, 146, 146);
    border-radius: 5px 5px 5px 5px;
    position: sticky;
    top: 0;
}
#Table tbody td{
    background-color: rgb(191, 191, 191);
    border-radius: 5px 5px 5px 5px;
}
#Table thead th,
#Table tbody td {
    padding: 10px;
    text-align: center;
    height: 40px;
}
#Table_header_id,
#Table_data_id {
    width: 10%;
    text-align: center;
}
#Table_header_assunto,
#Table_data_assunto {
    width: 60%;
    text-align: center;
}
#Table_header_status,
#Table_data_status {
    width: 20%;
    text-align: center;
}
#Table_header_tempo,
#Table_data_tempo {
    width: 10%;
    text-align: center;
}
</style>