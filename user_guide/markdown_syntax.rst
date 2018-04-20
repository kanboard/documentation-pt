Sintaxe do Markdown
===================

O Kanboard usa a `Sintaxe Markdown
<http://en.wikipedia.org/wiki/Markdown>`__ para comentários ou descrições
de tarefas. Aqui estão alguns exemplos:

Negrito e itálico
-----------------

- Texto em negrito: use 2 asteriscos ou 2 sublinhados
- Texto em itálico: use 1 asterisco ou 1 sublinhado

Fonte
~~~~~

::

    Essa **palavra** é muito __importante__ .

    E aqui, uma palavra em *itálico* com _sublinhado_.

Resultado
~~~~~~~~~

Esta **palavra** é muito **importante**.

E aqui, uma palavra em *itálico* com *sublinhado*.

Listas não ordenadas
--------------------

Lista não ordenada pode usar asteriscos, menos ou mais.

.. _source-1:

Fonte
~~~~~

::

    - Item 1
    - Item 2
    - Item 3

    ou

    * Item 1
    * Item 2
    * Item 3

.. _result-1:

Resultado
~~~~~~~~~

- Item 1
- Item 2
- Item 3

Listas ordenadas
----------------

Listas ordenadas são prefixadas por um número como esse:

.. _source-2:

Fonte
~~~~~

::

    1. Faça isso primeiro
    2. Faça isso
    3. E isso

.. _result-2:

Resultado
~~~~~~~~~

1. Faça isso primeiro
2. Faça isso
3. E isso

Links
-----

.. _source-3:

Fonte
~~~~~

::

    [Título do meu link] (https://kanboard.org/)

    <https://kanboard.org>

.. _result-3:

Resultado
~~~~~~~~~

`Título do meu link <https://kanboard.org/>`__

https://kanboard.org

Código fonte
------------

Código embutido
~~~~~~~~~~~~~~~

Use uma crase.

::

    Execute este comando: `tail -f / var / log / messages`.

.. _result-4:

Resultado
~~~~~~~~~

Execute este comando: ``tail -f / var / log / messages``.

Blocos de Código
~~~~~~~~~~~~~~~~

Use 3 crases com eventualmente o nome da linguagem.

.. raw:: html

   <pre>
   <code class="language-markdown">```php
   &lt;?php

   phpinfo();

   ?&gt;
   ```
   </code>
   </pre>

.. _result-5:

Resultado
~~~~~~~~~

::

    <?php

    phpinfo();

    ?>

Títulos
-------

.. _source-4:

Fonte
~~~~~

::

  # Nível de título 1

  ## nível de título 2

  ### nível de título 3
