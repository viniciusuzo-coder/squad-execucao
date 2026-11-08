# Fila · Projeto IVR

Atualizada em **2026-11-08**. Contém as pendências operacionais atuais. Itens antigos do diagnóstico que não contribuírem para prospecção, venda, entrega ou resultados devem ser arquivados, não perpetuados.

| Tarefa | Dono (Piloto ou Vinicius) | Semáforo | Estado | Pronto quando | Tempo estimado | Prazo |
|---|---|---|---|---|---|---|
| Reautenticar a sessão do Make.com | Vinicius | 🔴 | Bloqueado por login expirado | painel do Make.com abre autenticado para verificação | 5 min | 2026-11-08 |
| Verificar saúde real do C5 Instagram DM → Olga — Orientadora de Jornada VR | Piloto | 🟢 | Não verificado; depende do login | cenário `5835241` ativo, última execução lida, sem erro de autenticação e teste real registrado | 30 min | 2026-11-09 |
| Monitorar diariamente o C5 e alertar apenas por mudança relevante | Piloto | 🟢 | Automação ativa | monitor `sa-de-do-funil-instagram-ivr` permanece silencioso quando saudável e alerta falha comprovada | 10 min/dia | Contínuo; revisão 2026-11-30 |
| Acompanhar resposta humana do suporte WhatsApp | Piloto | 🟢 | Aguardando fornecedor; tickets `#2353912`, `#2388091` e `2333952827450564` | orientação humana não destrutiva recebida e registrada | 15 min | 2026-11-09 12:00 |
| Decidir fallback para número dedicado do WhatsApp Cloud se não houver correção | Vinicius | 🟡 | Gate pendente | manter coexistência ou aprovar número dedicado, sem Z-API | 10 min | 2026-11-09 12:30 |
| Implementar a decisão do WhatsApp Business Cloud | Piloto | 🟢 | Bloqueado pelo gate anterior | conexão oficial criada no Make.com sem apagar o número/histórico atual | 1 h | 2026-11-10 |
| Validar C2 → Renata — Retomada de ponta a ponta | Piloto | 🟢 | Bloqueado pela conexão WhatsApp | mensagem sai do cenário `5643849`, chega ao número real e a execução fica registrada | 1 h | 2026-11-10 |
| Auditar e corrigir C4 Relatório Semanal | Piloto | 🟢 | Erros anteriores registrados | causa dos erros identificada, correção aplicada e uma execução limpa comprovada | 1 h | 2026-11-11 |
| Validar C1 Notificação de Agendamento Calendly | Piloto | 🟢 | Existe; saúde atual não verificada | agendamento de teste gera notificação e evidência no Make.com | 45 min | 2026-11-11 |
| Revisar C3 Alerta de Anomalia para a arquitetura sem Chatvolt | Piloto | 🟢 | Registro antigo incompatível com stack atual | alerta monitora recursos atuais e dispara teste controlado | 1 h 30 | 2026-11-12 |
| Decidir se C6 Carrossel Automático será ativado ou arquivado | Vinicius | 🟡 | Inativo; não prioritário | decisão registrada sem desviar do funil comercial | 10 min | 2026-11-12 |
| Alinhar fluxo de Olga — Orientadora de Jornada VR | Piloto | 🟡 | Em andamento | diagnóstico → valor → qualificação → conversão aprovado e testado; sem pedir dados cedo | 2 h | 2026-11-13 |
| Alinhar fluxo de Renata — Retomada | Piloto | 🟡 | Em andamento | pós-sessão, retomada, limites e escalonamento aprovados e testados | 2 h | 2026-11-13 |
| Corrigir CTA do site que ainda aponta para Chatvolt | Piloto | 🟡 | Pendente | novo destino preparado, validado e pronto para publicação | 1 h | 2026-11-14 |
| Publicar o CTA corrigido no site | Vinicius | 🔴 | Aguarda versão validada | alteração pública aprovada e link real testado | 10 min | 2026-11-14 |
| Concluir ADR-071 Etapas 4–9 do gerador de carrosséis | Piloto | 🟢 | Etapas 1–3 concluídas; 4–9 pendentes | referências, templates e materialização usam o Design Brief aprovado | 4 h | 2026-11-14 |
| Executar smoke test real do pipeline de carrossel | Piloto | 🟢 | Pendente | roteiro gera arquivos e PNGs válidos com evidência visual | 2 h | 2026-11-15 |
| Aprovar/publicar primeiro conteúdo do novo ciclo | Vinicius | 🔴 | Aguarda smoke test e funil | conteúdo aprovado e publicado em canal definido | 15 min | 2026-11-15 |
| Provar o funil conteúdo → DM → qualificação → Calendly → retomada → CRM | Piloto | 🟡 | Parcial | uma jornada completa real fica registrada em todos os pontos | 4 h | 2026-11-20 |
| Limpar ClickUp: duplicatas, tarefas falsas, prazos vencidos e nomes antigos | Piloto | 🟢 | Em andamento | nenhuma duplicata ativa; itens sem função arquivados; tarefas reais com prazo | 3 h | 2026-11-16 |
| Limpar Drive e manter apenas versões atuais ativas | Piloto | 🟢 | Em andamento | versões superadas em `99_ARQUIVO`; documentos atuais com links válidos | 3 h | 2026-11-18 |
| Atualizar Roadmap e Mapa Arquitetural com estado comprovado | Piloto | 🟡 | Materiais existentes podem estar desatualizados | ambos refletem os canais, cenários e bloqueios verificados | 3 h | 2026-11-20 |
| Auditar pendências das Fases 1 e 2 e arquivar o que não serve ao funil | Piloto | 🟢 | Pendente | cada item antigo é mantido, atualizado ou arquivado com justificativa | 3 h | 2026-11-20 |
| Aprovar oferta e caminho comercial prioritário | Vinicius | 🟡 | Pendente | oferta, público, promessa, preço e CTA têm uma decisão única | 45 min | 2026-11-21 |
| Executar piloto de 3 tentativas reais de venda | Piloto | 🟡 | Pendente | três oportunidades percorrem o funil e resultados são registrados | 2 semanas | 2026-11-30 |
| Ativar CRM mínimo de leads, conversas, agendamentos, vendas e motivos de perda | Piloto | 🟢 | Estrutura parcial | painel recebe dados reais sem digitação duplicada | 4 h | 2026-11-30 |
| Definir e testar onboarding e entrega da mentoria/travessia | Piloto | 🟡 | Pendente | cliente de teste recebe sequência completa e critérios de sucesso | 1 dia | 2026-12-07 |
| Instrumentar painel de prospecção, vendas, entrega e resultados | Piloto | 🟢 | Pendente | indicadores reais atualizados e auditáveis | 1 dia | 2026-12-15 |
| Decidir entrada nas Fases 4 e 5 | Vinicius | 🟡 | Bloqueada pelo Gate v1 | decisão baseada em receita, volume e gargalos reais | 30 min | 2026-12-31 |

## Regra de tentativa

Cada linha admite no máximo **2 tentativas**. Na segunda falha, o estado muda para **Bloqueado**, as evidências são registradas e uma alternativa é apresentada. Não reiniciar o mesmo caminho indefinidamente.
