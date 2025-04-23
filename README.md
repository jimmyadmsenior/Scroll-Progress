# Scroll-Progress

## Descrição

O repositório **Scroll Progress** implementa uma funcionalidade que permite visualizar o progresso de rolagem (scroll) de uma página. Essa funcionalidade é útil para melhorar a experiência do usuário, fornecendo um indicador visual de quão longe o usuário está na página.

## Funcionalidades

- **Indicador de Progresso**: Mostra uma barra de progresso que se atualiza conforme o usuário rola a página.
- **Personalização**: Permite personalizar a cor e a altura da barra de progresso.
- **Compatibilidade**: Funciona em todos os navegadores modernos.
- **Design Responsivo**: Adapta-se a diferentes tamanhos de tela, com suporte para dispositivos móveis.

## Instalação

Para usar o Scroll Progress em seu projeto, siga os passos abaixo:

1. Clone o repositório:
   ```bash
   git clone https://github.com/jimmyadmsenior/Scroll-Progress
   ```

2. Navegue até o diretório do projeto:
   ```bash
   cd scroll-progress
   ```

3. Adicione os arquivos CSS e JS ao seu projeto:
   ```html
   <link rel="stylesheet" href="style.css">
   <script src="scroll-progress.js"></script>
   ```

## Uso

### JavaScript

Adicione o seguinte código ao seu arquivo JavaScript para calcular e atualizar o progresso da barra:

```javascript
window.onscroll = function() {
    var scrollTop = document.documentElement.scrollTop;
    var scrollHeight = document.documentElement.scrollHeight - document.documentElement.clientHeight;
    var scrollPercent = (scrollTop / scrollHeight) * 100;

    document.getElementById("progress-bar").style.width = scrollPercent + "%";
};
```

### HTML

Adicione a seguinte estrutura HTML para a barra de progresso e navegação:

```html
<div id="progress-container">
    <div id="progress-bar"></div>
</div>

<header>
    <nav>
        <a href="#html">Html</a>
        <a href="#css">CSS</a>
        <a href="#js">JS</a>
        <a href="#php">PHP</a>
        <a href="#sql">SQL</a>
    </nav>
</header>

<div class="section" id="html">
    <h2>HTML</h2>
    <p>HyperText Markup Language</p>
</div>

<div class="section" id="css">
    <h2>CSS</h2>
    <p>Cascading Style Sheets</p>
</div>

<div class="section" id="js">
    <h2>JS</h2>
    <p>Client-Side Scripting Language</p>
</div>

<div class="section" id="php">
    <h2>PHP</h2>
    <p>Hypertext Preprocessor</p>
</div>

<div class="section" id="sql">
    <h2>SQL</h2>
    <p>Structured Query Language</p>
</div>
```

### CSS

Certifique-se de incluir o arquivo `style.css` para estilizar a barra de progresso e as seções. O arquivo já está configurado para suportar animações e design responsivo.

## Observação

- A barra de progresso foi projetada para funcionar melhor no navegador **Google Chrome**. Você até pode tentar utilizar outros navegadores, porém pode ocasionar pequenas falhas de design responsivo na tela.
- Para dispositivos móveis, o design é ajustado automaticamente.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.

## Licença

Este projeto está licenciado sob a MIT License. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## Contato

Para mais informações, entre em contato com meu e-mail: jimmycastilho555@gmail.com