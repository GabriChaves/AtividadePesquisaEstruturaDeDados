# Atividade Pesquisa: Estrutura De Dados

📌Objetivo:
-
- Escolher uma situação real — não necessariamente comercial — em que uma Estrutura de Dados seja fundamental para o funcionamento da solução e responder as seguintes perguntas:
  
  1- Onde existe uma pilha no Windows?

  2- Onde uma árvore aparece no Linux?

  3- Como o Spotify organiza músicas?

  4- Por que um banco de dados usa B-tree?

↩️O Atalho de Desfazer (Ctrl + Z)
-
Sempre que quando digitamos uma frase em um editor de código ou de texto, será que tudo está sendo registrado? Claro! Apagar um parágrafo ou alterar a formatação, o software precisa registrar cada ação para permitir a reversão.
  
Sem uma estrutura adequada, guardar o histórico inteiro em uma lista comum tornaria o salvamento e a navegação extremamente mais lentos. A Pilha (Stack) faz parte de uma solução fundamental, operando no formato LIFO (Last In, First Out - O último a entrar é o primeiro a sair), a ação mais recente vai ser a primeira a ser desfeita ao pressionar Ctrl + Z.
  
O sistema faz um "push" de cada alteração na pilha e, ao desfazer, faz um "pop" para restaurar o estado anterior com complexidade $O(1)$.

1️⃣- Onde existe uma pilha no Windows?
-
Na Call Stack (Pilha de Chamadas de Funções) que cada thread de execução gerencia na memória RAM, assim como no mecanismo de navegação de pastas do Windows Explorer (para voltar à pasta anterior). Quando um programa no Windows chama uma função, as variáveis locais e o endereço de retorno são empilhados; ao finalizar a função, esses dados são desempilhados.

2️⃣- Onde uma árvore aparece no Linux?
-
No Virtual File System (VFS) e no sistema de diretórios (a raiz / que se desdobra em /bin, /home, /etc). Internamente no kernel Linux, árvores rubro-negras (Red-Black Trees) também são usadas pelo agendador de processos (Completely Fair Scheduler - CFS) para gerenciar o tempo de CPU de forma altamente eficiente.

3️⃣- Como o Spotify organiza músicas?
-
- O Spotify combina múltiplas estruturas dependendo do contexto:

  Tabelas Hash (Hash Maps): Para busca instantânea $O(1)$ de metadados das músicas por ID ou nome.
  
  Grafos (Graphs): Para o sistema de recomendação, onde nós representam usuários/músicas e as arestas representam conexões de afinidade ou histórico de escuta.
  
  Listas Encadeadas (Linked Lists): Para gerenciar a fila de reprodução atual (Queue), permitindo reordenar ou adicionar faixas dinamicamente.

4️⃣- Por que um banco de dados usa B-tree?
-
Porque arquivos de banco de dados são gigantescos e ficam armazenados no disco (SSD/HD), que possui leitura muito mais lenta do que a memória RAM. As B-Trees (e B+ Trees) reduzem drasticamente o número de acessos ao disco ao manterem muitos dados por nó (auto-balanceamento com alta ramificação). Isso permite encontrar qualquer registro em milhões de linhas fazendo apenas 3 ou 4 leituras de bloco de disco.
