# Log de Versões

## 🚀 Versão 1.0.18 - 07/04/2025

### Correções e Melhorias:
- 🛠️ **Gestão de Arquivos no Servidor**: Otimizamos o processo de conversão de arquivos (áudio, vídeo, fotos e documentos). Agora, após a conversão, apenas o arquivo final é mantido na pasta da empresa, eliminando duplicidades e economizando espaço no servidor.
- 🛠️ **Respostas de Mensagens**: Agora é possível responder a áudios, imagens e vídeos diretamente na conversa.


### Atualizações:
-  🔄 **API Atualizada**: Aprimoramos a performance e adicionamos suporte a novos recursos.

### Novas Funcionalidades:
- ✨ **Botão de Sair**: Incluímos um botão que permite encerrar a conversa sem enviar notificações. Com essa funcionalidade, o ticket é automaticamente fechado e o fluxo do bot é reiniciado.

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
