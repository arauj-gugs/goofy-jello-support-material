# Pessoa 3 — Prazo e custos

Integrante: ______

## Seus artefatos

- 04 Cronograma
- 05 Planejamento de Custos
- No kick-off: "Quando?" e "Por quanto?"

## Aulas que você precisa dominar

| Aula | Conceito que vira artefato |
|---|---|
| 08 — Planejamento e Gestão do Cronograma | Escopo → atividades → dependências → durações → datas. Atividade x marco (duração zero). Predecessora, sucessora, paralelismo. Esforço é diferente de duração. Caminho crítico. |
| 08.1 — Exemplo do Cronograma (png) e 08.2/08.3 — Atividade prática | Formato: tabela de atividades, predecessoras, paralelos, marcos, caminho crítico, prazo. |
| 09 — Estimativas e Gestão de Custos | Estimar → orçar → controlar. Mão de obra, tecnologia, ferramentas, outros. Análoga, paramétrica (quantidade x taxa), bottom-up, três pontos. Reserva de contingência. |
| 09.1 — Exemplo de Estimativas (png) e 09.2 — Atividade prática | Formato: atividade, responsável, horas, valor/h, custo, contingência, impacto de mudança. |
| 02 — Tripla restrição | Mudar escopo, prazo ou custo afeta os outros dois. |

## Insumos do PDF

- Seção 6.6 Estimativa da pré-venda (1.180 h por frente).
- Seção 8 Equipe, disponibilidade semanal, custo/h e observações de capacidade.
- Seção 8.2 Teto R$ 158.000 de custo direto de equipe.
- Seção 5.3 Parcelas do cliente (20/30/30/20) e seção 9 marcos.
- Seção 5.5 Exclusões: cloud, licenças, mensageria ficam com o cliente.
- Backlog e Roadmap da Pessoa 2.

## Equipe (seção 8)

| Pessoa | Função | h/semana | R$/h |
|---|---|---|---|
| Camila Rocha | GP | 12 | 150 |
| Bruno Ferraz | Analista de Negócios | 16 | 120 |
| Lívia Monteiro | UX/UI | 8 | 105 |
| Rafael Nunes | Backend | 24 | 165 |
| Diego Prado | Full Stack | 24 | 130 |
| Natália Campos | QA | 16 | 105 |
| Igor Mendes | DevOps | 4 | 180 |

## Contas de verificação (confirmar no seu artefato)

- Equipe toda na disponibilidade máxima: cerca de R$ 14.040/semana. Em 14 semanas, cerca de R$ 196.560, acima do teto.
- 1.180 h da pré-venda, cada frente no profissional mais provável: entre R$ 163.000 e R$ 167.000. Isso também fica acima do teto.
- Backend 330 h com Rafael a 24 h/semana: cerca de 14 semanas. Esse é provavelmente o caminho crítico.

Você precisa mostrar como o plano cabe em R$ 158.000. As alavancas são: realocar frentes entre pessoas, reduzir horas onde o backlog permitir e adiar itens cinzentos com a Pessoa 2. Não vale inventar pessoa nova nem mudar a taxa.

## 04 Cronograma — o que precisa ter

- [ ] Atividades derivadas do backlog e das fases (descoberta, desenho, protótipo, construção E1, construção E2, testes, homologação, preparação, go-live, estabilização).
- [ ] Predecessoras e paralelismos (ex.: UX junto da descoberta, frontend em paralelo ao backend depois do desenho funcional).
- [ ] Marcos nas datas vendidas (Decisão 4).
- [ ] Recesso de fim de ano tratado explicitamente.
- [ ] Capacidade real: Natália dividida com sustentação, Igor sob demanda e agrupado, Bruno sem dedicação integral, Rafael com teto de 24 h.
- [ ] Caminho crítico identificado.
- [ ] Dependências do cliente como atividades com dono (API VidaFin, CSV, salas, regras).
- [ ] Representação visual (Gantt ou tabela por semana).

## 05 Planejamento de Custos — o que precisa ter

- [ ] Bottom-up: atividade, responsável, horas, R$/h, custo.
- [ ] Comparação com a análoga (1.180 h da pré-venda).
- [ ] Total de mão de obra comparado com o teto de R$ 158.000.
- [ ] Contingência: decidir se cabe e de onde sai. O PDF não informa reserva gerencial.
- [ ] Custos excluídos listados como "responsabilidade do cliente" e fora da conta.
- [ ] Linha separada: entrada de caixa por parcela (assinatura, desenho funcional, homologação, go-live).
- [ ] Margem resultante (receita menos custo direto).
- [ ] Exemplo de impacto de uma mudança, no formato da Aula 09.2.

## Depende de / alimenta

- Depende da Pessoa 2 (backlog e roadmap) e da Pessoa 1 (quem participa de quê).
- Alimenta a Pessoa 4: caminho crítico vira risco, folga vira resposta, custo de mudança vira regra do fluxo.

## Perguntas que a banca pode fazer

- Qual é o caminho crítico? E se o Rafael atrasar?
- Como vocês chegaram em R$ ______ se a pré-venda estimou 1.180 h?
- O que acontece com o prazo no recesso?
- Onde está a contingência?
