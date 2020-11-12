<template>
    <div class="main">
        <div class="sidebar">
            <SidebarComponent/>
        </div>

        <div class="content-right">
            <div class="navbar">
                <NavbarComponent/>
            </div>
            <div class="pages">
                <slot name="slot-pages"></slot>
            </div>
        </div>
    </div>
</template>

<script>
import SidebarComponent from './components/Sidebar/SidebarComponent'
import NavbarComponent from './components/Navbar/NavbarComponent'

export default {
    name: 'DashboardComponent',
    components: {
        SidebarComponent,
        NavbarComponent
    }
}
</script>

<style scoped>
.main{
    display: flex;
    width: 100%;
    height: 100vh;
    background-color: whitesmoke;
}

.sidebar{
    width: 250px;
    height: 100vh;
    background-color: blueviolet;
}

.content-right{
     width: calc(100% - 250px);
    height: 100vh;
}

.navbar{
    width: 100%;
    padding: 1px;
    background-color: #9f7aea;
}

.pages{
    width: 100%;
    height: auto;
}
</style>