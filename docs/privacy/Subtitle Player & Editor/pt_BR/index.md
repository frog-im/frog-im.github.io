---
title: Política de Privacidade | Subtitle Tool
description: Política de privacidade do Subtitle Player & Editor (Subtitle Tool)
lang: pt-br
last_updated: 2025-12-12
---

# Política de Privacidade (Subtitle Player & Editor / “Subtitle Tool”)

- **Nome do app:** Subtitle Player & Editor (doravante, “Subtitle Tool”)  
- **Desenvolvedor:** frog-im  
- **Contato:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Data de vigência:** 2025-12-12  

> Esta Política foi elaborada com referência a leis aplicáveis, incluindo a Lei Coreana de Proteção de Informações Pessoais (PIPA), o GDPR/UK GDPR, a lei suíça FADP e leis estaduais de privacidade nos EUA.  
> Sempre que houver requisitos específicos em determinada jurisdição, esses requisitos prevalecerão sobre o texto geral desta Política.

---

## 1. Finalidade e Escopo

Este aplicativo oferece recursos de **edição de metadados de arquivos de áudio** (título, artista etc.) armazenados no dispositivo, bem como uma função de **sobreposição de letras/legendas**.  
O app **não cria conta de usuário** e **não envia o conteúdo do usuário** para nossos servidores. O processamento é realizado, por padrão, **localmente no dispositivo**.

No entanto, para fins de **publicidade** e **cumprimento de obrigações legais**, parceiros terceiros (por exemplo, Google Mobile Ads SDK (AdMob) e UMP) podem coletar e processar informações como **identificadores de publicidade**.  
A coleta de consentimento e o gerenciamento de preferências de privacidade seguem as especificações da **Google UMP (User Messaging Platform)**.

---

## 2. Categorias de Informações Tratadas

### 2-1) Arquivos Escolhidos Explicitamente pelo Usuário

- **Caminhos e conteúdo de arquivos de áudio/imagens de capa:** processados **localmente** no dispositivo, exclusivamente para edição e salvamento.  
- **FFmpegKit** é utilizado localmente para codificação, edição de metadados e extração de miniaturas.  
- O app **não envia** esses arquivos selecionados pelo usuário para nossos servidores.

### 2-2) Configurações Locais e Valores Armazenados

Para oferecer as funções principais e conveniência ao usuário, o app armazena os seguintes valores **localmente no dispositivo**.  
Esses dados não são enviados a nossos servidores e são **removidos quando o app ou seus dados são apagados**.

#### (1) Preferências (`shared_preferences`)

| Tipo | Chave/Conteúdo | Finalidade | Armazenamento | Exclusão |
|---|---|---|---|---|
| Posição/fonte da sobreposição | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Restaurar posição da sobreposição e tamanho da fonte | SharedPreferences no dispositivo | Excluídas ao apagar dados do app ou desinstalá-lo |
| Configurações de anúncios/privacidade | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Anúncios não personalizados, sinal U.S. RDP, marcação COPPA (conteúdo infantil), indicação de idade, limite de classificação de conteúdo de anúncios | SharedPreferences no dispositivo | Igual à coluna anterior |

#### (2) Arquivos Temporários (diretório temporário do sistema)

- **Exemplos:** `cover_*.jpg`, `tmp_*.flac`  
- **Uso:** extração de capas, marcação FLAC, codificação temporária  
- **Localização:** pasta temporária do sistema operacional (`systemTemp`)  
- **Retenção:** o app tenta remover esses arquivos após o fim do processamento; eles também podem ser removidos pelas rotinas de limpeza do sistema.

#### (3) Salvamento Escolhido pelo Usuário (SAF)

- Quando o usuário usa “Salvar como”, os arquivos de áudio finais podem ser gravados em locais escolhidos por ele (por exemplo, Downloads, armazenamento em nuvem).  
- Esses arquivos ficam em **armazenamento externo** e **podem permanecer mesmo após a desinstalação do app**. O usuário pode apagá-los manualmente.

#### (4) Estado de Consentimento (cache do UMP)

- Nas regiões EEE/Reino Unido/Suíça, o SDK UMP **armazenará em cache, localmente, o estado de consentimento de anúncios do usuário**.  
- Esse estado pode ser redefinido ao apagar os dados do app ou pela tela de **Opções de privacidade** dentro do app, quando disponível.

---

### 2-3) Dados Relacionados a Anúncios e Consentimento (SDKs de Terceiros)

- **Google Mobile Ads SDK (AdMob) e UMP** podem coletar e processar, por exemplo: **identificadores de publicidade (AAID/IDFA)**, **intervalos de IP**, **informações do dispositivo/app**, **sinais de interação com anúncios**, **estado de consentimento**, etc.  
- **Finalidades:** exibição de anúncios, limitação de frequência, prevenção de fraude, medição de desempenho, conformidade legal.  
- **Regiões que exigem consentimento (EEE/Reino Unido/Suíça):** o consentimento é coletado por meio das telas do UMP, e uma tela de **Opções de privacidade** é apresentada quando exigido.  
  Em regiões sem essa exigência (por exemplo, Coreia), essa opção **pode não ser exibida**.

---

## 3. Tratamento e Retenção

- **Configurações locais:** armazenadas no dispositivo até que o usuário apague os dados do app ou desinstale o app.  
- **Arquivos temporários:** criados durante codificação/extração, são removidos após o processamento ou podem permanecer temporariamente nos caches do sistema.  
- **Dados de anúncios/consentimento (terceiros):** são retidos e descartados conforme as **políticas do Google**.

---

## 4. Transferência a Terceiros e Fluxos Transfronteiriços

Para publicidade e gerenciamento de consentimento, certas informações do usuário podem ser transmitidas e processadas na infraestrutura do Google.

| Item | Detalhes |
|---|---|
| **Destinatário** | Google LLC e suas afiliadas/subprocessadoras |
| **Destino** | Estados Unidos (e outras regiões onde a infraestrutura do Google está localizada) |
| **Finalidade** | Exibição de anúncios, medição e desempenho, conformidade legal, gerenciamento de consentimento |
| **Dados** | Identificadores de publicidade, intervalos de IP, informações de dispositivo/app, interações com anúncios, estado de consentimento, etc. |
| **Retenção** | De acordo com as políticas do Google |
| **Efeito da recusa** | Anúncios personalizados podem ser limitados; anúncios não personalizados podem ser exibidos |

Cumprimos os requisitos de divulgação da seção de **Segurança de dados** na Google Play Console e mantemos essas informações alinhadas com o processamento real.

---

## 5. Seus Direitos e Como Exercê-los

- **Desativar anúncios personalizados / alterar consentimento**  
  - Em regiões suportadas (EEE/Reino Unido/Suíça): altere suas preferências em **Configurações → Opções de privacidade**.  
  - Em outras regiões: use as configurações do sistema operacional para **redefinir IDs de publicidade / limitar o rastreamento de anúncios**.
- **Redefinir informações locais:** ao apagar os dados do app ou desinstalá-lo, as coordenadas da sobreposição, o tamanho da fonte e outras configurações locais serão redefinidas.  
- Os direitos previstos em **GDPR/UK GDPR/FADP suíça/leis estaduais de privacidade dos EUA** (acesso, retificação, exclusão, portabilidade, limitação, revogação de consentimento etc.) podem ser exercidos conforme tais leis.  
  Para dados de anúncios processados pelo Google, utilize os **mecanismos fornecidos pelo próprio Google**.

---

## 6. Privacidade de Crianças

Este app **não é direcionado a crianças**.  
Se uma pessoa menor que a idade mínima legal utilizar o app, recomenda-se que interrompa o uso e ative, com ajuda de um responsável, as funções de limitação de anúncios disponibilizadas pelo sistema operacional.  
Quando adequado, poderemos aplicar sinalizações como **TFUA (child-directed tag)** ou opções semelhantes de proteção infantil.

---

## 7. Medidas de Segurança

- **Minimização de dados** na coleta e no armazenamento  
- Uso limitado de arquivos temporários e remoção após o processamento, sempre que possível  
- Processamento estritamente **dentro do escopo de permissões do sistema operacional**  
- Criptografia **TLS ou equivalente** nas transmissões para terceiros (conforme os padrões dos SDKs)

---

## 8. Segurança de Dados (Google Play)

Mantemos a seção de **Segurança de dados** na Google Play Console de forma precisa e a atualizamos prontamente em caso de mudanças.

---

## 9. Avisos de Código Aberto

O app utiliza software de código aberto, como **FFmpeg**.  
Um arquivo informativo (por exemplo, `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) dentro do app explica como obter o código-fonte.  
Mediante solicitação, forneceremos o código-fonte conforme indicado nesse arquivo.

---

## 10. Contato

- E-mail: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Alterações a Esta Política

Poderemos atualizar esta Política devido a mudanças legais ou de serviço.  
Publicaremos atualizações **dentro do app** e nesta **página de política**.  
Em caso de alterações significativas, forneceremos aviso com **pelo menos 7 dias de antecedência** da nova data de vigência.
