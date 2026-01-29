---
title: Política de Privacidade | Power lucky lotto
description: Política de Privacidade do Power lucky lotto (Português - Brasil)
lang: pt-br
last_updated: 2026-01-29
---

# Política de Privacidade (Power lucky lotto)

- **Nome do app:** Power lucky lotto  
- **Desenvolvedor:** frog-im  
- **Contato:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Data de vigência:** 2026-01-29  

> Esta política foi elaborada com referência a leis de privacidade aplicáveis, como a PIPA da Coreia, GDPR/UK GDPR, FADP da Suíça e leis estaduais relevantes dos EUA.  
> Se a sua região tiver requisitos obrigatórios específicos, esses requisitos terão prioridade.

---

## 1. Finalidade e escopo

Power lucky lotto é um aplicativo para gerenciar jogos de loteria e visualizar registros. Os principais recursos incluem:

- Seleção e configuração de país/jogo (ex.: KR 6/45, US Powerball)  
- Geração/salvamento de números e visualização de logs (histórico)  
- Visualização e exclusão de tabelas de log (lista/detalhe)  
- Edição/gerenciamento de dados de resultados via JSON (para estatísticas/visualização)  
- Anúncios (incluindo anúncios recompensados) e gestão de consentimento (quando exigido)

O app **não exige criação de conta** e, por padrão, **não envia seus dados para servidores do desenvolvedor.**  
A maior parte do processamento ocorre **no seu dispositivo**.

No entanto, para **publicidade**, **gestão de consentimento** e **conformidade legal**, SDKs de terceiros como  
**Google Mobile Ads SDK (AdMob)** e **Google UMP (User Messaging Platform)** podem coletar e processar alguns dados (por exemplo, identificadores de publicidade).

---

## 2. Tipos de dados processados

### 2-1) Dados armazenados no seu dispositivo (armazenamento local)

O app armazena certos dados **localmente no seu dispositivo** para fornecer recursos e melhorar a usabilidade.  
Esses dados, em geral, **não são transmitidos aos servidores do desenvolvedor** e são removidos quando você apaga os dados do app ou desinstala o app (exceto arquivos exportados para outro local).

#### (1) Configurações (SharedPreferences)

| Categoria | Chave (exemplo) | Finalidade | Armazenamento | Exclusão |
|---|---|---|---|---|
| Configuração concluída | `setup_done` | Armazenar estado de configuração inicial | SharedPreferences | Removido ao apagar dados/desinstalar |
| Histórico de países | `selected_countries` | Manter países selecionados recentemente | Mesmo | Mesmo |
| País ativo | `active_country` | Armazenar o país selecionado atualmente | Mesmo | Mesmo |
| Jogos selecionados | `selected_lotto_ids` | Armazenar IDs de jogos marcados | Mesmo | Mesmo |
| Jogo ativo | `active_lotto_id` | Armazenar o ID do jogo ativo | Mesmo | Mesmo |
| **Seleção de horário seed (opcional)** | `birth_datetime_iso` | Armazenar um horário de referência seed escolhido pelo usuário (pode ser usado para seed/personalização) | Mesmo | Mesmo |

> **Observação:** “Seleção de horário seed (opcional)” só é coletada se o usuário optar por definir, e pode não ser necessária para o uso principal do app.

#### (2) Dados de log (SQLite)

O app pode armazenar registros gerados/salvos em um banco de dados SQLite local.

- Tabelas de exemplo: `log_...`  
- Campos de exemplo:  
  - `id`, `date_id` ou `date_text` (timestamp), `choice1..choiceN` (números escolhidos), `isFinger` (flag relacionada a impressão digital, etc.)

Você pode visualizar os logs nas telas de lista/detalhe de tabelas e excluí-los (por tabela ou por linha), se desejar.

#### (3) Arquivos JSON (por jogo)

O app pode armazenar dados JSON específicos do jogo no diretório de documentos do app.

- Exemplo: `game_json/<gameId>.json`  
- Finalidade: dados de sorteios/resultados gerenciados/editáveis pelo usuário (por exemplo, para estatísticas/visualização)

Esses arquivos são armazenados no dispositivo e, em muitos casos, são removidos ao desinstalar o app, sujeito ao comportamento de backup do sistema operacional.

---

### 2-2) Anúncios, consentimento e dados relacionados (SDKs de terceiros)

O app usa **Google Mobile Ads SDK (AdMob)** e **Google UMP** para:

- Exibir anúncios (incluindo **anúncios recompensados**)  
- Gerenciar o consentimento legalmente exigido para publicidade

Esses SDKs podem coletar/processar, por exemplo:

- **ID de publicidade** (ex.: AAID, IDFA)  
- Informações baseadas em IP, localização aproximada, informações de rede  
- Informações do dispositivo/app (versão do SO, versão do app, idioma, informações de diagnóstico)  
- Interações com anúncios (impressões, cliques, conclusão de recompensa)  
- Escolhas de consentimento registradas pelo UMP

Em algumas regiões (por exemplo, EEE/Reino Unido/Suíça), um formulário de consentimento UMP pode ser exibido e uma opção de **Privacy Options** pode ser fornecida quando exigido.

---

## 3. Retenção

- **Configurações locais (SharedPreferences):** mantidas até exclusão de dados do app ou desinstalação  
- **Dados de log (SQLite):** mantidos até você excluir ou limpar dados do app/desinstalar  
- **Arquivos JSON:** armazenados no diretório de documentos do app; removidos ao desinstalar em muitos casos, mas exportações/backups são gerenciados pelo usuário  
- **Dados de anúncios/consentimento (terceiros):** retidos conforme políticas do Google e leis aplicáveis

---

## 4. Compartilhamento com terceiros e transferências internacionais

Para anúncios e gestão de consentimento, alguns dados podem ser processados pelo **Google e seus parceiros**.

| Item | Detalhes |
|---|---|
| **Destinatários** | Google LLC, afiliadas e subprocessadores |
| **Destinos de transferência** | Estados Unidos e outras regiões onde a infraestrutura do Google está localizada |
| **Finalidade** | Entrega de anúncios, medição, prevenção de fraudes, gestão de consentimento, conformidade |
| **Dados** | ID de publicidade, info baseada em IP, info do dispositivo/app, dados de interação com anúncios, status de consentimento |
| **Retenção** | Conforme políticas do Google e leis aplicáveis |
| **Impacto se você recusar** | Anúncios personalizados podem ser limitados; anúncios não personalizados ou menos anúncios podem ser exibidos |

---

## 5. Seus direitos e como exercê-los

Dependendo da lei aplicável, você pode ter direitos como acesso, correção, exclusão, restrição, oposição, portabilidade e retirada do consentimento (quando o consentimento for a base legal).

Exemplos:

- **Ajustar escolhas de anúncios/consentimento:** via Privacy Options no app (quando disponível) ou configurações de anúncios do sistema (redefinir ID de publicidade, limitar personalização).  
- **Redefinir dados locais:** limpar dados do app ou desinstalar o app para remover configurações/logs/arquivos armazenados pelo app.

---

## 6. Privacidade de crianças

Este app **não foi projetado para crianças**. Se uma criança usar o app, um responsável deve considerar usar controles parentais do sistema e recursos de limitação de anúncios.

---

## 7. Medidas de segurança

Dentro do escopo do app, buscamos:

- Armazenar apenas o mínimo necessário de dados localmente  
- Manter o processamento no dispositivo sempre que possível  
- Utilizar TLS/transporte seguro para comunicações de rede de SDK (dentro das capacidades do SDK)

---

## 8. Google Play Data safety

Se distribuído no Google Play, buscamos manter as declarações de Data safety precisas e atualizadas, especialmente quando SDKs ou práticas de processamento mudarem.

---

## 9. Avisos de código aberto

O app pode usar bibliotecas open source para ícones de países, armazenamento, anúncios/consentimento e UI.  
Os avisos de licença estão disponíveis na tela “Licenças de código aberto” do app (ou equivalente).

---

## 10. Contato

Para questões de privacidade:

- **E-mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Mencione **“Power lucky lotto”** na sua mensagem.

---

## 11. Alterações nesta política

Esta política pode mudar devido a atualizações legais, mudanças de recursos (por exemplo, novos SDKs) ou ajustes internos.  
Mudanças menores serão publicadas no app ou nesta página; mudanças materiais serão anunciadas com antecedência conforme exigido.
