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
                <h3 class="cartao__tema">Pokémon</h3>
                <div class="cartao__conteudo">
                    <div class="cartao__conteudo__pergunta">
                        <p>Quem é o mascote da Pokemon chompany? ?</p>
                    </div>
                    <div class="cartao__conteudo__resposta">
                        <p>Pikachu é o mascote.</p>
                    </div>
                </div>
            </article>

            <article class="cartao">
                <h3 class="cartao__tema">Pokémon</h3>
                <div class="cartao__conteudo">
                    <div class="cartao__conteudo__pergunta">
                        <p>como surgiu?</p>
                    </div>
                    <div class="cartao__conteudo__resposta">
                        <p>O conceito do universo Pokémon foi inspirado no passatempo do diretor executivo Satoshi Tajiri de colecionar insetos quando era criança, Então como as crianças estavam prestando mais atencão aos videogames do que a brincar ao ar livre (Ou fazer isso) Ele decidiu fazer um videogame onde as crianças podiam fazer isso, ...</p> 
                    </div>
                </div>
            </article>

        </section>
    </main>

    <footer>
        <p>Projeto desenvolvido pela Alura, sem fins lucrativos</p>
    </footer>
</body>
</html>
        Assets/style.css

body{
    background-color: rgba(0, 0, 0, 0.781);
    color: aqua;
:root {More actions
    --card-front-color: #04;
    --card-back-color: #444;
    --card-title-color: gold;
    --text-color: white;
    --footer-color: black;
}

body {
    background-image: url('img/274c1dd4b2c16056c25c470070625835 (1).jpg');
    background-size: cover;
    background-position: center;
    font-family: Arial, Helvetica, sans-serif;
    color: var(--text-color);
    margin: 0;
    padding: 0;
}

/* Container principal dos cartões */
#container {
    display: flex;
    perspective: 1000px;
    padding: 2rem;
    gap: 2rem;
    justify-content: center;
    flex-wrap: wrap;
}

/* Cada cartão individual */
.cartao {
    background-color: transparent;
    width: 300px;
    height: 320px;
    position: relative;
}

/* Título fixo (tema do cartão) */
.cartao__tema {
    background-color: var(--card-title-color);
    color: black;
    text-align: left;
    padding: 8px;
    position: absolute;
    top: 0.6rem;
    left: 0.6rem;
    border-radius: 0.6rem;
    font-size: 1rem;
    margin: 0;
    z-index: 2;
    width: calc(100% - 1.2rem);
    box-sizing: border-box;
}

/* Parte que gira */
.cartao__conteudo {
    background-color: var(--card-front-color);
    text-align: center;
    height: 100%;
    width: 100%;
    transform-style: preserve-3d;
    transition: transform 0.6s;
    position: relative;
    border-radius: 10px;
}

/* Aplica a rotação ao passar o mouse */
.cartao:hover .cartao__conteudo {
    transform: rotateY(180deg);
}

/* Faces frontal e traseira */
.cartao__conteudo__pergunta,
.cartao__conteudo__resposta {
    backface-visibility: hidden;
    position: absolute;
    height: 100%;
    width: 100%;
    padding: 1rem;
    box-sizing: border-box;
    border-radius: 10px;
}

/* Frente */
.cartao__conteudo__pergunta {
    background-color: var(--card-front-color);
    color: var(--text-color);
}

/* Verso */
.cartao__conteudo__resposta {
    background-color: var(--card-back-color);
    color: var(--text-color);
    transform: rotateY(180deg);
}

/* Texto das perguntas/respostas */
.cartao__conteudo p {
    margin-top: 4rem;
    padding: 1rem;
}

/* Rodapé fixo */
footer {
    background-color: var(--footer-color);
    color: var(--text-color);
    bottom: 0;
    position: fixed;
    width: 100%;
    height: 2rem;
}

footer p {
    text-align: center;
    font-size: 0.6rem;
    margin-top: 0.5rem;
    font-family: Arial, Helvetica, sans-serif;
}
