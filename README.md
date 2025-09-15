# Log de Versões

## 🚀 Versão 1.0.21.v3 - 10/08/2025

### Correções e Melhorias:
- 🛠️ **Tratamento do erro unhandledRejection**: Implementação de sistema global de captura de Promises rejeitadas.
- 🛠️ **Remoção de listeners conflitantes no Wbot**: Ajustes em wbot.ts para evitar múltiplos process listeners.
- 🛠️ **Melhoria no Cleanup do Wbot**: Função cleanupWbot() agora assíncrona e robusta.
- 🛠️ **Tratamento centralizado de erros**: Logs detalhados antes de crash, com integração ao Sentry.
- 🛠️ **Server.ts e Server-cluster.ts**: Integração com novo sistema de tratamento de erros.

### Atualizações:
- 🔄 **Configuração do Nodemon**: Inclusão de nodemon.json com crash handling robusto.
- 🔄 **Scripts de desenvolvimento**: Novos scripts test:cleanup, test:auth-state e melhorias em npm start e start:prod.
- 🔄 **Monitoramento de memória**: Logs periódicos a cada 5 minutos com alertas automáticos.
- 🔄 **Timeouts de segurança**: Prevenção contra travamentos em operações longas.
- 🔄 **Integração Sentry**: Captura automática de erros para monitoramento e alertas.

### Novas Funcionalidades:
- ✨ **Arquivo errorHandler.ts**: Novo sistema centralizado de tratamento global de erros.
- ✨ **Reinicialização robusta**: Nodemon configurado com "crash": false, "exitcrash": false, delay e restart manual com rs.
- ✨ **Alertas inteligentes de cache**: Notificação quando cache de mensagens/grupos atinge limites configurados.
- ✨ **Logs detalhados de operação**: Uso de memória, estatísticas de cache e estado de sessões agora visíveis nos logs.

---

## 🚀 Versão 1.0.21.V2 - 09/07/2025

### Correções e Melhorias:
- 🛠️ **Correção de Vazamentos de Memória**: Removidos event listeners duplicados e centralizados em wbotMessageListener.ts.
- 🛠️ **Compilação TypeScript Corrigida**: Ajustadas chamadas de removeAllListeners() com eventos específicos.
- 🛠️ **Cleanup Coordenado**: Implementada função cleanupWbot() global com integração ao graceful shutdown.
- 🛠️ **Controle de setInterval: Todos os setInterval agora possuem variáveis de controle e são limpos no shutdown.
- 🛠️ **Isolamento de Cache por Empresa**: Cada empresa agora possui cache próprio com rotina de manutenção automática.
- 🛠️ **Remoção de Process Listeners Conflitantes**: Handlers duplicados eliminados em wbot.ts.
- 🛠️ **Tratamento de Erros Melhorado**: Logs detalhados substituíram catches vazios, garantindo visibilidade de falhas.

### Atualizações:
- 🔄 **useMultiFileAuthState Refatorado**: TTL de 24h para sessões, limpeza automática a cada hora e monitoramento de memória com alertas.
- 🔄 **Servidor e Cluster**: Graceful shutdown coordenado com timeout de segurança, integração com cleanupAuthState e Redis validado antes de operações críticas.
- 🔄 **Métricas e Logs Detalhados**: Novos logs de cache, cleanup e estatísticas de sessões para auditoria e monitoramento contínuo.

### Novas Funcionalidades:
- ✨ **Monitoramento Automático de Memória**: Alertas em tempo real para consumo excessivo no Redis e estatísticas de uso por sessão.
- ✨ **Limpeza Automática de Sessões Obsoletas**: Sessões inativas por mais de 7 dias são removidas e chaves corrompidas são eliminadas.- 
- ✨ **Funções de Utilidade Exportadas**: cleanupExpiredSessions, getSessionMemoryUsage, checkMemoryUsage e cleanupAuthState disponíveis para uso externo.

---

## 🚀 Versão 1.0.21 - 18/04/2025

### Correções e Melhorias:
- 🛠️ **Organização dos campos de configuração**: Reordenação e agrupamento lógico.  
- 🛠️ **Campos Table para Switch**: Substituição de campos table por switches.  
- 🛠️ **Layout responsivo com Grid**: Remodelagem de Planos de assinatura e Ajuda.  
- 🛠️ **Plano de fundo do Login**: Alterado para assets da pasta frontend.  
- 🛠️ **Correção do layout da página de assinatura**: Ajustes de estilo e responsividade.  
- 🛠️ **Remoção do modo escuro**: UI padronizada apenas em tema claro.  
- 🛠️ **Barra superior sólida**: Aplicação de cor sólida na navegação.  
- 🛠️ **Ícones coloridos**: Substituição de ícones monocromáticos por coloridos.  

### Atualizações:
- 🔄 **API Atualizada**: Melhorias gerais na performance.  
- 🔄 **Transcrição de áudio**: Mecanismo de transcrição aprimorado.  
- 🔄 **Financeiro**: Suporte a Cartão de Crédito, Débito e PIX.  
- 🔄 **OpenAI Atualizado**: Versão da API atualizada.  
- 🔄 **NodeJS Atualizado**: Atualização do runtime.  
- 🔄 **Cron na instalação**: Inclusão de task scheduler no setup.  
- 🔄 **Botão de cadastro**: Novo botão “Entrar no sistema” em fluxo de cadastro.  
- 🔄 **Tarefas com Editor de texto e Emojis**: Nova funcionalidade de tarefas.  
- 🔄 **Ajuda no Menu**: Seção de suporte adicionada.  
- 🔄 **Versão no Sidebar**: Exibição dinâmica da versão via package.json.  

### Novas Funcionalidades:
- ✨ **Campo Repetir senha no cadastro**: Validação de confirmação de senha.  
- ✨ **Campo Repetir senha na edição de usuário**: Mesma validação na edição.  
- ✨ **Documentação da API**: Documentação integrada ao sistema.  
- ✨ **Novo Dashboard**: Painel inicial reformulado.  
- ✨ **Novo Atendimento**: Nova estrutura de atendimento.  
- ✨ **Novo Instalador**: Processo de instalação refeito.  

---

## 🚀 Versão 1.0.20 - 15/04/2025

### Novas Funcionalidades:
- ✨ **Integração com WhatsApp**: Suporte a mensagens via WhatsApp.  
- ✨ **Integração com Facebook**: Suporte a envios e recebimentos via Facebook.  
- ✨ **Integração com Instagram**: Suporte a envios e recebimentos via Instagram.  
- ✨ **Integração ChatGPT**: Conexão com API do ChatGPT.  
- ✨ **Integração DialogFlow**: Conexão com Google DialogFlow.  
- ✨ **Integração TypeBot**: Conexão com TypeBot.  
- ✨ **Suporte a Webhooks**: Recebimento de eventos via Webhook.  
- ✨ **CRM Kanban**: Painel Kanban de leads e tickets.  
- ✨ **FlowBuilder nova versão**: Atualização do construtor de fluxos.  
- ✨ **Integração Mercado Pago**: Pagamentos via Mercado Pago.  
- ✨ **Integração Stripe**: Pagamentos via Stripe.  
- ✨ **Integração Asaas**: Pagamentos via Asaas.  
- ✨ **Integração OpenAI**: Conexão com API OpenAI.  
- ✨ **Integração EFI (GerenciaNET)**: Conexão com EFI GerenciaNET.  

---

## 🚀 Versão 1.0.19 - 10/04/2025

### Novas Funcionalidades:
- ✨ **Sistema SaaS**: Plataforma como serviço habilitada.  
- ✨ **Multiempresas**: Suporte a múltiplas empresas.  
- ✨ **Dashboard de atendimentos**: Visão geral das interações.  
- ✨ **Criação de Chatbot por fluxos**: Editor de fluxos integrado.  
- ✨ **CRM Kanban**: Painel Kanban de tickets.  
- ✨ **Integrações com fluxos do mercado**: Conexões com ferramentas de automação.  
- ✨ **Controle de Grupos**: Gerenciamento de grupos de atendimento.  
- ✨ **Disparo em Massa**: Envio massivo de mensagens.  
- ✨ **Relatórios avançados**: Geração de relatórios customizados.  
- ✨ **Controle de equipes**: Gestão de permissões e atribuições.  
- ✨ **Controle de notas de atendimento**: Anotações internas por ticket.  
- ✨ **Controle de protocolos**: Registro de protocolos únicos.  
- ✨ **Controle de avaliações**: Coleta e análise de feedback.  
- ✨ **Atendimento por carteiras**: Distribuição de tickets por carteiras.  
- ✨ **Transferência automática de filas**: Redistribuição automática de tickets.  
- ✨ **Encerramento por inatividade**: Tickets fechados após inatividade.  
- ✨ **Organização de ordem de fila**: Configuração de prioridades.  
- ✨ **Saudação ao aceitar ticket**: Mensagem de boas-vindas automática.  
- ✨ **Mensagem de transferência**: Notificação ao mover ticket.  
- ✨ **Atendentes múltiplos por conta**: Vários agentes em um login.  
- ✨ **Sem limite de WhatsApp**: Remoção de restrições de contas.  
- ✨ **Sem limite de mensagens**: Remoção de limites de envio.  
- ✨ **Criação de filas personalizadas**: Comercial, Suporte, Financeiro etc.  
- ✨ **Menu interativo inicial**: Navegação simplificada.  
- ✨ **Transferência de filas manual**: Opção de mover tickets manualmente.  
- ✨ **Cadastro de usuários**: Novo fluxo de cadastro.  
- ✨ **Envio de arquivos e áudio**: Suporte a anexos e gravações.  
- ✨ **Respostas Rápidas**: Sugestões de mensagens pré-definidas.  
- ✨ **Responsividade móvel**: Uso otimizado em dispositivos móveis.  
- ✨ **API via POST com token**: Endpoints seguros.  
- ✨ **Etiquetas**: Tags customizáveis.  
- ✨ **Horários de atendimento**: Definição de janelas de suporte.  
- ✨ **Códigos curtos**: Identificadores personalizados.  
- ✨ **Campanhas em massa**: Configuração e relatórios.  
- ✨ **Usuários simultâneos**: Várias sessões ativas.  
- ✨ **Mensagens de saudação e finalização**: Automação de início e fim.  
- ✨ **Ignorar mensagens de grupos**: Filtro de mensagens de grupos.  


## 🚀 Versão 1.0.18 - 10/03/2025

### Correções e Melhorias:
- 🛠️ **Gestão de Arquivos no Servidor**: Otimizamos o processo de conversão de arquivos (áudio, vídeo, fotos e documentos). Agora, após a conversão, apenas o arquivo final é mantido na pasta da empresa, eliminando duplicidades e economizando espaço no servidor.
- 🛠️ **Botão 'Sair' Exclusivo para Administradores**: Agora, apenas administradores podem usar este botão para encerrar a conversa sem enviar mensagens, reiniciando o fluxo do bot de forma discreta e controlada.


### Atualizações:
-  🔄 **API Atualizada**: Aprimoramos a performance e adicionamos suporte a novos recursos.

### Novas Funcionalidades:
- ✨ **Botão de Sair**: Incluímos um botão que permite encerrar a conversa sem enviar notificações. Com essa funcionalidade, o ticket é automaticamente fechado e o fluxo do bot é reiniciado.
- ✨ **Respostas de Mensagens**: Agora é possível responder a áudios, imagens e vídeos diretamente na conversa.

---

## 🚀 Versão 1.0.17 - 23/02/2025

### Correções e Melhorias:
- 🛠️ **Redimensionamento da Área de Ticket**: Resolvido erro ao redimensionar.
- 🛠️ **ToastError.js**: Corrigido problema no arquivo `toastError.js`.
- 🛠️ **Validação de Número no ContactModal**: Validação aprimorada para maior precisão.
- 🛠️ **Avaliações de 1 a 5 Estrelas**: Ajuste nas avaliações de tickets.
- 🛠️ **Mensagem de Avaliação Condicional**: Exibição de avaliações apenas para tickets ativos.
- 🛠️ **Correção de Áudio no iPhone**: Áudio agora reproduz corretamente.
- 🛠️ **Compatibilidade com Modo Dark**: Correção no chat e logos adaptadas para temas claro/escuro.
- 🛠️ **Correção das mensagens editadas no chat**: Agora as mensagens editadas pelo sistema e pelo celular retornam à atualização correta.
- 🛠️ **Correção das mensagens respondidas no chat**: Agora as mensagens respondidas pelo lado do cliente e do atendente funcionam corretamente.
- 🛠️ **Melhoria na recepção das mensagens**: Agora as mensagens recebidas e enviadas são validadas de forma correta, evitando perda de mensagens no chat.
- 🛠️ **Melhoria na mensagem de opção invalida**: Agora quando é informada uma mensagem que não existe no menu de opções,
ele retorna a mensagem ao usuário informando para digitar # para voltar ao menu de opções e informar uma opção valida do menu.

### Atualizações:
- 🔄 **OpenAI e wbotMessageListener.ts**: Atualizado para `"openai": "3.3.0"`.
- 🔄 **Horários Intercalados**: Implementação de funcionalidade para horários alternados.
- 🔄 **Estrutura de Pastas por Empresas**: Adicionada em `public`.

### Novas Funcionalidades:
- ✨ **Integração com Kanban**: Kanban integrado e reformulado.
- ✨ **Adicionado paleta de emojis no Chat Interno**: Agora é possível mandar emojis no chat interno.
- ✨ **Adicionado ao Editar mensagens, paleta de emoji**: Agora é possível mandar emoji ao editar as mensagens.
- ✨ **Adicionado Log de atualização do sistema**: Agora é possível ver o que foi modificado e implementado no sistema.
- ✨ **Adicionados novos gráficos ao Dashboard**: Agora é possível visualizar os gráficos por:
Atendimentos dos atendentes, Atendimentos por Departamentos/Filas, Horário de Pico - Troca de mensagens.

---

## 🚀 Versão 1.0.16 - 12/01/2025

### Correções e Melhorias:
- 🛠️ **Data de Vencimento no Topo**: Fixa e visível em todas as telas.
- 🛠️ **Automação em Grupos**: Impedida para grupos de usuários.
- 🛠️ **Mensagens Citadas**: Erros corrigidos.
- 🛠️ **Envio de Áudio OGG em Respostas Rápidas**: Agora funcionando corretamente.
- 🛠️ **Visualização de Tickets e Grupos**: Ajustada no painel de operadores.
- 🛠️ **Atualização Financeira Automática**: Valor ajustado ao alterar planos.

### Novas Funcionalidades:
- ✨ **Botão disableBot**: Possibilidade de desabilitar bots ou automações.
- ✨ **Expiração Automática de Conexões**: Empresas vencidas são desconectadas.
- ✨ **Exclusão de Contatos**: Seleção em massa na página "Contatos".

---

## 🚀 Versão 1.0.15 - 05/01/2025

### Correções e Melhorias:
- 🛠️ **Notificação de Mensagens Apagadas**: Informativo exibido no chat.
- 🛠️ **API Atualizada**: Melhor performance e suporte.

### Novas Funcionalidades:
- ✨ **Encerramento de Tickets**: Fechar todos os tickets abertos ou em espera.
- ✨ **Reações e Encaminhamentos**: Reagir e encaminhar mensagens para outro ticket.
- ✨ **Melhoria no Menu**: Aparência refinada e botão "Sair" adicionado.
- ✨ **Indicação de Atividade**: Exibe "Digitando" ou "Gravando" no canto inferior do ticket.
- ✨ **Novo Layout**: Tela de login reformulada.

---

## 🚀 Versão 1.0.8 - 21/09/2024

### Correções e Melhorias:
- 🛠️ **Correção no Vcard**: Problemas de funcionalidade ajustados.
- 🛠️ **Finalização de Tickets pelo Administrador**: Corrigido envio incorreto de mensagens de transferência.

### Novas Funcionalidades:
- ✨ **Controle de Registros**: Opção para habilitar/desabilitar novos registros.
- ✨ **Tempo de Trial no Painel**: Exibição de prazo de teste.
- ✨ **Respostas Rápidas Personalizadas**: Separação por usuários.
- ✨ **Indicador de Contatos Abertos**: Mostra qual operador está gerenciando a conversa.
- ✨ **Cadastro de Empresas**: Nova aba para registrar empresas.
- ✨ **Novas Opções de Planos**: Adicionadas ao sistema.
