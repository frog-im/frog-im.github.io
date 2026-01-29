---
title: Política de Privacidade | Power lucky lotto
description: Política de Privacidade do Power lucky lotto (Português)
lang: pt
last_updated: 2026-01-29
---

# Política de Privacidade (Power lucky lotto)

- **Nome da aplicação:** Power lucky lotto  
- **Desenvolvedor:** frog-im  
- **Contacto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Data de entrada em vigor:** 2026-01-29  

> Esta política foi redigida com referência a leis de privacidade aplicáveis, como a PIPA (Coreia), GDPR/UK GDPR, FADP (Suíça) e leis de privacidade relevantes de estados dos EUA.  
> Se a sua região tiver requisitos obrigatórios específicos, esses requisitos prevalecem.

---

## 1. Finalidade e âmbito

O Power lucky lotto é uma aplicação para gerir jogos de lotaria e visualizar registos. As principais funcionalidades incluem:

- Seleção e configuração de país/jogo (por exemplo, KR 6/45, US Powerball)  
- Geração/armazenamento de números e visualização de logs (histórico)  
- Visualização e eliminação de tabelas de log (lista/detalhe)  
- Edição/gestão de dados de resultados via JSON (para estatísticas/visualização)  
- Anúncios (incluindo anúncios recompensados) e gestão de consentimento (quando aplicável)

A aplicação **não exige criação de conta** e, por defeito, **não envia os seus dados para servidores do desenvolvedor.**  
A maior parte do processamento ocorre **no seu dispositivo**.

No entanto, para **publicidade**, **gestão de consentimento** e **conformidade legal**, SDKs de terceiros, como  
**Google Mobile Ads SDK (AdMob)** e **Google UMP (User Messaging Platform)**, podem recolher e processar certos dados (por exemplo, identificadores de publicidade).

---

## 2. Tipos de dados processados

### 2-1) Dados armazenados no seu dispositivo (armazenamento local)

A aplicação armazena alguns dados **localmente no seu dispositivo** para fornecer funcionalidades e melhorar a usabilidade.  
Estes dados, em geral, **não são transmitidos para servidores do desenvolvedor** e são removidos quando elimina os dados da aplicação ou desinstala a aplicação (exceto ficheiros que exporte para outro local).

#### (1) Definições (SharedPreferences)

| Categoria | Chave (exemplo) | Finalidade | Armazenamento | Eliminação |
|---|---|---|---|---|
| Configuração concluída | `setup_done` | Guardar o estado de configuração inicial | SharedPreferences | Removido ao eliminar dados/desinstalar |
| Histórico de países | `selected_countries` | Guardar países selecionados recentemente | Idem | Idem |
| País ativo | `active_country` | Guardar o país atualmente selecionado | Idem | Idem |
| Jogos selecionados | `selected_lotto_ids` | Guardar IDs de jogos assinalados | Idem | Idem |
| Jogo ativo | `active_lotto_id` | Guardar o ID do jogo ativo | Idem | Idem |
| **Seleção de hora seed (opcional)** | `birth_datetime_iso` | Guardar uma hora de referência seed escolhida pelo utilizador (pode ser usada para seeding/personalização) | Idem | Idem |

> **Nota:** “Seleção de hora seed (opcional)” só é tratada se o utilizador optar por a definir e pode não ser necessária para o uso principal da aplicação.

#### (2) Dados de log (SQLite)

A aplicação pode armazenar registos gerados/guardados numa base de dados SQLite local.

- Exemplos de tabelas: `log_...`  
- Exemplos de campos:  
  - `id`, `date_id` ou `date_text` (timestamp), `choice1..choiceN` (números escolhidos), `isFinger` (sinalizador relacionado com impressão digital, etc.)

Pode visualizar os logs nos ecrãs de lista/detalhe de tabelas e eliminá-los (por tabela ou por linha), se desejar.

#### (3) Ficheiros de dados JSON (por jogo)

A aplicação pode guardar dados JSON específicos por jogo no diretório de documentos da aplicação.

- Exemplo: `game_json/<gameId>.json`  
- Finalidade: dados de sorteios/resultados geridos/editáveis pelo utilizador (por exemplo, para estatísticas/visualização)

Estes ficheiros são armazenados no dispositivo e, em geral, são removidos ao desinstalar, dependendo do comportamento do sistema/backup.

---

### 2-2) Anúncios, consentimento e dados relacionados (SDK de terceiros)

A aplicação utiliza **Google Mobile Ads SDK (AdMob)** e **Google UMP** para:

- Exibir anúncios (incluindo **anúncios recompensados**)  
- Gerir o consentimento legalmente exigido para publicidade

Estes SDKs podem recolher/processar, por exemplo:

- **ID de Publicidade** (por exemplo, AAID, IDFA)  
- Informações baseadas em IP, localização aproximada, informações de rede  
- Informações do dispositivo/aplicação (versão do SO, versão da app, idioma, informações de diagnóstico)  
- Interações com anúncios (impressões, cliques, conclusão de recompensa)  
- Opções de consentimento registadas pelo UMP

Em algumas regiões (por exemplo, EEA/UK/CH), pode ser apresentado um formulário de consentimento UMP e pode existir uma entrada **Privacy Options** quando exigido.

---

## 3. Retenção

- **Definições locais (SharedPreferences):** mantidas até eliminar dados da app ou desinstalar  
- **Dados de log (SQLite):** mantidos até os eliminar ou desinstalar/limpar dados da app  
- **Ficheiros JSON:** armazenados no diretório de documentos; muitas vezes removidos ao desinstalar, mas exportações/backups são geridos pelo utilizador  
- **Dados de anúncios/consentimento (terceiros):** retidos segundo as políticas da Google e a lei aplicável

---

## 4. Partilha com terceiros e transferências internacionais

Para anúncios e gestão de consentimento, alguns dados podem ser tratados pela **Google e pelos seus parceiros**.

| Item | Detalhes |
|---|---|
| **Destinatários** | Google LLC, afiliadas e subcontratantes (subprocessadores) |
| **Destinos de transferência** | Estados Unidos e outras regiões onde a infraestrutura da Google está localizada |
| **Finalidade** | Entrega de anúncios, medição, prevenção de fraude, gestão de consentimento, conformidade |
| **Dados** | ID de Publicidade, informações baseadas em IP, informações do dispositivo/app, dados de interação com anúncios, estado de consentimento |
| **Retenção** | Conforme políticas da Google e lei aplicável |
| **Impacto se recusar** | Anúncios personalizados podem ser limitados; podem ser exibidos anúncios não personalizados ou menos anúncios |

---

## 5. Os seus direitos e como exercê-los

Dependendo da lei aplicável, pode ter direitos como acesso, correção, eliminação, limitação, oposição, portabilidade e retirada de consentimento (quando o consentimento for a base legal).

Exemplos:

- **Ajustar opções de anúncios/consentimento:** via Privacy Options na app (quando disponível) ou definições de anúncios do SO (repor ID de publicidade, limitar personalização).  
- **Repor dados locais:** limpar dados da app ou desinstalar para remover definições/logs/ficheiros locais guardados pela app.

---

## 6. Privacidade de crianças

Esta aplicação **não foi concebida para crianças**. Se uma criança a utilizar, o responsável deve considerar controlos parentais ao nível do SO e funcionalidades de limitação de anúncios.

---

## 7. Medidas de segurança

No âmbito da aplicação, esforçamo-nos por:

- Armazenar localmente apenas o mínimo de dados necessário  
- Manter o processamento no dispositivo sempre que possível  
- Utilizar TLS/transporte seguro para comunicações de rede dos SDKs (dentro das capacidades dos SDKs)

---

## 8. Google Play Data safety

Se distribuída no Google Play, procuramos manter as divulgações de Data safety corretas e atualizadas, especialmente quando os SDKs ou práticas de tratamento mudam.

---

## 9. Avisos de código aberto

A aplicação pode utilizar bibliotecas open-source para ícones de países, armazenamento, anúncios/consentimento e UI.  
Os avisos de licença estão disponíveis no ecrã “Open-source licenses” (ou equivalente) na aplicação.

---

## 10. Contacto

Para questões de privacidade:

- **E-mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Indique **“Power lucky lotto”** na sua mensagem.

---

## 11. Alterações a esta política

Esta política pode mudar devido a atualizações legais, alterações de funcionalidades (por exemplo, novos SDKs) ou ajustes internos.  
Alterações menores serão publicadas na app ou nesta página; alterações materiais serão anunciadas antecipadamente conforme exigido.
