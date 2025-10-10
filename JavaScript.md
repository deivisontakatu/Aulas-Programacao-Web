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