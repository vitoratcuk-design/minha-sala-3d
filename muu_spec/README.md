# NEXUS — MUU v1.0

Pacote de especificação e memória inicial do agente de trading Muu. **Não é ainda uma integração funcional com ChatGPT ou com o escritório 3D.**

## Arquivos
- `system_prompt.md`: instruções centrais do agente e modos de operação.
- `training_plan.json`: plano de formação estruturado.
- `memory_schema.json`: formato dos dados persistentes, com histórico e separação por mercado.
- `initial_memory.json`: estado inicial sem progresso inventado.

## Integração futura
1. Criar serviço backend seguro que chama um provedor de IA; nunca colocar chaves API no HTML público.
2. Guardar memória por usuário em banco de dados, com autenticação, edição e exportação.
3. Selecionar modo no frontend e enviar modo, mensagem e contexto mínimo ao backend.
4. Registrar operações apenas após confirmação do usuário; cálculos devem ser reproduzíveis.
5. Não vincular automaticamente dados do projeto ChatGPT: é necessária exportação/importação autorizada ou integração suportada.

## Privacidade
Registros financeiros e de trading devem ficar sob controle do usuário. Permitir exclusão/exportação e evitar armazenar senhas, chaves de carteira ou credenciais de corretora.
