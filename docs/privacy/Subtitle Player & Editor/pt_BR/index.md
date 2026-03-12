---
title: Política de Privacidade | Subtitle Tool
description: Política de Privacidade do Subtitle Tool (Subtitle Player & Editor) - Português (Brasil)
lang: pt-BR
last_updated: 2026-03-11
---

# Política de Privacidade (Subtitle Tool / Subtitle Player & Editor)

- **Nome do app:** Subtitle Player & Editor (também referido como **Subtitle Tool** nesta Política)
- **Desenvolvedor:** frog-im
- **Contato:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data de vigência:** 2026-03-11

> Esta Política foi elaborada com referência às leis aplicáveis, incluindo a Lei Coreana de Proteção de Informações Pessoais (PIPA), o GDPR / UK GDPR, a Swiss FADP e leis estaduais de privacidade relevantes dos EUA. Se regras locais obrigatórias se aplicarem, essas regras prevalecerão.

---

## 1. Finalidade e Escopo

Este app oferece:

- Reprodução e edição de legendas
- Reprodução de vídeo + legenda a partir de arquivos selecionados pelo usuário
- Sobreposição flutuante de legendas / letras exibida sobre outros apps no Android

O tratamento de legendas compatível pode incluir formatos como:

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

O app **não** cria uma conta de usuário e **não** envia arquivos de legenda ou mídia do usuário para os servidores próprios do desenvolvedor. A análise, edição, visualização prévia de legendas e a maior parte do processamento relacionado à reprodução são realizados **localmente no dispositivo**.

No entanto, para publicidade, gerenciamento de consentimento e conformidade legal, SDKs de terceiros como **Google Mobile Ads SDK (AdMob)** e **Google UMP** podem processar determinadas informações, como identificadores de publicidade, sinais do dispositivo e escolhas de consentimento.

---

## 2. Categorias de Informações que Processamos

### 2-1) Arquivos Explicitamente Escolhidos pelo Usuário

O app interage com arquivos explicitamente selecionados pelo usuário, incluindo:

- **Arquivos de legenda**
  - Exemplos: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Usos:
    - Reprodução de legendas dentro do app
    - Edição de legendas
    - Exibição de legendas em sobreposição
    - Conversão e exportação de legendas

- **Arquivos de mídia**
  - Exemplos: arquivos locais de vídeo ou áudio escolhidos pelo usuário
  - Usos:
    - Reprodução de vídeo + legenda
    - Alinhamento do tempo da sobreposição com a mídia em reprodução

Pontos importantes:

- Os arquivos selecionados pelo usuário são processados localmente no dispositivo.
- O app não envia esses arquivos para os servidores próprios do desenvolvedor.
- Os caminhos e conteúdos dos arquivos são usados apenas para reprodução, sobreposição, edição, salvamento e ações solicitadas pelo usuário.

### 2-2) Configurações Locais e Valores Armazenados

Para fornecer configurações persistentes e restaurar o estado anterior, o app armazena alguns valores localmente no dispositivo usando `SharedPreferences` ou armazenamento local semelhante fornecido pelo sistema operacional.

Esses valores não são enviados aos servidores próprios do desenvolvedor e normalmente são removidos se os dados do app forem apagados ou se o app for desinstalado.

#### (1) Configurações de sobreposição

Os exemplos incluem:

- `overlay_box_x`
- `overlay_box_y`
- `overlay_text_font`
- `overlay_text_color`
- `overlay_outline_enabled`
- `overlay_outline_color`
- `overlay_outline_width`
- `overlay_force_landscape`
- `overlay_interstitial_count`

Finalidade:

- Restaurar a posição da sobreposição
- Restaurar o estilo da legenda para a sobreposição e para a reprodução de legendas dentro do app
- Manter preferências de contorno / fonte / orientação
- Controlar a lógica de frequência de exibição de anúncios em alguns fluxos relacionados à sobreposição

#### (2) Posições recentes de reprodução ou sobreposição

Os exemplos incluem:

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Finalidade:

- Restaurar ou sugerir posições iniciais recentes de legenda/sobreposição
- Retomar a reprodução de vídeo + legenda de forma mais conveniente

#### (3) Valores de preferência de anúncios e privacidade

Os exemplos podem incluir:

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Finalidade:

- Armazenar escolhas de privacidade relacionadas a anúncios
- Aplicar configurações de privacidade e anúncios do UMP / AdMob

#### (4) Saída de legenda criada pelo usuário

Quando o usuário salva ou exporta arquivos de legenda, o app pode gravar novos arquivos de legenda em um local selecionado pelo usuário, como:

- Downloads
- Outra pasta selecionada por meio de um seletor do sistema
- Um local de armazenamento gerenciado pelo usuário

Esses arquivos salvos pelo usuário podem permanecer no dispositivo após a exclusão do app, a menos que o usuário os apague manualmente.

#### (5) Arquivos temporários e cache

O app e bibliotecas de terceiros podem criar arquivos temporários ou de cache para o funcionamento normal, como:

- dados de cache do seletor de arquivos
- dados temporários de conversão de legenda
- dados de cache relacionados à reprodução

Esses arquivos destinam-se apenas ao funcionamento local e não são enviados aos servidores próprios do desenvolvedor.

#### (6) Cache do estado de consentimento do UMP

Nas regiões em que o Google UMP se aplica, o SDK pode armazenar localmente no dispositivo o estado de consentimento em cache.

Isso geralmente pode ser redefinido por meio de:

- limpeza dos dados do app, ou
- alteração das escolhas de consentimento dentro do app, quando houver uma entrada disponível de opções de privacidade

### 2-3) Processamento Relacionado à Sobreposição Android e Permissões

No Android, a sobreposição flutuante de legenda pode usar:

- a permissão `SYSTEM_ALERT_WINDOW` / exibir sobre outros apps
- a permissão `POST_NOTIFICATIONS`
- uma notificação de serviço em primeiro plano necessária para o serviço de sobreposição

Finalidade:

- exibir a sobreposição de legenda sobre outros apps
- manter o serviço de sobreposição em execução
- permitir que o Android exiba as notificações necessárias de sobreposição / serviço
- ler informações de notificações de mídia quando necessário para suporte à progressão das legendas

Essas permissões são usadas apenas para recursos do app que o usuário escolhe usar.

### 2-4) Anúncios, Consentimento e Dados Relacionados (SDKs de Terceiros)

O app usa SDKs de anúncios / consentimento do Google, incluindo:

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

O app pode exibir:

- anúncios em banner
- anúncios intersticiais
- anúncios recompensados ou intersticiais recompensados

Esses SDKs podem processar dados como:

- identificadores de publicidade (por exemplo, AAID / IDFA, quando aplicável)
- informações baseadas em IP e relacionadas à rede
- metadados do dispositivo e do app
- sinais de interação com anúncios
- escolhas de consentimento

As finalidades podem incluir:

- exibição de anúncios
- medição e relatórios de anúncios
- limitação de frequência
- prevenção de fraude
- conformidade legal

O desenvolvedor busca configurar esses SDKs de forma consistente com as escolhas de consentimento do usuário e com a legislação aplicável.

---

## 3. Como Processamos e Retemos os Dados

- **Configurações locais e dados de posição recente**
  - retidos no dispositivo até que os dados do app sejam apagados ou o app seja removido

- **Arquivos temporários / cache**
  - retidos apenas pelo tempo necessário para a operação, sendo depois removidos pelo app quando isso for viável na prática ou limpos posteriormente pelo sistema operacional

- **Arquivos de legenda salvos pelo usuário**
  - permanecem no local de salvamento escolhido pelo usuário até serem apagados por ele

- **Dados de anúncios / consentimento tratados por terceiros**
  - retidos de acordo com as políticas do Google e com a legislação aplicável

---

## 4. Processamento por Terceiros e Transferências Internacionais

Para anúncios e gerenciamento de consentimento, algumas informações podem ser processadas pelo Google e parceiros relacionados.

| Item | Detalhes |
|---|---|
| Destinatário | Google LLC e afiliadas / operadores relacionados |
| Finalidade | Exibição de anúncios, medição, prevenção de fraude, gerenciamento de consentimento e conformidade legal |
| Dados possíveis | Identificadores de publicidade, informações do dispositivo/app, informações baseadas em IP, dados de interação com anúncios, estado de consentimento |
| Destino | Estados Unidos e outras regiões onde a infraestrutura do Google opera |
| Retenção | De acordo com as políticas do Google e com a legislação aplicável |

O desenvolvedor busca manter as divulgações de privacidade na loja de apps consistentes com o comportamento real dos SDKs.

---

## 5. Seus Direitos e Escolhas

Dependendo da sua jurisdição, você pode ter direitos como:

- acesso
- correção
- exclusão
- restrição
- portabilidade
- objeção
- retirada do consentimento quando o consentimento for a base legal

Os controles práticos incluem:

- alterar escolhas de anúncios / privacidade no app, quando disponíveis
- apagar os dados do app para remover configurações locais e preferências armazenadas em cache
- desinstalar o app
- apagar manualmente arquivos de legenda exportados do armazenamento do usuário
- usar controles no nível do sistema operacional, como configurações de notificações, redefinição do ID de publicidade ou configurações de personalização de anúncios

Para dados processados pelo Google, os usuários também devem consultar, quando relevante, as próprias ferramentas de privacidade e conta do Google.

---

## 6. Privacidade Infantil

Este app não é destinado principalmente a crianças.

Sua principal finalidade é a reprodução de legendas, edição, exibição em sobreposição e recursos utilitários relacionados. Quando apropriado, a configuração dos SDKs de anúncios pode aplicar sinalizadores relacionados à idade ou voltados para crianças, em conformidade com os requisitos da plataforma e as configurações do desenvolvedor.

---

## 7. Medidas de Segurança

Dentro dos limites da arquitetura do app, o desenvolvedor busca:

- minimizar a coleta mantendo a maior parte do processamento de legendas e mídia no dispositivo
- usar seletores de arquivos do sistema e acesso a arquivos iniciado pelo usuário
- usar permissões do sistema com transparência
- contar com o transporte de rede criptografado utilizado por SDKs de terceiros, quando aplicável

Nenhum método de armazenamento ou transmissão é perfeitamente seguro, mas o app foi projetado para evitar coleta desnecessária pelo desenvolvedor.

---

## 8. Software de Código Aberto

O app usa software de código aberto, incluindo bibliotecas relacionadas a:

- análise e serialização de legendas
- seleção de arquivos
- preferências locais
- janelas de sobreposição
- reprodução de vídeo
- WebView

Avisos de código aberto estão disponíveis dentro do app. Para alguns componentes, o app pode usar uma cópia localmente modificada de um pacote de código aberto, preservando o aviso de licença original.

---

## 9. Contato

Se você tiver dúvidas ou solicitações relacionadas à privacidade:

- **E-mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Inclua o nome do app **Subtitle Player & Editor** em sua mensagem.

---

## 10. Alterações nesta Política

Esta Política pode ser atualizada se:

- os recursos do app mudarem
- as permissões ou o uso dos SDKs mudarem
- os requisitos legais ou da plataforma mudarem

Alterações relevantes serão refletidas na página atualizada da política e, quando apropriado, no app.
