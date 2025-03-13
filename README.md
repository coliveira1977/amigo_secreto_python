<h1 align="center"> Desafio Amigo Secreto - Alura - Lógica de Programação. </h1>

![Amigo Secreto!!!](https://github.com/coliveira1977/desafio_amigo_secreto/blob/mai/assets/amigo-secreto.png?raw=true)

[![Ver Página](https://img.shields.io/badge/Acessar%20Site-007EC6?style=for-the-badge&logo=googlechrome&logoColor=white)][https://coliveira1977.github.io/desafio_amigo_secreto/]

Realiza o sorteio de um nome através de uma lista de nomes coletada na página HTML.
Tem como obejtivo realizar o código em atendimento ao desafio de forma mais simples e limpa possível.


# :hammer: Funcionalidades do projeto

Adiciona "amigos" em um array, limpa o campo da página HTML:

    function adicionarAmigo() {
        let inputNome = document.getElementById("amigo").value.trim();
        let listaAmigos = document.getElementById("listaAmigos");
    
        if (inputNome === "") {
            alert("Por favor, insira um nome válido.");
    } else {
        nomes.push(inputNome);
        let novoItem = document.createElement("li");
        novoItem.textContent = inputNome;
        listaAmigos.appendChild(novoItem);
        document.getElementById("amigo").value = ""; // Limpar campo
        }
    }

Realiza o sorteio dentre os nomes contidos no array:

    function sortearAmigo() {
        let resultado = document.getElementById("resultado");
        resultado.innerHTML = ""; // Limpa a lista anterior
    
        if (nomes.length === 0) {
        alert("Nenhum nome disponível para o sorteio.");
    } else {
        let sorteado = nomes[Math.floor(Math.random() * nomes.length)];
        let itemResultado = document.createElement("li");
        itemResultado.textContent = `O amigo secreto sorteado foi: ${sorteado}`;
        resultado.appendChild(itemResultado);
        }
    }

Exibirá mensagem de "ERRO" caso a lista de nomes esteja vazia:

    if (nomes.length === 0) {
        alert("Nenhum nome disponível para o sorteio.");

Exibirá mensagem de "ERRO" caso o campo de nomes esteja vazio:

    if (inputNome === "") {
        alert("Por favor, insira um nome válido.");


# 📁 Acesso ao projeto

    https://github.com/coliveira1977/desafio_amigo_secreto.git


![HTML Badge](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS Badge](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript Badge](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

<p align="center">
<img loading="lazy" src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge"/>
</p>

## Autor

<img src="https://github.com/coliveira1977/desafio_amigo_secreto/blob/mai/assets/autor.jpg" width="100">

**[Christian Oliveira](https://github.com/coliveira1977)**  
📌 GitHub: [coliveira1977](https://github.com/coliveira1977)  
📧 E-mail: chr.oliveira@gmail.com

![GitHub Org's stars](https://img.shields.io/github/stars/coliveira1977?style=social)
