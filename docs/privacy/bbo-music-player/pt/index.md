---
title: Política de Privacidade | LyriFloat
description: Política de Privacidade do LyriFloat (Português)
lang: pt
last_updated: 2025-10-30
---

# Política de Privacidade (LyriFloat)

- **Nome do app:** LyriFloat  
- **Desenvolvedor:** frog-im  
- **Contato:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Data de vigência:** 2025-10-30  

> Esta Política foi elaborada com base em leis aplicáveis, incluindo a Lei de Proteção de Informações Pessoais da Coreia (PIPA), o GDPR/UK GDPR, a FADP suíça e leis estaduais relevantes de privacidade dos EUA. Caso existam requisitos específicos por jurisdição, esses requisitos prevalecem.

---

## 1. Finalidade e Escopo

Este app oferece **edição de metadados de arquivos de áudio** (título, artista etc.) armazenados no dispositivo e recursos de **sobreposição/flutuação de letras (lyrics overlay)**.  
O app **não cria conta de usuário** e **não envia conteúdo do usuário** para nenhum servidor. O processamento ocorre **no dispositivo do usuário**, por padrão.

No entanto, para fins de **publicidade** e **conformidade legal**, parceiros terceirizados (por exemplo, Google Mobile Ads SDK (AdMob) e UMP) podem coletar e processar informações como **identificadores de publicidade**. A coleta de consentimento e as escolhas de privacidade seguem as especificações do **Google UMP (User Messaging Platform)**, com disponibilização do ponto de entrada de **“opções de privacidade”** quando aplicável.

---

## 2. Categorias de Informações que Processamos

### 2-1) Arquivos explicitamente escolhidos pelo usuário
- **Caminhos e conteúdos de áudio/capa:** processados **localmente** no dispositivo apenas para edição/salvamento.  
- O **FFmpegKit** é usado localmente para codificação, edição de metadados e extração de miniaturas.  
- O app **não faz upload** dos arquivos selecionados pelo usuário para nossos servidores.

### 2-2) Configurações locais e valores armazenados

Para funcionamento e conveniência, o app armazena os seguintes valores **localmente no dispositivo**.  
Esses valores não são enviados aos nossos servidores e são **removidos quando o app ou os dados do app são excluídos**.

#### (1) Preferências (`shared_preferences`)
| Tipo | Chave/Conteúdo | Finalidade | Armazenamento | Exclusão |
|---|---|---|---|---|
| Posição/fonte do overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Restaurar posição do overlay e tamanho da fonte | SharedPreferences do dispositivo | Removido ao excluir dados do app ou desinstalar |
| Configs de Ads/Privacidade | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Anúncios não personalizados, RDP (EUA), tag COPPA, tag de idade, limite de classificação de conteúdo | SharedPreferences do dispositivo | Igual ao lado |

#### (2) Arquivos temporários (diretório temporário do sistema)
- **Exemplos:** `cover_*.jpg`, `tmp_*.flac`  
- **Uso:** extração de capa, tagging FLAC, codificação temporária  
- **Local:** pasta temporária do sistema (`systemTemp`)  
- **Retenção:** removidos pelo app quando possível após concluir; também sujeitos à limpeza do sistema

#### (3) Salvamento escolhido pelo usuário (SAF)
- Ao escolher “Salvar como”, arquivos finais podem ser gravados em locais definidos pelo usuário (ex.: Downloads, nuvem).  
- Esses arquivos ficam no **armazenamento externo** e **permanecem após a desinstalação**. O usuário pode excluí-los manualmente.

#### (4) Estado de consentimento (cache do UMP SDK)
- Em regiões EEE/Reino Unido/Suíça, o UMP SDK **armazena em cache localmente** o estado de consentimento do usuário para anúncios.  
- Pode ser redefinido ao excluir dados do app ou pela tela de **“Opções de privacidade”** no app, quando disponível.

---

### 2-3) Dados relacionados a anúncios e consentimento (SDKs de terceiros)
- **Google Mobile Ads SDK (AdMob) e UMP** podem coletar/processar, por exemplo: **identificadores de publicidade (AAID/IDFA)**, **faixas de IP**, **info do dispositivo/app**, **sinais de interação com anúncios**, **estado de consentimento** etc.  
- **Finalidades:** veiculação de anúncios, controle de frequência, prevenção de fraude, medição de desempenho, conformidade legal  
- **Regiões que exigem consentimento (EEE/UK/CH):** o consentimento é coletado via prompts do UMP e um ponto de entrada de **“Opções de privacidade”** é fornecido quando exigido.  
  Em regiões sem essa exigência (ex.: KR), a opção **pode não ser exibida**.

---

## 3. Processamento e Retenção

- **Configurações locais:** permanecem até o usuário excluir dados do app ou desinstalar  
- **Arquivos temporários:** criados durante codificação/extração; excluídos após o processamento ou podem ficar temporariamente em caches do sistema  
- **Dados de anúncios/consentimento (terceiros):** retidos e descartados conforme as **políticas do Google**

---

## 4. Transferências para terceiros e fluxos internacionais

Para publicidade e gestão de consentimento, informações do usuário podem ser transmitidas e processadas na infraestrutura do Google.

| Item | Detalhes |
|---|---|
| **Destinatário** | Google LLC e suas afiliadas/subprocessadores |
| **Destino** | Estados Unidos (e outras regiões onde há infraestrutura do Google) |
| **Finalidade** | Veiculação de anúncios, medição/desempenho, conformidade legal, gestão de consentimento |
| **Dados** | Identificadores de publicidade, faixas de IP, info do dispositivo/app, interações com anúncios, estado de consentimento etc. |
| **Retenção** | Conforme as políticas do Google |
| **Efeito da recusa** | Anúncios personalizados podem ser limitados; anúncios não personalizados podem ser exibidos |

Cumprimos os requisitos de divulgação do **Data safety do Google Play** e mantemos as informações alinhadas ao processamento real.

---

## 5. Seus direitos e como exercê-los

- **Desativar anúncios personalizados / alterar consentimento**  
  - Regiões compatíveis (EEE/UK/CH): altere em **Configurações → Opções de privacidade**.  
  - Outras regiões: use as configurações do sistema para **redefinir IDs de anúncios / limitar rastreamento**.  
- **Redefinir informações locais:** excluir dados do app ou desinstalar redefine coordenadas do overlay, fonte e outras preferências locais.  
- Direitos sob **GDPR/UK GDPR/FADP suíça/leis estaduais dos EUA** (acesso, retificação, exclusão, portabilidade, restrição, retirada do consentimento etc.) podem ser exercidos conforme essas leis.  
  Para dados de anúncios processados pelo Google, utilize os **processos do Google**.

---

## 6. Privacidade de crianças

Este app **não é direcionado a crianças**. Se uma criança abaixo da idade mínima legal usar o app, deve parar e usar recursos do sistema para limitar anúncios com um responsável. Quando apropriado, podemos aplicar **TFUA (tag de serviço direcionado a crianças)** ou opções semelhantes.

---

## 7. Medidas de segurança

- **Minimização** de coleta e armazenamento  
- Uso **limitado** de arquivos temporários e tentativas de exclusão após o processamento  
- Processamento estritamente dentro do escopo de permissões do sistema  
- Criptografia em trânsito via **TLS ou equivalente** para transferências de terceiros (conforme padrões dos SDKs)

---

## 8. Data Safety (Google Play)

Mantemos a seção **Data safety** do Play Console de forma precisa e a atualizamos rapidamente quando houver mudanças.

---

## 9. Avisos de código aberto

O app usa software de código aberto como o **FFmpeg**. Um arquivo informativo (ex.: `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) no app explica como obter o código-fonte. Mediante solicitação, forneceremos o código conforme instruído nesse arquivo.

---

## 10. Contato

- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Alterações nesta Política

Podemos revisar esta Política devido a mudanças legais ou de serviço. Publicaremos atualizações **no app** e nesta **página de política**.  
Para mudanças materiais, avisaremos com **pelo menos 7 dias** de antecedência da data de vigência.

---

## Apêndice: Guia do usuário

- **Link no app:** abra esta página em **Configurações → Privacidade**.  
- **Comportamento regional:** no EEE/UK/CH, “Opções de privacidade” são exibidas. **Na Coreia (KR) e em algumas outras regiões, o botão pode não mostrar opções adicionais** quando não for legalmente exigido.
