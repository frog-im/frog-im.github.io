---
title: Política de Privacidade | Subtitle Tool
description: Subtitle Tool (Subtitle Player & Editor) Política de Privacidade (Português)
lang: pt
last_updated: 2025-12-12
---

# Política de Privacidade (Subtitle Tool / Subtitle Player & Editor)

- **Nome do app:** Subtitle Player & Editor (também referido como **“Subtitle Tool”** nesta Política)  
- **Desenvolvedor:** frog-im  
- **Contato:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Data de vigência:** 2025-12-12  

> Esta Política foi redigida com referência a leis aplicáveis, incluindo a Lei de Proteção de Informações Pessoais da Coreia (PIPA), o GDPR/UK GDPR, a FADP suíça e leis estaduais relevantes dos EUA. Quando houver requisitos específicos por jurisdição, esses requisitos prevalecerão.

---

## 1. Finalidade e Escopo

Este app oferece:

- **Reprodução e edição de legendas** (ex.: SRT, VTT, ASS, SSA, LRC)  
- **Reprodução de vídeo + legendas** a partir de arquivos selecionados pelo usuário  
- **Sobreposição flutuante de legendas/letras** exibida sobre outros apps (Android)

O app **não** cria conta de usuário e **não** envia mídias ou conteúdo de legendas do usuário para nossos próprios servidores.  
O processamento é realizado **no dispositivo do usuário** por padrão.

No entanto, para fins de **publicidade**, **gerenciamento de consentimento** e **conformidade legal**, parceiros terceiros (como o **Google Mobile Ads SDK (AdMob)** e o **Google UMP**) podem coletar e processar informações, incluindo **identificadores de publicidade** e sinais relacionados.  
A coleta de consentimento e as escolhas de privacidade seguem as especificações do **Google UMP (User Messaging Platform)** quando aplicável.

---

## 2. Categorias de Informações que Processamos

### 2-1) Arquivos Explicitamente Escolhidos pelo Usuário

O app interage apenas com **arquivos que o usuário seleciona explicitamente**, tais como:

- **Arquivos de legenda**  
  - Exemplos: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`  
  - **Uso:**  
    - Exibir legendas/letras em uma sobreposição flutuante ou dentro do app  
    - Editar tempo e texto das legendas e salvar em um novo arquivo  
  - **Processamento:** realizado **localmente no dispositivo** (análise e salvamento via bibliotecas como `subtitle`)

- **Arquivos de mídia (opcional)**  
  - Exemplos: arquivos locais de vídeo/áudio selecionados pelo usuário (ex.: via seletor de arquivos)  
  - **Uso:** reproduzir vídeo/áudio junto com as legendas selecionadas dentro do app  
  - **Processamento:** decodificação e reprodução são feitas **localmente** (ex.: usando `better_player` ou bibliotecas semelhantes)

> **Importante:**  
> - O app **não** envia legendas ou arquivos de mídia selecionados pelo usuário para nossos próprios servidores.  
> - Caminhos e conteúdos são usados estritamente para reprodução, exibição em sobreposição e edição iniciada pelo usuário.

### 2-2) Configurações Locais e Valores Armazenados

Para o app funcionar e fornecer uma experiência consistente, algumas configurações são armazenadas **localmente no dispositivo** usando `SharedPreferences` ou mecanismos equivalentes do sistema.

Esses valores **não** são enviados para nossos próprios servidores e são **removidos quando o app ou seus dados são excluídos**.

#### (1) Posição, tamanho e estilo da sobreposição (`SharedPreferences`)

| Tipo | Chave (exemplo) | Finalidade | Armazenamento | Exclusão |
|---|---|---|---|---|
| Posição da sobreposição (Y) | `overlay_box_y` | Restaurar a posição vertical da caixa de legendas | SharedPreferences do dispositivo | Removido ao limpar dados ou desinstalar |
| Posição da sobreposição (X / alinhamento à esquerda) | `overlay_box_x` | Alinhamento horizontal / deslocamento (normalmente fixo ou 0) | Mesmo | Mesmo |
| Tamanho da fonte | `overlay_text_font` | Manter o tamanho de fonte para a sobreposição e o player | Mesmo | Mesmo |
| Cor do texto | `overlay_text_color` | Manter a cor do texto na sobreposição | Mesmo | Mesmo |
| Uso de contorno | `overlay_outline_enabled` | Desenhar contorno no texto ou não | Mesmo | Mesmo |
| Cor do contorno | `overlay_outline_color` | Cor do contorno do texto | Mesmo | Mesmo |
| Largura do contorno | `overlay_outline_width` | Espessura do contorno | Mesmo | Mesmo |
| Largura/altura da caixa | `overlay_box_w`, `overlay_box_h` | Tamanho padrão ou ajustado pelo usuário (dp) | Mesmo | Mesmo |
| Contador de anúncios | `overlay_interstitial_count` | Contador interno para exibir anúncios periodicamente | Mesmo | Mesmo |

Essas chaves são usadas para:

- Restaurar a última posição utilizada da sobreposição na tela  
- Sincronizar o estilo das legendas entre **Overlay Box Editor**, **player de vídeo** e a **sobreposição Android**  
- Controlar com que frequência anúncios em tela cheia ou recompensados são **tentados** (ex.: “a cada 3 usos da sobreposição”)

#### (2) Preferências relacionadas a anúncios/privacidade

Dependendo da região e das configurações do app, podem ser armazenadas flags como:

- `pref_npa_always` (preferência de anúncios não personalizados)  
- `pref_us_rdp` (U.S. Restricted Data Processing)  
- `pref_child_directed` / `pref_under_age` (marcação de direcionamento a crianças / idade)  
- `pref_max_ad_rating` (classificação máxima de conteúdo de anúncios)

**Finalidade:**  
- Lembrar suas escolhas de privacidade e anúncios e configurar AdMob/UMP para respeitar essas escolhas.

**Armazenamento/exclusão:**  
- Armazenado localmente via `SharedPreferences`.  
- Removido ao limpar dados do app ou desinstalar.

#### (3) Arquivos temporários

Durante o uso normal, o app pode criar **arquivos temporários**, por exemplo:

- Conteúdos de legenda analisados/convertidos usados internamente  
- Pequenos caches criados por bibliotecas de terceiros ou seletores de arquivos

Esses arquivos temporários:

- Ficam em pastas de cache/temporárias gerenciadas pelo sistema  
- São excluídos pelo app quando viável e também podem ser limpos pelo sistema ao longo do tempo  
- **Não** são enviados para nossos próprios servidores

#### (4) Locais de salvamento escolhidos pelo usuário

Ao usar “Salvar como” ou recursos semelhantes:

- O app pode **gravar arquivos de legenda** em um diretório escolhido por você (ex.: Downloads ou outra pasta selecionada via seletor do sistema).  
- Esses arquivos ficam em **armazenamento externo ou gerenciado pelo usuário** e podem **permanecer após a desinstalação**.  
- Você pode removê-los manualmente pelo gerenciador de arquivos ou interface de nuvem.

#### (5) Estado de Consentimento (cache do SDK UMP)

Em determinadas regiões (EEE/Reino Unido/Suíça e outras conforme definido pelo Google UMP):

- O **SDK UMP** pode armazenar em cache seu estado de consentimento localmente no dispositivo.  
- Isso normalmente pode ser redefinido por:
  - Limpar os dados do app, ou  
  - Usar uma tela interna de **Opções de Privacidade/Consentimento**, quando disponível.

---

### 2-3) Anúncios, Consentimento e Dados Relacionados (SDKs de Terceiros)

O app usa **Google Mobile Ads SDK (AdMob)** e **Google UMP** para:

- Exibir anúncios (incluindo **anúncios recompensados** para algumas operações, como salvar legendas)  
- Gerenciar consentimento relacionado a anúncios quando exigido por lei

Esses SDKs de terceiros podem coletar ou processar, por exemplo:

- **Identificadores de publicidade** (ex.: AAID/IDFA)  
- **Informações baseadas em IP**, localização aproximada e informações gerais de rede  
- Informações do dispositivo e do app (versão do SO, versão do app, idioma, logs de falhas relevantes para anúncios)  
- Sinais de interação/engajamento com anúncios (ex.: impressões, cliques, visualizações completas em anúncios recompensados)  
- Escolhas de consentimento registradas via UMP

**Finalidades:**

- Entrega e relatórios de anúncios  
- Frequency capping  
- Prevenção de fraude e abuso  
- Conformidade legal (ex.: consentimento e flags de idade)

Em regiões como **EEE/Reino Unido/Suíça**:

- O consentimento é solicitado por **prompts UMP** quando exigido.  
- Um botão de **Opções de Privacidade** pode ser exibido para revisar escolhas.

Em regiões sem tais exigências explícitas (ex.: Coreia):

- A interface pode **não** mostrar um botão separado de Opções de Privacidade se não for necessário,  
  mas configurações do sistema (ex.: redefinir ID de anúncios) continuam disponíveis.

---

## 3. Processamento e Retenção

- **Configurações locais (SharedPreferences):**  
  - Retidas no dispositivo até você limpar os dados do app ou desinstalar.

- **Arquivos temporários:**  
  - Criados e usados durante operações com legendas e reprodução.  
  - Excluídos quando viável pelo app; também sujeitos à limpeza de cache do sistema.

- **Arquivos de legendas salvos pelo usuário:**  
  - Gravados nos destinos que você escolher (ex.: Downloads, outras pastas ou locais em nuvem).  
  - Permanecem sob seu controle e **não são removidos automaticamente** ao desinstalar.

- **Dados de anúncios/consentimento (terceiros):**  
  - Armazenados, processados e retidos conforme **políticas do Google** e a lei aplicável.

---

## 4. Transferências a Terceiros e Fluxos Internacionais

Para publicidade e gerenciamento de consentimento, certos dados são processados pelo **Google** e seus parceiros.

| Item | Detalhes |
|---|---|
| **Destinatário** | Google LLC e suas afiliadas/subprocessadores |
| **Destino** | Estados Unidos e outras regiões onde a infraestrutura do Google está localizada |
| **Finalidade** | Entrega de anúncios, medição de desempenho, prevenção de fraude, gerenciamento de consentimento e conformidade legal |
| **Dados** | Identificadores de publicidade, info baseada em IP, info de dispositivo/app, sinais de interação com anúncios, estado de consentimento etc. |
| **Retenção** | Conforme as políticas do Google e leis aplicáveis |
| **Efeito da recusa** | Anúncios personalizados podem ser limitados; anúncios não personalizados ou menos anúncios podem ser exibidos |

Buscamos manter as divulgações de **Data safety do Google Play** consistentes com o processamento real do app e de seus SDKs.

---

## 5. Seus Direitos e Como Exercê-los

Dependendo da sua jurisdição, você pode ter direitos como:

- Acesso aos seus dados pessoais  
- Retificação ou exclusão  
- Restrição de processamento  
- Portabilidade  
- Oposição a certos processamentos  
- Retirada de consentimento (quando o consentimento for a base legal)

**Na prática:**

- **Escolhas de anúncios e consentimento**  
  - Em regiões suportadas pelo UMP (ex.: EEE/Reino Unido/Suíça): ajuste em **Configurações → Opções de Privacidade** (se disponibilizado no app).  
  - Caso contrário, use configurações do sistema para **redefinir o ID de anúncios** ou limitar personalização.

- **Configurações locais e sobreposição**  
  - Limpar dados do app ou desinstalar redefine:  
    - Coordenadas e tamanho da sobreposição  
    - Tamanho/cor/contorno da fonte  
    - Preferências de anúncios/privacidade armazenadas

Para dados de anúncios processados pelo Google, consulte e utilize as ferramentas e processos do próprio Google (ex.: configurações de anúncios da conta Google, diálogo UMP etc.).

---

## 6. Privacidade de Crianças

Este app **não é direcionado a crianças**.

- A finalidade principal é **editar legendas/letras e usar sobreposição flutuante**, o que presume uso por adolescentes mais velhos ou adultos.  
- Se uma criança abaixo da idade mínima exigida por lei usar o app, deve interromper o uso e utilizar recursos de limitação de anúncios do sistema com um responsável.

Quando apropriado, o desenvolvedor pode ativar flags **child-directed** (ex.: TFUA) ou configurações equivalentes em SDKs de anúncios para melhor proteger menores, conforme políticas da plataforma.

---

## 7. Medidas de Segurança

Dentro da arquitetura e do escopo do app, buscamos:

- Minimizar coleta de dados ao necessário para legendas e sobreposição  
- Manter processamento **no dispositivo** sempre que possível  
- Limitar acesso a arquivos estritamente aos que você selecionar explicitamente via seletores do sistema  
- Usar permissões do sistema de forma transparente (ex.: permissão de sobreposição, permissão de notificações no Android)  
- Confiar em **TLS** ou criptografia equivalente em trânsito para tráfego de rede de SDKs de terceiros (anúncios/consentimento)

---

## 8. Data Safety (Google Play)

Para distribuição em lojas como o **Google Play**, nós:

- Preparamos e mantemos uma seção de **Data safety** que reflete com precisão como o app e SDKs de terceiros tratam dados  
- Atualizamos a divulgação sem demora indevida quando houver mudanças materiais (ex.: ativação futura de analytics ou crash reporting)

---

## 9. Avisos de Código Aberto

Este app usa software de código aberto (por exemplo, bibliotecas para:

- Análise e serialização de legendas  
- Reprodução de vídeo  
- Janelas de sobreposição  
- Integrações WebView  
- Localização e componentes de UI)

Licenças e avisos de código aberto são fornecidos **dentro do app** (ex.: em “Licenças de Código Aberto”).  
Quando exigido, instruções de acesso ao código-fonte para componentes relevantes serão fornecidas nos arquivos de aviso correspondentes.

---

## 10. Contato

Se você tiver dúvidas sobre esta Política ou solicitações relacionadas à privacidade:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Inclua o nome do app **“Subtitle Player & Editor (Subtitle Tool)”** na mensagem para identificarmos o app correto.

---

## 11. Alterações nesta Política

Podemos atualizar esta Política devido a:

- Mudanças em leis ou regulamentos  
- Atualizações de recursos do app (ex.: adição de novos SDKs/serviços)  
- Ajustes internos de política

**Atualizações menores:**  
- Serão publicadas na seção de privacidade do app e na página da política.

**Mudanças materiais:**  
- Forneceremos aviso **com pelo menos 7 dias** de antecedência da nova data de vigência, quando exigido por lei ou por políticas da plataforma.
