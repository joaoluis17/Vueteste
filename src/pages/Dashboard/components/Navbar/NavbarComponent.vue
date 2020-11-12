<template>
    <div class="navbar">
        <h3 class="logo">Logo</h3>
        <a href="" class="logout">Sair</a>
    </div>
</template>

<script>
export default {
    name: 'NavbarComponent',
    
}
</script>

<style scoped>

.logo {
    color: darkmagenta;
    font-style: italic;	
}

.logout {
    color: darkred;
    position:absolute; 
    top:10%;
    left:95%;
    transform: translate(-50%, -50%);
}
</style>