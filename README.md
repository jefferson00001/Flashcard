<!DOCTYPE html>
<html lang="pt-br">
                   <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="assets/style.css">
    <title>Flashcard</title>
                   </head>
        <body>
    <main>
<section id="container">
    <article class="cartao">
        <div class="cartao__conteudo">
            <h3>pokémon</h3>
            <div class="cartao__conteudo__pergunta">
            <P>o que são os pokémons?</P>
            </div>
            <div class="cartao__conteudo__resposta">
                <P>Concebido por Satoshi Tajiri no início de 1989, os Pokémon são criaturas que habitam o mundo fictício Pokémon. 
                Os projetos para a multiplicidade de espécies podem inspirar-se em qualquer coisa como animais, plantas, criaturas mitológicas e até objetos inanimados.
                </P>
            </div>
    <article class="cartao">
        <div class="cartao__conteudo">
            <h3>pokémon</h3>
            <div class="cartao__conteudo__pergunta">
            <P>como surgiu pokémons?</P>
            </div>
            <div class="cartao__conteudo__resposta">
                <p>A série dos “Monstros de Bolso” 
                    começou quando o criador de jogos 
                    e presidente da Game Freak, Satoshi Tajiri, 
                    teve uma ideia inspirada em suas experiências 
                    de captura de insetos na escola, quando ainda era criança.
                </P>
            </div>
        </div>
    </article>
</main>
</section>
    <footer>
Projeto feito por um aluno do Alura sem fins lucrativos,apenas estudos
    </footer>
        </body>
</html>


        Assets/style.css

body{
    background-color: rgba(0, 0, 0, 0.781);
    color: aqua;
}

#container{
    display: flex;
}

.cartao {
        margin: 1rem 1rem;
        background-color: rgb(64, 0, 255);
        height: 20rem;
        flex-grow: 1;
        flex-basis: calc(33% -6rem);
    }
    
footer{
background-color: blueviolet;
color: black;
position: fixed;
bottom: 0;
width: 100%;
height: 2rem;
}
footer p{
    text-align: center;
    font-size: 0.60rex;
}
