# Protocolo Piloto ↔ Copiloto

O canal é o `DIARIO-DE-BORDO.md` de cada projeto. Entradas novas no topo, neste formato:

```
## AAAA-MM-DD · PILOTO | COPILOTO
- Fiz: ...
- Decidido: ...           (só Piloto)
- Travou: ... (tentativa 1/2 ou 2/2, erro exato)
- Preciso de: ...         (de Vinicius ou do outro papel)
- Próximo: ...
```

## Inventário inicial (uma vez, ao conectar um projeto em andamento)
1. Ler as fontes atuais do projeto listadas em `ROTA.md` (ClickUp, repositório, Make, arquivos de continuidade, issues abertas).
2. Listar cada pendência na `FILA.md` com dono, prazo proposto, tempo estimado e modo de execução.
3. Marcar como "travado" o que está parado esperando alguém, dizendo quem e desde quando.
4. Escrever no Diário: `Inventário feito: N pendências, M travadas, prazos propostos no Resumo`.
5. Levar os prazos propostos ao Resumo do Dia para Vinicius aprovar em lote.

## Ciclo diário do Copiloto
1. Abrir `projetos/`. Para cada projeto:
   - ler `FILA.md` e as entradas do Diário mais novas que a última entrada do Copiloto;
   - executar tarefas 🟢 (máx. 2 tentativas cada);
   - registrar no Diário e atualizar a Fila.
2. Se nenhum projeto tinha trabalho, encerrar sem escrever nada.
3. Escrever `resumo/AAAA-MM-DD.md`:

```
# Resumo do dia · AAAA-MM-DD
Responda com os números: "1 sim, 2 não, 3 sim"

## Decisões (🟡 e 🔴)
1. [IVR] ...
2. [MINGO] ...

## Passos seus (logins, permissões)
3. [IVR] ... (checklist curto)

## Avanços
- [SOIO] ...

## Prazos para aprovar
4. [MINGO] tarefa X: proposto AAAA-MM-DD

## Alertas (vencido ou parado > 2 dias)
- ...
```

## Ciclo do Piloto (a cada sessão com Vinicius)
1. Ler Diário desde a última entrada do Piloto e o Resumo do Dia mais recente.
2. Aplicar as respostas de Vinicius: mover tarefas para 🟢 ou descartar.
3. Ajustar a rota se preciso, registrar "Decidido" no Diário.

## Fim de rota
O Copiloto propõe "rota concluída" no Resumo. O Piloto confirma com Vinicius e registra no Diário. Só então a rota fecha.
