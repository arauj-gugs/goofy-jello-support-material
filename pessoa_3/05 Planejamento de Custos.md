# 05 — Planejamento de Custos

**Projeto:** Vida+ — Sistema de Gestão e Agendamento de Clínica  
**Responsável pelo artefato:** Gustavo Vieira (Pessoa 3 — Prazo e custos)  
**Status:** Versão consolidada — revisão cruzada #26  
**Base:** handoff `VidaMais - KT Projetos - Goofy Jello.pdf` (seções 5.3, 6.6, 8 e 8.2), [Decisão 4](../planejamento/00-reuniao-de-decisoes.md), [02 Escopo](../pessoa_2/02%20Escopo%20Premissas%20e%20Restricoes.md), [04 Cronograma](04%20Cronograma.md), Aula 09 — Estimativas e Gestão de Custos.

## 1. Objetivo

Responder **por quanto** o plano de entrega cabe no **teto interno de R$ 158.000,00** de custo direto de equipe, com estimativa **bottom-up** rastreável ao cronograma, comparada à **análoga de pré-venda (1.180 h)**, e com **fluxo de caixa** alinhado às parcelas vendidas (R$ 248.000,00).

**Resposta executiva (kick-off):** custo direto de mão de obra planejado **R$ 151.550,00** (**1.096 h**), **R$ 6.450,00** abaixo do teto; margem bruta sobre o preço vendido **R$ 96.450,00**. **Sem reserva de contingência** informada no contrato — folga fica dentro do teto como buffer operacional (ver §6).

## 2. Critérios adotados

| Conceito | Definição aplicada | Fonte |
|---|---|---|
| **Estimar → orçar → controlar** | Horas por atividade viram orçamento; acompanhamento por pacote A01–A18 | Aula 09 |
| **Bottom-up** | Soma de atividade × responsável × taxa | Aula 09 + [04 Cronograma](04%20Cronograma.md) |
| **Análoga** | 1.180 h da pré-venda (PDF §6.6) alocadas na frente mais provável | Aula 09 + guia Pessoa 3 |
| **Paramétrica** | Custo = horas × R$/h (taxas fixas seção 8) | Aula 09 |
| **Tripla restrição** | Mudança de escopo/prazo exige replanejamento de horas e custo | Aula 02 |
| **Custos excluídos** | Cloud, licenças e mensageria — responsabilidade Vida+ | PDF 5.5 + artefato 02 §7.2 |

Não foram alteradas **taxas** nem incluídos **profissionais adicionais** (restrição do handoff).

## 3. Taxas de mão de obra (fixas)

| Pessoa | Função | R$/h |
|---|---|---:|
| Camila Rocha | GP | 150 |
| Bruno Ferraz | Analista de negócios | 120 |
| Lívia Monteiro | UX/UI | 105 |
| Rafael Nunes | Backend | 165 |
| Diego Prado | Full Stack | 130 |
| Natália Campos | QA | 105 |
| Igor Mendes | DevOps | 180 |

## 4. Estimativa analógica (pré-venda — PDF §6.6)

Referência comercial **1.180 h**, cada frente no profissional mais provável do PDF §8. Backend **330 h** conforme handoff (base do alerta na [reunião de decisões](../planejamento/00-reuniao-de-decisoes.md)).

| Frente | Profissional | Horas | R$/h | Custo (R$) |
|---|---|---:|---:|---:|
| Gestão / GP | Camila Rocha | 100 | 150 | 15.000 |
| Análise / desenho | Bruno Ferraz | 140 | 120 | 16.800 |
| UX/UI | Lívia Monteiro | 90 | 105 | 9.450 |
| Backend | Rafael Nunes | 330 | 165 | 54.450 |
| Full stack / frontend | Diego Prado | 300 | 130 | 39.000 |
| QA / testes | Natália Campos | 160 | 105 | 16.800 |
| DevOps | Igor Mendes | 60 | 180 | 10.800 |
| **Total analógico** | | **1.180** | | **162.300** |

O total analógico **excede** o teto de **R$ 158.000,00** em **R$ 4.300,00** (~2,7%), coerente com o intervalo **R$ 163.000–167.000** do guia quando se aplicam arredondamentos por frente.

## 5. Orçamento bottom-up (plano do grupo)

Horas derivadas do [04 Cronograma](04%20Cronograma.md) (pacotes A01–A18 e alocação semanal), com **capacidade real** (Bruno e Natália não no máximo contínuo; recesso sem dev; Diego absorve parte de APIs/telas para concentrar Rafael no núcleo).

### 5.1 Por pacote de atividade (cronograma)

| ID | Pacote (resumo) | Resp. principal | Horas | R$/h | Custo (R$) | PB |
|---|---|---|---:|---:|---:|---|
| A01 | Kick-off e integração de planos | Camila | 16 | 150 | 2.400 | — |
| A02 | Descoberta e refinamento backlog | Bruno | 52 | 120 | 6.240 | PB-01–15 |
| A03 | Desenho funcional e workshops | Bruno | 48 | 120 | 5.760 | PB-06–08, 12 |
| A04 | Protótipo UX | Lívia | 78 | 105 | 8.190 | PB-06, 10, 12, 14 |
| A05 | Backend — admin e cadastros E1 | Rafael | 108 | 165 | 17.820 | PB-01–04 |
| A06 | Backend — pacientes e agenda E1 | Rafael | 130 | 165 | 21.450 | PB-05–08 |
| A07 | Frontend interno E1 | Diego | 112 | 130 | 14.560 | PB-01–08 |
| A08 | Carga inicial | Diego / Rafael | 36 | 130* | 4.680 | PB-09 |
| A09 | QA ciclo E1 | Natália | 42 | 105 | 4.410 | PB-01–09 |
| A10 | Apoio aceite E1 | Camila / Natália | 24 | 128† | 3.060 | Marco M1 |
| A11 | Recepção, portal, notificações (back) | Rafael / Diego | 132 | 148† | 19.536 | PB-10–14, 13 |
| A12 | Frontend E2 | Diego | 88 | 130 | 11.440 | PB-10–12 |
| A13 | Integração VidaFin | Rafael / Diego | 40 | 148† | 5.920 | PB-15 |
| A14 | QA ciclo E2 | Natália | 46 | 105 | 4.830 | PB-10–15 |
| A15 | Apoio aceite E2 | Camila / Natália | 20 | 128† | 2.560 | Marco M2 |
| A16 | Homologação integrada | Natália + dev | 58 | 110† | 6.380 | Anexo C |
| A17 | Preparação produção | Igor / Camila | 36 | 158† | 5.688 | Implantação |
| A18 | Go-live assistido | Camila + equipe | 30 | 133† | 3.990 | Marco M3 |
| | **Total bottom-up** | | **1.096** | | **151.550** | |

\* Pacote A08: custo médio ponderado quando Rafael e Diego dividem o trabalho.  
† Pacotes com mais de um responsável: taxa média ponderada do esforço na atividade; o consolidado por pessoa (§5.2) usa taxas cheias e é a referência de controle.

### 5.2 Consolidado por profissional (controle primário)

| Profissional | Horas plano | R$/h | Custo (R$) | Δ vs analógica (h) |
|---|---:|---:|---:|---:|
| Camila Rocha | 128 | 150 | 19.200 | +28 |
| Bruno Ferraz | 132 | 120 | 15.840 | −8 |
| Lívia Monteiro | 78 | 105 | 8.190 | −12 |
| Rafael Nunes | 308 | 165 | 50.820 | −22 |
| Diego Prado | 278 | 130 | 36.140 | −22 |
| Natália Campos | 128 | 105 | 13.440 | −32 |
| Igor Mendes | 44 | 180 | 7.920 | −16 |
| **Total** | **1.096** | | **151.550** | **−84** |

### 5.3 Comparação analógica × plano

| Indicador | Analógica (pré-venda) | Plano (bottom-up) | Diferença |
|---|---:|---:|---:|
| Horas | 1.180 | 1.096 | −84 h (−7,1%) |
| Custo mão de obra | 162.300 | 151.550 | −10.750 |
| vs teto R$ 158.000 | Acima do teto | **Abaixo do teto** | Folga **6.450** |

### 5.4 Como o plano cabe no teto (defesa)

1. **Realocação:** Diego assume maior parcela de frontend e APIs (A07, A11–A13); Rafael foca núcleo administrativo e agenda (A05–A06), sem manter 330 h isoladas no backend.
2. **Escopo já decidido:** itens Z-01, Z-02 e Z-07 **fora** do go-live; sem horas de WhatsApp, reagendamento autônomo do paciente nem dashboard executivo ([Decisão 2](../planejamento/00-reuniao-de-decisoes.md)).
3. **Capacidade real:** Natália com ~50% do teto no Vida+ (sustentação); Bruno não em 16 h/sem durante toda a construção; **recesso sem horas de desenvolvimento**; Igor em bateladas (A17–A18).
4. **Sem hora extra nem nova contratação:** qualquer acréscimo ⇒ Fluxo de Mudança e trade-off prazo/escopo/custo ([R14](../pessoa_4/Matriz%20de%20Riscos.md)).

## 6. Contingência

| Item | Registro |
|---|---|
| Reserva gerencial no PDF | **Não informada** (artefato 02 §7.2) |
| Contingência separada neste plano | **R$ 0,00** — não há rubrica formal |
| Folga disponível | **R$ 6.450,00** dentro do teto (não equivale a ~40 h na taxa média; uso apenas para micro-desvios ou replanejamento interno) |
| Se custo realizado > 158.000 | Escalonar a Camila/Ricardo; cortar escopo via CR ou renegociar prazo — não assumir overrun silencioso |

## 7. Custos excluídos (fora desta planilha)

Responsabilidade da **Vida+**, conforme PDF 5.5 e [02 Escopo §7.2](../pessoa_2/02%20Escopo%20Premissas%20e%20Restricoes.md):

- Infraestrutura **cloud** e hospedagem de produção  
- **Licenças** de software de terceiros  
- **Mensageria** (SMS, e-mail transacional, eventual WhatsApp API)  
- Certificados, meios de pagamento e custos de telefonia  

Esses itens **não** entram na margem de R$ 96.450,00 calculada abaixo.

## 8. Receita e fluxo de caixa (PDF 5.3)

Preço vendido ao cliente: **R$ 248.000,00**.

| Parcela | % | Valor (R$) | Gatilho comercial (alinhamento ao cronograma) |
|---|---:|---:|---|
| Assinatura / início | 20 | 49.600 | Contrato / kick-off (26/11/2026) |
| Desenho funcional | 30 | 74.400 | Conclusão da janela descoberta+desenho (até 16/12/2026) |
| Homologação | 30 | 74.400 | Após Entrega 2 e entrada na homologação integrada (a partir de 04/02/2027) |
| Go-live | 20 | 49.600 | Aceite do go-live (**03/03/2027**) |

### 8.1 Margem (visão projeto)

| Linha | Valor (R$) |
|---|---:|
| Receita (preço vendido) | 248.000 |
| (−) Custo direto de equipe (plano) | 151.550 |
| **= Margem bruta-alvo (antes de overhead Goofy Jello)** | **96.450** |

Margem-alvo informada no handoff: **R$ 90.000,00**; o plano bottom-up **atinge acima** do alvo sem extrapolar o teto de custo.

## 9. Exemplo de impacto de mudança (Aula 09.2)

Cenário: cliente solicita **confirmação por WhatsApp (Z-01)** no primeiro go-live, via [Fluxo de Mudança](../pessoa_4/Fluxo%20de%20Mudança.md).

| Item | Sem mudança | Com CR (estimativa indicativa) |
|---|---|---|
| Escopo | Baseline e-mail (P-03) | Novo canal + templates + custo mensageria cliente |
| Horas adicionais | — | + BA 16 h, Backend 24 h, FS 20 h, QA 12 h, DevOps 8 h = **80 h** |
| Custo incremental (mão de obra) | — | **≈ R$ 11.200** (taxas §3) |
| Custo planejado total | 151.550 | **≈ 162.750** → **acima do teto** |
| Prazo | Marco 03/03/2027 | +1 a 2 semanas no caminho crítico (integração + homologação) |
| Decisão | — | Ricardo Salles: **adiar para pós go-live** (decisão grupo Z-01) **ou** trade-off formal (prazo/custo) |

Conclusão pedagógica: mudanças que reintroduzem itens da zona cinzenta **não cabem** na folga de R$ 6.450; exigem CR aprovado e atualização deste artefato e do [04 Cronograma](04%20Cronograma.md).

## 10. Coerência com os demais artefatos

| Artefato | Alinhamento |
|---|---|
| [04 Cronograma](04%20Cronograma.md) | Mesmos IDs A01–A18 e **1.096 h** por pacote (sincronizado na revisão cruzada); horas semanais compatíveis com §5.2 |
| [09 Roadmap](../pessoa_2/09%20Roadmap.md) | Parcela “homologação” 30% após Entrega 2 |
| [Matriz de Riscos](../pessoa_4/Matriz%20de%20Riscos.md) | **R13** — backend/capacidade Rafael; **R14** — este plano mitiga ultrapassar teto |
| [08 Backlog](../pessoa_2/08%20Product%20Backlog.md) | Custo atribuído por PB na coluna da tabela §5.1 |
| [02 Escopo](../pessoa_2/02%20Escopo%20Premissas%20e%20Restricoes.md) | Teto §7.2; exclusões §7.2 e 5.5 |

## 11. Contas de verificação (guia Pessoa 3)

| Verificação | Resultado no artefato |
|---|---|
| Equipe no máximo × 14 semanas ≈ R$ 196.560 | Plano usa **1.096 h**, não o teto semanal pleno |
| 1.180 h analógica ≈ R$ 163k–167k | **R$ 162.300** na tabela §4 |
| Backend 330 h × Rafael 24 h/sem ≈ 14 semanas | Plano **308 h** Rafael em **~12 semanas úteis** + apoio Diego — ainda crítico (R13) |
| Cabe em R$ 158.000? | **Sim** — **R$ 151.550** |

## 12. Decisões registradas

- Redução de **84 h** versus analógica (**aceita** na revisão cruzada; bottom-up **1.096 h / R$ 151.550** é a baseline de controle).
- **R13/R14** na [Matriz de Riscos](../pessoa_4/Matriz%20de%20Riscos.md) refletem este artefato e o [04 Cronograma](04%20Cronograma.md).
- PB-01 a PB-15 rastreáveis a pacotes A01–A18 em §5.1 (sincronizado com o cronograma).