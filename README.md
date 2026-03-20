# [SECAL 2026 CAECOMP] | Minicurso desenvolvimento WEB 

### 1. A Estrutura Semântica (HTML)
Em vez de usar `<div>` para tudo, o site usa tags com significados claros:
* **`<header id="navbar">`**: O cabeçalho. Guarda a logo e o menu.
* **`<main>`**: O "corpo" principal da página.
* **`<section>`**: Os blocos de conteúdo (Início, Sobre, Contato). O `id` (ex: `#sobre`) serve como um "endereço" para a página rolar até o lugar certo quando clicamos no menu.
* **`<footer>`**: O rodapé, onde fica a assinatura.

### 2. O Motor do Layout: Flexbox (CSS)
Usei o `display: flex;` para organizar os elementos na tela de um jeito bem prático e sem complicação:
* **`justify-content: space-between;`**: Usado na Navbar. Ele pega a logo e os links e empurra cada um para um canto da tela (um para a extrema esquerda, outro para a direita).
* **`gap: 70px;`**: Usado na seção Sobre para afastar o texto da foto. É um atalho perfeito para criar um "respiro" entre os itens sem precisar calcular margens.
* **`align-items: flex-start;`**: Garante que a caixa de texto e a foto fiquem alinhadas retinhas lá em cima (pelo topo).

### 3. Variáveis de Cor (`:root`)
```css
:root {
    --cor-principal: #061a6c;
}