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
            <h3>programaçao</h3>
            <div class="cartao__conteudo__pergunta">
            <P>o que é java script?</P>
            </div>
            <div class="cartao__conteudo__resposta">
            <P>
            O Java Script é uma linguagem de programação.
            </P>
            </div>
            <article class="cartao">
            <div class="cartao__conteudo">
            <h3> Programação </h3>
            <div class="cartao__conteudo__pergunta">
            O que é CSS?
            </div>                        
            <div class="cartao__conteudo__resposta">
            O CSS é uma linguagem de estilização.
            </div>
            </div>
            </article>
            </main>
            </section>
            <footer>
            <p>Projeto desenvolvido pela Alura, sem fins lucrativos.</p>
            </footer>
            </body>

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
