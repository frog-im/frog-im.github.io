---
title: Política de Privacidade | LyriFloat
description: Política de Privacidade do LyriFloat (Português - Portugal)
lang: pt-pt
last_updated: 2025-10-30
---

# Política de Privacidade (LyriFloat)

- **Nome da aplicação:** LyriFloat  
- **Programador/Developer:** frog-im  
- **Contacto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Data de entrada em vigor:** 2025-10-30  

> Esta Política foi redigida com referência a leis aplicáveis, incluindo a Lei Coreana de Proteção de Informações Pessoais (PIPA), o GDPR/UK GDPR, a FADP suíça e leis estaduais relevantes dos EUA. Se existirem requisitos específicos por jurisdição, esses requisitos prevalecem.

---

## 1. Finalidade e âmbito

Esta aplicação disponibiliza **edição de metadados de ficheiros de áudio** (título, artista, etc.) guardados no dispositivo e funcionalidades de **sobreposição de letras (lyrics overlay)**.  
A aplicação **não cria conta de utilizador** e **não carrega conteúdo do utilizador** para qualquer servidor. O processamento é feito, por defeito, **no dispositivo do utilizador**.

No entanto, para efeitos de **publicidade** e **conformidade legal**, parceiros terceiros (por exemplo, Google Mobile Ads SDK (AdMob) e UMP) podem recolher e tratar informações como **identificadores de publicidade**. A recolha de consentimento e as escolhas de privacidade seguem as especificações da **Google UMP (User Messaging Platform)**, com disponibilização do ponto de entrada de **“opções de privacidade”** quando aplicável.

---

## 2. Categorias de informações que tratamos

### 2-1) Ficheiros escolhidos explicitamente pelo utilizador
- **Caminhos e conteúdos de áudio/capa:** tratados **localmente** no dispositivo apenas para edição/guardar.  
- O **FFmpegKit** é utilizado localmente para codificação, edição de metadados e extração de miniaturas.  
- A aplicação **não carrega** os ficheiros selecionados pelo utilizador para os nossos servidores.

### 2-2) Definições locais e valores armazenados

Para funcionamento e conveniência, a aplicação guarda os seguintes valores **localmente no dispositivo**.  
Estes valores não são enviados para os nossos servidores e são **removidos quando a aplicação ou os respetivos dados são eliminados**.

#### (1) Preferências (`shared_preferences`)
| Tipo | Chave/Conteúdo | Finalidade | Armazenamento | Eliminação |
|---|---|---|---|---|
| Posição/fonte do overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Restaurar posição do overlay e tamanho da fonte | SharedPreferences do dispositivo | Removido ao eliminar dados da app ou ao desinstalar |
| Definições de Ads/Privacidade | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Anúncios não personalizados, RDP (EUA), tag COPPA, tag de idade, limite de classificação de conteúdo | SharedPreferences do dispositivo | Igual ao lado |

#### (2) Ficheiros temporários (diretório temporário do sistema)
- **Exemplos:** `cover_*.jpg`, `tmp_*.flac`  
- **Utilização:** extração de capa, tagging FLAC, codificação temporária  
- **Localização:** pasta temporária do sistema (`systemTemp`)  
- **Retenção:** removidos pela app quando possível após concluir; também sujeitos à limpeza do sistema

#### (3) Guardar escolhido pelo utilizador (SAF)
- Quando o utilizador escolhe “Guardar como”, os ficheiros finais podem ser escritos em locais definidos pelo utilizador (por ex., Transferências, cloud).  
- Estes ficheiros ficam em **armazenamento externo** e **permanecem após a desinstalação**. O utilizador pode eliminá-los manualmente.

#### (4) Estado de consentimento (cache do UMP SDK)
- Em regiões EEE/Reino Unido/Suíça, o UMP SDK **armazena localmente em cache** o estado de consentimento do utilizador para anúncios.  
- Pode ser reposto ao eliminar dados da app ou através do ecrã de **“Opções de privacidade”** na aplicação, quando disponível.

---

### 2-3) Dados relacionados com anúncios e consentimento (SDKs de terceiros)
- **Google Mobile Ads SDK (AdMob) e UMP** podem recolher/tratar, por exemplo: **identificadores de publicidade (AAID/IDFA)**, **intervalos de IP**, **informação do dispositivo/app**, **sinais de interação com anúncios**, **estado de consentimento**, etc.  
- **Finalidades:** apresentação de anúncios, limitação de frequência, prevenção de fraude, medição de desempenho, conformidade legal  
- **Regiões que exigem consentimento (EEE/UK/CH):** o consentimento é recolhido via UMP e é fornecido um ponto de entrada de **“Opções de privacidade”** quando exigido.  
  Em regiões sem essa exigência (por ex., KR), a opção **pode não ser apresentada**.

---

## 3. Tratamento e retenção

- **Definições locais:** guardadas no dispositivo até o utilizador eliminar dados da app ou desinstalar  
- **Ficheiros temporários:** criados durante codificação/extração, eliminados após o processamento ou podem permanecer temporariamente em caches do sistema  
- **Dados de anúncios/consentimento (terceiros):** retidos e eliminados de acordo com as **políticas da Google**

---

## 4. Transferências para terceiros e fluxos internacionais

Para publicidade e gestão de consentimento, informações do utilizador podem ser transmitidas e tratadas na infraestrutura da Google.

| Item | Detalhes |
|---|---|
| **Destinatário** | Google LLC e as suas afiliadas/subprocessadores |
| **Destino** | Estados Unidos (e outras regiões onde exista infraestrutura da Google) |
| **Finalidade** | Apresentação de anúncios, medição/desempenho, conformidade legal, gestão de consentimento |
| **Dados** | Identificadores de publicidade, intervalos de IP, info do dispositivo/app, interações com anúncios, estado de consentimento, etc. |
| **Retenção** | De acordo com as políticas da Google |
| **Efeito da recusa** | Anúncios personalizados podem ser limitados; podem ser apresentados anúncios não personalizados |

Cumprimos os requisitos de divulgação do **Data safety do Google Play** e mantemos as informações alinhadas com o tratamento efetivo.

---

## 5. Os seus direitos e como exercê-los

- **Desativar anúncios personalizados / alterar consentimento**  
  - Regiões suportadas (EEE/UK/CH): alterar em **Definições → Opções de privacidade**.  
  - Outras regiões: usar as definições do sistema para **repor IDs de anúncios / limitar rastreio**.  
- **Repor informações locais:** eliminar dados da app ou desinstalar repõe coordenadas do overlay, tamanho da fonte e outras definições locais.  
- Direitos ao abrigo do **GDPR/UK GDPR/FADP suíça/leis estaduais dos EUA** (acesso, retificação, apagamento, portabilidade, limitação, retirada do consentimento, etc.) podem ser exercidos conforme previsto.  
  Para dados de anúncios tratados pela Google, use os **processos da Google**.

---

## 6. Privacidade de crianças

Esta aplicação **não se destina a crianças**. Se uma criança abaixo da idade mínima legal usar a aplicação, deve parar e usar funcionalidades do sistema para limitar anúncios com um responsável. Quando apropriado, podemos aplicar **TFUA (tag de serviço dirigido a crianças)** ou opções semelhantes.

---

## 7. Medidas de segurança

- **Minimização** na recolha e armazenamento  
- Utilização **limitada** de ficheiros temporários e tentativas de eliminação após o processamento  
- Tratamento estritamente dentro do âmbito de permissões do sistema  
- Encriptação em trânsito via **TLS ou equivalente** para transferências de terceiros (conforme padrões dos SDKs)

---

## 8. Data Safety (Google Play)

Mantemos a secção **Data safety** na Play Console de forma precisa e atualizamo-la prontamente quando houver alterações.

---

## 9. Avisos de código aberto

A aplicação utiliza software de código aberto como o **FFmpeg**. Um ficheiro informativo (por ex., `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) na aplicação explica como obter o código-fonte. Mediante pedido, forneceremos o código conforme indicado nesse ficheiro.

---

## 10. Contacto

- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Alterações a esta Política

Podemos rever esta Política devido a alterações legais ou de serviço. Publicaremos atualizações **na aplicação** e nesta **página de política**.  
Para alterações materiais, forneceremos aviso com **pelo menos 7 dias** de antecedência da data de entrada em vigor.

---

## Apêndice: Orientação ao utilizador

- **Link na app:** abrir esta página em **Definições → Privacidade**.  
- **Comportamento regional:** no EEE/UK/CH, são mostradas Opções de privacidade. **Na Coreia (KR) e nalgumas outras regiões, o botão pode não mostrar opções adicionais** quando não for exigido por lei.
