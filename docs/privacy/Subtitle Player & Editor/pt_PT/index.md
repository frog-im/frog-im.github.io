---
title: Política de Privacidade | Subtitle Tool
description: Política de Privacidade do Subtitle Tool (Português - Portugal)
lang: pt-pt
last_updated: 2025-12-12
---

# Política de Privacidade (Subtitle Tool / Subtitle Player & Editor)

- **Nome da aplicação:** Subtitle Tool (pode aparecer como “Subtitle Player & Editor” na loja)  
- **Programador:** frog-im  
- **Contacto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Data de entrada em vigor:** 2025-12-12  

> Esta Política foi elaborada com referência à legislação aplicável, incluindo a Lei coreana de Proteção de Dados Pessoais (PIPA), o RGPD / RGPD do Reino Unido, a FADP suíça e leis estaduais de privacidade dos EUA. Em caso de requisitos específicos por jurisdição, esses requisitos prevalecem.

---

## 1. Finalidade e âmbito

A aplicação oferece principalmente:  
- **edição de metadados de ficheiros de áudio** armazenados no dispositivo (título, artista, etc.);  
- funcionalidades de **sobreposição de letras/legendas (lyrics overlay)** no próprio dispositivo.  

A aplicação **não cria uma conta de utilizador** e **não carrega o conteúdo do utilizador** para servidores do programador.  
O tratamento é efetuado **localmente no dispositivo**, por defeito.

No entanto, para fins de **publicidade** e **cumprimento legal**, podem ser utilizados serviços de terceiros (por exemplo, Google Mobile Ads SDK (AdMob) e Google UMP). Esses serviços podem recolher e tratar informações como **identificadores de publicidade**.  
A recolha de consentimento e as opções de privacidade seguem as especificações da **Google UMP (User Messaging Platform)**.

---

## 2. Categorias de informação tratada

### 2-1) Ficheiros selecionados explicitamente pelo utilizador

- **Caminhos e conteúdos de áudio/imagem de capa:**  
  Utilizados apenas localmente para leitura, edição de metadados e gravação.  
- **FFmpegKit** é usado localmente para codificação, edição de metadados e extração de miniaturas.  
- A aplicação **não carrega estes ficheiros** para servidores do programador.

### 2-2) Definições locais e valores armazenados

Para garantir o funcionamento básico e a conveniência do utilizador, a aplicação guarda os seguintes valores **localmente no dispositivo**.  
Estes dados **não são enviados** para os servidores do programador e são **apagados quando a aplicação ou os dados da aplicação são removidos**.

#### (1) Preferências (`shared_preferences`)

| Tipo | Chave / conteúdo | Finalidade | Local de armazenamento | Eliminação |
|---|---|---|---|---|
| Posição/Tipo de letra da sobreposição | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Restaurar posição e tamanho do texto da sobreposição de letras | SharedPreferences do dispositivo | Apagado ao eliminar os dados ou a aplicação |
| Definições de anúncios / privacidade | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Marcação de anúncios não personalizados, definições RDP dos EUA, indicação de conteúdo dirigido a crianças, marca de idade, limite de classificação de anúncios | SharedPreferences do dispositivo | Igual ao anterior |

#### (2) Ficheiros temporários (diretório temporário do sistema)

- **Exemplos:** `cover_*.jpg`, `tmp_*.flac`  
- **Utilização:** extração de capas, escrita de metadados FLAC, codificação temporária  
- **Localização:** pasta temporária do sistema operativo (`systemTemp`)  
- **Retenção:** o objetivo é apagar após a conclusão; podem permanecer temporariamente em cache até o sistema os remover

#### (3) Guardar em local escolhido pelo utilizador (SAF)

- Quando o utilizador seleciona “Guardar como”, os ficheiros finais podem ser gravados em locais escolhidos (por exemplo, transferências, armazenamento em nuvem).  
- Estes ficheiros ficam em **armazenamento externo** e **podem permanecer após a desinstalação**. O utilizador pode apagá-los manualmente.

#### (4) Estado de consentimento (cache do UMP)

- Nas regiões EEE/Reino Unido/Suíça, o SDK UMP **guarda localmente** o estado de consentimento do utilizador para anúncios.  
- Pode ser redefinido apagando os dados da aplicação ou, quando disponível, através do ecrã interno de **Opções de Privacidade**.

---

### 2-3) Dados relacionados com anúncios e consentimento (terceiros)

- **Google Mobile Ads SDK (AdMob) e UMP** podem recolher/tratar, por exemplo:  
  - Identificadores de publicidade (AAID/IDFA)  
  - Faixas de IP  
  - Informações do dispositivo e da aplicação  
  - Sinais de interação com anúncios  
  - Estado de consentimento e configurações associadas  

- **Finalidades:**  
  - Entrega e apresentação de anúncios  
  - Limitação de frequência  
  - Prevenção de fraude e abuso  
  - Medição de desempenho e relatórios  
  - Cumprimento de obrigações legais de consentimento e privacidade  

- **Regiões que exigem consentimento (EEE/Reino Unido/Suíça):**  
  - O consentimento é obtido por meio de avisos UMP.  
  - Um ecrã de **Opções de Privacidade** é disponibilizado para gerir ou alterar o consentimento.  

- **Outras regiões (por ex., Coreia):**  
  - Este ecrã pode **não estar visível** quando não for legalmente exigido.

---

## 3. Tratamento e períodos de retenção

- **Definições locais:** armazenadas no dispositivo até que o utilizador elimine os dados ou desinstale a aplicação.  
- **Ficheiros temporários:** criados durante processos de codificação/extração; apagados após o uso sempre que possível, podendo permanecer temporariamente em cache.  
- **Dados de anúncios/consentimento (terceiros):** geridos e retidos pelos próprios terceiros (por exemplo, Google), de acordo com as respetivas políticas.

---

## 4. Transferências para terceiros e fluxos transfronteiriços de dados

Para fins de publicidade e gestão de consentimento, algumas informações podem ser transferidas e tratadas nas infraestruturas da Google.

| Item | Detalhes |
|---|---|
| **Destinatário** | Google LLC e suas afiliadas/subprocessadores |
| **Destino** | Estados Unidos e outras regiões onde a Google mantém infraestruturas |
| **Finalidade** | Entrega de anúncios, medição de desempenho, prevenção de fraude, cumprimento legal, gestão de consentimento |
| **Dados tratados** | Identificadores de publicidade, dados de IP, informações de dispositivo/aplicação, sinais de interação, estado de consentimento, etc. |
| **Retenção** | De acordo com as políticas da Google |
| **Efeito da recusa** | Os anúncios personalizados podem ser limitados; anúncios não personalizados podem continuar a ser mostrados |

Cumprimos os requisitos de divulgação da secção **“Segurança de dados” do Google Play** e atualizamos as informações quando o tratamento de dados se altera.

---

## 5. Os seus direitos e como exercê-los

- **Opt-out de anúncios personalizados / alterar consentimento**  
  - Nas regiões EEE/Reino Unido/Suíça: utilize **Definições → Opções de Privacidade** na aplicação.  
  - Noutras regiões: utilize as definições do sistema operativo para redefinir identificadores de publicidade ou limitar a personalização de anúncios.  

- **Repor informações locais**  
  - Eliminar os dados da aplicação ou desinstalá-la remove as definições locais (posição da sobreposição, tamanho de letra, etc.).

Nos termos do **RGPD / RGPD do Reino Unido / FADP suíça / leis de privacidade de vários estados dos EUA**, poderá ter direitos como acesso, retificação, apagamento, portabilidade, restrição de tratamento e retirada de consentimento.  
Para dados de anúncios tratados pela Google, utilize os **mecanismos oficiais da Google**.

---

## 6. Privacidade de crianças

Esta aplicação **não se destina especificamente a crianças**.  
Se uma criança abaixo da idade mínima legal utilizar a aplicação, deverá interromper o uso e, com o apoio de um responsável, utilizar as funcionalidades de limitação de anúncios do sistema operativo.  
Quando apropriado, podemos aplicar **TFUA (etiqueta de conteúdo direcionado a crianças)** ou configurações semelhantes de proteção infantil.

---

## 7. Medidas de segurança

Adotamos, na medida do razoável:

- **Minimização de dados** na recolha e armazenamento  
- Uso limitado de ficheiros temporários e tentativa de os apagar após utilização  
- Tratamento restrito ao âmbito das permissões do sistema operativo  
- Utilização de **cifra TLS ou equivalente** nas transmissões para terceiros (de acordo com a implementação dos SDKs)

---

## 8. Segurança de dados no Google Play

Preenchemos e mantemos a secção **“Segurança de dados”** na Play Console de forma precisa, atualizando-a sempre que os nossos tratamentos de dados se alterem.

---

## 9. Avisos de código aberto

A aplicação utiliza software de código aberto, incluindo **FFmpeg**.  
Um ficheiro de informação na aplicação (por exemplo, `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) explica como obter o código-fonte.  
Mediante pedido, forneceremos o código-fonte conforme descrito nesse ficheiro.

---

## 10. Contacto

- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Alterações a esta Política

Podemos atualizar esta Política por motivos legais ou para refletir alterações no serviço.  
As atualizações serão comunicadas **na aplicação** e nesta página de política.  
Em caso de alterações materiais, daremos avisos **pelo menos 7 dias antes** da data de entrada em vigor.
