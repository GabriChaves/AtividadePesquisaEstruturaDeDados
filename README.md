# Atividade Pesquisa Estrutura De Dados

📌Objetivo:
-
- Escolher uma situação real — não necessariamente comercial — em que uma Estrutura de Dados seja fundamental para o funcionamento da solução, respondendo as seguintes perguntas:
- 1- Onde existe uma pilha no Windows?
- 2- Onde uma árvore aparece no Linux?
- 3- Como o Spotify organiza músicas?
- 4- Por que um banco de dados usa B-tree?

# 📂 Atividade: Pesquisa sobre Estruturas de Dados

> **Status do Projeto:** 🚀 Concluído  
> **Objetivo:** Identificar e explicar a aplicação de Estruturas de Dados em situações e sistemas reais do dia a dia.

---

## 📌 Perguntas e Respostas

### 1️⃣ Onde existe uma pilha no Windows?
A **pilha (stack)** funciona na lógica **LIFO** (*Last In, First Out* — o último que entra é o primeiro que sai). No Windows, ela é a base de duas funções muito comuns:

*   **Ctrl + Z / Ctrl + Y (Desfazer e Refazer):** Cada alteração que você faz no sistema ou em um arquivo de texto vai para o topo de uma pilha. Ao apertar `Ctrl + Z`, o Windows remove e reverte a última ação do topo.
*   **Gerenciamento de Janelas:** O Windows usa pilhas para controlar quais janelas estão sobrepostas na tela, sabendo exatamente qual está no topo (ativa) e quais estão atrás.

---

### 2️⃣ Onde uma árvore aparece no Linux?
A **árvore (tree)** é uma estrutura hierárquica. No Linux, ela organiza todo o **Sistema de Arquivos (Filesystem)**.

*   **A Raiz (`/`):** É o ponto de partida de tudo, o topo da árvore.
*   **Diretórios e Arquivos:** A partir da raiz, surgem os galhos (pastas como `/home`, `/etc`, `/bin`). Dentro dessas pastas, surgem novos galhos ou as folhas (que são os arquivos finais, como fotos e textos).

> 💡 *Dica:* O Linux possui um comando nativo chamado `tree` que desenha essa estrutura de árvore direto no terminal!

---

### 3️⃣ Como o Spotify organiza músicas?
Para gerenciar a fila de reprodução, o Spotify utiliza uma **Lista Duplamente Encadeada (Doubly Linked List)**.

*   **Como funciona:** Cada música é um nó que conhece a música atual e possui dois "ponteiros" (setas): um que aponta para a **próxima** música e outro que aponta para a música **anterior**.
*   **Ações rápidas:** É por isso que os botões de "Avançar" e "Voltar" funcionam instantaneamente, sem precisar recarregar toda a sua biblioteca.

---

### 4️⃣ Por que um banco de dados usa B-tree?
A **B-tree (Árvore B)** é uma árvore de busca sempre balanceada, usada pelos bancos de dados (como MySQL e PostgreSQL) para criar **Índices**.

*   **Busca ultra rápida:** Em vez de ler milhões de linhas de uma tabela uma por uma, a B-tree divide os dados em blocos ordenados, permitindo que o sistema encontre qualquer informação em pouquíssimos passos.
*   **Feita para o HD/SSD:** Ela é desenhada para ser "baixa e larga" (ter muitos filhos por nó), o que reduz drasticamente o número de acessos físicos ao disco rígido, economizando tempo e processamento.

---

## 🛠️ Tecnologias Estudadas

* ![Markdown](https://shields.io)
* ![Linux](https://shields.io)
* ![Windows](https://shields.io)

---
Feito com ❤️ por [Seu Nome](https://github.com)
