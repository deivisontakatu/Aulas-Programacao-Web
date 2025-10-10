# ⚡ JavaScript – Sintaxe, Variáveis e Estruturas

O JavaScript é uma linguagem de programação que atua principalmente no lado do cliente (client side), ou seja, é executada diretamente no navegador do usuário.  
Essa característica permite maior interatividade nas páginas da web, tornando a experiência mais dinâmica, responsiva e envolvente.

## 🧠 Introdução ao JavaScript

O JavaScript é essencial para criar páginas modernas e funcionais.  
Com ele, é possível:

- Validar formulários em tempo real
- Alterar estilos dinamicamente
- Inserir ou remover conteúdo do DOM
- Criar animações e efeitos visuais
- Interagir com APIs e servidores

Além disso, é uma das três tecnologias fundamentais da web, junto com HTML e CSS.

## 🧩 Inserindo JavaScript no HTML

O JavaScript pode ser incluído de três maneiras diferentes:

1. **Interno (no corpo do HTML)**
   ```html
   <script>
     alert("Olá, mundo!");
   </script>
   ```

2. **Externo (arquivo separado)**
   ```html
   <script src="script.js"></script>
   ```
   > ✅ Essa é a forma recomendada em projetos maiores, pois facilita a organização e manutenção do código.

3. **Inline (dentro de atributos)**
   ```html
   <button onclick="alert('Você clicou!')">Clique Aqui</button>
   ```
   > Embora funcione, o uso inline não é indicado em projetos profissionais, pois mistura HTML e JavaScript.

## 📦 Variáveis

As variáveis são usadas para armazenar informações que podem ser manipuladas pelo programa.

Em JavaScript, é possível declarar variáveis com:

```javascript
var nome = "Maria";      // escopo de função
let idade = 25;          // escopo de bloco
const cidade = "Sorocaba"; // constante
```

**Diferenças principais:**
- `var` → escopo de função, visível em todo o bloco.
- `let` → escopo de bloco `{}`, mais previsível e seguro.
- `const` → valor constante, não pode ser reatribuído.

> 💡 As variáveis são case sensitive: nome, Nome e NOME são diferentes!

## 🔀 Estruturas Condicionais

Permitem executar blocos de código diferentes dependendo de uma condição.

**Exemplo com if e else:**
```javascript
let idade = 18;

if (idade >= 18) {
  console.log("Maior de idade");
} else {
  console.log("Menor de idade");
}
```

**Exemplo com else if:**
```javascript
let nota = 7;

if (nota >= 9) {
  console.log("Excelente!");
} else if (nota >= 6) {
  console.log("Aprovado");
} else {
  console.log("Reprovado");
}
```

Essas estruturas são fundamentais para criar lógicas de decisão no código.

## ⚙️ Funções

Funções são blocos de código que executam uma tarefa específica.  
Elas ajudam a organizar, reutilizar e modularizar o código.

**Declaração tradicional:**
```javascript
function saudacao(nome) {
  return `Olá, ${nome}!`;
}
console.log(saudacao("João"));
```

**Arrow function:**
```javascript
const soma = (a, b) => a + b;
console.log(soma(2, 3)); // 5
```

As funções podem receber parâmetros e retornar valores, tornando o código mais eficiente e legível.

## 🧮 Funções e Métodos Comuns

| Função / Método              | Descrição                                 |
|------------------------------|-------------------------------------------|
| console.log()                | Exibe mensagens no console (debug)        |
| alert(), prompt(), confirm() | Interagem com o usuário                   |
| document.getElementById()    | Seleciona elementos HTML                  |
| document.querySelector()     | Seleciona elementos com seletor CSS       |
| .addEventListener()          | Adiciona eventos (cliques, inputs etc.)   |
| .innerHTML / .textContent    | Modificam conteúdo de elementos           |
| .push() / .pop()             | Adicionam ou removem itens de um array    |
| .map() / .filter() / .forEach| Manipulam arrays de forma funcional       |
| setTimeout() / setInterval() | Executam funções com atraso ou intervalo  |
| Math.random() / Math.floor() | Geram e arredondam números aleatórios     |
| new Date() / .getFullYear()  | Trabalham com datas e horários            |

## 🧱 DOM (Document Object Model)

O DOM é uma representação em árvore da estrutura de uma página web.  
Com ele, o JavaScript pode acessar e modificar qualquer elemento HTML.

**Exemplo:**
```javascript
document.getElementById("titulo").textContent = "Novo Título!";
```

**Virtual DOM:**  
Usado em frameworks como React, é uma versão otimizada do DOM.  
Ele cria uma cópia virtual e atualiza apenas as partes que mudaram, tornando o processo mais rápido e eficiente.

## 💻 Exemplos de Código

**Exemplo 1: Alterando texto com clique**
```html
<button id="botao">Clique aqui</button>
<p id="mensagem"></p>

<script>
  const botao = document.getElementById('botao');
  botao.addEventListener('click', () => {
    document.getElementById('mensagem').textContent = 'Você clicou no botão!';
  });
</script>
```

**Exemplo 2: Manipulando arrays**
```javascript
let frutas = ["Maçã", "Banana"];
frutas.push("Laranja");
console.log(frutas); // ["Maçã", "Banana", "Laranja"]
```

## 🧾 Boas Práticas

- ✅ Sempre use `let` e `const` em vez de `var`.
- ✅ Nomeie funções e variáveis com verbos e substantivos claros.
- ✅ Organize o código em funções curtas e modulares.
- ✅ Use o console para depurar erros e acompanhar execuções.
- ✅ Separe o HTML, CSS e JS em arquivos distintos.

## 📚 Referências

- CARDOSO, Márdel Vinicius de Faria. Desenvolvimento Web para o ensino superior. Axcel Books, 2004.
- CRANE, Dave; PASCARELLO, Eric; JAMES, Darren. Ajax em ação. Pearson Prentice Hall, 2007.
- FLANAGAN, David. JavaScript: o guia definitivo. Bookman, 2014.
- FRAIN, Ben. Responsive Web Design with HTML5 and CSS3. Packt Publishing, 2012.
- MILETTO, Evandro Manara. Desenvolvimento de Software II: Introdução ao Desenvolvimento Web com HTML, CSS, JavaScript e PHP. Bookman, 2014.
- MDN Web Docs – Guia JavaScript

---

> 💡 **Resumo Final:**  
Dominar os fundamentos de sintaxe, variáveis, condicionais e funções é essencial para se tornar um bom desenvolvedor JavaScript.  
Esses conceitos são a base para criar aplicações web dinâmicas, responsivas e modernas.

⚡ JavaScript e Eventos – Tornando a Página Interativa

O JavaScript é a chave para adicionar interatividade às páginas web.  
Ele permite que o navegador reaja às ações do usuário, tornando o conteúdo dinâmico e responsivo.

## 🧠 O que são Eventos em JavaScript?

Eventos são ações ou ocorrências que acontecem no sistema e que o navegador pode detectar para que possamos reagir.

**Exemplos de eventos:**
- Um usuário clicando em um botão
- Uma página web terminando de carregar
- Um campo de texto sendo modificado
- O mouse passando sobre um elemento
- Uma tecla sendo pressionada

📍 Eventos são a base da interatividade, permitindo que o JavaScript responda às ações do usuário em tempo real.

## 🔄 Como os Eventos Funcionam

O ciclo de eventos em JavaScript segue um padrão consistente:

1. **Evento:** uma ação ocorre (clique, tecla pressionada etc.)
2. **Escuta:** o navegador detecta o evento por meio de um event listener
3. **Reação:** uma função de callback é executada em resposta
4. **Modificação:** o DOM é atualizado, podendo gerar novos eventos

Este ciclo é a base da interatividade moderna na web.

## 🧩 Métodos de Implementação de Eventos

Existem duas principais formas de implementar eventos em JavaScript:

| Método          | Exemplo                              | Vantagens                          | Limitações                                |
|-----------------|-------------------------------------|------------------------------------|-------------------------------------------|
| HTML Inline      | `<button onclick="minhaFuncao()">Clique</button>` | Simples para iniciantes            | Mistura HTML e JS, apenas um evento por elemento |
| addEventListener | `botao.addEventListener('click', minhaFuncao);` | Separação de responsabilidades, múltiplos listeners | Requer um pouco mais de código            |

✅ **Recomendação:** use `addEventListener()` para um código mais organizado e manutenível.

## 🧱 Principais Tipos de Eventos

| Evento     | Descrição                              | Uso Comum                          |
|------------|----------------------------------------|------------------------------------|
| click      | Quando um elemento é clicado          | Botões, links, elementos interativos |
| change     | Quando o valor de um elemento muda    | Campos de formulário, seletores    |
| mouseover  | Quando o cursor passa sobre um elemento | Menus, tooltips, efeitos hover     |
| keydown    | Quando uma tecla é pressionada        | Atalhos de teclado, jogos, formulários |
| submit     | Quando um formulário é enviado        | Validação de formulários           |
| load       | Quando um recurso termina de carregar  | Inicialização de página, imagens   |

Cada tipo de evento captura diferentes interações do usuário.

## 💻 Exemplo Prático

**HTML**
```html
<button id="botao">Clique aqui</button>
<p id="mensagem"></p>
```

**JavaScript**
```javascript
const botao = document.getElementById('botao');
botao.addEventListener('click', () => {
  document.getElementById('mensagem')
    .textContent = 'Você clicou no botão!';
});
```

**Explicação**
- Selecionamos o botão pelo seu ID
- Adicionamos um ouvinte para o evento de clique
- Quando o evento ocorre, a função anônima é executada
- A função modifica o conteúdo do elemento com ID "mensagem"

## 🧠 Exercício Sugerido

Crie um campo de texto e um botão que mostre o valor digitado dentro de uma `<div>`.

```html
<input type="text" id="campoTexto" placeholder="Digite algo aqui">
<button id="botaoMostrar">Mostrar Texto</button>
<div id="resultado"></div>
```

```javascript
const campoTexto = document.getElementById('campoTexto');
const botaoMostrar = document.getElementById('botaoMostrar');
const resultado = document.getElementById('resultado');

botaoMostrar.addEventListener('click', () => {
  resultado.textContent = campoTexto.value;
});
```

💡 **Desafio extra:** adicione um evento para limpar o resultado quando o campo de texto for apagado.

## 🧾 Resumo e Dicas

**Conceitos Principais**
- Eventos são ações detectadas pelo navegador.
- Permitem criar páginas dinâmicas e interativas.
- O ciclo segue o padrão: evento → escuta → reação.
- Existem diversos tipos de eventos para diferentes interações.

**Boas Práticas**
- ✅ Use `addEventListener()` em vez de atributos inline.
- ✅ Separe a lógica JavaScript do HTML.
- ✅ Utilize o console do navegador para depurar eventos.
- ✅ Considere a performance ao adicionar muitos event listeners.

## ⚙️ Referência Rápida de Eventos Comuns

| Evento     | Descrição                              |
|------------|----------------------------------------|
| click      | Quando um elemento é clicado          |
| keydown    | Quando uma tecla é pressionada        |
| submit     | Quando um formulário é enviado        |
| load       | Quando a página termina de carregar    |
| mouseover  | Quando o mouse passa sobre um elemento |

## 🚀 Próximos Passos

- Explore eventos mais avançados (como drag & drop e touch).
- Aprenda sobre propagação de eventos (bubbling).
- Estude padrões de design para gerenciamento de eventos.

---

> 💡 **Resumo Final:**  
Dominar eventos em JavaScript é fundamental para criar interfaces interativas e responsivas.  
Cada ação do usuário pode ser uma oportunidade para melhorar a experiência e tornar a aplicação mais intuitiva.

✅ Agora é só copiar todo esse conteúdo e salvar em um arquivo chamado:
`README_Eventos_JS.md`

Quer que eu una este conteúdo com o anterior (`README_JS_focado.md`) em um único arquivo completo sobre JavaScript básico + eventos?