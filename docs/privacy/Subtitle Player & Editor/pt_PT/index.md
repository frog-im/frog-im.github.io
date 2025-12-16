---
title: Política de Privacidade | Subtitle Tool
description: Subtitle Tool (Subtitle Player & Editor) Política de Privacidade (Português - Portugal)
lang: pt-PT
last_updated: 2025-12-12
---

# Política de Privacidade (Subtitle Tool / Subtitle Player & Editor)

- **Nome da aplicação:** Subtitle Player & Editor (também referida como **“Subtitle Tool”** nesta Política)  
- **Programador:** frog-im  
- **Contacto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Data de entrada em vigor:** 2025-12-12  

> Esta Política foi redigida com referência a legislação aplicável, incluindo a Lei Coreana de Proteção de Informações Pessoais (PIPA), o RGPD/UK GDPR, a FADP suíça e legislação estadual relevante dos EUA. Caso existam requisitos específicos por jurisdição, esses requisitos prevalecem.

---

## 1. Finalidade e Âmbito

Esta aplicação disponibiliza:

- **Reprodução e edição de legendas** (por ex., SRT, VTT, ASS, SSA, LRC)  
- **Reprodução de vídeo + legendas** a partir de ficheiros selecionados pelo utilizador  
- **Sobreposição flutuante de legendas/letras** exibida sobre outras aplicações (Android)

A aplicação **não** cria uma conta de utilizador e **não** carrega multimédia ou conteúdo de legendas do utilizador para os nossos próprios servidores.  
O tratamento é efetuado **no dispositivo do utilizador** por predefinição.

No entanto, para efeitos de **publicidade**, **gestão de consentimento** e **conformidade legal**, parceiros terceiros (como o **Google Mobile Ads SDK (AdMob)** e o **Google UMP**) podem recolher e tratar informações, incluindo **identificadores de publicidade** e sinais relacionados.  
A recolha de consentimento e as opções de privacidade seguem as especificações do **Google UMP (User Messaging Platform)** quando aplicável.

---

## 2. Categorias de Informação que Tratamos

### 2-1) Ficheiros Explicitamente Selecionados pelo Utilizador

A aplicação interage apenas com **ficheiros que o utilizador seleciona explicitamente**, tais como:

- **Ficheiros de legendas**  
  - Exemplos: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`  
  - **Utilização:**  
    - Apresentar legendas/letras numa sobreposição flutuante ou dentro da aplicação  
    - Editar tempos e texto das legendas e guardar num novo ficheiro  
  - **Tratamento:** efetuado **localmente no dispositivo** (análise e gravação através de bibliotecas como `subtitle`)

- **Ficheiros multimédia (opcional)**  
  - Exemplos: ficheiros locais de vídeo/áudio selecionados pelo utilizador (por ex., via seletor de ficheiros)  
  - **Utilização:** reproduzir vídeo/áudio juntamente com as legendas selecionadas dentro da aplicação  
  - **Tratamento:** descodificação e reprodução são feitas **localmente** (por ex., usando `better_player` ou bibliotecas semelhantes)

> **Importante:**  
> - A aplicação **não** carrega ficheiros de legendas ou multimédia selecionados pelo utilizador para os nossos próprios servidores.  
> - Caminhos e conteúdos são usados estritamente para reprodução, apresentação em sobreposição e edição iniciada pelo utilizador.

### 2-2) Definições Locais e Valores Armazenados

Para a aplicação funcionar e proporcionar uma experiência consistente, certas definições são armazenadas **localmente no dispositivo** usando `SharedPreferences` ou mecanismos equivalentes do sistema.

Estes valores **não** são enviados para os nossos próprios servidores e são **removidos quando a aplicação ou os seus dados são eliminados**.

#### (1) Posição, tamanho e estilo da sobreposição (`SharedPreferences`)

| Tipo | Chave (exemplo) | Finalidade | Armazenamento | Eliminação |
|---|---|---|---|---|
| Posição da sobreposição (Y) | `overlay_box_y` | Restaurar a posição vertical da caixa de legendas | SharedPreferences do dispositivo | Removido ao limpar dados ou desinstalar |
| Posição da sobreposição (X / alinhamento à esquerda) | `overlay_box_x` | Alinhamento horizontal / deslocamento (normalmente fixo ou 0) | Mesmo | Mesmo |
| Tamanho da fonte | `overlay_text_font` | Manter o tamanho de fonte para a sobreposição e o leitor | Mesmo | Mesmo |
| Cor do texto | `overlay_text_color` | Manter a cor do texto na sobreposição | Mesmo | Mesmo |
| Utilização de contorno | `overlay_outline_enabled` | Desenhar contorno no texto ou não | Mesmo | Mesmo |
| Cor do contorno | `overlay_outline_color` | Cor do contorno do texto | Mesmo | Mesmo |
| Largura do contorno | `overlay_outline_width` | Espessura do contorno | Mesmo | Mesmo |
| Largura/altura da caixa | `overlay_box_w`, `overlay_box_h` | Tamanho padrão ou ajustado pelo utilizador (dp) | Mesmo | Mesmo |
| Contador de anúncios | `overlay_interstitial_count` | Contador interno para apresentar anúncios periodicamente | Mesmo | Mesmo |

Estas chaves são usadas para:

- Restaurar a última posição utilizada da sobreposição no ecrã  
- Sincronizar o estilo das legendas entre **Overlay Box Editor**, **leitor de vídeo** e a **sobreposição Android**  
- Controlar com que frequência anúncios intersticiais ou recompensados são **tentados** (por ex., “a cada 3 utilizações da sobreposição”)

#### (2) Preferências relacionadas com anúncios/privacidade

Dependendo da sua região e das definições da aplicação, podem ser armazenadas flags como:

- `pref_npa_always` (preferência de anúncios não personalizados)  
- `pref_us_rdp` (U.S. Restricted Data Processing)  
- `pref_child_directed` / `pref_under_age` (marcação para crianças / idade)  
- `pref_max_ad_rating` (classificação máxima de conteúdo de anúncios)

**Finalidade:**  
- Memorizar as suas opções de privacidade e anúncios e configurar AdMob/UMP de forma a respeitá-las.

**Armazenamento/eliminação:**  
- Armazenado localmente via `SharedPreferences`.  
- Removido ao limpar dados da aplicação ou ao desinstalar.

#### (3) Ficheiros temporários

Durante o funcionamento normal, a aplicação pode criar **ficheiros temporários**, por exemplo:

- Conteúdos de legendas analisados/convertidos usados internamente  
- Pequenas caches criadas por bibliotecas de terceiros ou seletores de ficheiros

Estes ficheiros temporários:

- Ficam em pastas de cache/temporárias geridas pelo sistema  
- São eliminados pela aplicação quando possível e também podem ser limpos pelo sistema ao longo do tempo  
- **Não** são carregados para os nossos próprios servidores

#### (4) Locais de gravação escolhidos pelo utilizador

Ao utilizar “Guardar como” ou funcionalidades semelhantes:

- A aplicação pode **gravar ficheiros de legendas** num diretório que escolher (por ex., Downloads ou outra pasta selecionada via seletor do sistema).  
- Esses ficheiros ficam em **armazenamento externo ou gerido pelo utilizador** e podem **permanecer após a desinstalação**.  
- Pode eliminá-los manualmente através do gestor de ficheiros ou de uma interface de armazenamento na nuvem.

#### (5) Estado de Consentimento (cache do SDK UMP)

Em determinadas regiões (EEE/Reino Unido/Suíça e outras conforme determinado pelo Google UMP):

- O **SDK UMP** pode armazenar em cache o seu estado de consentimento localmente no dispositivo.  
- Normalmente pode ser reposto por:
  - Limpar os dados da aplicação, ou  
  - Utilizar um ecrã interno de **Opções de Privacidade/Consentimento**, quando disponibilizado.

---

### 2-3) Anúncios, Consentimento e Dados Relacionados (SDKs de Terceiros)

A aplicação utiliza **Google Mobile Ads SDK (AdMob)** e **Google UMP** para:

- Apresentar anúncios (incluindo **anúncios recompensados** para algumas operações, como guardar legendas)  
- Gerir consentimento relacionado com anúncios quando exigido por lei

Estes SDKs de terceiros podem recolher ou tratar, por exemplo:

- **Identificadores de publicidade** (por ex., AAID/IDFA)  
- **Informação baseada em IP**, localização aproximada e informação geral de rede  
- Informação do dispositivo e da aplicação (versão do SO, versão da aplicação, idioma, registos de falhas relevantes para anúncios)  
- Sinais de interação/engajamento com anúncios (por ex., impressões, cliques, visualizações completas em anúncios recompensados)  
- Opções de consentimento registadas via UMP

**Finalidades:**

- Entrega e relatórios de anúncios  
- Limitação de frequência (frequency capping)  
- Prevenção de fraude e abuso  
- Conformidade legal (por ex., consentimento e flags de idade)

Em regiões como **EEE/Reino Unido/Suíça**:

- O consentimento é solicitado através de **prompts UMP** quando exigido.  
- Pode ser apresentado um botão de **Opções de Privacidade** para rever escolhas.

Em regiões sem tais requisitos explícitos (por ex., Coreia):

- A interface pode **não** apresentar um botão separado de Opções de Privacidade se não for necessário,  
  mas definições ao nível do sistema (por ex., repor o ID de publicidade) continuam disponíveis.

---

## 3. Tratamento e Conservação

- **Definições locais (SharedPreferences):**  
  - Mantidas no dispositivo até limpar dados da aplicação ou desinstalar.

- **Ficheiros temporários:**  
  - Criados e usados durante operações de legendas e reprodução.  
  - Eliminados quando possível pela aplicação; também sujeitos à limpeza de cache do sistema.

- **Ficheiros de legendas guardados pelo utilizador:**  
  - Gravados nos destinos que escolher (por ex., Downloads, outras pastas ou localizações na nuvem).  
  - Permanecem sob o seu controlo e **não são removidos automaticamente** ao desinstalar.

- **Dados de anúncios/consentimento (terceiros):**  
  - Armazenados, tratados e conservados de acordo com as **políticas do Google** e a lei aplicável.

---

## 4. Transferências para Terceiros e Fluxos Internacionais

Para publicidade e gestão de consentimento, certos dados são tratados pelo **Google** e pelos seus parceiros.

| Item | Detalhes |
|---|---|
| **Destinatário** | Google LLC e as suas afiliadas/subprocessadores |
| **Destino** | Estados Unidos e outras regiões onde a infraestrutura do Google está localizada |
| **Finalidade** | Entrega de anúncios, medição de desempenho, prevenção de fraude, gestão de consentimento e conformidade legal |
| **Dados** | Identificadores de publicidade, info baseada em IP, info de dispositivo/aplicação, sinais de interação com anúncios, estado de consentimento, etc. |
| **Conservação** | Conforme as políticas do Google e leis aplicáveis |
| **Efeito da recusa** | Anúncios personalizados podem ser limitados; podem ser mostrados anúncios não personalizados ou menos anúncios |

Procuramos manter as divulgações de **Data safety do Google Play** consistentes com o tratamento real da aplicação e dos seus SDKs.

---

## 5. Os Seus Direitos e Como Exercê-los

Dependendo da sua jurisdição, poderá ter direitos como:

- Acesso aos seus dados pessoais  
- Retificação ou eliminação  
- Limitação do tratamento  
- Portabilidade  
- Oposição a certos tratamentos  
- Retirada de consentimento (quando o consentimento é a base legal)

**Na prática:**

- **Opções de anúncios e consentimento**  
  - Em regiões suportadas pelo UMP (por ex., EEE/Reino Unido/Suíça): ajuste em **Definições → Opções de Privacidade** (se disponibilizado na aplicação).  
  - Caso contrário, use definições do sistema para **repor o ID de publicidade** ou limitar a personalização.

- **Definições locais e configuração da sobreposição**  
  - Limpar dados ou desinstalar repõe:  
    - Coordenadas e tamanho da sobreposição  
    - Tamanho/cor/contorno da fonte  
    - Preferências de anúncios/privacidade armazenadas

Para dados de anúncios tratados pelo Google, consulte e utilize as ferramentas e processos do próprio Google (por ex., definições de anúncios da conta Google, diálogo UMP, etc.).

---

## 6. Privacidade de Crianças

Esta aplicação **não é dirigida a crianças**.

- A finalidade principal é **edição de legendas/letras e sobreposição flutuante**, presumindo utilização por adolescentes mais velhos ou adultos.  
- Se uma criança abaixo da idade mínima legal utilizar a aplicação, deve parar de a utilizar e recorrer a funcionalidades do sistema para limitar anúncios com um responsável.

Quando apropriado, o programador pode ativar flags **child-directed** (por ex., TFUA) ou definições equivalentes nos SDKs de anúncios para melhor proteger menores, em linha com as políticas da plataforma.

---

## 7. Medidas de Segurança

Dentro da arquitetura e do âmbito da aplicação, procuramos:

- Minimizar recolha de dados ao estritamente necessário para legendas e sobreposição  
- Manter tratamento **no dispositivo** sempre que possível  
- Limitar acesso a ficheiros estritamente aos que selecionar explicitamente via seletores do sistema  
- Usar permissões do sistema de forma transparente (por ex., permissão de sobreposição e permissão de notificações no Android)  
- Confiar em **TLS** ou encriptação equivalente em trânsito para tráfego de rede tratado por SDKs de terceiros (anúncios/consentimento)

---

## 8. Data Safety (Google Play)

Para distribuição em lojas como o **Google Play**, nós:

- Preparamos e mantemos uma secção de **Data safety** que reflete com precisão como a aplicação e os seus SDKs de terceiros tratam dados  
- Atualizamos a divulgação sem demora indevida caso existam alterações materiais (por ex., ativação futura de analytics ou crash reporting)

---

## 9. Avisos de Código Aberto

Esta aplicação utiliza software de código aberto (por exemplo, bibliotecas para:

- Análise e serialização de legendas  
- Reprodução de vídeo  
- Janelas de sobreposição  
- Integrações WebView  
- Localização e componentes de UI)

Licenças e avisos de código aberto são disponibilizados **dentro da aplicação** (por ex., em “Licenças de Código Aberto”).  
Quando exigido, instruções de acesso ao código-fonte para componentes relevantes serão fornecidas nos ficheiros de aviso correspondentes.

---

## 10. Contacto

Se tiver questões sobre esta Política ou pedidos relacionados com privacidade:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Inclua o nome da aplicação **“Subtitle Player & Editor (Subtitle Tool)”** no seu contacto para identificarmos a aplicação correta.

---

## 11. Alterações a Esta Política

Podemos atualizar esta Política devido a:

- Alterações legais ou regulamentares  
- Atualizações de funcionalidades da aplicação (por ex., adição de novos SDKs/serviços)  
- Ajustes internos de política

**Atualizações menores:**  
- Serão publicadas na secção de privacidade da aplicação e na página da política.

**Alterações materiais:**  
- Forneceremos aviso **com pelo menos 7 dias** de antecedência da nova data de entrada em vigor, quando exigido por lei ou por políticas da plataforma.
