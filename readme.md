# Guia de Tipografia Responsiva

Um projeto simples, educacional e interativo criado para demonstrar como funciona a escala tipográfica responsiva na prática. Desenvolvido em um único arquivo HTML, o guia adapta visualmente os tamanhos de fonte baseados na largura da tela, utilizando as melhores práticas do mercado e classes do Tailwind CSS.

## 🚀 Funcionalidades

*   **Monitoramento em Tempo Real:** Detecta o redimensionamento da janela do navegador e exibe no topo a resolução exata e qual breakpoint está ativo.
*   **Tabela Dinâmica Interativa:** Uma tabela que recalcula e se atualiza automaticamente, exibindo os tamanhos em pixels (px), a tag HTML correspondente e a classe utilitária do Tailwind CSS (`text-sm`, `text-2xl`, etc.).
*   **Pré-visualização (Live Preview):** O texto de exemplo dentro da tabela ajusta seu próprio `font-size` em tempo real para você sentir a harmonia visual da escala, de H1 a P.
*   **Layout 100% Responsivo:** O site funciona perfeitamente no celular, com a tabela colocada em um container com rolagem horizontal (`overflow-x-auto`) para nunca quebrar o layout da página.

## 🛠️ Tecnologias Utilizadas

*   **HTML5:** Estruturação limpa e semântica.
*   **Tailwind CSS (via CDN):** Todo o visual, espaçamento, cores e responsividade da casca do projeto.
*   **JavaScript (Vanilla):** Lógica simples para escutar o evento de `resize`, identificar o breakpoint atual e injetar os dados (pixels e classes) corretos na tabela.
*   **Google Fonts:** Utiliza a fonte geométrica "Inter", excelente para interfaces digitais.

## 💻 Como executar o projeto

Como o projeto foi arquitetado em um único arquivo sem a necessidade de um ambiente de desenvolvimento complexo (Node.js, Webpack, etc.), é extremamente fácil testá-lo:

1. Salve o código em um arquivo chamado `tipografia-responsiva.html`.
2. Dê um duplo clique no arquivo para abri-lo diretamente no seu navegador favorito (Chrome, Firefox, Safari, Edge).
3. **Faça o teste:** Clique nas bordas da janela do seu navegador e a diminua lentamente. Observe a barra superior mudando as numerações e a tabela redesenhando o tamanho das fontes!

## 📏 Sistema de Breakpoints Adotado

O projeto monitora ativamente três larguras de tela para mudar a proporção matemática dos textos:

*   📱 **Mobile (< 640px):** Utiliza fonte base de 16px e uma escala de menor contraste (títulos não crescem exageradamente para caber na tela pequena).
*   💻 **Tablet (640px - 1024px):** Utiliza fonte base de 18px e um contraste intermediário.
*   🖥️ **Desktop (> 1024px):** Utiliza fonte base de 20px e uma escala de alto contraste, criando títulos imponentes (H1 de 48px) para aproveitar o espaço horizontal do monitor.