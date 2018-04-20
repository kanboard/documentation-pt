Notificações
============

Kanboard é capaz de enviar notificações através de vários canais:

- Email
- Web (lista de mensagens não lidas)

Plugins externos permitem que você envie notificações para o Slack, Hipchat,
Jabber ou qualquer sistema de chat.

Configuração
------------

Cada usuário deve ativar as notificações em seu perfil: **Perfil do usuário
> Notificações**. Está desativado por padrão.

Para receber notificações por e-mail, você precisa de um endereço de e-mail
válido em seu perfil e o aplicativo deve ser configurado para enviar emails.

.. figure:: /_static/notifications.png
   :alt: Notificações

Você pode escolher seu método de notificação favorito:

- Emails
- Web (veja abaixo)

Para cada projeto você é um membro, você pode optar por receber notificações
para:

- Todas as tarefas
- Apenas para tarefas atribuídas a você
- Apenas para tarefas criadas por você
- Somente para tarefas criadas por você e atribuídas a você

Você também pode selecionar apenas alguns projetos. Por padrão, todos os projetos
onde você é um membro.

Notificações pela Web
---------------------

As notificações da Web estão disponíveis no painel ou no ícone no topo:

.. figure:: /_static/web-notifications-icon.png
   :alt: ícone de notificações da Web

As notificações são mostradas em uma lista, para que você possa marcar
notificação como lido ou tudo.

.. figure:: /_static/web-notifications.png
   :alt: Notificações da Web

Desta forma, você ainda pode ser notificado sem ter que receber e-mails.

Menções do usuário
------------------

O Kanboard oferece a possibilidade de enviar notificações quando alguém
mencionado.

Se você precisar chamar a atenção de alguém em um comentário ou em uma tarefa,
use o símbolo @ seguido do nome de usuário. Kanboard será automaticamente
sugerir uma lista de usuários:

.. figure:: /_static/user-mentions.png
   :alt: Menção do usuário

- No momento, apenas a descrição da tarefa e a área de texto do comentário
  tem esse recurso ativado.
- O usuário menciona funciona apenas durante a criação de tarefas e comentários.
- Para ser notificado, os usuários mencionados precisam ser membros do projeto.
- Quando alguém é mencionado, esse usuário receberá uma notificação.
- A menção @username está vinculada ao perfil do usuário público.

A notificação é enviada de acordo com as configurações do usuário, pode ser uma
e-mail, uma notificação na web ou até mesmo uma mensagem no Slack/Hipchat/Jabber
se você instalou os plugins corretos.
