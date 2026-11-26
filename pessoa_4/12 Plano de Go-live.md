# 12 — Plano de Go-live

**Projeto:** Vida+ — Sistema de Gestão e Agendamento de Clínica  
**Responsável pelo artefato:** Luís Gabriel (Pessoa 4 — Controle e go-live)  
**Status:** Rascunho alinhado à semana 13–14 do [cronograma](../pessoa_3/04%20Cronograma.md) e [Decisão 2](../planejamento/00-reuniao-de-decisoes.md) (Z-06 Indaiatuba fora da operação em 03/03/2027)

## 1. Objetivo

Planejar a **entrada em produção em 03/03/2027** nas **quatro unidades já em operação**, com critérios go/no-go, comunicação às unidades, plantão e transição para estabilização/garantia.

## 2. Escopo do go-live

| Incluído em 03/03/2027 | Fora desta data (Decisão 2) |
|---|---|
| PB-01 a PB-14 aceitos + homologação integrada; PB-15/VidaFin incluído somente se P-01 for atendida | Operação plena **Indaiatuba** (Z-06); apenas cadastro estrutural se existir |
| Quatro unidades atuais em **onda única** (decisão do grupo: simultâneo com treinamento reforçado) | WhatsApp (Z-01), reagendamento paciente (Z-02) |

## 3. Checklist — semana 13 (18–24/02/2027)

| # | Atividade | Dono | Critério pronto |
|---:|---|---|---|
| 1 | Carga final de dados essenciais | Rafael/Diego + Paula | Amostra conferida ([11 Qualidade](11%20Plano%20de%20Qualidade.md) §7) |
| 2 | Treinamento usuários-chave (recepção/coordenação) | Bruno + Paula | Lista de presença; material entregue |
| 3 | Acessos de produção por perfil/unidade | Marcelo + Igor | P-04 aprovado |
| 4 | Ambiente produção (cloud **cliente**) | Marcelo + Igor | Backup, URL, monitoramento mínimo |
| 5 | Comunicação às quatro unidades | Paula + Camila | E-mail/data go-live + canal suporte |
| 6 | Runbook de suporte dia D | Camila + Natália | Contatos plantão |
| 7 | Teste de implantação em produção (dry-run) | Igor | Rollback testado |

## 4. Go / no-go — 03/03/2027

| Critério | Go | No-go |
|---|---|---|
| Defeitos bloqueadores | Zero conhecidos | Qualquer bloqueador em fluxo vendido |
| Homologação integrada | Aceite registrado ou tácito expirado sem inconformidade fundada | Inconformidade bloqueante aberta |
| Ambiente produção | Acessível e monitorado | Falha infra sem contorno |
| P-08 LGPD | Responsável da Vida+ formalmente indicado; regras de acesso/uso/retenção validadas; dados e controles de produção aprovados | Responsável não indicado ou dados reais sem governança validada |
| P-01 VidaFin | Integração homologada se a premissa foi atendida; se não foi, PB-15 formalmente retirado da baseline e limitação comunicada | PB-15 tratado como obrigatório sem documentação, credenciais e ambiente disponíveis |
| Equipe plantão | Escala Goofy + pontos focais Vida+ confirmados | Indisponibilidade crítica |

**Quem decide:** **Ricardo Salles (A* provisório)** no go-live conforme o [RACI](../pessoa_1/Matriz%20RACI%20Vida%20Mais.md); a Vida+ precisa ratificar formalmente essa autoridade. **Camila Rocha (R)** consolida evidências e recomenda go/no-go; **Marcelo (R)** confirma condições de TI; **Paula (R)** confirma prontidão operacional. A equipe Goofy Jello apoia implantação, testes e ambiente. Camila também depende da confirmação formal de sua designação como GP.

## 5. Plano de retorno (rollback / contorno)

1. **Rollback de aplicação:** Igor restaura versão anterior em produção se falha crítica na abertura (backup validado na semana 13); executar procedimento ensaiado e preservar transações/logs para reconciliação.
2. **Contorno operacional:** retorno temporário a procedimento manual acordado com Paula por unidade (máx. 48h) enquanto correção — registrado como incidente, não como mudança de escopo.  
3. Comunicação imediata às unidades e a Ricardo via [plano de comunicação](../pessoa_1/07%20Plano%20de%20Comunicação.md).

## 6. Plantão — semana do go-live

| Papel | Pessoa | Cobertura |
|---|---|---|
| Coordenação GP | Camila Rocha | Comercial + cliente |
| Backend/API | Rafael Nunes | Integração VidaFin se em escopo |
| Frontend/ops app | Diego Prado | |
| QA/incidentes | Natália Campos | Triagem defeito × mudança |
| Infra | Igor Mendes | Sob demanda (4 h/sem planejadas) |
| Cliente TI | Marcelo Viana | Acessos/produção |
| Cliente operação | Paula Ribeiro | Unidades |

## 7. Estabilização e garantia (30 dias)

- Período: **04/03–02/04/2027** (PDF 7.4 / [04 Cronograma](../pessoa_3/04%20Cronograma.md)).  
- Escopo: **defeitos** do que foi entregue; melhorias → [Fluxo de Mudanças](Fluxo%20de%20Mudança.md).  
- Capacidade: sem horas adicionais no [05 Custos](../pessoa_3/05%20Planejamento%20de%20Custos.md) — priorizar defeitos no canal de suporte acordado com cliente; evoluções seguem CR.

## 8. Sustentação pós-contrato

Fora do escopo deste projeto (handoff); passagem documentada para contrato de sustentação Goofy Jello — entregáveis: repositório, runbook, matriz de acessos, backlog residual (itens Depois/CR).

## 9. Coerência

- Riscos R09, R16, R12, R01 (dependência VidaFin) e R08 (LGPD) no [06 Riscos](Matriz%20de%20Riscos.md).
- Qualidade e aceite no [11 Plano de Qualidade](11%20Plano%20de%20Qualidade.md).
