---
title: Política de Privacidade | QDiary
description: Política de Privacidade do QDiary
---

# Política de Privacidade (QDiary)

- Nome do aplicativo: QDiary
- Desenvolvedor: frog-im
- Contato: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Data de vigência: 2026-04-19
- Última atualização: 2026-04-19

Esta Política de Privacidade foi elaborada com base na implementação atual do aplicativo QDiary. O QDiary oferece recursos de escrita de diário, geração e reflexão de quests, login, salvamento manual na nuvem, publicidade e notificações e, nesse processo, pode tratar dados pessoais ou informações que possam constituir dados pessoais, na medida do necessário.

## 1. Recursos oferecidos

O QDiary oferece os seguintes recursos:

- Escrever, editar e visualizar diários
- Classificação por categorias e visualização em calendário
- Geração de quests, reflexão sobre quests e tratamento da conclusão de quests
- Bloqueio local do aplicativo de diário e criptografia local
- Login por e-mail, verificação de e-mail, login anônimo (convidado) e redefinição de senha
- Salvamento e carregamento na nuvem iniciados pelo usuário
- Exibição de anúncios e tratamento das opções de privacidade de anúncios
- Notificações de lembrete de quests

## 2. Categorias de informações tratadas

### 2-1. Informações inseridas diretamente pelo usuário

- Endereço de e-mail
- Senha
- Título, conteúdo, data, categoria e dificuldade do diário
- Respostas de quests, conteúdo de reflexão e informações da quest selecionada
- Seleções relacionadas ao perfil da quest e texto de resumo
- Frase-senha para o bloqueio do aplicativo de diário

### 2-2. Informações armazenadas pelo aplicativo no dispositivo

- Banco de dados local do diário (SQLite)
- Informações de status de quests para diários locais
- Valores de estado relacionados a presença, configurações, idioma, notificações e anúncios
- Valores de verificação do bloqueio do aplicativo, salt e metadados de criptografia
- Informações de agendamento de notificações de quests

### 2-3. Informações de conta e identificação

As seguintes informações podem ser tratadas por meio do Firebase Authentication:

- Firebase UID
- Endereço de e-mail
- Se a verificação de e-mail foi concluída
- Se o login anônimo está sendo utilizado

### 2-4. Informações de publicidade e consentimento

Ao utilizar o Google AdMob e o SDK UMP, as seguintes informações podem ser tratadas:

- Identificadores de publicidade (como Android AD_ID)
- Endereço IP e informações de rede
- Informações do dispositivo, versão do sistema operacional e informações do aplicativo
- Informações sobre impressões de anúncios, cliques e processamento de recompensas
- Status de consentimento para anúncios e status das opções de privacidade

### 2-5. Informações relacionadas a notificações

- Se a permissão de notificação foi concedida
- Valores identificadores de diários que contêm quests em andamento
- Texto da notificação da quest
- Horários programados das notificações

## 3. Finalidades do tratamento

O aplicativo trata informações para as seguintes finalidades:

- Cadastro, login, verificação de e-mail e redefinição de senha
- Escrita, salvamento e visualização de diários
- Geração de quests, reflexão e determinação de conclusão
- Criptografia e descriptografia locais associadas ao bloqueio do aplicativo
- Salvamento e carregamento na nuvem solicitados pelo usuário
- Fornecimento de notificações de quests
- Fornecimento de anúncios, processamento de recompensas de anúncios e aplicação do status de consentimento para anúncios
- Segurança, tratamento de erros e operação do serviço

## 4. Armazenamento local, armazenamento na nuvem e tratamento externo

### 4-1. Armazenamento local

As informações de diário e quests são armazenadas principalmente no banco de dados local do dispositivo.

- Se o bloqueio do aplicativo não estiver ativado: armazenadas localmente em formato geral
- Se o bloqueio do aplicativo estiver ativado: algumas informações, como título do diário, conteúdo e status da quest, podem ser criptografadas e armazenadas localmente

### 4-2. Armazenamento na nuvem

O aplicativo armazena dados no Firebase Firestore somente quando o usuário executa diretamente o recurso `Save`.

De acordo com a configuração atual do projeto:

- Não é utilizada sincronização automática completa
- Os dados são armazenados no Firestore `savedDiaries` somente quando o usuário os salva manualmente
- Quando salvos, o título do diário, o conteúdo e o status da quest podem ser armazenados em formato criptografado, dependendo do status atual do bloqueio do aplicativo
- Os dados são carregados novamente para o armazenamento local somente quando o usuário executa `Load`

### 4-3. Tratamento externo para geração e reflexão de quests

Quando o usuário solicita a geração de uma quest ou uma reflexão, as seguintes informações podem ser utilizadas para tratamento externo por meio do Firebase Functions:

- Título do diário
- Conteúdo do diário ou conteúdo da reflexão
- Categoria
- Dificuldade
- Quest selecionada
- Informações resumidas do perfil da quest

Essas informações são utilizadas para geração e avaliação de quests por meio da API da OpenAI.

Importante:

- O conteúdo relevante do diário é utilizado para tratamento externo somente quando o recurso de quest é utilizado.
- De acordo com a configuração atual do projeto, não é utilizado código que armazene logs de quests em uma coleção separada chamada `questLogs`.

## 5. Serviços de terceiros e tratamento terceirizado

### 5-1. Google Firebase

Finalidade:

- Autenticação (Firebase Authentication)
- Armazenamento no Firestore
- Execução do Cloud Functions

Informações que podem ser tratadas:

- UID, endereço de e-mail e status de autenticação
- Dados de diário salvos manualmente pelo usuário
- Dados de solicitação de quest

### 5-2. OpenAI

Finalidade:

- Geração de quests
- Reflexão sobre quests e avaliação de conclusão

Informações que podem ser tratadas:

- Título/conteúdo do diário
- Texto da quest
- Dificuldade e categoria
- Conteúdo de reflexão inserido pelo usuário
- Informações resumidas do perfil da quest

### 5-3. Google AdMob / UMP

Finalidade:

- Fornecimento de anúncios em banner, intersticiais e recompensados
- Tratamento do consentimento para anúncios e das opções de privacidade

Informações que podem ser tratadas:

- Identificadores de publicidade
- Informações do dispositivo e da rede
- Informações de interação com anúncios
- Status de consentimento

## 6. Aviso sobre transferência internacional

O aplicativo pode tratar dados pessoais ou informações relacionadas fora do país do usuário nos seguintes casos:

| Item | Detalhes |
|---|---|
| Destinatário | Google LLC, OpenAI e operadores de infraestrutura relacionados |
| País de destino | Estados Unidos, etc. |
| Momento da transferência | Durante o login, a geração/reflexão de quests, as solicitações de anúncios e o tratamento do consentimento |
| Método de transferência | Comunicação de rede criptografada |
| Finalidade da transferência | Autenticação, armazenamento de dados, processamento serverless, geração/avaliação de quests por IA e publicidade |

## 7. Período de retenção e uso

O aplicativo retém as informações de acordo com os seguintes critérios:

- Informações locais de diário/configurações: até que o usuário as exclua ou desinstale o aplicativo
- Informações da conta Firebase: enquanto o usuário mantiver a conta
- Dados armazenados no Firestore: enquanto o usuário mantiver os itens salvos
- Dados de processamento de solicitações de quests: na medida necessária para o processamento serverless
- Dados relacionados a anúncios/consentimento: de acordo com a política de cada fornecedor externo

Além disso, o projeto atual inclui a seguinte lógica de limpeza automática:

- Limpeza de contas de usuários anônimos e de dados do Firestore em subcoleções do usuário após determinado período
- Limpeza de contas de usuários regulares inativos por longo período e de dados do Firestore em subcoleções do usuário

No entanto, se isso é efetivamente refletido no ambiente de produção pode variar dependendo do status de implantação e das configurações do servidor.

## 8. Aviso sobre bloqueio do aplicativo e criptografia local

O aplicativo oferece um recurso separado chamado `Diary App Lock`.

- A frase-senha do bloqueio do aplicativo é separada da senha da conta.
- A frase-senha do bloqueio do aplicativo é utilizada para a criptografia e descriptografia local do diário.
- Mesmo que uma frase-senha incorreta seja inserida, o próprio aplicativo pode não ficar totalmente bloqueado em todos os casos; em vez disso, alguns conteúdos do diário podem permanecer ilegíveis.
- Alguns diários podem ser criptografados separadamente com base na frase-senha utilizada no momento da escrita ou do desbloqueio temporário.

Os usuários devem manter sua frase-senha em segurança e, se ela for perdida, a recuperação de alguns dados locais pode ser difícil.

## 9. Aviso sobre notificações de quests

Se o usuário ativar as notificações de quests, notificações locais podem ser programadas para cada diário com uma quest em andamento.

- O agendamento é tratado principalmente pelo sistema interno de agendamento do dispositivo.
- De acordo com a configuração atual do projeto, não há estrutura confirmada em que o texto-fonte do diário seja transmitido periodicamente para um servidor central exclusivamente para fins de notificação.

## 10. Aviso sobre uso de permissões

O aplicativo pode utilizar as seguintes permissões para oferecer seus recursos:

- `INTERNET`: comunicação com Firebase, OpenAI e SDKs de anúncios
- `com.google.android.gms.permission.AD_ID`: uso de identificadores de publicidade
- `POST_NOTIFICATIONS`: exibição de notificações de quests
- `RECEIVE_BOOT_COMPLETED`: restauração de notificações programadas após a reinicialização do dispositivo

As permissões são utilizadas somente na medida necessária para executar as funções correspondentes.

## 11. Direitos do titular dos dados e como exercê-los

Os usuários podem exercer os seguintes direitos:

- Acessar, modificar e excluir dados dentro do aplicativo
- Excluir ou sobrescrever dados armazenados na nuvem
- Solicitar logout e exclusão da conta
- Alterar as opções de privacidade de anúncios
- Desativar permissões de notificação

Como exercer esses direitos:

- Excluir ou editar diretamente os diários dentro do aplicativo
- Excluir o aplicativo ou redefinir os dados locais
- Fazer logout da conta e solicitar a exclusão separadamente
- Alterar notificações, identificadores de publicidade e permissões nas configurações do dispositivo
- E-mail de contato: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Medidas de segurança

O aplicativo aplica ou pode aplicar as seguintes medidas de proteção:

- Comunicação baseada em HTTPS
- Bloqueio local do aplicativo de diário e criptografia
- Armazenamento separado dos valores de verificação da frase-senha
- Uso do Firebase Authentication
- Solicitação do mínimo necessário de permissões

No entanto, podem surgir riscos dependendo do estado de segurança do dispositivo do usuário, como root, jailbreak, malware ou uso de dispositivo compartilhado.

## 13. Dados pessoais de crianças

O aplicativo não foi projetado como um serviço destinado principalmente a crianças. No entanto, opções relacionadas à idade dentro do UMP podem ser aplicadas durante o tratamento de anúncios/consentimento.

## 14. Alterações nesta Política

Esta Política pode ser revisada em razão de alterações nas leis, nos serviços de terceiros ou nos recursos do aplicativo.

- Última atualização da versão atual: **2026-04-19**

## 15. Contato

- Desenvolvedor: frog-im
- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

