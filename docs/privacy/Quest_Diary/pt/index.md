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

Esta Política de Privacidade foi elaborada com base na implementação atual da aplicação QDiary. O QDiary fornece funcionalidades de escrita de diário, geração e reflexão de quests, início de sessão, gravação manual na cloud, publicidade e notificações e, nesse processo, poderá tratar dados pessoais ou informações que possam constituir dados pessoais, na medida do necessário.

## 1. Funcionalidades disponibilizadas

O QDiary disponibiliza as seguintes funcionalidades:

- Escrever, editar e visualizar diários
- Classificação por categorias e visualização em calendário
- Geração de quests, reflexão sobre quests e gestão de conclusão de quests
- Bloqueio local da aplicação de diário e encriptação local
- Início de sessão por e-mail, verificação de e-mail, início de sessão anónimo (convidado) e reposição de palavra-passe
- Gravação e carregamento na cloud iniciados pelo utilizador
- Apresentação de anúncios e tratamento de opções de privacidade relacionadas com anúncios
- Notificações de lembrete de quests

## 2. Categorias de informações tratadas

### 2-1. Informações introduzidas diretamente pelo utilizador

- Endereço de e-mail
- Palavra-passe
- Título, conteúdo, data, categoria e dificuldade do diário
- Respostas de quests, conteúdo de reflexão e informações sobre a quest selecionada
- Valores selecionados relacionados com o perfil da quest e texto de resumo
- Frase-passe para o bloqueio da aplicação de diário

### 2-2. Informações armazenadas pela aplicação no dispositivo

- Base de dados local do diário (SQLite)
- Informações de estado de quests dos diários locais
- Valores de estado relacionados com presença, definições, idioma, notificações e anúncios
- Valores de verificação do bloqueio da aplicação, salt e metadados de encriptação
- Informações de agendamento de notificações de quests

### 2-3. Informações de conta e identificação

As seguintes informações podem ser tratadas através do Firebase Authentication:

- Firebase UID
- Endereço de e-mail
- Se a verificação de e-mail foi concluída
- Se está a ser utilizado o início de sessão anónimo

### 2-4. Informações de publicidade e consentimento

Ao utilizar o Google AdMob e o SDK UMP, as seguintes informações podem ser tratadas:

- Identificadores de publicidade (como Android AD_ID)
- Endereço IP e informações de rede
- Informações do dispositivo, versão do sistema operativo e informações da aplicação
- Informações sobre impressões de anúncios, cliques e processamento de recompensas
- Estado do consentimento para publicidade e estado das opções de privacidade

### 2-5. Informações relacionadas com notificações

- Se a permissão de notificações foi concedida
- Valores identificadores de diários que contêm quests em curso
- Texto das notificações de quests
- Horários agendados das notificações

## 3. Finalidades do tratamento

A aplicação trata informações para as seguintes finalidades:

- Registo, início de sessão, verificação de e-mail e reposição de palavra-passe
- Escrita, gravação e visualização de diários
- Geração de quests, reflexão e determinação de conclusão
- Encriptação e desencriptação locais associadas ao bloqueio da aplicação
- Gravação e carregamento na cloud solicitados pelo utilizador
- Fornecimento de notificações de quests
- Fornecimento de anúncios, processamento de recompensas de anúncios e aplicação do estado de consentimento para publicidade
- Segurança, tratamento de erros e operação do serviço

## 4. Armazenamento local, armazenamento na cloud e tratamento externo

### 4-1. Armazenamento local

As informações de diário e de quests são armazenadas principalmente na base de dados local do dispositivo.

- Se o bloqueio da aplicação não estiver ativado: são armazenadas localmente em formato geral
- Se o bloqueio da aplicação estiver ativado: algumas informações, como o título do diário, o conteúdo e o estado das quests, podem ser encriptadas e armazenadas localmente

### 4-2. Armazenamento na cloud

A aplicação armazena dados no Firebase Firestore apenas quando o utilizador executa diretamente a funcionalidade `Save`.

De acordo com a configuração atual do projeto:

- Não é utilizada sincronização automática completa
- Os dados são armazenados no Firestore `savedDiaries` apenas quando o utilizador os grava manualmente
- Ao serem gravados, o título do diário, o conteúdo e o estado das quests podem ser armazenados em formato encriptado, dependendo do estado atual do bloqueio da aplicação
- Os dados são carregados novamente para o armazenamento local apenas quando o utilizador executa `Load`

### 4-3. Tratamento externo para geração e reflexão de quests

Quando o utilizador solicita a geração de uma quest ou uma reflexão, as seguintes informações podem ser utilizadas para tratamento externo através do Firebase Functions:

- Título do diário
- Conteúdo do diário ou conteúdo da reflexão
- Categoria
- Dificuldade
- Quest selecionada
- Informações resumidas do perfil da quest

Estas informações são utilizadas para geração e avaliação de quests através da API da OpenAI.

Importante:

- O conteúdo relevante do diário é utilizado para tratamento externo apenas quando a funcionalidade de quest é utilizada.
- De acordo com a configuração atual do projeto, não é utilizado código que armazene registos de quests numa coleção separada chamada `questLogs`.

## 5. Serviços de terceiros e tratamento subcontratado

### 5-1. Google Firebase

Finalidade:

- Autenticação (Firebase Authentication)
- Armazenamento no Firestore
- Execução de Cloud Functions

Informações que podem ser tratadas:

- UID, endereço de e-mail e estado de autenticação
- Dados do diário gravados manualmente pelo utilizador
- Dados de pedidos de quests

### 5-2. OpenAI

Finalidade:

- Geração de quests
- Reflexão sobre quests e avaliação de conclusão

Informações que podem ser tratadas:

- Título/conteúdo do diário
- Texto da quest
- Dificuldade e categoria
- Conteúdo de reflexão introduzido pelo utilizador
- Informações resumidas do perfil da quest

### 5-3. Google AdMob / UMP

Finalidade:

- Fornecimento de anúncios em banner, intersticiais e com recompensa
- Tratamento do consentimento para publicidade e das opções de privacidade

Informações que podem ser tratadas:

- Identificadores de publicidade
- Informações do dispositivo e da rede
- Informações de interação com anúncios
- Estado do consentimento

## 6. Aviso sobre transferências internacionais

A aplicação pode tratar dados pessoais ou informações relacionadas fora do país do utilizador nos seguintes casos:

| Item | Detalhes |
|---|---|
| Destinatário | Google LLC, OpenAI e operadores de infraestruturas relacionados |
| País de destino | Estados Unidos, etc. |
| Momento da transferência | Durante o início de sessão, geração/reflexão de quests, pedidos de anúncios e tratamento de consentimento |
| Método de transferência | Comunicação de rede encriptada |
| Finalidade da transferência | Autenticação, armazenamento de dados, processamento serverless, geração/avaliação de quests com IA e publicidade |

## 7. Período de conservação e utilização

A aplicação conserva as informações de acordo com os seguintes critérios:

- Informações locais do diário/definições: até que o utilizador as elimine ou desinstale a aplicação
- Informações da conta Firebase: enquanto o utilizador mantiver a conta
- Dados armazenados no Firestore: enquanto o utilizador mantiver os itens gravados
- Dados de processamento de pedidos de quests: na medida do necessário para o processamento serverless
- Dados relacionados com anúncios/consentimento: de acordo com a política de cada fornecedor externo

Além disso, o projeto atual inclui a seguinte lógica de limpeza automática:

- Limpeza de contas de utilizadores anónimos e de dados Firestore das subcoleções do utilizador após um determinado período
- Limpeza de contas de utilizadores regulares inativos por um longo período e de dados Firestore das subcoleções do utilizador

No entanto, a aplicação efetiva desta lógica no ambiente de produção pode variar consoante o estado da implementação e as definições do servidor.

## 8. Aviso sobre o bloqueio da aplicação e a encriptação local

A aplicação disponibiliza uma funcionalidade separada chamada `Diary App Lock`.

- A frase-passe do bloqueio da aplicação é distinta da palavra-passe da conta.
- A frase-passe do bloqueio da aplicação é utilizada para a encriptação e desencriptação local do diário.
- Mesmo que seja introduzida uma frase-passe incorreta, a própria aplicação poderá não ficar sempre totalmente bloqueada; em vez disso, alguns conteúdos do diário poderão permanecer ilegíveis.
- Alguns diários podem ser encriptados separadamente com base na frase-passe utilizada no momento da escrita ou do desbloqueio temporário.

Os utilizadores devem manter a sua frase-passe em segurança e, caso a percam, a recuperação de alguns dados locais poderá ser difícil.

## 9. Aviso sobre notificações de quests

Se o utilizador ativar notificações de quests, poderão ser agendadas notificações locais para cada diário com uma quest em curso.

- O agendamento é tratado principalmente pelo sistema interno de agendamento do dispositivo.
- De acordo com a configuração atual do projeto, não existe uma estrutura confirmada em que o texto original do diário seja transmitido periodicamente para um servidor central apenas para fins de notificação.

## 10. Aviso sobre a utilização de permissões

A aplicação pode utilizar as seguintes permissões para fornecer as suas funcionalidades:

- `INTERNET`: comunicação com Firebase, OpenAI e SDKs de publicidade
- `com.google.android.gms.permission.AD_ID`: utilização de identificadores de publicidade
- `POST_NOTIFICATIONS`: apresentação de notificações de quests
- `RECEIVE_BOOT_COMPLETED`: restauro de notificações agendadas após reinício do dispositivo

As permissões são utilizadas apenas na medida necessária para executar as funcionalidades correspondentes.

## 11. Direitos do titular dos dados e forma de exercício

Os utilizadores podem exercer os seguintes direitos:

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

Esta Política poderá ser revista devido a alterações na legislação, nos serviços de terceiros ou nas funcionalidades da aplicação.

- Última atualização da versão atual: **2026-04-19**

## 15. Contacto

- Desenvolvedor: frog-im
- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

