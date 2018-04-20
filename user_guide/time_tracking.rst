Rastreamento de tempo
=====================

As informações de rastreamento de tempo podem ser definidas no nível da tarefa
ou no nível de subtarefa.

Rastreamento de tempo da tarefa
-------------------------------

.. figure:: /_static/task-time-tracking.png
   :alt: rastreamento do tempo da tarefa

Tarefas possuem dois campos:

- Tempo estimado
- Tempo gasto

Esses valores representam horas de trabalho e precisam ser definidos manualmente.

Acompanhamento de tempo de subtarefa
------------------------------------

.. figure:: /_static/subtask-time-tracking.png
   :alt: rastreamento de tempo de subtarefa

As subtarefas também têm os campos “tempo gasto” e “tempo estimado”.

Quando você altera o valor desses campos, **o rastreamento do tempo da tarefa
os valores são atualizados automaticamente e se tornam a soma de todas as
subtarefas valores**.

Kanboard registra o tempo entre cada mudança de status de subtarefa em um
tabela separada.

- Alterar o status da subtarefa de **A fazer** para **em pogresso** registra
  hora de início
- Alterar o status da subtarefa de **em andamento** para **concluído** registra
  o final tempo, mas também atualizar o tempo gasto da subtarefa e da tarefa

A divisão de todos os registros é visível na página de visualização de tarefas:

.. figure:: /_static/task-timesheet.png
   :alt: quadro de horários da tarefa

Para cada subtarefa, o cronômetro pode ser interrompido/iniciado a qualquer momento:

.. figure:: /_static/subtask-timer.png
   :alt: temporizador de subtarefa

- O cronômetro não depende do status da subtarefa
- Cada vez que você inicia o temporizador, um novo registro é criado no tempo
  tabela de rastreamento
- Cada vez que você parar o relógio, a data final é gravada no tempo
  tabela de rastreamento
- O tempo gasto é arredondado para o trimestre mais próximo (somente para
  Kanboard < 1.0.32)
