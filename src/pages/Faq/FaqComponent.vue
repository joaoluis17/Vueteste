<template>
    <DashboardComponent>
        <div slot="slot-pages" class="content-pages">
            <header class="title-pages">
                <p>Perguntas Frequentes</p>
            </header>

           

        </div> 
    </DashboardComponent>
</template>

<script>
import DashboardComponent from '../Dashboard/DashboardComponent';


export default {
    name: 'Faq',

    components: {
        DashboardComponent,
    }  
}
</script>

<style scoped>
.content-pages {
    padding: 15px;
}

.title-pages {
    font-size: 24px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #68d391; 
    font-weight: 700;
    font-style: italic;
}

</style>