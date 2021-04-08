<template>
<div>
  <div class="cabecalho">
        <div class="logo">
            <h1>
                <img src="src/logo_an 1.png" alt="Analytics">
            </h1>
        </div>
        <div class="busca">
            <input type="text" placeholder="Buscar Funcionalidade">
        </div>
        <div class="perfil">
            <img src="src/Rectangle.svg" alt="retangulo" id="ret">
        </div>
        <div>
            Super Admin
            <br>
            SUPER ADMIN
        </div>
    </div>
    <div class="titulo">
        <div class="title">
            Usuários com acesso a plataforma
        </div>
        <div class="botao">
            <button type="is-success">Novo usuário</button>
        </div>
    </div>
    <div class="menu">
        <div class="menu-item">
            <img src="src/dash.svg" alt="Analitcs">
            Dashboard
        </div>
        <div class="menu-item">
            <img src="src/grupos.svg" alt="Analitcs">
            Grupos
        </div>
        <div class="menu-item">
            <img src="src/users.svg" alt="Analitcs">
            Usuários
        </div>
        <div class="menu-item">
            <img src="src/sistemas.png" alt="Analitcs">
            Sistemas
        </div>
        <div class="menu-item">
            <img src="src/categ.svg" alt="Analitcs">
            Categorias
        </div>

    </div>
   </div>

</template>

<script>
export default {
  name: "Usuários",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
template
{
    background-color: #090A0A;
}

.cabecalho{
    display: flex;
    align-items: flex-start;

}

.cabecalho input[type=text]{

    padding: 6px;
    border: none;
    margin-top: 30px;
    margin-right: 10cm;
    font-size: 17px;
    background-color: #313131;
    border-radius: 5px;
}

.perfil {
    margin-left: 460px;
    margin-right: 10px;
}

.menu-item{
    justify-content: left;
    align-items:center;
    margin-bottom: 10px;
    margin-left: 10px;
}

.titulo{
    display: flex;
}

.title{
    font-family: Rubik;
    font-size: 28px;
    font-style: normal;
    font-weight: 500;
    line-height: 40px;
    letter-spacing: 0px;
    text-align: left;
    text-emphasis-color: #9EA7AC;

    margin-left: 210px;
}

.botao button{
    background-color: lightgreen;
    margin-left: 700px;
    border-radius: 5px;
}
</style>
