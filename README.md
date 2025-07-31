# Jogo do Número Secreto 🔮

![Status do Projeto](https://img.shields.io/badge/status-concluído-brightgreen)

Um divertido e interativo jogo de "Adivinhe o Número" desenvolvido com JavaScript puro, HTML5 e CSS3. O projeto foi criado como uma excelente forma de praticar lógica de programação, manipulação do DOM e a utilização de funções em JavaScript.

## 📝 Descrição do Projeto

O objetivo do jogador é adivinhar um número secreto sorteado entre 1 e 10. A cada tentativa, o sistema fornece dicas, informando se o número secreto é maior ou menor que o palpite. O jogo termina quando o jogador acerta o número, exibindo o total de tentativas utilizadas.

## ✨ Funcionalidades

-   **Lógica de Jogo Completa:** Gerencia o número secreto, os palpites e o contador de tentativas.
-   **Interatividade com o DOM:** Atualiza o conteúdo da página dinamicamente para exibir dicas, mensagens de vitória e o número de tentativas, tudo sem recarregar a página.
-   **Geração Inteligente de Números:** Impede que números já sorteados em partidas anteriores (dentro da mesma sessão) sejam sorteados novamente, até que todas as possibilidades se esgotem.
-   **Feedback por Voz:** Utiliza a biblioteca `ResponsiveVoice.js` para ler as mensagens e dicas em voz alta (em português), tornando a experiência mais acessível e envolvente.
-   **Reiniciar o Jogo:** Permite que o jogador inicie uma nova partida facilmente após vencer.

## 🛠️ Tecnologias Utilizadas

-   **HTML5:** Para a estrutura semântica da página.
-   **CSS3:** Para a estilização e o layout do jogo.
-   **JavaScript:** Para toda a lógica do jogo, manipulação de eventos e do DOM.
-   **[ResponsiveVoice.js](https://responsivevoice.org/):** Biblioteca externa para a funcionalidade de Text-to-Speech.

## 🚀 Como Executar o Projeto

Para executar o projeto em sua máquina local, siga estes passos simples:

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
    ```

2.  **Crie a estrutura de arquivos:**
    Certifique-se de que você tem os três arquivos principais na mesma pasta:
    ```
    /
    ├── index.html
    ├── style.css
    └── app.js
    ```

3.  **Configure o `index.html`:**
    Este é um exemplo básico da estrutura HTML necessária. O mais importante é incluir o script da `ResponsiveVoice` **antes** do seu `app.js`.

    ```html
    <!DOCTYPE html>
    <html lang="pt-br">
    
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <script src="https://code.responsivevoice.org/responsivevoice.js"></script>
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Chakra+Petch:wght@700&family=Inter:wght@400;700&display=swap"
            rel="stylesheet">
        <link rel="stylesheet" href="style.css">
        <title>JS Game</title>
    </head>
    
    <body>

    <div class="container">
        <div class="container__conteudo">
            <div class="container__informacoes">
                <div class="container__texto">
                    <h1></h1>
                    <p class="texto__paragrafo"></p>
                </div>
                <input type="number" min="1" max="10" class="container__input">
                <div class="chute container__botoes">
                    <button onclick="verificarChute()" class="container__botao">Chutar</button>
                    <button onclick="reiniciarJogo()" id="reiniciar" class="container__botao" disabled>Novo jogo</button>
                </div>
            </div>
            <img src="./img/ia.png" alt="Uma pessoa olhando para a esquerda" class="container__imagem-pessoa" />
        </div>
    </div>




    <script src="app.js" defer></script>
</body>

</html>
    ```

4.  **Abra no navegador:**
    Abra o arquivo `index.html` no seu navegador de preferência e comece a jogar!

## ✒️ Autor

Desenvolvido por **MHSilvaDev**.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mhsilvadev/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MHSilvaDev)

