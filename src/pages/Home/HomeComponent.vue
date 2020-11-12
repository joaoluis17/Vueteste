<template>
    <DashboardComponent>
        <div slot="slot-pages" class="content-pages">
            <header class="title-pages">
                <p>Início</p>
            </header>

            <div class="rows">
                <div class="row">
                    <div class="col-12 col-end-3"   
                        <CardsComponent :type="'Clientes'" :number="'1046'"/>
                    </div>
                
                <div class="row">
                    <div class="col-12 col-end-3"   
                        <CardsComponent :type="'Crescimento de Clientes'" :number="'10% a cada dia'"/>
                    </div>
                </div>
            </div>
        </div> 
    </DashboardComponent>
</template>

<script>
import DashboardComponent from '../Dashboard/DashboardComponent';
import CardsComponent from '../Dashboard/components/Cards/CardsComponents';

export default {
    name: 'Home',

    components: {
        DashboardComponent,
        CardsComponent
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

.rows {
    display: flex;
}
</style>