---
title: Política de Privacidade | FileGuard
description: Política de Privacidade do FileGuard
lang: pt-PT
last_updated: 2026-06-23
---

# Política de Privacidade (FileGuard)

- **Aplicação:** FileGuard
- **Programador:** frog-im
- **Contacto de privacidade:** frog-im
- **E-mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Data de vigência:** 23 de junho de 2026
- **Última atualização:** 23 de junho de 2026

> Esta Política descreve a implementação atual do aplicação FileGuard. Leis obrigatórias do seu país ou região podem prevalecer.

---

## 1. Escopo e finalidade

O FileGuard é um utilitário de segurança que permite manter arquivos selecionados, media capturada, notas e texto da área de transferência em cofres criptografados no seu dispositivo e criar arquivos de backup criptografados.

O aplicação não exige registro nem login. O programador não opera servidor que receba seus arquivos de cofre, conteúdo de arquivos, senhas, nomes de cofres ou histórico de atividades. No Android, contudo, o aplicação pode usar Google AdMob e Google User Messaging Platform (UMP) para publicidade e escolhas de privacidade.

## 2. Informações processadas

### 2.1 Dados de cofre selecionados ou criados por você

O aplicação pode processar as seguintes informações no seu dispositivo:

- Fotos, vídeos, documentos e outros arquivos que você seleciona pelo seletor de arquivos do sistema
- Fotos ou vídeos capturados com o aplicação, incluindo áudio gravado com um vídeo
- Texto da área de transferência que você salva manualmente ou que é detectado quando você ativa a proteção automática da área de transferência
- Nome do arquivo, tipo MIME, tamanho, hora de criação, legenda e informações relacionadas à pré-visualização
- Nome e identificador do cofre, classificação de segurança, status do arquivo original e referência ao arquivo original
- Pacotes criptografados de exportação, transferência ou backup que você cria

Essas informações são processadas no seu dispositivo para fornecer os recursos do aplicação. O programador não as envia para um servidor operado pelo programador.

### 2.2 Informações de autenticação e segurança

O aplicação pode processar as seguintes informações em armazenamento seguro no seu dispositivo:

- Salts, configurações de derivação de chaves e pacotes de chaves criptografados usados para derivar ou proteger chaves de criptografia
- Credenciais de acesso ao cofre e chaves locais protegidas por uma chave vinculada ao dispositivo para acesso biométrico
- Preferências de segurança, como proteção contra captura de tela, limpeza da área de transferência, reautenticação biométrica e proteção automática

Sua senha em texto puro não é enviada ao programador. A autenticação biométrica é realizada pelo sistema operacional. O aplicação não coleta imagens de impressões digitais ou do rosto nem modelos biométricos; ele recebe apenas o resultado da autenticação.

### 2.3 Informações locais de atividade e backup

O aplicação pode armazenar localmente:

- O tipo, a descrição, a hora e os identificadores de itens relacionados para eventos de proteção, bloqueio, exclusão, exclusão do original, backup e restauração
- Até 500 entradas de registro de atividades
- Destino do backup, hora do último backup, contagem de itens e status de sucesso ou falha
- Se o backup automático está ativado e a senha necessária para atualizar esse backup
- Escolhas de privacidade de anúncios, escolha de processamento restrito de dados e uma contagem de itens protegidos usada para frequência de anúncios

Configurações sensíveis, incluindo o estado do backup e a senha do backup automático, são armazenadas em um armazenamento local criptografado por chave do dispositivo. Você é responsável por manter segura a sua senha de backup.

### 2.4 Informações processadas durante publicidade e consentimento

Na plataforma de publicidade compatível, atualmente Android, o aplicação pode usar Google AdMob e UMP. O Google e fornecedores de tecnologia de publicidade podem processar:

- Identificadores de publicidade, de instância do aplicação ou relacionados ao dispositivo
- Endereço IP e localização aproximada inferida a partir de informações como o endereço IP
- Modelo do dispositivo, sistema operacional, versão do aplicação, idioma e informações de rede
- Solicitações de anúncios, impressões, cliques, interações e diagnósticos
- Status de consentimento e escolhas regionais de privacidade

Essas informações podem ser usadas para veiculação de anúncios, anúncios não personalizados, limitação de frequência, medição, prevenção de fraudes, gerenciamento de consentimento, segurança e conformidade legal. O aplicação é implementado para inicializar o SDK Google Mobile Ads apenas depois que a UMP indicar que anúncios podem ser solicitados.

Consulte a [Política de Privacidade do Google](https://policies.google.com/privacy) e as [informações sobre tecnologias de publicidade do Google](https://policies.google.com/technologies/ads).

## 3. Finalidades do processamento

O FileGuard processa informações para:

- Armazenar e exibir conteúdo selecionado ou capturado em cofres criptografados
- Controlar o acesso ao cofre com bloqueio, senhas e autenticação biométrica
- Importar, exportar, mover, excluir e acompanhar o status do arquivo original do conteúdo
- Criar e restaurar backups criptografados em um local selecionado por você
- Manter preferências de segurança e limpar arquivos temporários descriptografados e conteúdos da área de transferência
- Exibir atividade de segurança local e status de erro
- Veicular anúncios Android, controlar a frequência de anúncios e fornecer escolhas de privacidade
- Prevenir abuso, proteger o serviço e cumprir obrigações legais

## 4. Armazenamento e retenção

| Categoria | Armazenamento e retenção | Como excluir |
|---|---|---|
| Arquivos e metadados criptografados do cofre | Armazenados no armazenamento local privado do aplicação até que você os exclua | Excluir o item ou cofre no aplicação, limpar os dados do aplicação ou desinstalar |
| Credenciais e configurações de segurança | Armazenadas em armazenamento seguro do sistema operacional e em armazenamento criptografado por chave do dispositivo até serem alteradas ou os dados do aplicação serem removidos | Desativar o recurso relevante, limpar os dados do aplicação ou desinstalar |
| Histórico de atividades | Até 500 entradas em armazenamento local criptografado | Limpar os dados do aplicação ou desinstalar |
| Arquivos temporários descriptografados | Gravados temporariamente no cache do aplicação e limpos na inicialização, ao ir para segundo plano ou ao concluir o recurso, em regime de melhor esforço | Fechar o aplicação ou limpar seu cache/dados |
| Conteúdo da área de transferência | Processado pela área de transferência do sistema operacional quando cópia ou proteção automática é usada | Limpeza automática em regime de melhor esforço, copiar outro conteúdo ou reiniciar o dispositivo |
| Arquivos de backup criptografados | Armazenados em uma pasta do dispositivo, provedor de documentos ou local sincronizado em nuvem selecionado por você até que os exclua | Excluir pelo gerenciador de arquivos ou serviço de armazenamento relevante |
| Dados de publicidade do Google | Retidos conforme as políticas e obrigações legais do Google e de processadores | Alterar configurações de anúncios do aplicação/dispositivo ou usar controles de privacidade do Google |

O sistema operacional, fabricante do dispositivo, provedor de documentos ou provedor de backup em nuvem pode manter cópias separadas dos dados do aplicação ou dos arquivos de backup que você cria. Essas cópias são regidas pelas políticas do provedor relevante.

## 5. Terceiros, prestadores de serviços e venda

O programador não vende conteúdo de cofres, senhas ou histórico de atividades no aplicação e não os fornece a terceiros por meio de servidor operado pelo programador.

Quando recursos de publicidade ou consentimento do Android operam, Google LLC, afiliadas do Google, fornecedores de tecnologia de publicidade e processadores relacionados podem processar as informações descritas na Seção 2.4. Consulte o [Aviso de Transferência Internacional de Dados](policy/) separado.

Se você selecionar diretamente um aplicação externo ou serviço em nuvem por meio de seletor de arquivos, função de compartilhamento ou destino de backup, esse provedor pode processar arquivos conforme sua orientação. A política de privacidade e as configurações de segurança dele se aplicam, e o programador não controla as práticas do provedor.

## 6. Transferências internacionais de dados

O conteúdo do cofre não é transferido para servidor operado pelo programador. Informações de publicidade e consentimento podem ser processadas pelo Google e processadores relacionados nos Estados Unidos e em outros países onde operem infraestrutura.

Se você escolher um serviço em nuvem no exterior como local para um backup criptografado, o arquivo pode ser sincronizado para servidores fora do seu país conforme sua orientação. Consulte o [Aviso de Transferência Internacional de Dados](policy/) para detalhes.

## 7. Permissões

O aplicação pode usar as seguintes permissões ou capacidades do sistema quando você usa o recurso relevante:

- **Arquivos e fotos:** Importar apenas conteúdo que você seleciona
- **Câmera:** Capturar fotos ou vídeos para o cofre
- **Microfone:** Incluir áudio ao gravar vídeo
- **Biometria:** Confirmar acesso ao cofre ou alterações de configurações sensíveis
- **Internet e estado da rede no Android:** Solicitar anúncios AdMob e informações de consentimento UMP
- **ID de publicidade no Android:** Dar suporte a recursos de publicidade do Google
- **Área de transferência:** Copiar conteúdo ou proteger texto da área de transferência quando você ativa explicitamente a proteção automática

Negar uma permissão pode desativar apenas o recurso relacionado. Quando o seletor de arquivos do sistema é usado, o acesso geralmente fica limitado aos itens que você seleciona.

## 8. Medidas de segurança e limitações

A implementação atual usa medidas que incluem:

- Criptografia AES-256-GCM para conteúdo e índices de cofres
- Derivação de chaves PBKDF2-HMAC-SHA256 para chaves baseadas em senha
- Proteção Android Keystore ou StrongBox para chaves locais em dispositivos Android compatíveis
- Criptografia por chave do dispositivo para configurações sensíveis e histórico de atividades
- Bloqueio de cofre e limpeza de arquivos temporários e área de transferência em regime de melhor esforço quando o aplicação entra em segundo plano
- Proteção opcional contra capturas de tela e reautenticação biométrica
- Pacotes de backup portáteis criptografados por senha

Nenhum método de segurança elimina todos os riscos. Roubo do dispositivo, malware, vulnerabilidades do sistema operacional, senhas fracas, arquivos compartilhados por você ou problemas de segurança em provedor de armazenamento externo podem expor informações.

Abrir ou exportar conteúdo descriptografado para outro aplicação pode criar uma cópia separada. A exclusão do arquivo original e a limpeza de arquivos temporários ou da área de transferência podem ser restringidas pelo sistema operacional, portanto você deve verificar a remoção de conteúdo sensível.

## 9. Seus direitos e escolhas

A maioria das informações permanece apenas no seu dispositivo, portanto o programador não pode acessá-las, corrigi-las ou excluí-las remotamente. Você pode:

- Excluir itens de cofre ou cofres no aplicação
- Alterar configurações de segurança, biometria, proteção automática, área de transferência e backup automático
- Limpar dados ou cache do aplicação, ou desinstalar o aplicação
- Excluir arquivos de backup e exportados do local de armazenamento
- Onde disponível, alterar consentimento pelas opções de privacidade de anúncios do Google no aplicação
- Excluir ou redefinir o identificador de publicidade ou limitar a personalização de anúncios nas configurações do dispositivo

Você pode nos contactar sobre informações que forneceu diretamente ao programador, como um e-mail de consulta. Quando aplicável, a legislação local pode conceder direitos de acesso, correção, exclusão, restrição, retirada de consentimento e reclamação a uma autoridade supervisora.

## 10. Crianças

O FileGuard não foi projetado principalmente para crianças e não exige que crianças forneçam informações pessoais. Responsáveis podem usar controles parentais fornecidos pelo dispositivo ou pela loja de aplicações. A configuração de consentimento para menores em publicidade Android deve ser analisada separadamente em relação ao público pretendido e à lei aplicável antes da distribuição.

## 11. Contato

Para dúvidas sobre esta Política:

- **Contato:** frog-im
- **E-mail:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Para dados de publicidade processados pelo Google, use os controles de privacidade e procedimentos de contato descritos na [Política de Privacidade do Google](https://policies.google.com/privacy).

## 12. Alterações desta Política

Podemos atualizar esta Política quando leis, recursos do aplicação, permissões ou práticas de SDKs de terceiros mudarem. Alterações materiais podem ser comunicadas nesta página, no aplicação ou pela página de distribuição.

Última atualização: **23 de junho de 2026**
