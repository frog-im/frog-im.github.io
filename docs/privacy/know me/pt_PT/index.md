---
title: Política de Privacidade | know_me
description: know_me (PeopleNote, Memory for People) Política de Privacidade (Português de Portugal)
---

# Política de Privacidade (know_me / PeopleNote, Memory for People)

- **Nome da aplicação:** know_me (PeopleNote, Memory for People)
- **Programador:** frog-im
- **Responsável pela Proteção de Dados Pessoais / Pessoa de Contacto:** frog-im
- **Contacto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data de Entrada em Vigor:** 2026-03-04
- **Última Atualização:** 2026-03-04

> A presente Política foi elaborada com base nas informações tratadas pela aplicação e nas respetivas funcionalidades.  
> Caso existam leis ou regulamentos obrigatórios aplicáveis num país ou região específica, essas leis ou regulamentos poderão prevalecer.

---

## 1. Finalidade e Âmbito

`know_me` é uma aplicação concebida para ajudar os utilizadores a registar e gerir informações sobre pessoas e, quando necessário, a efetuar cópias de segurança, restaurar e partilhar essas informações em ficheiros PDF.

As suas principais funcionalidades incluem:

- Armazenar informações específicas sobre cada pessoa (tais como nome, texto de identificação, notas, traços de personalidade, país, género, informações de contacto, etc.)
- Classificação em pastas, pesquisa e funções de fusão
- Anexar fotografias e gerir descrições
- Exportar e importar cópias de segurança (`.knm`)
- Exportar PDFs
- Bloqueio da aplicação (palavra-passe / padrão)
- Gestão de publicidade e consentimento (AdMob / UMP)

A aplicação não exige um registo de conta separado e os dados principais do utilizador são, em geral, armazenados localmente no dispositivo do utilizador.  
No entanto, determinados SDK de terceiros incluídos para efeitos de gestão de publicidade e consentimento podem tratar algumas informações.

---

## 2. Categorias de Dados Pessoais Tratados

### 2-1) Informações introduzidas diretamente pelo utilizador

As seguintes informações são armazenadas apenas quando o utilizador as introduz diretamente:

- Nome
- Texto de identificação (por exemplo, aparência / características usadas como texto de nota)
- Notas
- Traços de personalidade, país, género
- Número de telefone
- Texto relacionado com o momento de aparição / momento do encontro
- Informações de plataforma / site
- Nome / cor da pasta
- Descrição da imagem (caption)

### 2-2) Ficheiros selecionados no dispositivo

- Ficheiros de imagem selecionados pelo utilizador ao anexar fotografias
- Ficheiros de cópia de segurança `.knm` selecionados pelo utilizador ao importar cópias de segurança
- Caminhos de gravação e ficheiros guardados selecionados pelo utilizador ao exportar PDFs / cópias de segurança

### 2-3) Dados armazenados localmente na aplicação

Os seguintes dados podem ser armazenados no dispositivo do utilizador para disponibilizar as funcionalidades da aplicação:

- Base de dados SQLite (`people_note.db`): metadados relativos a pessoas / pastas / plataformas / sites / imagens
- Ficheiros de imagem: encriptados e armazenados na pasta de documentos da aplicação (`.enc`)
- Definições da aplicação (`SharedPreferences`): tema, ordenação, opções de privacidade / publicidade, opções de mascaramento de PDF, políticas de bloqueio da aplicação, etc.
- Informações de bloqueio da aplicação: valores hash e salts de palavras-passe / padrões (`SharedPreferences`)
- Chaves de encriptação locais: armazenadas em `flutter_secure_storage`
- Ficheiros temporários: pré-visualizações de desencriptação de imagens, ficheiros de cache de importação / exportação, etc. (pasta temporária)

### 2-4) Informações que podem ser tratadas automaticamente durante a gestão de publicidade e consentimento

Quando as funcionalidades de publicidade ou gestão de consentimento estão ativadas, os SDK da Google LLC e de parceiros relacionados (como AdMob e UMP) podem tratar automaticamente as seguintes informações:

- Identificadores de publicidade (AAID / IDFA, etc.)
- Endereço IP e informações de rede
- Informações do dispositivo (versão do sistema operativo, modelo do dispositivo, versão da aplicação, etc.)
- Informações de interação com anúncios (impressões, cliques, etc.)
- Estado do consentimento e informações sobre escolhas de privacidade
- Informações relacionadas com diagnóstico, desempenho e segurança

Os registos principais do utilizador da aplicação não são, em geral, carregados para o servidor do programador, mas parte das informações acima poderá ser transmitida a serviços de terceiros enquanto as funcionalidades de publicidade / consentimento estiverem em utilização.

---

## 3. Finalidade do Tratamento de Dados Pessoais

A aplicação trata dados pessoais ou informações relacionadas para as seguintes finalidades:

- Registar e consultar informações sobre pessoas com foco em contactos / notas
- Disponibilizar funcionalidades de organização, como classificação em pastas, pesquisa e fusão
- Anexar e apresentar fotografias
- Executar funcionalidades solicitadas pelo utilizador, como cópia de segurança / restauro e exportação para PDF
- Disponibilizar funcionalidades de segurança de bloqueio da aplicação
- Disponibilizar publicidade, gerir o consentimento, prevenir atividades fraudulentas e cumprir obrigações legais

---

## 4. Prazo de Conservação e Armazenamento de Dados Pessoais

- Dados internos da aplicação (SQLite, definições locais, imagens encriptadas): conservados no dispositivo do utilizador até que a aplicação seja eliminada, os dados da aplicação sejam apagados ou o utilizador elimine diretamente os dados
- Ficheiros temporários: eliminados após a conclusão da tarefa relevante ou limpos de acordo com a política de cache do sistema operativo
- Ficheiros exportados pelo utilizador (PDF, ficheiros de cópia de segurança): podem permanecer no local de armazenamento selecionado pelo utilizador e devem ser eliminados diretamente pelo utilizador
- Dados relacionados com publicidade / consentimento (tratados por terceiros): sujeitos às políticas de cada prestador de serviços e às leis aplicáveis

Em princípio, a aplicação não armazena os registos principais do utilizador no servidor do programador.  
No entanto, os ficheiros que o utilizador guarda diretamente em armazenamento externo são geridos no próprio ambiente do utilizador.

---

## 5. Procedimentos e Métodos de Eliminação de Dados Pessoais

Quando a finalidade do tratamento tiver sido atingida, ou quando o utilizador solicitar a eliminação, a aplicação elimina as informações relevantes ou trata-as de forma a deixarem de ser referenciadas, da seguinte forma.

### 5-1) Procedimentos de eliminação

- Quando o utilizador elimina diretamente registos individuais de pessoas, pastas, imagens, dados de cópia de segurança, etc., esses dados são considerados sujeitos a eliminação imediata.
- Quando o utilizador elimina a aplicação ou apaga os dados da aplicação nas definições do dispositivo, os dados armazenados na área de armazenamento interno da aplicação são removidos de acordo com os procedimentos de eliminação do sistema operativo.
- Os ficheiros temporários tornam-se sujeitos a limpeza após o término da tarefa relevante, e alguns dados em cache podem permanecer durante um determinado período, consoante a política do sistema operativo.

### 5-2) Métodos de eliminação

- Dados SQLite: eliminação dos registos relevantes
- Definições da aplicação (`SharedPreferences`): eliminação da chave relevante ou de todas as definições
- Valores de `flutter_secure_storage`: eliminação dos itens relevantes de armazenamento seguro
- Ficheiros internos da aplicação (imagens encriptadas, ficheiros temporários, etc.): eliminação dos ficheiros relevantes
- PDFs / ficheiros de cópia de segurança guardados diretamente pelo utilizador em armazenamento externo: não são eliminados automaticamente pela aplicação e devem ser eliminados diretamente pelo utilizador

Salvo se as leis aplicáveis exigirem o contrário, o programador não armazena separadamente os registos principais do utilizador no servidor do programador.

---

## 6. Comunicação a Terceiros, Subcontratação do Tratamento e Transferência Transfronteiriça

A aplicação pode utilizar serviços da Google para a gestão de publicidade e consentimento.

| Item | Detalhes |
|---|---|
| **Destinatário / Entidade Subcontratada** | Google LLC e as suas afiliadas (operadores do AdMob / UMP) |
| **País de transferência** | Estados Unidos e regiões onde a infraestrutura da Google é operada |
| **Momento da transferência** | De forma contínua durante pedidos de anúncios, verificações do estado do consentimento, inicialização do SDK e funcionamento |
| **Método de transferência** | Transmissão através de comunicação em rede entre a aplicação e servidores de terceiros |
| **Base jurídica para a transferência transfronteiriça** | Tratamento efetuado no âmbito necessário para prestar o serviço com base nos fundamentos jurídicos aplicáveis ou, quando necessário, com base no consentimento do titular dos dados |
| **Finalidade** | Apresentação de anúncios, medição de anúncios, gestão do consentimento, prevenção de fraude e conformidade com políticas / leis |
| **Categorias de dados (exemplos)** | Identificadores de publicidade (AAID / IDFA), informações de IP / rede, informações do dispositivo / aplicação, informações de interação com anúncios, estado do consentimento |
| **Prazo de conservação** | Sujeito às políticas da Google e às leis aplicáveis |
| **Efeito da recusa** | Os anúncios personalizados podem ser limitados, podem ser apresentados anúncios não personalizados ou algumas funcionalidades relacionadas com anúncios podem ser restringidas |

O programador não recolhe nem vende os dados principais dos registos de pessoas da aplicação através do seu próprio servidor.

---

## 7. Informações sobre as Permissões Utilizadas

A aplicação pode utilizar as seguintes permissões:

- `INTERNET`: comunicação para SDK de publicidade e funcionalidades de rede relacionadas
- `com.google.android.gms.permission.AD_ID`: utilização de identificadores de publicidade (AdMob)
- `READ_MEDIA_IMAGES` (Android 13+), `READ_EXTERNAL_STORAGE` (Android 12 e anteriores): anexar / selecionar fotografias

As permissões são utilizadas apenas no âmbito necessário para disponibilizar as funcionalidades relevantes.

---

## 8. Instalação, Funcionamento e Recusa de Mecanismos de Recolha Automática

Esta aplicação não utiliza diretamente cookies gerais de websites.  
No entanto, em ligação com as funcionalidades de publicidade e gestão de consentimento, SDK de terceiros podem tratar automaticamente identificadores de publicidade, informações de rede, informações do dispositivo e dados semelhantes.

Os utilizadores podem ajustar as definições relevantes das seguintes formas:

- Alterar as seleções nas opções de privacidade da aplicação ou no ecrã de gestão de consentimento (quando disponível)
- Repor ou eliminar o identificador de publicidade nas definições do sistema operativo do dispositivo
- Limitar anúncios personalizados ou ajustar opções de privacidade relacionadas nas definições do sistema operativo do dispositivo

Se o utilizador limitar a publicidade personalizada, poderão ser apresentados anúncios não personalizados ou determinadas funcionalidades relacionadas com anúncios poderão ser restringidas.

---

## 9. Direitos do Utilizador e Como Exercê-los

Sujeito às leis aplicáveis, os utilizadores podem ter os seguintes direitos:

- Solicitar acesso, retificação ou eliminação de dados pessoais
- Solicitar a suspensão ou limitação do tratamento
- Retirar o consentimento para tratamento baseado em consentimento
- Alterar as opções de publicidade / consentimento

Estes direitos podem ser exercidos das seguintes formas:

- Modificar ou eliminar dados diretamente na aplicação
- Inicializar dados locais eliminando os dados da aplicação ou desinstalando a aplicação
- Alterar o consentimento de publicidade através das opções de privacidade / ecrã de consentimento da aplicação (nas regiões em que tal esteja disponível)
- Repor / eliminar o identificador de publicidade ou limitar anúncios personalizados através das definições do sistema operativo do dispositivo
- Contacto: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Medidas de Segurança

O programador aplica ou procura aplicar as seguintes medidas:

- Os registos do utilizador são, em geral, armazenados localmente no dispositivo
- Os ficheiros de imagem anexados são armazenados localmente de forma encriptada (com base em AES-GCM)
- As informações de bloqueio da aplicação são armazenadas sob a forma de hash, e não em texto simples
- Os ficheiros de cópia de segurança são armazenados após serem encriptados com base numa palavra-passe do utilizador
- A comunicação com SDK de terceiros é encriptada (HTTPS / TLS)
- As permissões são utilizadas com o mínimo de acesso necessário

No entanto, os riscos decorrentes do estado de segurança do dispositivo do utilizador (como root / jailbreak, aplicações maliciosas ou exposição de armazenamento partilhado) não podem ser totalmente eliminados.

---

## 11. Informações Relativas a Dados Sensíveis

Esta aplicação não exige a introdução de dados sensíveis.  
Os utilizadores são aconselhados a não introduzir conteúdos sensíveis, como informações de saúde, opiniões políticas, religião, informações biométricas ou informações relacionadas com a vida sexual, em notas ou campos de entrada livre.

Se um utilizador introduzir voluntariamente conteúdo sensível, essas informações poderão ser armazenadas como dados locais no dispositivo gerido diretamente pelo utilizador.

---

## 12. Proteção de Dados Pessoais de Crianças

Esta aplicação não foi concebida principalmente para crianças.  
Os encarregados de educação podem gerir a utilização através de funcionalidades de controlo parental disponibilizadas pelo dispositivo ou pela loja de aplicações.

---

## 13. Tomada de Decisão Automatizada

Esta aplicação não realiza tomada de decisão automatizada com base em dados pessoais que produza efeitos jurídicos ou impactos significativos semelhantes.

---

## 14. Aviso de Segurança dos Dados (Google Play, etc.)

O programador procura manter e atualizar os elementos de divulgação de segurança dos dados nas lojas de aplicações (como a Google Play) de acordo com as práticas reais de tratamento da aplicação e as práticas reais de tratamento dos SDK de terceiros.

No entanto, as informações apresentadas nas lojas de aplicações podem variar consoante a versão da aplicação, o país de distribuição, a configuração dos SDK de terceiros e as alterações de políticas.

---

## 15. Aviso de Código Aberto

A aplicação utiliza determinadas bibliotecas de código aberto.  
As informações sobre as licenças correspondentes podem ser encontradas no ecrã relevante dentro da aplicação ou nos avisos disponibilizados através do canal de distribuição.

---

## 16. Contacto

Para questões relacionadas com a presente Política de Privacidade:

- **Responsável pela Proteção de Dados Pessoais / Pessoa de Contacto:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 17. Alterações a esta Política de Privacidade

A presente Política poderá ser revista devido a alterações em leis / políticas, funcionalidades da aplicação ou SDK de terceiros.  
Se existirem alterações materiais, poderá ser efetuada uma notificação através de avisos na aplicação, da página de distribuição ou de atualizações da página da política.

Última Atualização: **2026-03-04**