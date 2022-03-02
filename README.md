# friends-gallery-frontend

- upload de fotos
- galeria unificada
- aprovar as fotos antes de ser visível para todos
- apenas sendo aprovados pelo casal (admins)
- usuários deve ser possível curtir e comentar as fotos

-- fotos serem salvas em Amazon AWS S3
front-end - Vue.js

cada casal receber um código de sua galeria de fotos
= Tela *Login*
  = Tela do código e senha da galeria de fotos
  = Dentro da tela vai ter um botão de criar código de galeria de fotos
  = é gerado um código aleatório ou um código específico que o usuário escreveu
  = pegar email e senha para administrador, podendo adicionar outros administradores posteriormente
  = encaminhar usuário para tela home

= Tela *Home*
  = se o campo de nickname estiver vazio pedir ao usuario o seu nickname para a galeria
  = se o usuario for admin
    = header
      = logo do site
      = notificações de aprovações de fotos
      = configurações para editar o nickname, email, senha. E adicionar novos admins
    = body
      = local para uploads de fotos
      = feed de fotos aprovadas pelos admins
        = curtir as fotos
        = comentar as fotos

  se o usuario nao for admin
    = header
      = logo do site

    = body
      = local para uploads de fotos
      = feed de fotos aprovadas pelos admins
        = curtir as fotos
        = comentar as fotos

= Tela *Notificações*
  = se o usuario for admin
    = header
      = logo do site
      = notificações de aprovações de fotos
      = configurações para editar o nickname, email, senha. E adicionar novos admins
    = body
      = todos as requisições para aprovação das fotos

= Tela *Configurações*

= se o usuario for admin
    = header
      = logo do site
      = notificações de aprovações de fotos
      = configurações para editar o nickname, email, senha. E adicionar novos admins
    = body
      = Editar nickname
      = editar email
      = editar senha
      = add novos admins