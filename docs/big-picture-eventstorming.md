# Big Picture EventStorming: Serviço de Agentes por Assinatura

🏁 Contexto: Pré-Qualificação Consultiva

👤 Actor: Cliente entra em contato via site, WhatsApp ou Slack
🟧 Event: Cliente demonstra interesse no serviço
🔷 Command: Agente realiza entrevista de diagnóstico
🟧 Event: Contexto de negócio foi mapeado
🔷 Command: Coletar e sugerir ideias de automação
🟧 Event: Lista de automações identificadas
🔷 Command: Estimar tempo e ROI de cada automação
🟧 Event: Simulação de ROI e payback do serviço gerada
🔷 Command: Gerar tarefas preparatórias para o cliente
🟧 Event: E-mail com checklist enviado (mesmo sem contrato)
🟧 Event: Painel de preparação liberado para preenchimento
🔷 Command: Avaliar lead e gerar Score de Qualificação
🟧 Event: Score do lead calculado com base em perfil e resposta
🟪 Policy: Clientes podem preencher tarefas antes de pagar, o que melhora o score
🟨 External System: Ferramenta de CRM com lead scoring + painel de onboarding

⸻

🗂️ Contexto: Adesão ao Serviço

👤 Actor: Cliente decide contratar após preparar onboarding
🟧 Event: Cliente escolhe plano com base na simulação e urgência
🔷 Command: Confirmar pagamento e ativar assinatura
🟧 Event: Assinatura confirmada
🟨 External System: Plataforma de pagamento

⸻

🗂️ Contexto: Setup Inicial

👤 Actor: Agente revisa tarefas preparatórias preenchidas
🟧 Event: Informações do cliente estão completas
🔷 Command: Selecionar automações para o primeiro ciclo
🟧 Event: Tarefas são adicionadas ao Kanban
🟧 Event: Cliente recebe boas-vindas e explicação do painel
🟪 Policy: Nenhuma automação é iniciada antes do pagamento, mas o preenchimento antecipado agiliza a entrega
🟨 External System: Painel do cliente

⸻

🗂️ Contexto: Atendimento Assíncrono

👤 Actor: Cliente envia novas ideias ou dúvidas
🟧 Event: Solicitação registrada no sistema
🔷 Command: Agente qualifica e estima escopo
🟧 Event: Tarefa é priorizada ou agendada para ciclo futuro
🟪 Policy: SLA e limites de automação conforme plano contratado
🟧 Event: Automação entregue
🟧 Event: Cliente notificado da entrega
🟨 External System: Painel, WhatsApp, Slack

⸻

🗂️ Contexto: Gestão e Acompanhamento

👤 Actor: Cliente acessa painel
🟧 Event: Visualiza tarefas, entregas, uso do plano
🟧 Event: Acompanha ROI acumulado, performance e metas
🟧 Event: Recebe alertas de SLA, novas entregas e propostas de expansão
🟨 External System: Dashboard de performance e uso

⸻

🗂️ Contexto: Expansão e Renovação

👤 Actor: Cliente atinge limite mensal ou quer mais automações
🟧 Event: Sistema notifica limite alcançado
🔷 Command: Sugerir upgrade com base em ROI e uso
🟧 Event: Cliente faz upgrade OU tarefas seguem para fila futura
🟪 Policy: O sistema pode reestimar ROI com base em novas entregas para fomentar upsell

💬 Comment: O serviço combina estratégia comercial, entrega contínua e educação do cliente. A jornada começa antes do contrato e recompensa engajamento com agilidade e previsibilidade.
