# Atividade com Projetos Front-end

**Disciplina:** Desenvolvimento Web  
**Professor:** Prof. Me. Deivison S. Takatu  
**Contato:** deivison.takatu@facens.br  

---

## 📚 Conteúdo da Aula

- Instalando o Node.js  
- Criando um Projeto React  
- Criando um Projeto Angular  
- Criando um Projeto Vue  
- Importação de Projetos  
- Atividade prática  

---

## 🟢 Instalando o Node.js

**Node.js** é um ambiente de execução JavaScript que permite rodar código no **backend** (servidor), usando a mesma linguagem no servidor e no navegador, integrando melhor frontend e backend.

### Instalação
1. Acesse [nodejs.org/en/download](https://nodejs.org/en/download).  
2. Escolha a versão para seu sistema operacional.  
3. Execute o instalador e siga as etapas “Next > Install”.  
4. Para testar:
   ```bash
   node --version
   ```
   Se aparecer a versão instalada, a instalação está correta.

---

## 📦 Node Package Manager (NPM)

O **NPM** é o gerenciador de pacotes do Node.js, instalado automaticamente com ele.

- Instala, atualiza e remove bibliotecas e frameworks JavaScript.
- Permite criação e compartilhamento de módulos públicos ou privados.
- Gerencia dependências automaticamente via **package.json**.
- Comando essencial:
   ```bash
   npm install
   ```
   Baixa automaticamente os pacotes listados no `package.json`.

---

## ⚛️ Criando um Projeto React

### Requisitos
- Node.js instalado.  
- Conhecimento em **JSX** e **Hooks**:
  - [JSX](https://react.dev/learn/writing-markup-with-jsx)
  - [Hooks](https://react.dev/reference/react/hooks)

### Destaques
- Flexibilidade (não impõe estrutura rígida).  
- Grande ecossistema: Redux, React Router, Next.js.  
- Componentização eficiente.  
- **Virtual DOM** para performance otimizada.  
- Comunidade ativa.

### Passos
```bash
npx create-react-app meu-projeto-react
cd meu-projeto-react
code .
npm start
```

### Estrutura
- **node_modules**: bibliotecas instaladas.
- **public**: HTML, JSON, imagens.
- **src**: código React.
- **.gitignore**: arquivos ignorados pelo Git.
- **package.json** / **package-lock.json**: dependências e scripts.
- **index.js**: ponto de entrada (renderiza App no DOM).
- **App.js**: componente raiz.
- **App.css**: estilos do App.
- **index.css**: estilos globais.

---

## 🅰️ Criando um Projeto Angular

### Requisitos
- Node.js instalado.  
- Conceitos de POO:
  - [Classes em Angular](https://angular.dev/cli/generate/class#)

### Destaques
- Framework completo (roteamento, HTTP client, injeção de dependências).  
- Suporte nativo a **TypeScript**.  
- Arquitetura **MVC**.  
- CLI poderosa para geração de componentes e serviços.  
- Alta performance com **Change Detection**.

### Conceitos Fundamentais
- **Componentes**: `@Component` (HTML + CSS + TypeScript).  
- **Módulos**: `@NgModule`.  
- **Serviços**: `@Injectable`.  
- **Data Binding**: `[(ngModel)]`, `{{ }}`.  
- **Injeção de Dependência**: hierarquia de providers.  
- **Roteamento**: `RouterModule`.

### Passos
```bash
npm install -g @angular/cli
ng new meu-app-angular
cd meu-app-angular
code .
ng serve
```

### Estrutura
- **node_modules**: bibliotecas e dependências.  
- **public**: arquivos estáticos.  
- **src**: código Angular (componentes, serviços, módulos).  
- **.angular**: cache/configurações de build.  
- **.vscode**: configs do VS Code.  
- **.gitignore**: arquivos ignorados pelo Git.  
- **package.json** / **package-lock.json**: dependências e scripts.  
- **angular.json**: configuração de build, testes e estilos globais.  
- **tsconfig.json** / **tsconfig.app.json** / **tsconfig.spec.json**: configurações do TypeScript.  
- **.editorconfig**: padrão de formatação.  
- **README.md**: informações essenciais.  

Principais arquivos:
- **app/**: componentes e serviços principais.  
- **index.html**: ponto de entrada.  
- **main.ts**: inicializa o `AppModule`.  
- **main.server.ts** / **server.ts**: configuração para SSR.  
- **styles.css**: estilos globais.

---

## 🟣 Criando um Projeto Vue

### Requisitos
- Node.js instalado.
- Conhecimento em JavaScript/TypeScript:
  - [Introdução ao Vue](https://vuejs.org/guide/introduction.html)

### Destaques
- **Progressivo**: adote gradualmente.  
- **Reatividade eficiente**.  
- **Single-File Components (SFC)**: HTML, CSS e JS em um único arquivo `.vue`.  
- Curva de aprendizado suave.  
- **Virtual DOM** de alta performance.

### Passos
```bash
npm create vue@latest
cd meu-projeto-vue
npm install
code .
npm run dev
```

### Estrutura
- **node_modules**: bibliotecas e dependências.  
- **public**: arquivos estáticos não processados pelo Vite.  
- **src**: código-fonte (componentes, serviços).  
- **assets**: imagens, fontes, CSS global.  
- **components**: componentes reutilizáveis.  
- **App.vue**: componente raiz.  
- **main.js**: ponto de entrada.  
- **index.html**: HTML principal com div `#app`.  
- **.gitignore**, **package.json**, **package-lock.json**, **vite.config.js**: configurações do projeto.

---

## 📥 Importando Projetos

Encontre templates prontos para acelerar o desenvolvimento:

- **GitHub**: pesquise e use `git clone <url>`.  
- **Vercel Templates**: baixe partes de repositórios prontos.  
- **CodeSandbox**: [Template Search](https://codesandbox.io/).

---

## 🧪 Atividade Prática

1. Crie **três projetos**: React, Angular e Vue.  
2. Faça alterações iniciais no código.  
3. Versione cada projeto com **Git** e faça commit em **repositórios separados** no GitHub.  
4. Pesquise um template pronto, importe, personalize e faça commit em um quarto repositório.  
5. Faça **deploy de todos os projetos na Vercel**.  
6. Documente o processo em um único arquivo com:
   - Descrições e prints.
   - Links dos repositórios GitHub e dos projetos na Vercel.
7. Envie no **Canvas**.

---

## 🎯 Aprendizagens da Aula

- Instalar e configurar **Node.js** e **NPM**.  
- Criar projetos front-end em **React**, **Angular** e **Vue**.  
- Comparar frameworks em arquitetura e fluxo de desenvolvimento.  
- Importar e personalizar projetos existentes.  
- Versionar projetos com **Git** e realizar **deploy** na Vercel.

---

## 🛡️ Dicas Extras e Melhorias

### Exemplos Visuais
- Inclua capturas de tela do processo de criação dos projetos, estrutura de pastas e resultado dos componentes.
- Documente cada etapa com imagens para facilitar o acompanhamento.

### Glossário Rápido
- **SPA:** Aplicação de página única, navegação sem recarregar a página.
- **JSX:** Sintaxe que mistura JavaScript e HTML no React.
- **Virtual DOM:** Representação otimizada do DOM para atualizações rápidas.
- **SFC:** Single-File Component, usado no Vue.
- **CLI:** Interface de linha de comando para criação e gerenciamento de projetos.
- **Data Binding:** Sincronização automática entre dados e interface.

### Checklist de Publicação
- [ ] Node.js instalado
- [ ] Projetos React, Angular e Vue criados
- [ ] Componentes desenvolvidos e testados
- [ ] Código versionado no GitHub
- [ ] Deploy realizado na Vercel
- [ ] Documentação e prints incluídos

### Dicas de Boas Práticas
- Organize componentes em pastas separadas.
- Utilize prop-types (React) e tipagem (Angular/Vue) para validação.
- Mantenha dependências atualizadas.
- Use variáveis sensíveis em arquivos `.env`.

### Segurança e Acessibilidade
- Adicione textos alternativos em imagens.
- Garanta contraste adequado nas cores.
- Teste navegação por teclado e leitores de tela.
- Atualize dependências regularmente.

### Links Úteis
- [Documentação React](https://react.dev/)
- [Documentação Angular](https://angular.io/)
- [Documentação Vue.js](https://vuejs.org/)
- [Guia de Acessibilidade Web](https://www.w3.org/WAI/test-evaluate/)
- [Deploy na Vercel](https://vercel.com/docs)

### Comparativo Prático
- Implemente um componente simples (ex.: contador) em React, Angular e Vue para ilustrar diferenças de sintaxe e estrutura.

---

💡 **Dica Final:** Revise seus projetos em diferentes dispositivos e peça feedback de usuários reais para aprimorar a experiência.
