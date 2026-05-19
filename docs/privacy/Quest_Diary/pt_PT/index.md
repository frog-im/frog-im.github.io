---
title: Política de Privacidade | QDiary
description: Política de Privacidade do QDiary
---

# Política de Privacidade (QDiary)

- Nome da aplicação: QDiary
- Desenvolvedor: frog-im
- Contacto: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Data de entrada em vigor: 2026-04-19
- Última atualização: 2026-04-19

A presente Política de Privacidade foi elaborada com base na implementação atual da aplicação QDiary. O QDiary disponibiliza funcionalidades de escrita de diário, geração e reflexão de quests, início de sessão, gravação manual na cloud, publicidade e notificações e, nesse processo, poderá tratar dados pessoais ou informações que possam constituir dados pessoais, na medida do necessário.

## 1. Funcionalidades disponibilizadas

O QDiary disponibiliza as seguintes funcionalidades:

- Escrever, editar e visualizar diários
- Classificação por categorias e visualização em calendário
- Geração de quests, reflexão sobre quests e gestão da conclusão de quests
- Bloqueio local da aplicação de diário e encriptação local
- Início de sessão por e-mail, verificação de e-mail, início de sessão anónimo (convidado) e reposição de palavra-passe
- Gravação e carregamento na cloud iniciados pelo utilizador
- Apresentação de anúncios e tratamento de opções de privacidade relacionadas com anúncios
- Notificações de lembrete de quests

## 2. Categorias de informação tratada

### 2-1. Informação introduzida diretamente pelo utilizador

- Endereço de e-mail
- Palavra-passe
- Título, conteúdo, data, categoria e dificuldade do diário
- Respostas a quests, conteúdo de reflexão e informação sobre a quest selecionada
- Valores selecionados relacionados com o perfil da quest e texto de resumo
- Frase-passe para o bloqueio da aplicação de diário

### 2-2. Informação armazenada pela aplicação no dispositivo

- Base de dados local do diário (SQLite)
- Informação sobre o estado das quests dos diários locais
- Valores de estado relacionados com assiduidade, definições, idioma, notificações e anúncios
- Valores de verificação do bloqueio da aplicação, salt e metadados de encriptação
- Informação de agendamento de notificações de quests

### 2-3. Informação de conta e identificação

A seguinte informação poderá ser tratada através do Firebase Authentication:

- Firebase UID
- Endereço de e-mail
- Indicação de que a verificação de e-mail foi concluída
- Indicação de que está a ser utilizado o início de sessão anónimo

### 2-4. Informação de publicidade e consentimento

Ao utilizar o Google AdMob e o SDK UMP, a seguinte informação poderá ser tratada:

- Identificadores de publicidade (como o Android AD_ID)
- Endereço IP e informação de rede
- Informação do dispositivo, versão do sistema operativo e informação da aplicação
- Informação sobre impressões de anúncios, cliques e processamento de recompensas
- Estado do consentimento para publicidade e estado das opções de privacidade

### 2-5. Informação relacionada com notificações

- Indicação de que a permissão de notificações foi concedida
- Valores identificadores de diários que contêm quests em curso
- Texto das notificações de quests
- Horários agendados para notificações

## 3. Finalidades do tratamento

A aplicação trata a informação para as seguintes finalidades:

- Registo, início de sessão, verificação de e-mail e reposição de palavra-passe
- Escrita, gravação e visualização de diários
- Geração de quests, reflexão e determinação de conclusão
- Encriptação e desencriptação locais associadas ao bloqueio da aplicação
- Gravação e carregamento na cloud solicitados pelo utilizador
- Disponibilização de notificações de quests
- Disponibilização de anúncios, processamento de recompensas de anúncios e aplicação do estado de consentimento para publicidade
- Segurança, tratamento de erros e funcionamento do serviço

## 4. Armazenamento local, armazenamento na cloud e tratamento externo

### 4-1. Armazenamento local

A informação de diário e de quests é armazenada principalmente na base de dados local do dispositivo.

- Se o bloqueio da aplicação não estiver ativado: é armazenada localmente de forma geral
- Se o bloqueio da aplicação estiver ativado: alguma informação, como o título do diário, o conteúdo e o estado das quests, poderá ser encriptada e armazenada localmente

### 4-2. Armazenamento na cloud

A aplicação armazena dados no Firebase Firestore apenas quando o utilizador executa diretamente a funcionalidade `Save`.

De acordo com a configuração atual do projeto:

- Não é utilizada sincronização automática completa
- Os dados são armazenados no Firestore `savedDiaries` apenas quando o utilizador os grava manualmente
- No momento da gravação, o título do diário, o conteúdo e o estado das quests poderão ser armazenados de forma encriptada, consoante o estado atual do bloqueio da aplicação
- Os dados são carregados novamente para o armazenamento local apenas quando o utilizador executa `Load`

### 4-3. Tratamento externo para geração e reflexão de quests

Quando o utilizador solicita a geração de uma quest ou uma reflexão, a seguinte informação poderá ser utilizada para tratamento externo através do Firebase Functions:

- Título do diário
- Conteúdo do diário ou conteúdo da reflexão
- Categoria
- Dificuldade
- Quest selecionada
- Informação resumida do perfil da quest

Esta informação é utilizada para a geração e avaliação de quests através da API da OpenAI.

Importante:

- O conteúdo relevante do diário é utilizado para tratamento externo apenas quando a funcionalidade de quest é utilizada.
- De acordo com a configuração atual do projeto, não é utilizado código que armazene registos de quests numa coleção separada chamada `questLogs`.

## 5. Serviços de terceiros e subcontratação de tratamento

### 5-1. Google Firebase

Finalidade:

- Autenticação (Firebase Authentication)
- Armazenamento no Firestore
- Execução de Cloud Functions

Informação que poderá ser tratada:

- UID, endereço de e-mail e estado de autenticação
- Dados do diário gravados manualmente pelo utilizador
- Dados de pedidos de quests

### 5-2. OpenAI

Finalidade:

- Geração de quests
- Reflexão sobre quests e avaliação da sua conclusão

Informação que poderá ser tratada:

- Título/conteúdo do diário
- Texto da quest
- Dificuldade e categoria
- Conteúdo de reflexão introduzido pelo utilizador
- Informação resumida do perfil da quest

### 5-3. Google AdMob / UMP

Finalidade:

- Disponibilização de anúncios em banner, intersticiais e recompensados
- Tratamento do consentimento para publicidade e das opções de privacidade

Informação que poderá ser tratada:

- Identificadores de publicidade
- Informação do dispositivo e da rede
- Informação de interação com anúncios
- Estado do consentimento

## 6. Aviso sobre transferências internacionais

A aplicação poderá tratar dados pessoais ou informação relacionada fora do país do utilizador nos seguintes casos:

| Item | Detalhes |
|---|---|
| Destinatário | Google LLC, OpenAI e operadores de infraestruturas relacionados |
| País de destino | Estados Unidos, etc. |
| Momento da transferência | Durante o início de sessão, geração/reflexão de quests, pedidos de anúncios e tratamento do consentimento |
| Método de transferência | Comunicação de rede encriptada |
| Finalidade da transferência | Autenticação, armazenamento de dados, processamento serverless, geração/avaliação de quests com IA e publicidade |

## 7. Período de conservação e utilização

A aplicação conserva a informação de acordo com os seguintes critérios:

- Informação local do diário/definições: até que o utilizador a elimine ou desinstale a aplicação
- Informação da conta Firebase: enquanto o utilizador mantiver a conta
- Dados armazenados no Firestore: enquanto o utilizador mantiver os itens gravados
- Dados de processamento de pedidos de quests: na medida do necessário para o processamento serverless
- Dados relacionados com anúncios/consentimento: de acordo com a política de cada fornecedor externo

Além disso, o projeto atual inclui a seguinte lógica de limpeza automática:

- Limpeza de contas de utilizadores anónimos e de dados Firestore das subcoleções do utilizador após um determinado período
- Limpeza de contas de utilizadores regulares inativos durante um longo período e de dados Firestore das subcoleções do utilizador

No entanto, a aplicação efetiva desta lógica no ambiente de produção poderá variar consoante o estado da implementação e as definições do servidor.

## 8. Aviso sobre o bloqueio da aplicação e a encriptação local

A aplicação disponibiliza uma funcionalidade separada chamada `Diary App Lock`.

- A frase-passe do bloqueio da aplicação é distinta da palavra-passe da conta.
- A frase-passe do bloqueio da aplicação é utilizada para a encriptação e desencriptação local do diário.
- Mesmo que seja introduzida uma frase-passe incorreta, a própria aplicação poderá não ficar sempre totalmente bloqueada; em vez disso, alguns conteúdos do diário poderão permanecer ilegíveis.
- Alguns diários poderão ser encriptados separadamente com base na frase-passe utilizada no momento da escrita ou do desbloqueio temporário.

Os utilizadores devem manter a sua frase-passe em segurança e, caso a percam, a recuperação de alguns dados locais poderá ser difícil.

## 9. Aviso sobre notificações de quests

Se o utilizador ativar notificações de quests, poderão ser agendadas notificações locais para cada diário com uma quest em curso.

- O agendamento é tratado principalmente pelo sistema interno de agendamento do dispositivo.
- De acordo com a configuração atual do projeto, não existe uma estrutura confirmada em que o texto original do diário seja transmitido periodicamente para um servidor central apenas para fins de notificação.

## 10. Aviso sobre a utilização de permissões

A aplicação poderá utilizar as seguintes permissões para disponibilizar as suas funcionalidades:

- `INTERNET`: comunicação com Firebase, OpenAI e SDKs de publicidade
- `com.google.android.gms.permission.AD_ID`: utilização de identificadores de publicidade
- `POST_NOTIFICATIONS`: apresentação de notificações de quests
- `RECEIVE_BOOT_COMPLETED`: restauro de notificações agendadas após reinício do dispositivo

As permissões são utilizadas apenas na medida necessária para executar as funcionalidades correspondentes.

## 11. Direitos do titular dos dados e forma de exercício

Os utilizadores poderão exercer os seguintes direitos:

- Aceder, modificar e eliminar dados dentro da aplicação
- Eliminar ou sobrescrever dados armazenados na cloud
- Solicitar o fim da sessão e a eliminação da conta
- Alterar as opções de privacidade da publicidade
- Desativar permissões de notificações

Como exercer estes direitos:

- Eliminar ou editar diretamente os diários dentro da aplicação
- Eliminar a aplicação ou repor os dados locais
- Terminar a sessão da conta e solicitar separadamente a eliminação
- Alterar notificações, identificadores de publicidade e permissões nas definições do dispositivo
- E-mail de contacto: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Medidas de segurança

A aplicação aplica ou poderá aplicar as seguintes medidas de proteção:

- Comunicação baseada em HTTPS
- Bloqueio da aplicação de diário local e encriptação
- Armazenamento separado dos valores de verificação da frase-passe
- Utilização de Firebase Authentication
- Pedido do mínimo de permissões necessário

No entanto, poderão surgir riscos consoante o estado de segurança do dispositivo do utilizador, como rooting, jailbreaking, malware ou utilização de dispositivo partilhado.

## 13. Dados pessoais de crianças

A aplicação não foi concebida como um serviço destinado principalmente a crianças. No entanto, opções relacionadas com a idade no UMP poderão ser aplicadas durante o tratamento de anúncios/consentimento.

## 14. Alterações a esta Política

A presente Política poderá ser revista devido a alterações na legislação, nos serviços de terceiros ou nas funcionalidades da aplicação.

- Última atualização da versão atual: **2026-04-19**

## 15. Contacto

- Desenvolvedor: frog-im
- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Guia de eliminação de conta: [Instruções de eliminação](https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog)

