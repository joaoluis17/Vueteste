<template>
    <div class="ay-card">
        <div class="top">
            <h3>{{ type }}</h3>
        </div>

        <div class="footer">
            <p class="number">{{ number }}</p>
        </div>
        
        
    </div>
</template>

<script>
export default {
    name: 'CardsComponent',
    props: {
        type: String,
        number: String,
    }
}
</script>

<style scoped>
.ay-card {
    display: flex;
    flex-direction: column;
    width: 300px;
    background-color: blueviolet;
    border-style: solid;
    border-color: darkmagenta;
    border-radius: 8px;
    height: 14rem;	
}

h3 {
    margin-left: 2%;
    margin-bottom: 0;
    font-style: italic;
    font-weight: 500;
    color: #68d391; 
}

p {
    margin-left: 10%;
    font-size: 1.5rem;
    font-weight: 400;
    color: #faf089;	 
}
</style>