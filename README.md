<h1 align="center">Olá 👋, Eu sou Marcelo Ferreira Lopez</h1>
<h3 align="center">Um desenvolvedor front-end</h3>

- 🔭 Eu estou trabalhando no projeto [Workshop](https://github.com/MarceloFLopez/formtosendemail)

- 💬 Pergunte-me sobre **Javascript, Html, CSS, Springboot**

- 📫 Contato **marceloferreiralope@gmail.com**

- ⚡ Fato engraçado **Gosto de programar, assistir filmes de ficção cientifica, jogar MTG.**

 # Formulário em Html para envio de email.

## Descrição

Este projeto é um formulário de inscrição para um workshop de marketing. Ele permite que os usuários se inscrevam fornecendo seu nome, email, local e uma mensagem opcional. O formulário envia os dados via EmailJS e inclui um contador de caracteres para o campo de mensagem.

## Tecnologias Utilizadas

- **HTML5**
- **CSS3**
- **JavaScript**
- **EmailJS**
- **Visual Studio Code (VS Code)**
- **Extensão Live Server Preview (VS Code)**

## Funcionalidades

- **Formulário de Inscrição**: Permite aos usuários inserir nome, email, local e uma mensagem opcional.
- **Envio de Email**: Usa EmailJS para enviar os dados do formulário diretamente para o seu email.
- **Contador de Caracteres**: Exibe um contador de caracteres em tempo real para o campo de mensagem, limitando a 255 caracteres.
- **Interface Responsiva**: Adaptada para funcionar bem em diferentes tamanhos de tela.

## Como Executar

1. **Clone o Repositório**:
    ```bash
    git clone https://github.com/seu-usuario/seu-repositorio.git
    cd seu-repositorio
    ```

2. **Abra no VS Code**:
    ```bash
    code .
    ```

3. **Inicie o Live Server**:
    - Certifique-se de ter a extensão [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) instalada no VS Code.
    - Clique com o botão direito no arquivo `index.html` e selecione **"Open with Live Server"**.

4. **Acesse no Navegador**:
    - O Live Server abrirá o projeto automaticamente no navegador, mas você também pode acessá-lo manualmente em `http://127.0.0.1:5500`.

## Estrutura de Pastas

```plaintext
/seu-projeto
|-- /css
|   |-- style.css
|-- /image
|   |-- github-logo.png
|   |-- people-removebg-preview.png
|-- /js
|   |-- script.js
|-- index.html
````

# EmailJS

## Descrição

EmailJS é um serviço que permite enviar emails diretamente do JavaScript sem necessidade de um backend próprio. Ele facilita o envio de emails a partir de aplicações web utilizando APIs fáceis de integrar.

## Funcionalidades

- **Envio de Emails**: Permite enviar emails diretamente do cliente (navegador).
- **Modelos de Email**: Suporte para criação e uso de templates de email.
- **Serviços de Email**: Integração com vários serviços de email populares como Gmail, Outlook, etc.
- **API Simples**: API fácil de usar com suporte para promessas (Promises).

## Como Usar

1. **Configuração**:
   - Crie uma conta no [EmailJS](https://www.emailjs.com/).
   - Configure um serviço de email (ex: Gmail).
   - Crie um template de email.

2. **Integração**:
   - Adicione o EmailJS ao seu projeto:
     ```html
     <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/@emailjs/browser@4/dist/email.min.js"></script>
     <script type="text/javascript">
         emailjs.init('YOUR_USER_ID'); // Substitua 'YOUR_USER_ID' pelo seu User ID do EmailJS
     </script>
     ```

3. **Envio de Email**:
   - Utilize o seguinte código JavaScript para enviar emails:
     ```javascript
     document.getElementById('form')
         .addEventListener('submit', function (event) {
             event.preventDefault();

             const btn = document.getElementById('button');
             btn.value = 'Enviando...';

             const serviceID = 'default_service';
             const templateID = 'YOUR_TEMPLATE_ID'; // Substitua 'YOUR_TEMPLATE_ID' pelo seu Template ID

             emailjs.sendForm(serviceID, templateID, this)
                 .then(() => {
                     btn.value = 'INSCREVA-SE';
                     alert('Enviado!');
                 }, (err) => {
                     btn.value = 'INSCREVA-SE';
                     alert(JSON.stringify(err));
                 });
         });
     ```

## Exemplos de Uso

- Formulários de contato
- Inscrições para newsletters
- Feedback de usuários

## Links Úteis

- [Documentação Oficia EmailJS](https://www.emailjs.com/docs/)
- [Documentação Html](https://www.w3schools.com/html/).
- [Documentação Css](https://www.w3schools.com/css/).
- [Visão geral do Javascript e referência de comandos](https://www.w3schools.com/js/).


