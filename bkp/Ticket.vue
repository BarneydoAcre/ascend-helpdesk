<template>
    <div id="Ticket">
        <Filter />
        <Action />
        <!-- <table id="Ticket_table" class="striped">
            <tr id="Ticket_table_header_row">
                <th id="Ticket_table_header_id">id</th>
                <th id="Ticket_table_header_assunto">Assunto</th>
                <th id="Ticket_table_header_status">Status</th>
                <th id="Ticket_table_header_tempo">Tempo</th>
            </tr>
            <tr id="Ticket_table_row">
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
        </table> -->
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
#Ticket {
    background-color: rgb(216,216,216);
    margin: 16px 32px 32px 32px;
    border-radius: 5px;
    width: inherit;
    height: inherit;
}
#Ticket_table_header_id {
    text-align: center;
}
#Ticket_table_data_id {
    text-align: center;
}
#Ticket_table_header_status {
    text-align: center;
}
#Ticket_table_data_status {
    text-align: center;
}
#Ticket_table_header_tempo {
    text-align: center;
}
#Ticket_table_data_tempo {
    text-align: center;
}
</style>