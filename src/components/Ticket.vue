<template>
    <div id="Ticket">
        <Filter />
        <Action />
        <Data />
        <Table />
    </div>
</template>

<script>
import Table from '@/components/Table.vue';
import Data from '@/components/Data.vue';
import Filter from '@/components/Filter.vue';
import Action from '@/components/Action.vue';

export default {
    name: 'Ticket',
    props: {},
    components: {
        Filter,
        Action,
        Table,
        Data
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
    grid-template-columns: 60px repeat(3, calc(33.33% - 20px));
    grid-template-rows: 10vh 30vh 60vh;
    grid-template-areas: 
    "action action action data"
    "filter filter filter data"
    "table  table  table  table";

    /* grid-template-columns: 3fr 2fr;
    grid-template-rows: 3fr 6fr;
    grid-template-areas: 
    "filter action"
    "ticket ticket"; */

    background-color: white;
    width: inherit;
    height: inherit;
}
#Action {
    grid-area: action;
    margin: 16px 8px 8px 6px;
}
#Data {
    grid-area: data;
    margin: 16px 16px 16px 8px;
}
#Filter {
    grid-area: filter;
    margin: 8px 8px 16px 6px;
}
#Table {
    grid-area: table;
    margin: 16px 16px 16px 6px;
}
</style>