# Conexões do Squad

## Piloto GPT (cenário único no Make)
- Cenário: "Squad · Piloto GPT" (Make, cenário 6952518, webhook 3038896), ativo.
- O endereço do webhook NÃO fica salvo aqui (funciona como senha). O gerente busca o endereço no Make (webhook 3038896) na hora de chamar.
- O gerente envia: `projeto` (nome), `memoria` (ROTA + FILA + diário recente), `tarefa`.
- Volta: texto começando com "PROJETO: <nome>" e a entrada de diário (Fiz / Travou / Preciso de / Próximo).
- Modelo: gpt-4o-mini, até 1500 tokens por resposta (teto de gasto). Usa a conexão OpenAI do Make.
- O gerente grava a resposta no diário da pasta do projeto que ele mesmo nomeou.

## Piloto Claude
- Uma sessão do Claude por projeto ("Piloto · <nome>"). O gerente acorda com uma mensagem. (a criar)
