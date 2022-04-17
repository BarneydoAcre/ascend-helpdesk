<template>
    <div id="SideBar" @mouseover="mouse_over" @mouseout="mouse_out">
        <div id="SideBar_logo" :style="{'background-image': 'url('+logo+')'}"></div>
        <form id="SideBar_search">
            <div>
                <input type="text" id="SideBar_search_text" @keyup="search($event)">
                <div type="submit" id="SideBar_search_send"><i class="material-icons-outlined">search</i></div>
            </div>
            <table id="SideBar_search_result">
                <ul>
                    <li>{{ search_text }}</li>
                    <li></li>
                </ul>
            </table>
        </form>
        <div id="SideBar_menu">
            <ul>
                <li><button class="btn waves-effect waves-light"><span class="material-icons-outlined">person</span>Perfil</button></li>
                <li><button class="btn waves-effect waves-light"><span class="material-icons-outlined">settings</span>Configurações</button></li>
                <li><button class="btn waves-effect waves-light"><span class="material-icons-outlined">help_outline</span>Ajuda</button></li>
            </ul>
        </div>
        <div id="SideBar_version">v1.00.001</div>
    </div>
</template>

<script>
export default {
    name: 'SideBar',
    data () {
        return {
            logo: null,
            logo_min: require("@/static/logo.png"),
            logo_max: require("@/static/logo_ext.png"),
            search_text: null,
        }
    },
    props: {
    },
    mounted () {
        this.logo = this.logo_min
    },
    methods: {
        search (e) {
            console.log(event.target.value)
            this.search_text = self.SideBar_search_text.value
        },
        mouse_over () {
            this.logo = this.logo_max
            console.log('test')
        },
        mouse_out () {
            this.logo = this.logo_min
        }
    }
}
</script>

<style scoped>
#SideBar {
    position: absolute;
    left: 0;
    width: 50px;
    height: 100vh;
    padding: 8px;
    background-color: #222;
    transition: .3s ease-in-out;
    z-index: 1000;

    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
}
#SideBar:hover {
    width: 250px;
}

/************************************************/

#SideBar_logo {
    background-position: center;
    background-size: cover;
    width: 50px;
    height: 100px;
    margin-bottom: 25px;
    transition: .3s ease-in-out;

    /* object-position: center;
    object-fit: cover; */
}
#SideBar:hover #SideBar_logo  {
    transition: .3s ease-in-out;
    width: 200px;
}

/************************************************/

#SideBar_search {
    position: relative;
    width: 50px;
    height: 100%;
    transition: .3s ease-in-out;

    display: flex;
    flex-direction: column;
    justify-content: flex-start;
}
#SideBar:hover #SideBar_search  {
    transition: .3s ease-in-out;
    width: 200px;
    border-radius: 8px;
}
#SideBar_search_text {
    width: 50px;
    height: 30px !important;
    color: #444;
    background-color: #444 !important;
    text-align: center;
    transition: .3s ease-in-out;
}
#SideBar:hover #SideBar_search_text  {
    width: 200px;
    color: #cacaca;
    transition: .3s ease-in-out;
}
/* #SideBar:not(:hover) #SideBar_search_text {
} */
#SideBar_search_text:focus {
    border-bottom: 1px solid #cacaca !important;
    box-shadow: 0 1px 0 #cacaca !important;
}
#SideBar_search_send{
    position: absolute;
    top: 0;
    left: 0;
    width: 50px;
    height: 30px;
    color: #cacaca;
    background-color: rgb(0, 0, 0, 0);
    border: 0;

    display: flex;
    justify-content: center;
    align-items: center;
}
#SideBar_search_result {
    color: #cacacaca;
}

/************************************************/

#SideBar ul {
    padding-inline-start: 0;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
#SideBar ul li .btn {
    width: 50px;
    margin: 2px;
    background-color: #777;

    display: flex;
    align-items: center;
}
#SideBar ul li .btn:hover {
    background-color: #888;
}
#SideBar ul li .btn .material-icons-outlined {
    margin-right: 12px;
}
#SideBar:hover ul li .btn  {
    transition: .3s ease-in-out;
    width: 200px;
}
#SideBar:not(:hover) ul li .btn  {
    transition: .3s ease-in-out;
    width: 50px;
}

/************************************************/

#SideBar_version {
    color: #999;
    font-size: 10px;
}
</style>