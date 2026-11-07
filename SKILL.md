---
name: squad-execucao
description: Central autônoma que conduz e finaliza os projetos em curso de Vinicius Ribeiro (Diagnóstico IVR, MINGO, SOIO e outros que forem conectados) sem looping. Define dois papéis, Piloto (o chat ou sessão de cada projeto) e Copiloto (a central que acorda sozinha e executa), que se comunicam pelo Diário de Bordo. Use sempre que o usuário falar em squad de execução, piloto, copiloto, rota, diário de bordo, looping, projeto travado, "seguir sem eu aprovar tudo", conectar um projeto novo à central, resumo do dia, ou quando abrir uma sessão de trabalho em qualquer projeto conectado.
---

# Squad de Execução

Objetivo: fazer cada projeto andar até o fim, sem pontas soltas e sem looping, gastando o mínimo de tokens.

## Os dois papéis

| Papel | Quem é | O que faz |
|---|---|---|
| **Piloto** | O chat ou sessão de cada projeto, onde Vinicius conversa | Traça a rota (o plano), toma decisões com Vinicius, escreve no Diário de Bordo o que foi decidido |
| **Copiloto** | A central, que acorda sozinha 1x por dia | Lê o Diário e a Fila, executa o que está verde, registra o resultado, junta o que depende de Vinicius no Resumo do Dia |

Os dois **nunca dependem da memória da conversa**. Tudo que importa fica nos arquivos do projeto. Se a conversa acabar ou o limite de uso estourar, nada se perde.

## Arquivos de cada projeto (kit do projeto)

Cada projeto conectado tem uma pasta `projetos/<nome>/` com 4 arquivos (moldes em `modelos/`):

1. `ROTA.md`: objetivo, o que significa "pronto", prazo, onde o trabalho mora (ClickUp, Drive, repositório).
2. `FILA.md`: tarefas com dono, estado e critério de pronto.
3. `REGRAS.md`: o semáforo deste projeto (o que pode seguir sozinho).
4. `DIARIO-DE-BORDO.md`: o canal entre Piloto e Copiloto. Entradas novas no topo.

## Prazo é obrigatório

Tarefa ou rota sem prazo nunca termina. Por isso:
- Toda **rota** tem prazo final e marcos com data.
- Toda **tarefa** tem prazo (data), tempo estimado e modo de execução (quem executa, com qual ferramenta, automático ou manual).
- Se faltar prazo, o Copiloto **propõe** um no Resumo do Dia (🟡) em vez de travar. Vinicius aceita ou ajusta.
- Prazo vencido vira alerta no Resumo do Dia com nova data proposta. Nunca fica vencido em silêncio.

## Projetos que já estão em andamento

Os projetos não começam do zero. Na primeira vez que um projeto é conectado, o Copiloto faz o **inventário inicial** (ver protocolo): lê as fontes que já existem (ClickUp, repositório, Make, arquivos de continuidade), lista todas as pendências atuais na FILA com prazo proposto e escreve no Diário "Inventário feito". A partir daí conduz essas pendências até a conclusão.

## Ao abrir uma sessão (Piloto)

1. Ler `kit-universal/regras.md` e os 4 arquivos do projeto. Não reler histórico antigo.
2. Ler as entradas do Diário desde a última sessão do Piloto e mostrar a Vinicius, em até 5 linhas, o que o Copiloto fez e o que espera dele.
3. Trabalhar com Vinicius. Ao decidir algo, registrar no Diário e atualizar a Fila **antes de encerrar**.

## Ao acordar (Copiloto)

Seguir `kit-universal/protocolo-piloto-copiloto.md`. Em resumo:
1. Para cada projeto em `projetos/`: ler Fila e Diário. Se não houver nada verde a fazer, pular. Se nenhum projeto tiver nada, encerrar na hora.
2. Executar só tarefas verdes, no máximo 2 tentativas cada.
3. Registrar resultado no Diário e atualizar a Fila.
4. Montar `resumo/AAAA-MM-DD.md` com tudo amarelo, vermelho, travado ou parado há mais de 2 dias, numerado para Vinicius responder "1 sim, 2 não".

## Regras invioláveis

Ver `kit-universal/regras.md` e `kit-universal/semaforo.md`. As principais:
- **Máximo de 2 tentativas** por tarefa. Na segunda falha, parar e escrever o diagnóstico (o que tentou, o erro exato, o que falta).
- **Login, senha, permissão e pagamento são sempre de Vinicius.** Entregar um passo a passo curto, nunca tentar adivinhar.
- **Nada espera escondido.** Toda trava aparece no Resumo do Dia.
- **Quem termina atualiza a Fila antes de sair.**

## Economia de tokens

- Modelo forte só para coordenar e revisar. Execução simples em modelo barato.
- Ler só os 4 arquivos e as entradas novas do Diário, nunca o histórico inteiro.
- Copiloto acorda 1x por dia e encerra imediatamente se a fila estiver vazia.

## Conectar um projeto novo

Copiar `modelos/` para `projetos/<nome>/`, preencher ROTA e REGRAS com Vinicius na primeira sessão do Piloto, listar as tarefas abertas na FILA.
