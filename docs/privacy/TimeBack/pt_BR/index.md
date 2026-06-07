---
title: Política de Privacidade | TimeBack
description: Política de Privacidade TimeBack
lang: pt-BR
last_updated: 2026-06-06
---

# Política de Privacidade (TimeBack)

- **Nome do aplicativo:** TimeBack
- **Desenvolvedor:** frog-im
- **Contato:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data de vigência:** 03/06/2026
- **Última atualização:** 06/06/2026

Esta Política de Privacidade é baseada na implementação atual do aplicativo TimeBack. O TimeBack fornece revisão do tempo de tela, metas diárias, registros de tempo recuperado, reflexões, desafios, notificações, compartilhamento e recursos de publicidade.

## 1. Recursos

TimeBack oferece os seguintes recursos:

- Revisão do tempo de uso do aplicativo por meio da permissão de acesso de uso do Android
- Metas de uso diário, lembretes e notificações de uso da barra de status
- Notificações de aviso com limite máximo e exibição de sobreposição
- Seleção de aplicativo de exceção de sobreposição
- Registros de atividades de tempo recuperado
- Registros diários de reflexão
- Desafie o progresso e o gerenciamento da lista de verificação
- Compartilhamento de imagens com estatísticas de uso
- Anúncios da Google AdMob e opções de privacidade baseadas em UMP

## 2. Informações que processamos

### 2-1. Permissão de acesso de uso de leitura de informações

Se o usuário conceder permissão `PACKAGE_USAGE_STATS` ao Android, o aplicativo poderá ler as seguintes informações do dispositivo:

- Nome do pacote de aplicativos
- Nome do aplicativo
- Tempo de uso do aplicativo
- Intervalo de data e hora usado para agregação de uso

Essas informações são usadas para fornecer estatísticas de uso e comparar o uso com as metas do usuário.

### 2-2. Informações inseridas ou configuradas pelo usuário

- Meta de uso diário
- Estado e intervalo habilitados para lembrete de uso
- Configuração de exibição de uso da barra de status
- Categoria, título, horário de início e duração da atividade de tempo recuperado
- Texto de reflexão diária
- Progresso do desafio e entradas da lista de verificação
- Lista de aplicativos de exceção de sobreposição

### 2-3. Informações armazenadas no dispositivo

O aplicativo pode armazenar as seguintes informações em um banco de dados SQLite local ou SharedPreferences:

- Registros de tempo de uso do aplicativo
- Metas e configurações diárias
- Registros de atividades de tempo recuperado
- Registros diários de reflexão
- Progresso do desafio e estado da lista de verificação
- Estado de conclusão da integração
- Configurações como lembretes de uso, avisos de limite máximo, exibição da barra de status e aplicativos de exceção de sobreposição
- Consentimento de anúncio local e estado da opção de privacidade

Com base na implementação atual, esses registros locais não são carregados automaticamente nos servidores frog-im.

### 2-4. Dados de publicidade e consentimento

Quando os anúncios para celular do Google SDK (AdMob) e UMP são usados, o Google ou suas afiliadas podem processar informações como:

- Identificadores de publicidade, como Android AD_ID
- IP endereço e informações de rede
- Informações do dispositivo, versão OS e informações do aplicativo
- Impressões de anúncios, cliques, dados de medição e sinais de erro
- Consentimento do anúncio e estado da opção de privacidade
- Localização aproximada

## 3. Finalidades do Processamento

O aplicativo processa informações para os seguintes fins:

- Ler o tempo de uso, mostrar estatísticas e comparar o uso com as metas
- Armazenando registros de tempo recuperado e de reflexão inseridos pelo usuário
- Gerenciando o progresso do desafio
- Fornecimento de lembretes e notificações na barra de status
- Fornecimento de notificações de aviso de limite máximo, exibição de sobreposição e tratamento de exceções de sobreposição
- Compartilhando imagens de estatísticas de uso quando solicitado pelo usuário
- Veicular anúncios, medir o desempenho dos anúncios e aplicar opções de consentimento de anúncios
- Manter a estabilidade do aplicativo e responder a erros

## 4. Armazenamento local e processamento externo

### 4-1. Armazenamento local

O TimeBack armazena dados do usuário principalmente no armazenamento interno do aplicativo no dispositivo. Com base na implementação atual, registros de uso, metas, reflexões e informações de desafio não são carregados automaticamente nos servidores frog-im.

O armazenamento local pode incluir o seguinte.

| Armazenar | Itens armazenados | Propósito | Método de exclusão |
|---|---|---|---|
| SQLite banco de dados | Registros de uso de aplicativos, nomes de pacotes, nomes de aplicativos, tempo de uso, agregados baseados em data | Mostre estatísticas de uso e compare o uso com as metas | Recursos de exclusão no aplicativo, limpeza de dados do aplicativo ou desinstalação do aplicativo |
| SQLite banco de dados | Atividades de tempo recuperado, reflexões, progresso do desafio, entradas na lista de verificação | Mostre registros e gerencie o progresso | Recursos de exclusão no aplicativo, limpeza de dados do aplicativo ou desinstalação do aplicativo |
| Preferências Compartilhadas | Estado de conclusão da integração, configurações de lembrete, configurações de aviso de limite máximo, configurações de exibição da barra de status, lista de aplicativos de exceção de sobreposição, estado de consentimento de anúncio local | Manter as configurações do aplicativo | Limpando dados do aplicativo ou desinstalando o aplicativo |
| Arquivos/cache temporários | Imagens de estatísticas de uso compartilhadas e arquivos temporários semelhantes | Realizar compartilhamento solicitado pelo usuário | Excluído após compartilhamento sempre que possível ou de acordo com as políticas de limpeza de OS/app |

Quando o usuário limpa os dados do aplicativo ou o desinstala, os dados armazenados no armazenamento interno do aplicativo geralmente são excluídos. No entanto, backup do Android, backup do fabricante, backup na nuvem ou arquivos compartilhados diretamente pelo usuário podem ser retidos separadamente de acordo com as políticas desses serviços.

Os registros de uso e o texto de reflexão podem revelar rotinas ou interesses pessoais. Em dispositivos compartilhados, os usuários devem usar proteções apropriadas, como bloqueio de dispositivo ou contas OS separadas.

### 4-2. Carregamentos de servidor

Com base no projeto atual, o TimeBack não carrega automaticamente registros de uso, reflexões ou registros de desafio para servidores frog-im. Caso o usuário utilize o recurso de compartilhamento, uma imagem estatística gerada poderá ser transferida para o aplicativo ou serviço externo selecionado pelo usuário.

### 4-3. Processamento de Publicidade

Google AdMob e UMP são usados ​​para publicidade no aplicativo e gerenciamento de consentimento. As informações relacionadas à publicidade podem ser processadas na infraestrutura do Google.

## 5. Serviços e Processadores de Terceiros

### 5-1. Google AdMob/UMP

Propósito:

- Entrega de banner
- Consentimento de anúncios e tratamento de opções de privacidade
- Medição de desempenho de anúncios e prevenção de fraudes

Informações que podem ser processadas:

- Identificadores de publicidade
- Informações do dispositivo e da rede
- Informações de interação com anúncios
- Consentimento e estado da opção de privacidade

### 5-2. Compartilhando aplicativos ou serviços de destino

Se o usuário usar diretamente o recurso de compartilhamento de imagem de estatísticas de uso, o aplicativo ou serviço externo selecionado poderá processar a imagem compartilhada. Esse processamento é regido pela política de privacidade do serviço selecionado.

## 6. Aviso de transferência transfronteiriça

As informações podem ser processadas fora do país do usuário nos seguintes casos.

| Item | Detalhes |
|---|---|
| Destinatário | Google LLC e suas afiliadas |
| Destino | Estados Unidos e outros países/regiões onde a infraestrutura do Google está localizada |
| Tempo | Quando o aplicativo é executado, solicita anúncios, exibe ou avalia anúncios, processa cliques ou processa consentimento |
| Método | Comunicação de rede criptografada (HTTPS/TLS) |
| Propósito | Entrega de anúncios, tratamento de estado de personalização, medição, análise, melhoria de estabilidade de serviço, conformidade legal |
| Dados | Identificadores de publicidade, informações de dispositivo/aplicativo/rede, informações de interação com anúncios, estado de consentimento, localização aproximada, etc. |
| Retenção | De acordo com as políticas do Google e a legislação aplicável |

Para obter detalhes, consulte [Cross-Border Transfer Notice](./policy/).

## 7. Lista de aplicativos instalados e exceções de sobreposição

No Android, se o usuário configurar aplicativos de exceção de sobreposição, o aplicativo poderá ler os nomes dos pacotes e dos aplicativos inicializáveis ​​no dispositivo para exibir uma lista de seleção. Os nomes de pacotes selecionados pelo usuário como exceções são armazenados em SharedPreferences no dispositivo e são usados ​​apenas para evitar a exibição de sobreposições de aviso de limite máximo sobre esses aplicativos.

## 8. Retenção

O aplicativo retém informações de acordo com os seguintes padrões:

- Informações locais sobre uso, meta, reflexão e desafio: até que o usuário exclua, limpe os dados do aplicativo ou desinstale o aplicativo
- Configurações de SharedPreferences: até que o usuário limpe os dados do aplicativo ou desinstale o aplicativo
- Arquivos temporários para imagens compartilhadas: conforme necessário para compartilhamento ou de acordo com as políticas de limpeza OS
- Dados relacionados a publicidade e consentimento: de acordo com as políticas do Google e de outros terceiros relevantes

## 9. Permissões

O aplicativo pode usar as seguintes permissões:

- `PACKAGE_USAGE_STATS`: leia o tempo de uso do aplicativo
- `POST_NOTIFICATIONS`: mostra lembretes de uso e notificações na barra de status
- `SYSTEM_ALERT_WINDOW`: mostra sobreposições de aviso de limite máximo
- `INTERNET`: comunicar-se com anúncios SDKs e mostrar páginas de aviso legal
- `ACCESS_NETWORK_STATE`: verifica o estado da rede
- `com.google.android.gms.permission.AD_ID`: use identificadores de publicidade

As permissões são usadas apenas conforme necessário para recursos do aplicativo. Os usuários podem revogar permissões nas configurações do dispositivo, mas os recursos relacionados podem ser limitados.

## 10. Direitos e escolhas do usuário

Os usuários podem:

- Visualize, edite ou exclua registros dentro do aplicativo
- Exclua informações locais limpando os dados do aplicativo ou desinstalando o aplicativo
- Alterar as configurações de acesso de uso, notificação e identificador de publicidade nas configurações do dispositivo
- Revogar a permissão de sobreposição e alterar as configurações do aplicativo de exceção de sobreposição
- Alterar opções de privacidade de anúncios
- Contate-nos com perguntas sobre privacidade ou solicitações de exclusão

E-mail de contato: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Medidas de segurança

O aplicativo aplica ou pode aplicar as seguintes salvaguardas:

- Comunicação externa baseada em HTTPS/TLS
- Processamento de dados local
- Solicitações mínimas de permissão necessárias para recursos do aplicativo
- Aplicação do estado de consentimento de publicidade

Condições de segurança do dispositivo, como root, jailbreak, malware ou uso de dispositivos compartilhados, podem criar riscos adicionais.

## 12. Privacidade das Crianças

O TimeBack não foi projetado principalmente para crianças. As configurações relacionadas à idade ou as políticas da plataforma dos anúncios para celular do Google SDK e UMP podem ser aplicadas durante o processamento de publicidade e consentimento.

## 13. Mudanças

Esta Política pode ser atualizada devido a alterações na lei, na configuração de serviços de terceiros ou nos recursos do aplicativo. Mudanças materiais serão notificadas por meio de aviso no aplicativo ou atualizando esta página.

## 14. Contato

- Desenvolvedor: frog-im
- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
