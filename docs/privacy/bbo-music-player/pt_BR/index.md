---
title: Política de Privacidade | Lyrics Overlay & Tag Editorr
description: Política de Privacidade do Lyrics Overlay & Tag Editorr (Português do Brasil)
lang: pt_BR
last_updated: 2025-10-30
---

# Política de Privacidade (Lyrics Overlay & Tag Editorr)

- **Nome do app:** Lyrics Overlay & Tag Editorr  
- **Desenvolvedor:** frog-im  
- **Contato:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data de vigência:** 2025-10-30

> Esta Política foi elaborada com referência às leis aplicáveis, incluindo a Lei de Proteção de Informações Pessoais da Coreia (PIPA), o GDPR/UK GDPR, a Lei Federal Suíça de Proteção de Dados (FADP) e leis estaduais de privacidade dos EUA. Em caso de exigências específicas por jurisdição, essas exigências prevalecem.

---

## 1. Finalidade e escopo

Este app oferece **edição de metadados** (título, artista etc.) de arquivos de áudio **armazenados no dispositivo** e **sobreposição de letras (lyrics overlay)**.  
O app **não** cria conta de usuário e **não** envia conteúdo do usuário a servidores próprios. O tratamento ocorre **no dispositivo do usuário** por padrão.

Para **publicidade** e **conformidade legal**, parceiros de terceiros (por exemplo, Google Mobile Ads SDK (AdMob) e UMP) podem coletar e tratar informações como **identificadores de publicidade**. A coleta de consentimento e as escolhas de privacidade seguem as especificações da **Google UMP (User Messaging Platform)**.

---

## 2. Categorias de informações tratadas

### 2-1) Arquivos escolhidos explicitamente pelo usuário
- **Caminhos e conteúdo de áudio/imagem de capa:** tratados **localmente** no dispositivo apenas para editar/salvar.  
- **FFmpegKit** é usado localmente para codificação, edição de metadados e extração de miniaturas.  
- O app **não envia** arquivos escolhidos pelo usuário para nossos servidores.

### 2-2) Configurações locais e valores armazenados

Para funcionalidade e conveniência, o app armazena os seguintes valores **localmente no dispositivo**.  
Eles não são enviados aos nossos servidores e **são removidos ao excluir os dados do app ou desinstalá-lo**.

#### (1) Preferências (`shared_preferences`)
| Tipo | Chave/Conteúdo | Finalidade | Local de armazenamento | Exclusão |
|---|---|---|---|---|
| Posição/fonte do overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Restaurar posição do overlay e tamanho da fonte | SharedPreferences do dispositivo | Removido ao excluir dados do app ou desinstalar |
| Anúncios/Privacidade | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Anúncios não personalizados (NPA), RDP nos EUA, tag COPPA, tag etária, limite de classificação de conteúdo de anúncios | SharedPreferences do dispositivo | Igual à coluna à esquerda |

#### (2) Arquivos temporários (diretório temporário do sistema)
- **Exemplos:** `cover_*.jpg`, `tmp_*.flac`  
- **Uso:** extração de capa, marcação FLAC, codificações temporárias  
- **Local:** pasta temporária do SO (`systemTemp`)  
- **Retenção:** removidos pelo app após a conclusão quando possível; o SO também pode limpá-los periodicamente

#### (3) Salvamento escolhido pelo usuário (SAF)
- Com “Salvar como”, os arquivos finais podem ser gravados em locais escolhidos pelo usuário (por exemplo, Downloads, nuvem).  
- Esses arquivos ficam no **armazenamento externo** e **permanecem após a desinstalação**. O usuário pode apagá-los manualmente.

#### (4) Estado de consentimento (cache do SDK UMP)
- Em EEE/Reino Unido/Suíça, o SDK UMP **armazena em cache** localmente o estado de consentimento para anúncios.  
- Pode ser redefinido ao limpar os dados do app ou pela tela de **Opções de privacidade** no app, quando disponível.

---

### 2-3) Dados de publicidade e consentimento (SDKs de terceiros)
- **Google Mobile Ads SDK (AdMob) e UMP** podem coletar/tratar, por exemplo: **identificadores de publicidade (AAID/IDFA)**, **faixas de IP**, **informações de dispositivo/app**, **sinais de interação com anúncios**, **estado de consentimento** etc.  
- **Finalidades:** veiculação de anúncios, controle de frequência, prevenção a fraudes, mensuração de desempenho, conformidade legal  
- **Regiões com obrigação de consentimento (EEE/Reino Unido/Suíça):** consentimento coletado via UMP e exibição da tela de **Opções de privacidade** quando aplicável.  
  Em regiões sem tal obrigação (por exemplo, KR), a opção **pode não ser exibida**.

---

## 3. Tratamento e prazos de retenção

- **Configurações locais:** permanecem no dispositivo até que o usuário apague os dados do app ou desinstale o app  
- **Arquivos temporários:** gerados durante codificação/extração; removidos após o processamento ou podem permanecer temporariamente em caches do SO  
- **Dados de anúncios/consentimento (terceiros):** conforme as **políticas do Google**

---

## 4. Transferências a terceiros e fluxos transfronteiriços

Para publicidade e gestão de consentimento, informações do usuário podem ser transmitidas e tratadas na infraestrutura do Google.

| Item | Detalhes |
|---|---|
| **Destinatário** | Google LLC e suas afiliadas/suboperadoras |
| **Destino** | Estados Unidos (e outras regiões onde a infraestrutura do Google está localizada) |
| **Finalidade** | Veiculação de anúncios, desempenho/mensuração, conformidade legal, gestão de consentimento |
| **Dados** | Identificadores de publicidade, faixas de IP, info de dispositivo/app, interações com anúncios, estado de consentimento etc. |
| **Retenção** | De acordo com as políticas do Google |
| **Efeito da recusa** | Personalização limitada; podem ser exibidos apenas anúncios não personalizados |

Cumprimos os requisitos de divulgação do **módulo “Segurança de dados” do Google Play** e mantemos as divulgações alinhadas ao tratamento efetivo.

---

## 5. Seus direitos e como exercê-los

- **Desativar anúncios personalizados / alterar o consentimento**  
  - Em regiões suportadas (EEE/Reino Unido/Suíça): ajuste em **Configurações → Opções de privacidade**.  
  - Outras regiões: use as configurações do SO para **redefinir o ID de anúncios / limitar o rastreamento**.
- **Redefinir informações locais:** ao excluir os dados do app ou desinstalá-lo, coordenadas do overlay, tamanho da fonte e outras configurações locais são redefinidas.
- Direitos sob **GDPR/UK GDPR/FADP suíça/leis estaduais de privacidade dos EUA** (acesso, retificação, exclusão, portabilidade, restrição, retirada de consentimento etc.) podem ser exercidos conforme previsto nessas leis.  
  Para dados de anúncios tratados pelo Google, use os **procedimentos do Google**.

---

## 6. Privacidade de crianças e adolescentes

Este app **não é destinado a crianças**. Pessoas abaixo da idade mínima legal devem interromper o uso e, com um responsável, utilizar os recursos de limitação de anúncios no nível do SO. Quando cabível, podemos aplicar **TFUA (child-directed tag)** ou opções equivalentes de proteção infantil.

---

## 7. Medidas de segurança

- **Minimização de dados** na coleta e no armazenamento  
- **Uso limitado** de arquivos temporários e tentativa de remoção após o processamento  
- Tratamento **dentro do escopo de permissões do SO**  
- **Criptografia em trânsito** (TLS ou equivalente) para transferências a terceiros conforme os padrões dos SDKs

---

## 8. Segurança de dados (Google Play)

Mantemos precisa a seção **“Segurança de dados”** na Play Console e a atualizamos prontamente quando houver alterações.

---

## 9. Avisos de código aberto

O app usa software de código aberto como **FFmpeg**. Um arquivo informativo (por exemplo, `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) no app explica como obter o código-fonte. Mediante solicitação, forneceremos o código conforme indicado nesse arquivo.

---

## 10. Contato

- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Alterações a esta Política

Podemos revisar esta Política devido a mudanças legais ou de serviço. Publicaremos as atualizações **no app** e nesta **página de política**.  
Para alterações materiais, daremos aviso **com pelo menos 7 dias de antecedência** à data de vigência.

---

## Apêndice: Guia ao usuário

- **Link no app:** abra esta página em **Configurações → Privacidade**.  
- **Comportamento por região:** em EEE/Reino Unido/Suíça, as Opções de privacidade são exibidas. **Em KR e algumas outras regiões, o botão pode não mostrar opções adicionais** quando não houver exigência legal.

