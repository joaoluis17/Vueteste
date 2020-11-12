<template>
    <DashboardComponent>
        <div slot="slot-pages" class="content-pages">
            <header class="title-pages">
                <p>Todos os Nossos Serviços</p>
            </header>
            
             <div class="content">   
                <table class="table-services">
                        <tr>
                            <th scope="col">#</th>
                            <th scope="col">1</th>
                            <th scope="col">2</th>
                            <th scope="col">3</th>
                        </tr>
                    <tbody class="row">
                        <tr>
                            <th scope="row">1</th>
                            <td>Ana</td>
                            <td>João</td>
                            <td>Rafael</td>
                        </tr>
                        <tr>
                            <th scope="row">2</th>
                            <td>Ana</td>
                            <td>João</td>
                            <td>Rafael</td>
                        </tr>
                        <tr>
                            <th scope="row">3</th>
                            <td>Ana</td>
                            <td>João</td>
                            <td>Rafael</td>
                        </tr>
                    </tbody>
                </table>
            </div>

        </div> 
    </DashboardComponent>
</template>

<script>
import DashboardComponent from '../Dashboard/DashboardComponent';


export default {
    name: 'Services',
    
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

.content {
    display: flex;
    align-items: center;
    justify-items: center;
}

.table-services {
    border-style: solid;
    border-radius: 9999px;	
    border-color: #9f7aea;
    box-sizing: border-box;	
    width: 20rem;
    display: flex;
    height: 12rem;
    justify-content: space-between;	
    justify-items: center;

}
</style>