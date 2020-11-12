<template>
    <div class="sidebar">
        <div class="top">
            <div class="avatar">
                <div class="info">
                    <p class="name">João Luis</p>
                    <span class="situation">Online</span>
                </div>
            </div>
        </div>
            
        <div class="menu">
            <ul>
                <li<router-link :to="{name: 'home'}">Início</router-link></li>
                <br>
                <li<router-link :to="{name: 'services'}">Serviços</router-link></li>
                <br>
                <li<router-link :to="{name: 'faq'}">Perguntas Frequentes</router-link></li>
                <li></li>
                <li></li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SidebarComponent',
    
}
</script>

<style scoped>
.sidebar {
}

.top {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 25px 5px;
    margin-top: 60px;
}

.avatar {
    margin-right: 16px;   
}

.info {
    padding-bottom: 0;
    align-items: center;
}

p {
    font-size: 1.5rem;
    color: #ed8936;
    font-weight: 700;	
    widows: 50px;
    height: 50px;
    border-radius: 50%;
    }

span {
    color: #9ae6b4;	
    font-style: italic;	
    margin-top: 0%;
    padding-top: 0%;
    widows: 50px;
    height: 50px;
    border-radius: 50%;
}

.menu {
    padding: 20px;
}

ul li  {
    text-align: left;
}
</style>