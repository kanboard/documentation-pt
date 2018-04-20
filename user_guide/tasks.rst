Tarefas
=======

Criando Tarefas
---------------

No quadro, clique no sinal de mais ao lado do nome da coluna:

.. figure:: /_static/task-creation-board.png
   :alt: criação de tarefas a partir do quadro

Em seguida, o formulário de criação de tarefas é exibido:

.. figure:: /_static/task-creation-form.png
   :alt: formulário de criação de tarefas

- **Título**: O título da sua tarefa, que será exibido no quadro.
- **Descrição**: Descrição que usa a sintaxe do Markdown.
- **Etiquetas**: a lista de etiquetas associadas a tarefas.
- **Criar outra tarefa**: Marque esta caixa se você quiser criar uma tarefa
  similar (alguns campos serão pré-preenchidos).
- **Cor**: escolha a cor do cartão.
- **Responsável**: A pessoa que irá trabalhar na tarefa.
- **Categoria**: somente uma categoria pode ser atribuída a uma tarefa (visível
  somente se os projetos tiverem categorias).
- **Coluna**: A coluna onde a tarefa será criada, sua tarefa será posicionada na
  parte inferior.
- **Prioridade**: prioridade da tarefa, o intervalo pode ser definido nas
  configurações do projeto, os valores padrão são P0 a P3.
- **Complexidade**: Utilizado no gerenciamento ágil de projetos (Scrum), a 
  complexidade ou pontos de história é um número que diz à equipe o quão difícil
  a história é. Muitas vezes, as pessoas usam a série de Fibonacci.
- **Referência**: ID externo para a tarefa, por exemplo, pode ser o número do
  bilhete que vem de outro sistema
- **Estimativa original**: estimativa em horas para concluir a tarefa.
- **Tempo Gasto**: Tempo gasto trabalhando na tarefa.
- **Data de início**: este é um campo de data e hora.
- **Data de Vencimento**: as tarefas vencidas terão uma data de vencimento em
  vermelho e as devidas as datas estarão pretas no quadro. Vários formatos de
  data são aceitos além do selecionador de data.


Com o link de visualização, você pode ver a descrição da tarefa convertida da
sintaxe do Markdown.

Duplicando e Movendo Tarefas
----------------------------

Duplicar uma tarefa no mesmo projeto
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Vá em visualização de tarefas e escolha **Duplicar** à esquerda.

.. figure:: /_static/task-duplication.png
   :alt: duplicação de tarefas

Uma nova tarefa será criada com as mesmas propriedades do original.

Duplicar uma tarefa para outro projeto
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Vá em visualização da tarefa e escolha **Duplicar para outro projeto**.

.. figure:: /_static/task-duplication-another-project.png
   :alt: Duplicação de Tarefas Outro Projeto

Somente projetos nos quais você é membro serão exibidos na lista suspensa.

Antes de copiar as tarefas, o Kanboard perguntará as propriedades
destino que não são comuns entre o projeto origem e o
projeto destino.

Basicamente, você precisa definir:

- A raia destino
- A coluna
- A categoria
- O designado

Mover uma tarefa para outro projeto
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Vá para a visualização de tarefas e escolha **Mover para outro projeto**.

Mover uma tarefa para outro projeto funciona da mesma maneira que a
duplicação, você tem que escolher as novas propriedades da tarefa.

Lista de propriedades duplicadas
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

- title
- description
- date_due
- color_id
- project_id
- column_id
- owner_id
- score
- category_id
- time_estimated
- swimlane_id
- recurrence_status
- recorrência_trigger
- recurrence_factor
- recurrence_timeframe
- recurrence_basedate

Fechando Tarefas
----------------

Quando uma tarefa é fechada, ela fica oculta do quadro.

No entanto, você sempre pode acessar a lista de tarefas fechadas usando a
consulta **status:closed** em qualquer formulário de pesquisa ou simplesmente
selecionando **Tarefas fechadas** no menu suspenso do filtro.

Existem duas maneiras diferentes de fechar uma tarefa, do menu suspenso de
tarefas no quadro:

.. figure:: /_static/menu-close-task.png
   :alt: fecha uma tarefa no menu suspenso

Ou no menu da barra lateral da tarefa, na visualização dos detalhes da tarefa:

.. figure:: /_static/closing-tasks.png
   :alt: fechar tarefa

Nota: Quando você fechar uma tarefa, todas as subtarefas não concluídas serão
alteradas para o status "Finalizada".

Links de tarefas internas
-------------------------

As tarefas podem ser vinculadas a relacionamentos pré-definidos:

.. figure:: /_static/internal-task-links.png
   :alt: Links de tarefas

Também é possível vincular tarefas entre projetos.

Os relacionamentos padrão são:

- **refere-se à**
- **bloqueia** \ | está bloqueada por
- **está bloqueada por** \ | Bloqueia
- **duplicadas** \ | é duplicada por
- **é duplicada por** \ | duplicadas
- **é filha de** \ | é pai de
- **é pai de** \ | é um filha de
- **alvos marco** \ | é um marco de
- **é um marco de** \ | alvos marco
- **corrige** \ | é corrigido por
- **é corrigido por** \ | corrige

Esses rótulos podem ser alterados nas configurações do aplicativo.

Transições de tarefas
---------------------

Cada movimento de uma tarefa entre colunas é registrado no banco de dados.

.. figure:: /_static/task-transitions.png
   :alt: Transições de tarefa

Disponível na visualização de tarefas, você pode ver essas informações:

- Data da ação
- coluna de origem
- Coluna de destino
- Executor (usuários que moveram a tarefa)
- Tempo gasto na coluna de origem

Tarefas recorrentes
-------------------

Para se encaixar na metodologia Kanban, as tarefas recorrentes não são baseadas
em uma data, mas em eventos do quadro.

- As tarefas recorrentes são duplicadas para a primeira coluna do quadro quando
  os eventos selecionados ocorrem
- A data de vencimento pode ser recalculada automaticamente
- Cada tarefa registra o ID da tarefa pai que a criou e a tarefa filho criada

Configuração
~~~~~~~~~~~~

Vá para a página de visualização de tarefas ou use o menu suspenso no quadro;
selecione **Editar recorrência**.

.. figure:: /_static/recurring-tasks.png
   :alt: tarefa recorrente

Existem três gatilhos que atualmente criam uma nova tarefa recorrente:

- Movendo uma tarefa da primeira coluna
- Movendo uma tarefa para a última coluna
- Fechando a tarefa

As datas de vencimento, se definidas na tarefa atual, podem ser recalculadas por um dado
fator de dias, meses ou anos. A data base para o cálculo da
nova data de vencimento pode ser a data de vencimento existente ou a ação
encontro.

Adicionando Capturas de Tela
----------------------------

Você pode copiar e colar imagens diretamente no Kanboard para economizar tempo. Estas
imagens são carregadas como anexos da tarefa.

Isso é especialmente útil para fazer capturas de telas para descrever um problema,
por exemplo.

Você pode adicionar capturas de tela diretamente do quadro clicando no
menu suspenso ou na página de visualização de tarefas.

.. figure:: /_static/dropdown-screenshot.png
   :alt: menu de captura de tela suspensa

Para adicionar uma nova imagem, faça sua captura de tela e cole com CTRL+V ou
Comando+V:

.. figure:: /_static/task-screenshot.png
   :alt: Página de captura de tela

No Mac OS X, você pode usar esses atalhos para fazer capturas de tela:

- Command-Control-Shift-3: Faça uma captura de tela da tela e salve-a para a
  área de transferência
- Command-Control-Shift-4, em seguida, selecione uma área: faça uma captura de
  tela da área e salve-o na área de transferência
- Command-Control-Shift-4, depois espaço, depois clique em uma janela: Captura
  de tela de uma janela e salve-a na área de transferência

Existem também vários aplicativos de terceiros que podem ser usados ​​para
capturas de tela com anotações e formas.

.. warning:: **Este recurso não funciona com todos os navegadores.**
             Não funciona com o Safari devido a este bug: `<https://bugs.webkit.org/show_bug.cgi?id=49141>`_


Etiquetas
---------

Com o Kanboard, você pode associar uma ou mais etiquetas a uma tarefa. Você pode
definir etiquetas globalmente para todos os projetos ou apenas para um projeto específico.

.. figure:: /_static/tags-board.png
   :alt: Etiquetas no quadro

No formulário da tarefa, você pode inserir as etiquetas desejadas:

.. figure:: /_static/tags-task.png
   :alt: formulário de etiquetas

O formulário de preenchimento automático será exibido para sugerir as etiquetas disponíveis.

Você também pode criar etiquetas diretamente no formulário de tarefas. Por
padrão, quando você cria etiquetas de um formulário de tarefas que eles estão
associados ao atual projeto:

.. figure:: /_static/tags-projects.png
   :alt: Etiquetas do projeto

Todas as etiquetas podem ser gerenciadas nas configurações do projeto.

Para definir etiquetas globalmente para todos os projetos, vá para o aplicativo
configurações:

.. figure:: /_static/tags-global.png
   :alt: Etiquetas globais

Para pesquisar tarefas com base em etiquetas, basta usar o atributo “etiqueta”:

.. figure:: /_static/tags-search.png
   :alt: Pesquisar Etiquetas

Estatísticas
------------

Cada tarefa tem uma seção de estatísticas disponível no menu à esquerda na
exibição de tarefa.

Tempo de Execução e Tempo de Ciclo
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. figure:: /_static/task-lead-cycle-time.png
   :alt: lead e tempo de ciclo

- O tempo de execução é o tempo entre a criação da tarefa e a data da conclusão
  (tarefa fechada).
- O tempo de ciclo é o tempo entre a data de início e a data de conclusão.
- Se a tarefa não for fechada, a hora atual é usada em vez da data de conclusão.
- Se a data de início não for especificada, o tempo do ciclo não será calculado.

Nota: Você pode configurar uma ação automática para definir a data de início
automaticamente quando você move uma tarefa para a coluna de sua escolha.

Tempo gasto em cada coluna
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. figure:: /_static/time-into-each-column.png
   :alt: tempo gasto em cada coluna

- Este gráfico mostra o tempo total gasto em cada coluna para a tarefa.
- O tempo gasto é calculado até que a tarefa seja encerrada.
