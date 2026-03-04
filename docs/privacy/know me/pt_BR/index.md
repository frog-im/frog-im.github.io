---
title: Política de Privacidade | know_me
description: know_me (PeopleNote, Memory for People) Política de Privacidade (Português do Brasil)
---

# Política de Privacidade (know_me / PeopleNote, Memory for People)

- **Nome do aplicativo:** know_me (PeopleNote, Memory for People)
- **Desenvolvedor:** frog-im
- **Encarregado pela Proteção de Dados / Pessoa de Contato:** frog-im
- **Contato:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data de Vigência:** 2026-03-04
- **Última Atualização:** 2026-03-04

> Esta Política foi elaborada com base nas informações processadas pelo aplicativo e em seus recursos relacionados.  
> Caso leis ou regulamentos obrigatórios se apliquem em um país ou região específica, tais leis ou regulamentos poderão prevalecer.

---

## 1. Finalidade e Escopo

`know_me` é um aplicativo desenvolvido para ajudar os usuários a registrar e gerenciar informações sobre pessoas e, quando necessário, fazer backup, restaurar e compartilhar essas informações em arquivos PDF.

Seus principais recursos incluem:

- Armazenar informações específicas sobre cada pessoa (como nome, texto de identificação, notas, traços de personalidade, país, gênero, informações de contato etc.)
- Classificação em pastas, busca e funções de mesclagem
- Anexar fotos e gerenciar descrições
- Exportar e importar backups (`.knm`)
- Exportar PDFs
- Bloqueio do aplicativo (senha/padrão)
- Gerenciamento de publicidade e consentimento (AdMob/UMP)

O aplicativo não exige registro de conta separado, e os dados principais do usuário geralmente são armazenados localmente no dispositivo do usuário.  
No entanto, determinados SDKs de terceiros incluídos para gerenciamento de publicidade e consentimento podem processar algumas informações.

---

## 2. Categorias de Dados Pessoais Processados

### 2-1) Informações inseridas diretamente pelo usuário

As seguintes informações são armazenadas somente quando o usuário as insere diretamente:

- Nome
- Texto de identificação (como aparência/características usadas como texto de anotação)
- Notas
- Traços de personalidade, país, gênero
- Número de telefone
- Texto relacionado ao horário de aparição / momento do encontro
- Informações de plataforma/site
- Nome/cor da pasta
- Descrição da imagem (caption)

### 2-2) Arquivos selecionados no dispositivo

- Arquivos de imagem selecionados pelo usuário ao anexar fotos
- Arquivos de backup `.knm` selecionados pelo usuário ao importar backups
- Caminhos de salvamento e arquivos salvos selecionados pelo usuário ao exportar PDFs/backups

### 2-3) Dados armazenados localmente no aplicativo

Os seguintes dados podem ser armazenados no dispositivo do usuário para fornecer os recursos do aplicativo:

- Banco de dados SQLite (`people_note.db`): metadados de pessoas/pastas/plataformas/sites/imagens
- Arquivos de imagem: criptografados e armazenados na pasta de documentos do aplicativo (`.enc`)
- Configurações do aplicativo (`SharedPreferences`): tema, ordenação, opções de privacidade/publicidade, opções de mascaramento de PDF, políticas de bloqueio do aplicativo etc.
- Informações de bloqueio do aplicativo: valores de hash e salts para senhas/padrões (`SharedPreferences`)
- Chaves de criptografia locais: armazenadas em `flutter_secure_storage`
- Arquivos temporários: pré-visualizações de descriptografia de imagens, arquivos de cache de importação/exportação etc. (pasta temporária)

### 2-4) Informações que podem ser processadas automaticamente durante o gerenciamento de publicidade e consentimento

Quando os recursos de publicidade ou gerenciamento de consentimento estão habilitados, os SDKs da Google LLC e de parceiros relacionados (como AdMob e UMP) podem processar automaticamente as seguintes informações:

- Identificadores de publicidade (AAID/IDFA etc.)
- Endereço IP e informações de rede
- Informações do dispositivo (versão do sistema operacional, modelo do dispositivo, versão do aplicativo etc.)
- Informações de interação com anúncios (impressões, cliques etc.)
- Status de consentimento e informações sobre escolhas de privacidade
- Informações relacionadas a diagnóstico, desempenho e segurança

Os registros principais do usuário do aplicativo geralmente não são enviados ao servidor do desenvolvedor, mas algumas das informações acima podem ser transmitidas a serviços de terceiros enquanto os recursos de publicidade/consentimento estiverem em uso.

---

## 3. Finalidade do Tratamento de Dados Pessoais

O aplicativo processa dados pessoais ou informações relacionadas para as seguintes finalidades:

- Registrar e consultar informações sobre pessoas com foco em contatos/anotações
- Fornecer recursos de organização, como classificação em pastas, busca e mesclagem
- Anexar e exibir fotos
- Executar recursos solicitados pelo usuário, como backup/restauração e exportação em PDF
- Fornecer recursos de segurança de bloqueio do aplicativo
- Fornecer publicidade, gerenciar consentimento, prevenir atividades fraudulentas e cumprir obrigações legais

---

## 4. Período de Retenção e Armazenamento de Dados Pessoais

- Dados internos do aplicativo (SQLite, configurações locais, imagens criptografadas): mantidos no dispositivo do usuário até que o aplicativo seja excluído, os dados do aplicativo sejam apagados ou o usuário exclua os dados diretamente
- Arquivos temporários: excluídos após a conclusão da tarefa relevante ou limpos de acordo com a política de cache do sistema operacional
- Arquivos exportados pelo usuário (PDFs, arquivos de backup): podem permanecer no local de armazenamento selecionado pelo usuário e devem ser excluídos diretamente pelo usuário
- Dados relacionados à publicidade/consentimento (processados por terceiros): sujeitos às políticas de cada prestador de serviço e às leis aplicáveis

Em princípio, o aplicativo não armazena os registros principais do usuário no servidor do desenvolvedor.  
No entanto, arquivos que o usuário salva diretamente em armazenamento externo são gerenciados dentro do próprio ambiente do usuário.

---

## 5. Procedimentos e Métodos para Eliminação de Dados Pessoais

Quando a finalidade do tratamento tiver sido atingida ou quando o usuário solicitar a exclusão, o aplicativo elimina as informações relevantes ou as processa de forma que deixem de ser referenciadas, da seguinte forma.

### 5-1) Procedimentos de eliminação

- Quando o usuário exclui diretamente registros individuais de pessoas, pastas, imagens, dados de backup etc., esses dados são tratados como sujeitos à eliminação imediata.
- Quando o usuário exclui o aplicativo ou limpa os dados do aplicativo nas configurações do dispositivo, os dados armazenados na área de armazenamento interno do aplicativo são removidos de acordo com os procedimentos de exclusão do sistema operacional.
- Arquivos temporários ficam sujeitos à limpeza após o término da tarefa relevante, e alguns dados em cache podem permanecer por determinado período, dependendo da política do sistema operacional.

### 5-2) Métodos de eliminação

- Dados SQLite: exclusão dos registros relevantes
- Configurações do aplicativo (`SharedPreferences`): exclusão da chave relevante ou de todas as configurações
- Valores de `flutter_secure_storage`: exclusão dos itens relevantes de armazenamento seguro
- Arquivos internos do aplicativo (imagens criptografadas, arquivos temporários etc.): exclusão dos arquivos relevantes
- PDFs/arquivos de backup salvos diretamente pelo usuário em armazenamento externo: não são excluídos automaticamente pelo aplicativo e devem ser excluídos diretamente pelo usuário

Salvo quando exigido de outra forma pelas leis aplicáveis, o desenvolvedor não armazena separadamente os registros principais do usuário no servidor do desenvolvedor.

---

## 6. Fornecimento a Terceiros, Tratamento por Terceiros e Transferência Internacional

O aplicativo pode usar serviços do Google para gerenciamento de publicidade e consentimento.

| Item | Detalhes |
|---|---|
| **Destinatário / Operador encarregado** | Google LLC e suas afiliadas (operadores do AdMob/UMP) |
| **País de transferência** | Estados Unidos e regiões onde a infraestrutura do Google é operada |
| **Momento da transferência** | De forma contínua durante solicitações de anúncios, verificações do status de consentimento, inicialização do SDK e operação |
| **Método de transferência** | Transmissão por meio de comunicação em rede entre o aplicativo e servidores de terceiros |
| **Base legal para a transferência internacional** | Processamento realizado dentro do escopo necessário para fornecer o serviço com base em fundamentos legais aplicáveis ou, quando necessário, com base no consentimento do titular dos dados |
| **Finalidade** | Veiculação de anúncios, medição de anúncios, gerenciamento de consentimento, prevenção de fraude e conformidade com políticas/leis |
| **Categorias de dados (exemplos)** | Identificadores de publicidade (AAID/IDFA), informações de IP/rede, informações de dispositivo/aplicativo, informações de interação com anúncios, status de consentimento |
| **Período de retenção** | Sujeito às políticas do Google e às leis aplicáveis |
| **Efeito da recusa** | Anúncios personalizados podem ser limitados, anúncios não personalizados podem ser exibidos ou alguns recursos relacionados a anúncios podem ser restringidos |

O desenvolvedor não coleta nem vende os dados principais dos registros de pessoas do aplicativo por meio de seu próprio servidor.

---

## 7. Informações sobre as Permissões Utilizadas

O aplicativo pode usar as seguintes permissões:

- `INTERNET`: comunicação para SDKs de publicidade e recursos de rede relacionados
- `com.google.android.gms.permission.AD_ID`: uso de identificadores de publicidade (AdMob)
- `READ_MEDIA_IMAGES` (Android 13+), `READ_EXTERNAL_STORAGE` (Android 12 e anteriores): anexar/selecionar fotos

As permissões são usadas apenas dentro do escopo necessário para fornecer os recursos correspondentes.

---

## 8. Instalação, Operação e Recusa de Mecanismos de Coleta Automática

Este aplicativo não opera diretamente cookies gerais de websites.  
No entanto, em conexão com recursos de publicidade e gerenciamento de consentimento, SDKs de terceiros podem processar automaticamente identificadores de publicidade, informações de rede, informações do dispositivo e dados semelhantes.

Os usuários podem ajustar as configurações relevantes das seguintes maneiras:

- Alterar seleções nas opções de privacidade do aplicativo ou na tela de gerenciamento de consentimento (quando disponível)
- Redefinir ou excluir o identificador de publicidade nas configurações do sistema operacional do dispositivo
- Limitar anúncios personalizados ou ajustar opções de privacidade relacionadas nas configurações do sistema operacional do dispositivo

Se o usuário limitar a publicidade personalizada, anúncios não personalizados poderão ser exibidos ou determinados recursos relacionados a anúncios poderão ser restringidos.

---

## 9. Direitos do Usuário e Como Exercê-los

Sujeito às leis aplicáveis, os usuários podem ter os seguintes direitos:

- Solicitar acesso, correção ou exclusão de dados pessoais
- Solicitar suspensão ou limitação do tratamento
- Retirar o consentimento para tratamento baseado em consentimento
- Alterar escolhas de publicidade/consentimento

Esses direitos podem ser exercidos das seguintes maneiras:

- Modificar ou excluir dados diretamente no aplicativo
- Inicializar dados locais excluindo os dados do aplicativo ou desinstalando o aplicativo
- Alterar o consentimento de publicidade por meio das opções de privacidade/tela de consentimento do aplicativo (nas regiões em que isso for disponibilizado)
- Redefinir/excluir o identificador de publicidade ou limitar anúncios personalizados por meio das configurações do sistema operacional do dispositivo
- Contato: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Medidas de Segurança

O desenvolvedor aplica ou busca aplicar as seguintes medidas:

- Os registros do usuário geralmente são armazenados localmente no dispositivo
- Arquivos de imagem anexados são armazenados localmente em formato criptografado (com base em AES-GCM)
- As informações de bloqueio do aplicativo são armazenadas em formato hash, e não em texto simples
- Arquivos de backup são armazenados após serem criptografados com base em uma senha do usuário
- A comunicação com SDKs de terceiros é criptografada (HTTPS/TLS)
- As permissões são utilizadas com escopo de acesso minimizado

No entanto, riscos decorrentes da condição de segurança do dispositivo do usuário (como root/jailbreak, aplicativos maliciosos ou exposição de armazenamento compartilhado) não podem ser completamente eliminados.

---

## 11. Informações sobre Dados Sensíveis

Este aplicativo não exige a inserção de dados sensíveis.  
Os usuários são orientados a não inserir conteúdo sensível, como informações de saúde, opiniões políticas, religião, informações biométricas ou informações relacionadas à vida sexual, em notas ou campos de entrada livre.

Se um usuário inserir voluntariamente conteúdo sensível, essas informações poderão ser armazenadas como dados locais no dispositivo gerenciado diretamente pelo usuário.

---

## 12. Proteção de Dados Pessoais de Crianças

Este aplicativo não foi projetado principalmente para crianças.  
Responsáveis podem gerenciar o uso por meio de recursos de controle parental fornecidos pelo dispositivo ou pela loja de aplicativos.

---

## 13. Tomada de Decisão Automatizada

Este aplicativo não realiza tomada de decisão automatizada com base em dados pessoais que produza efeitos legais ou impactos significativos semelhantes.

---

## 14. Aviso de Segurança de Dados (Google Play etc.)

O desenvolvedor busca manter e atualizar os itens de divulgação de segurança de dados em lojas de aplicativos (como o Google Play) de acordo com as práticas reais de tratamento do aplicativo e as práticas reais de tratamento dos SDKs de terceiros.

No entanto, as informações exibidas nas lojas de aplicativos podem variar dependendo da versão do aplicativo, do país de distribuição, da configuração dos SDKs de terceiros e de mudanças nas políticas.

---

## 15. Aviso sobre Código Aberto

O aplicativo utiliza determinadas bibliotecas de código aberto.  
As informações sobre as licenças correspondentes podem ser encontradas na tela relacionada dentro do aplicativo ou em avisos fornecidos por meio do canal de distribuição.

---

## 16. Contato

Para dúvidas relacionadas a esta Política de Privacidade:

- **Encarregado pela Proteção de Dados / Pessoa de Contato:** frog-im
- **E-mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 17. Alterações nesta Política de Privacidade

Esta Política poderá ser revisada devido a alterações em leis/políticas, recursos do aplicativo ou SDKs de terceiros.  
Se houver alterações relevantes, um aviso poderá ser fornecido por meio de notificações dentro do aplicativo, da página de distribuição ou de atualizações na página da política.

Última Atualização: **2026-03-04**