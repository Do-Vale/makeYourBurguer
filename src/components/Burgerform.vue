<template>

<div>

<p>componente de mensagem</p>

<div>
    <form id="burger-form">
        <div class="input-container">

            <!-- NOME CLIENTE -->

            <label for="nome">Nome do cliente:</label>
            <input type="text" id="nome" name="nome" v-model="nome" placeholder="Nome do cliente" />
        </div>

            <!-- Escolha do Pão -->
        <div class="input-container">
            <label for="pao">Escolha o pão:</label>
            <select name="pao" id="pao" v-model="pao">
            <option value="">Selecione o seu pão</option>
            <option value="frances">Pão Francês</option>   
            </select>
        </div>
            <!-- Escolha a carne -->
            <div class="input-container">
            <label for="carne">Escolha a carne:</label>
            <select name="carne" id="carne" v-model="pao">
            <option value="">Selecione a carne do pão</option>
            <option value="carnedesol">Carne de sol</option>   
            </select>
        </div>


            <!-- Escolha opcionais -->
        <div class="input-container">
            <label id="opcionais-title" for="opcionais">Selecione os opcionais:</label>
            <div id="opcionais-container" class="checkbox-container">
                <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                <span>Salame</span>
                <input type="checkbox" name="opcionais" v-model="opcionais" value="salada">
                <span>Salada</span>
                <input type="checkbox" name="opcionais" v-model="opcionais" value="ervilha">
                <span>Ervilha</span>
                <input type="checkbox" name="opcionais" v-model="opcionais" value="milhoverde">
                <span>Milho verde</span>
            </div>

          
            
        </div>
          <div class="input-container">
        <input type="submit" class="submit-btn" value="Criar meu burger">            

        </div>

    </form>

    

    



</div>


</div>
    
</template>

<script>

export default {
name: "BurgerForm"


}


</script>

<style scoped>
    #burger-form { 
        max-width:400px;
        margin: 0 auto;   
       }
    .input-container {
        display: flex;
        flex-direction: column;
        margin-bottom: 20px;
        
        

    }

    label {
        font-weight:bold;
        margin-bottom: 15px;
        
        color:#222;
        padding: 5px 10px;
        border-left: 4px solid #fcba03;
        

    }

    input, select {
        padding:5px 10px;
        width: 300px;

    }

    #opcionais-container {
        flex-direction: row;
        flex-wrap: wrap;
      /*   border: 1px solid #222; */
        width:75%;
       /*  justify-content:space-around;
 */
    }
    #opcionais-title{
        width:100%;
        

    }
    .checkbox-container {
        display: flex;
        align-items: flex-start ;
        width:50%;
            
    
    }

    .checkbox-container span,
    .checkbox-container input {
        width: auto;
        margin-left: 50px; 
 
        

        
    }

        .checkbox-container span {
            margin-left: 6px;
            font-weight: bold;
            
        }

    .submit-btn {
        background-color:#222;
        color:#fcba03;
        font-weight: bold;
        border: 2px solid #222;
        padding:10px;
        font-size:16px;
        margin: 0 auto;
        cursor: pointer;
        transition: .5s;
        margin:5px;
        
            }

    .submit-btn:hover { background-color: transparent;
    color: #222; }

</style>