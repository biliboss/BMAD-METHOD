# Big Picture EventStorming: {{Process Name}}

[[LLM: The default path and filename unless specified is docs/big-picture-eventstorming.md]]

[[LLM: Use this template to outline the high-level flow of a service or business process. Replace the sample text with domain-specific details. Keep sections concise.]]

🏁 Contexto: {{First Context}}

👤 Actor: {{Main Actor}}
🟧 Event: {{Trigger Event}}
🔷 Command: {{First Command}}
🟧 Event: {{Resulting Event}}

⸻

🗂️ Contexto: {{Next Context}}

👤 Actor: {{Actor}}
🟧 Event: {{Event}}
🔷 Command: {{Command}}
🟧 Event: {{Event Result}}

⸻

💬 Comment: Cada contexto pode envolver diferentes áreas e sistemas externos.

@{example}
Exemplo simplificado inspirado em processos bancários digitais:

🏁 Contexto: Início da Jornada

👤 Actor: Cliente acessou o site/app
🟧 Event: Cliente manifestou interesse em abrir conta
🔷 Command: Iniciar abertura de conta
🟧 Event: Proposta de abertura de conta foi criada

⸻

🗂️ Contexto: Cadastro e Documentação

👤 Actor: Cliente preencheu dados cadastrais
🟧 Event: Dados cadastrais foram enviados
🔷 Command: Enviar documentação
🟧 Event: Documentos foram recebidos
🟧 Event: Documentos foram validados
🟪 Policy: Sempre que documentos forem validados, disparar análise de risco
🟧 Event: Validação automática foi aprovada/reprovada
🟨 External System: Sistema de verificação antifraude
🟧 Event: Consulta antifraude foi realizada

@{/example}
