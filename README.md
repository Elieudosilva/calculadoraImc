# ⚖️ IMCCalculator

Aplicativo Android nativo para cálculo do Índice de Massa Corporal (IMC), focado em auxiliar os usuários a monitorarem sua faixa de peso e saúde.

![Kotlin](https://img.shields.io/badge/Kotlin-B125EA?style=for-the-badge&logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)

## 📋 Sobre o projeto

O **IMCCalculator** é um aplicativo Android desenvolvido com foco em consolidar os fundamentos da programação Android nativa (XML + Kotlin). 

O app recebe o peso e a altura do usuário e, com base no cálculo matemático oficial do IMC (peso ÷ altura²), indica instantaneamente em qual categoria a pessoa se encontra (ex: Abaixo do peso, Peso normal, Sobrepeso, Obesidade).

Este projeto foi desenvolvido como resolução de um desafio prático proposto pela **Comunidade Nova Era**, buscando aplicar conceitos essenciais de UI, navegação e passagem de dados no Android.

## 📸 Screenshots

| Tela Inicial (Cálculo) | Tela de Resultado |
|:---:|:---:|
<!-- You can add more screenshots here if you like -->
<p align="center">
   <img src="https://github.com/user-attachments/assets/9131c8aa-837f-4e04-9fcc-08ac4dd8d4dd" alt="Screen_one" width="200"/>
   <img src="https://github.com/user-attachments/assets/3260df2d-e37a-43ed-a938-e7ac99523bd5" alt="Screen_two" width="200"/>
   </p>

   
## ✨ Funcionalidades

- **Cálculo de IMC:** processamento instantâneo do peso e altura para determinar o índice e a classificação corporal atual do usuário.
- **Navegação de telas:** transição fluida da tela de inserção de dados para a tela de resultado.
- **Interface clara:** design estruturado para facilitar o uso rápido, incluindo uma `Toolbar` personalizada e suporte visual com `ImageView`.

## 🏗️ Arquitetura e Tecnologias

O projeto foi construído utilizando a abordagem clássica de desenvolvimento Android:

| Tecnologia / Recurso | Aplicação no projeto |
|---|---|
| **Kotlin** | Linguagem principal, gerenciando a lógica de negócio e eventos de clique. |
| **ConstraintLayout (XML)** | Construção das telas garantindo responsividade e bom alinhamento dos elementos. |
| **Intents explícitas** | Responsáveis por gerenciar a navegação entre as `Activities`. |
| **PutExtra / Extras** | Passagem dos resultados dos cálculos e dados preenchidos entre as telas. |
| **FindViewById** | Conexão entre os elementos visuais do XML e o código Kotlin. |

## 🚧 Desafios técnicos e aprendizados

### 1. Comunicação entre telas
**Desafio:** transferir os dados digitados e o resultado do cálculo da primeira tela para a segunda sem perder informações.
**Solução:** utilização do objeto `Intent` aliado ao método `putExtra()`, permitindo enviar os dados encapsulados e recuperá-los no `onCreate` da Activity de destino usando `intent.extras`.
**Aprendizado:** compreender o ciclo de vida básico das Activities e como os pacotes de dados transitam entre elas.

### 2. Estruturação da Interface (ConstraintLayout)
**Desafio:** posicionar os campos de texto, botões e imagens de forma que a tela não "quebre" em dispositivos com tamanhos diferentes.
**Solução:** uso de amarrações (constraints) relativas entre os componentes no XML, garantindo que botões e textos respeitem as margens uns dos outros.
**Aprendizado:** o `ConstraintLayout` é uma ferramenta poderosa para criar interfaces complexas e responsivas sem a necessidade de aninhar múltiplos layouts.

### 3. Melhoria da Experiência do Usuário (UX)
**Desafio:** tornar o aplicativo mais amigável e com visual profissional.
**Solução:** adição de recursos visuais como `ImageView` para ilustrar o app.

## 💻 Como executar

### Pré-requisitos
- Android Studio;
- Emulador ou dispositivo Android físico.

### Passos para rodar
1. Faça o clone deste repositório:
   ```bash
   git clone git@github.com:Elieudosilva/calculadoraImc.git
   ```
### 👤 Autor e contato profissional

Desenvolvido por **Elieudo Silva** como projeto de portfólio em desenvolvimento Android.

- **LinkedIn:** https://www.linkedin.com/in/elieudo-silva-203838301
- **GitHub:** https://github.com/Elieudosilva

## License
```
The MIT License (MIT)

Copyright (c) 2024 Elieudo Silva

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```
