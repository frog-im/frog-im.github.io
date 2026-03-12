---
title: Política de Privacidade | Subtitle Tool
description: Política de Privacidade do Subtitle Tool (Subtitle Player & Editor) - Português (Portugal)
lang: pt-PT
last_updated: 2026-03-11
---

# Política de Privacidade (Subtitle Tool / Subtitle Player & Editor)

- **Nome da aplicação:** Subtitle Player & Editor (também referido como **Subtitle Tool** nesta Política)
- **Programador:** frog-im
- **Contacto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data de entrada em vigor:** 2026-03-11

> Esta Política foi preparada com referência às leis aplicáveis, incluindo a Lei Coreana de Proteção de Informações Pessoais (PIPA), o RGPD / UK GDPR, a FADP suíça e as leis estaduais relevantes de privacidade dos EUA. Se se aplicarem regras locais obrigatórias, essas regras prevalecem.

---

## 1. Finalidade e Âmbito

Esta aplicação disponibiliza:

- Reprodução e edição de legendas
- Reprodução de vídeo + legendas a partir de ficheiros selecionados pelo utilizador
- Sobreposição flutuante de legendas / letras apresentada sobre outras aplicações no Android

O tratamento de legendas suportado pode incluir formatos como:

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

A aplicação **não** cria uma conta de utilizador e **não** carrega os ficheiros de legendas ou multimédia do utilizador para os servidores próprios do programador. A análise, edição, pré-visualização de legendas e a maior parte do processamento relacionado com a reprodução são efetuados **localmente no dispositivo**.

No entanto, para publicidade, gestão de consentimento e conformidade legal, SDKs de terceiros como o **Google Mobile Ads SDK (AdMob)** e o **Google UMP** podem processar determinadas informações, tais como identificadores publicitários, sinais do dispositivo e escolhas de consentimento.

---

## 2. Categorias de Informações que Processamos

### 2-1) Ficheiros Explicitamente Escolhidos pelo Utilizador

A aplicação interage com ficheiros explicitamente selecionados pelo utilizador, incluindo:

- **Ficheiros de legendas**
  - Exemplos: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Utilizações:
    - Reprodução de legendas dentro da aplicação
    - Edição de legendas
    - Apresentação de legendas em sobreposição
    - Conversão e exportação de legendas

- **Ficheiros multimédia**
  - Exemplos: ficheiros locais de vídeo ou áudio escolhidos pelo utilizador
  - Utilizações:
    - Reprodução de vídeo + legendas
    - Alinhamento temporal da sobreposição com o conteúdo multimédia atualmente em reprodução

Pontos importantes:

- Os ficheiros selecionados pelo utilizador são processados localmente no dispositivo.
- A aplicação não carrega esses ficheiros para os servidores próprios do programador.
- Os caminhos e conteúdos dos ficheiros são utilizados apenas para reprodução, sobreposição, edição, gravação e ações solicitadas pelo utilizador.

### 2-2) Definições Locais e Valores Armazenados

Para disponibilizar definições persistentes e restaurar o estado anterior, a aplicação armazena alguns valores localmente no dispositivo utilizando `SharedPreferences` ou armazenamento local semelhante fornecido pelo sistema operativo.

Estes valores não são enviados para os servidores próprios do programador e são normalmente removidos se os dados da aplicação forem apagados ou se a aplicação for desinstalada.

#### (1) Definições da sobreposição

Exemplos incluem:

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
- Restaurar o estilo das legendas para a sobreposição e para a reprodução de legendas na aplicação
- Manter preferências de contorno / tipo de letra / orientação
- Controlar a lógica de frequência de apresentação de anúncios em alguns fluxos relacionados com a sobreposição

#### (2) Posições recentes de reprodução ou sobreposição

Exemplos incluem:

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Finalidade:

- Restaurar ou sugerir posições iniciais recentes de legendas/sobreposição
- Retomar a reprodução de vídeo + legendas de forma mais conveniente

#### (3) Valores de preferência de anúncios e privacidade

Os exemplos podem incluir:

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Finalidade:

- Armazenar escolhas de privacidade relativas a anúncios
- Aplicar definições de privacidade e configuração de anúncios do UMP / AdMob

#### (4) Saída de legendas criada pelo utilizador

Quando o utilizador guarda ou exporta ficheiros de legendas, a aplicação pode escrever novos ficheiros de legendas num local selecionado pelo utilizador, como por exemplo:

- Transferências
- Outra pasta selecionada através de um seletor do sistema
- Um local de armazenamento gerido pelo utilizador

Estes ficheiros guardados pelo utilizador podem permanecer no dispositivo após a eliminação da aplicação, salvo se o utilizador os apagar manualmente.

#### (5) Ficheiros temporários e cache

A aplicação e bibliotecas de terceiros podem criar ficheiros temporários ou de cache para o funcionamento normal, tais como:

- dados de cache do seletor de ficheiros
- dados temporários de conversão de legendas
- dados de cache relacionados com a reprodução

Estes destinam-se apenas ao funcionamento local e não são carregados para os servidores próprios do programador.

#### (6) Cache do estado de consentimento UMP

Nas regiões em que o Google UMP se aplica, o SDK pode armazenar localmente no dispositivo o estado do consentimento em cache.

Isto pode geralmente ser reposto através de:

- limpeza dos dados da aplicação, ou
- alteração das escolhas de consentimento dentro da aplicação, quando estiver disponível uma entrada de opções de privacidade

### 2-3) Processamento Relacionado com a Sobreposição Android e Permissões

No Android, a sobreposição flutuante de legendas pode utilizar:

- a permissão `SYSTEM_ALERT_WINDOW` / mostrar sobre outras aplicações
- a permissão `POST_NOTIFICATIONS`
- uma notificação de serviço em primeiro plano necessária para o serviço de sobreposição

Finalidade:

- apresentar a sobreposição de legendas sobre outras aplicações
- manter o serviço de sobreposição em execução
- permitir que o Android apresente as notificações necessárias de sobreposição / serviço
- ler informações de notificações multimédia quando necessário para suporte à progressão das legendas

Estas permissões são utilizadas apenas para funcionalidades da aplicação que o utilizador escolhe utilizar.

### 2-4) Anúncios, Consentimento e Dados Relacionados (SDKs de Terceiros)

A aplicação utiliza SDKs de anúncios / consentimento da Google, incluindo:

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

A aplicação pode apresentar:

- anúncios de banner
- anúncios intersticiais
- anúncios recompensados ou intersticiais recompensados

Estes SDKs podem processar dados como:

- identificadores publicitários (por exemplo, AAID / IDFA, quando aplicável)
- informações baseadas em IP e relacionadas com a rede
- metadados do dispositivo e da aplicação
- sinais de interação com anúncios
- escolhas de consentimento

As finalidades podem incluir:

- apresentação de anúncios
- medição e relatórios de anúncios
- limitação de frequência
- prevenção de fraude
- conformidade legal

O programador procura configurar estes SDKs de forma consistente com as escolhas de consentimento do utilizador e com a legislação aplicável.

---

## 3. Como Processamos e Conservamos os Dados

- **Definições locais e dados de posição recente**
  - conservados no dispositivo até que os dados da aplicação sejam apagados ou a aplicação seja removida

- **Ficheiros temporários / cache**
  - conservados apenas durante o tempo necessário para o funcionamento, sendo depois removidos pela aplicação quando praticável ou limpos mais tarde pelo sistema operativo

- **Ficheiros de legendas guardados pelo utilizador**
  - permanecem no local de gravação escolhido pelo utilizador até serem apagados pelo mesmo

- **Dados de anúncios / consentimento tratados por terceiros**
  - conservados de acordo com as políticas da Google e com a legislação aplicável

---

## 4. Processamento por Terceiros e Transferências Transfronteiriças

Para anúncios e gestão do consentimento, algumas informações podem ser processadas pela Google e por parceiros relacionados.

| Item | Detalhes |
|---|---|
| Destinatário | Google LLC e afiliadas / subcontratantes relacionados |
| Finalidade | Apresentação de anúncios, medição, prevenção de fraude, gestão do consentimento e conformidade legal |
| Dados possíveis | Identificadores publicitários, informações do dispositivo/aplicação, informações baseadas em IP, dados de interação com anúncios, estado de consentimento |
| Destino | Estados Unidos e outras regiões onde a infraestrutura da Google opera |
| Conservação | De acordo com as políticas da Google e com a legislação aplicável |

O programador procura manter as divulgações de privacidade na loja de aplicações consistentes com o comportamento real dos SDKs.

---

## 5. Os Seus Direitos e Escolhas

Dependendo da sua jurisdição, poderá ter direitos como:

- acesso
- retificação
- eliminação
- limitação
- portabilidade
- oposição
- retirada do consentimento quando o consentimento for a base legal

Os controlos práticos incluem:

- alterar escolhas de anúncios / privacidade na aplicação, quando disponíveis
- limpar os dados da aplicação para remover definições locais e preferências em cache
- desinstalar a aplicação
- eliminar manualmente ficheiros de legendas exportados do armazenamento do utilizador
- utilizar controlos ao nível do sistema operativo, tais como definições de notificações, reposição do ID de anúncios ou definições de personalização de anúncios

Para os dados processados pela Google, os utilizadores também devem consultar as ferramentas de privacidade e conta da própria Google, quando relevante.

---

## 6. Privacidade das Crianças

Esta aplicação não se destina principalmente a crianças.

O seu principal objetivo é a reprodução de legendas, edição, apresentação em sobreposição e funcionalidades utilitárias relacionadas. Quando apropriado, a configuração dos SDKs de anúncios pode aplicar sinalizadores relacionados com a idade ou direcionados a crianças, em conformidade com os requisitos da plataforma e com as definições do programador.

---

## 7. Medidas de Segurança

Dentro dos limites da arquitetura da aplicação, o programador procura:

- minimizar a recolha, mantendo a maior parte do processamento de legendas e multimédia no dispositivo
- utilizar seletores de ficheiros do sistema e acesso a ficheiros iniciado pelo utilizador
- utilizar permissões do sistema de forma transparente
- depender, quando aplicável, do transporte de rede cifrado utilizado pelos SDKs de terceiros

Nenhum método de armazenamento ou transmissão é completamente seguro, mas a aplicação foi concebida para evitar a recolha desnecessária por parte do programador.

---

## 8. Software de Código Aberto

A aplicação utiliza software de código aberto, incluindo bibliotecas relacionadas com:

- análise e serialização de legendas
- seleção de ficheiros
- preferências locais
- janelas de sobreposição
- reprodução de vídeo
- WebView

Os avisos de código aberto estão disponíveis dentro da aplicação. Para alguns componentes, a aplicação pode utilizar uma cópia modificada localmente de um pacote de código aberto, preservando o aviso de licença original.

---

## 9. Contacto

Se tiver questões ou pedidos relacionados com privacidade:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Inclua o nome da aplicação **Subtitle Player & Editor** na sua mensagem.

---

## 10. Alterações a esta Política

Esta Política pode ser atualizada se:

- as funcionalidades da aplicação mudarem
- as permissões ou a utilização dos SDKs mudarem
- os requisitos legais ou da plataforma mudarem

As alterações materiais serão refletidas na página de política atualizada e, quando apropriado, na aplicação.
