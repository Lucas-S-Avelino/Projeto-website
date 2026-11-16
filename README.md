# Portal Acadêmico — Ciências da Computação 2026.1

Portal web estático desenvolvido para a turma de Ciências da Computação (semestre 2026.1). O projeto reúne ementas curriculares, referências bibliográficas, materiais de apoio para estudos e canal de contato com os estudantes.

---

## 📌 Visão Geral

- **Público-alvo:** Alunos, professores e interessados na matriz curricular da turma.
- **Tipo de Aplicação:** Website estático multi-páginas (MPA — _Multi-Page Application_).
- **Sem Dependências Externas:** Desenvolvido puramente em **HTML5**, **CSS3** e **JavaScript Vanilla**, sem frameworks (React, Next.js, Vue), bibliotecas utilitárias (Tailwind, Bootstrap) ou compiladores/transpiladores (TypeScript, Vite).

---

## 📁 Estrutura de Arquivos

```text
.
├── assets/                          # Imagens e recursos visuais do portal
│   ├── arquitetura-hardware.png     # Ilustração de hardware/placa-mãe
│   ├── estudo-web.png               # Ilustração da seção de estudos
│   ├── modelagem-dados.png          # Diagrama/referência de banco de dados
│   ├── oficina-comunidade.png       # Registro ilustrativo da atividade de extensão
│   └── turma-laboratorio.png        # Imagem principal da seção hero
├── css/
│   ├── base.css           <-- Variáveis (:root), resets, tipografia, header e footer
│   ├── index.css          <-- Hero, estatísticas, cards de destaque e trilhas
│   ├── disciplinas.css    <-- Barra de busca e lista de ementas em accordion
│   ├── guia_de_estudos.css<-- Grid de recursos externos, bibliografia e dicas
│   └── contato.css        <-- Formulário de contato, grid de campos e sidebar
├── js/
│   └── script.js                    # Lógica client-side em JavaScript puro (por enquanto VAZIA)
├── paginas/
│   ├── disciplinas.html             # Ementas curriculares e busca interativa
│   ├── guia_de_estudos.html         # Documentações oficiais, livros recomendados e rotina de estudo
│   ├── materiais.html               # Biblioteca de resumos, referências visuais e simulados com filtro
│   └── contato.html                 # Formulário demonstrativo para dúvidas, mensagens e sugestões
├── index.html                       # Página inicial (Apresentação, estatísticas e visão geral)
└── README.md                        # Documentação do repositório
```

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 Semântico:** Marcação acessível utilizando tags estruturais (`<header>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`, `<details>`, `<summary>`).
- **CSS3 Puro:**
  - Variáveis nativas (CSS Custom Properties).
  - Flexbox e CSS Grid para layout responsivo.
  - Regras de acessibilidade com `@media (prefers-reduced-motion: reduce)`.
  - Breakpoints responsivos para dispositivos móveis, tablets e desktops.

---

## 🚀 Como Executar o Projeto

Como o site é totalmente estático e roda 100% no navegador, não é necessário instalar dependências com `npm` ou `yarn`.

### Opção 1: Execução Direta

1. Clone ou baixe este repositório.
2. Certifique-se de que os arquivos de imagem estejam salvos dentro da pasta `assets/`.
3. Dê dois cliques em `index.html` ou abra o arquivo no navegador de sua preferência.

### Opção 2: Servidor Local (Recomendado para evitar restrições de CORS em assets locais)

Usando a extensão **Live Server** no VS Code:

1. Abra a pasta do projeto no VS Code.
2. Clique com o botão direito sobre `index.html` e selecione **"Open with Live Server"**.

---

## 🧭 Páginas do Portal

1. **Início (`index.html`):** Apresentação do semestre 2026.1, destaques da extensão curricular e pontos de entrada para o portal.
2. **Disciplinas (`disciplinas.html`):** Relação dos 7 componentes curriculares em cards retráteis (`<details>`), com campo de busca por palavra-chave em tempo real.
3. **Guia de Estudos (`guia_de_estudos.html`):** Links para documentações de referência (MDN, Java, PostgreSQL, Scrum Guide, etc.), bibliografia fundamental e dicas de estudo.
4. **Materiais (`materiais.html`):** Coleção de resumos práticos, imagens de referência e simulado autoral com botões de filtro por categoria (`Todos`, `Textos`, `Referências visuais`, `Simulados`, `Provas antigas`).
5. **Contato (`contato.html`):** Interface de mensagens com validação nativa de campos, contador de caracteres em tempo real e aviso demonstrativo local.

---

## ♿ Acessibilidade e Boas Práticas

- **Navegação por Teclado:** Foco visível (`:focus-visible`) customizado e link de salto inicial (`skip-link`) para ir direto ao conteúdo principal.
- **Leitores de Tela:** Utilização de atributos ARIA (`aria-live`, `aria-current="page"`, `aria-expanded`, `aria-controls`) e marcação semântica adequada.
- **Fechamento Ágil:** O menu de navegação mobile pode ser dispensado pressionando a tecla `Esc`.
- **Desempenho:** Carregamento otimizado de imagens com atributos nativos `fetchpriority="high"` e `loading="lazy"`.

---

## 📄 Licença e Observações

- As fotos e recursos visuais incluídos são representações ilustrativas para fins educacionais da turma.
- O formulário de contato opera atualmente em modo demonstrativo.
