# Projeto Portfólio SECAL 2026 CAECOMP 

### 1. Semântica HTML
Em vez de usar apenas `<div>` para tudo, a estrutura do site foi construída com tags semânticas para melhorar a acessibilidade e o SEO:
* `<header>`: Para a barra de navegação principal.
* `<main>`: Envolvendo o conteúdo central e exclusivo da página (a tela inicial).
* `<section>`: Para dividir os assuntos da página (seções "Sobre" e "Contato").
* `<footer>`: Para o rodapé com a assinatura do projeto.

### 2. Layout com CSS Flexbox (`display: flex`)
O Flexbox foi a ferramenta principal para o alinhamento de quase todos os elementos:
* **Navbar:** Usado para empurrar a logo para a esquerda e o menu para a direita (`justify-content: space-between`).
* **Seção Sobre:** Criou as duas colunas (Texto e Foto) lado a lado, permitindo que elas quebrem de linha em telas menores de forma fluida (`flex-wrap: wrap`).
* **Centralização:** Usado extensivamente para alinhar textos e ícones perfeitamente no centro das caixas (`align-items: center`, `justify-content: center`).

### 3. Variáveis CSS (Custom Properties)
Implementei variáveis globais no `:root` do CSS. Isso permite alterar as cores principais do site mudando apenas uma linha de código, facilitando a manutenção e a criação de futuros temas (como um *Dark Mode*).
```css
:root {
    --cor-da-navbar: #ffcc00;
}
