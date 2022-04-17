<template>
    <div id="Ticket">
        <Filter />
        <Action />
        <div id="Ticket_div">
        <table id="Ticket_table">
            <thead id="Ticket_table_header">
                <tr id="Ticket_table_header_row">
                    <th id="Ticket_table_header_id">id</th>
                    <th id="Ticket_table_header_assunto">Assunto</th>
                    <th id="Ticket_table_header_status">Status</th>
                    <th id="Ticket_table_header_tempo">Tempo</th>
                </tr>
            </thead>
            <tbody id="Ticket_table_header">
                <tr id="Ticket_table_data_row">
                    <td id="Ticket_table_data_id">#00001</td>
                    <td id="Ticket_table_data_assunto">Ajuda com emissão de nota fiscal</td>
                    <td id="Ticket_table_data_status">Em Atendimento</td>
                    <td id="Ticket_table_data_tempo">1 hora e 30 minutos</td>
                </tr>
                <tr id="Ticket_table_row">
                    <td id="Ticket_table_data_id">#00002</td>
                    <td id="Ticket_table_data_assunto">Problema com impressora</td>
                    <td id="Ticket_table_data_status">Finalizado</td>
                    <td id="Ticket_table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Ticket_table_row">
                    <td id="Ticket_table_data_id">#00002</td>
                    <td id="Ticket_table_data_assunto">Problema com impressora</td>
                    <td id="Ticket_table_data_status">Finalizado</td>
                    <td id="Ticket_table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Ticket_table_row">
                    <td id="Ticket_table_data_id">#00002</td>
                    <td id="Ticket_table_data_assunto">Problema com impressora</td>
                    <td id="Ticket_table_data_status">Finalizado</td>
                    <td id="Ticket_table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Ticket_table_row">
                    <td id="Ticket_table_data_id">#00002</td>
                    <td id="Ticket_table_data_assunto">Problema com impressora</td>
                    <td id="Ticket_table_data_status">Finalizado</td>
                    <td id="Ticket_table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Ticket_table_row">
                    <td id="Ticket_table_data_id">#00002</td>
                    <td id="Ticket_table_data_assunto">Problema com impressora</td>
                    <td id="Ticket_table_data_status">Finalizado</td>
                    <td id="Ticket_table_data_tempo">27 minutos</td>
                </tr>
                <!-- <tr id="Ticket_table_row">
                    <td id="Ticket_table_data_id">#00002</td>
                    <td id="Ticket_table_data_assunto">Problema com impressora</td>
                    <td id="Ticket_table_data_status">Finalizado</td>
                    <td id="Ticket_table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Ticket_table_row">
                    <td id="Ticket_table_data_id">#00002</td>
                    <td id="Ticket_table_data_assunto">Problema com impressora</td>
                    <td id="Ticket_table_data_status">Finalizado</td>
                    <td id="Ticket_table_data_tempo">27 minutos</td>
                </tr>
                <tr id="Ticket_table_row">
                    <td id="Ticket_table_data_id">#00002</td>
                    <td id="Ticket_table_data_assunto">Problema com impressora</td>
                    <td id="Ticket_table_data_status">Finalizado</td>
                    <td id="Ticket_table_data_tempo">27 minutos</td>
                </tr> -->
            </tbody>
        </table>
        </div>
    </div>
</template>

<script>
import Filter from '@/components/Filter.vue';
import Action from '@/components/Action.vue';

export default {
    name: 'Ticket',
    props: {},
    components: {
        Filter,
        Action,
    },
    data () {
        return {

        }
    }
}
</script>

<style scoped>
* {
}
#Ticket {
    display: grid;
    grid-template-columns: 3fr 2fr;
    grid-template-rows: 3fr 6fr;
    grid-template-areas: 
    "filter action"
    "ticket ticket";

    background-color: white;
    padding: 16px 32px 32px 32px;
    width: inherit;
    height: inherit;
}
#Action {
    grid-area: action;
    padding: 16px 0 32px 16px;
}
#Filter {
    grid-area: filter;
    padding: 16px 16px 32px 0;
}


#Ticket #Ticket_div {
    background-color: rgb(216,216,216);
    border-radius: 5px 5px 5px 5px;
    grid-area: ticket;
    overflow-y: scroll;
}

th, td {
    border-collapse: collapse;
    border: 1px solid rgb(216,216,216);
    
}
#Ticket_table thead th{
    background-color: rgb(146, 146, 146);
    border-radius: 5px 5px 5px 5px;
    position: sticky;
    top: 0;
}
#Ticket_table tbody td{
    background-color: rgb(191, 191, 191);
    border-radius: 5px 5px 5px 5px;
}
#Ticket_table,
#Ticket_table thead th,
#Ticket_table tbody td {
    padding: 10px;
    text-align: center;
    height: 40px;
}
#Ticket_table_header_id,
#Ticket_table_data_id {
    width: 10%;
    text-align: center;
}
#Ticket_table_header_assunto,
#Ticket_table_data_assunto {
    width: 60%;
    text-align: center;
}
#Ticket_table_header_status,
#Ticket_table_data_status {
    width: 20%;
    text-align: center;
}
#Ticket_table_header_tempo,
#Ticket_table_data_tempo {
    width: 10%;
    text-align: center;
}
</style>