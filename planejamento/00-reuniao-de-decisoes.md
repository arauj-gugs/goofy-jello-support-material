# Reunião de decisões do grupo — Vida+

Fazer **antes** de qualquer pessoa escrever a versão final do seu artefato. Se cada um decidir sozinho, os 12 artefatos vão se contradizer, e coerência é o que o professor avalia (Aula 15).

Participantes: os 4 integrantes. Duração sugerida: 1h. Resultado: esta folha preenchida e compartilhada.

## Divisão

| Seat | Integrante | Artefatos |
|---|---|---|
| Pessoa 1 — Pessoas e governança | Jenifer Gomes | 01 Stakeholders, 03 RACI, 07 Comunicação |
| Pessoa 2 — Escopo e produto | Philipe Gonçalves | 02 Escopo/Premissas/Restrições, 08 Backlog, 09 Roadmap |
| Pessoa 3 — Prazo e dinheiro | Gustavo Vieira | 04 Cronograma, 05 Custos |
| Pessoa 4 — Controle e go-live | Luís Gabriel | 06 Riscos, 10 Mudanças, 11 Qualidade, 12 Go-live |

Todos precisam conseguir defender o plano inteiro na apresentação.

## Limites que ninguém altera

Fonte: `VidaMais - KT Projetos - Goofy Jello.pdf`.

- Kick-off 26/11/2026. Go-live 03/03/2027 (14 semanas, atravessando o recesso). OS: até 100 dias corridos.
- Receita R$ 248.000. Teto interno de custo direto de equipe R$ 158.000. Margem-alvo R$ 90.000. Sem reserva gerencial informada.
- Equipe e taxas fixas (seção 8 do PDF). Não existe profissional extra para picos.
- Escopo macro fechado. Pedidos novos viram Change Request.
- Notas informais da negociação (seção 4) não são compromisso contratual.

## Decisão 1 — Abordagem

Proposta: **híbrida**. Linha de base preditiva (escopo, prazo e preço contratados) e execução ágil dentro dela: backlog priorizado, duas entregas incrementais já vendidas, roadmap. O quadro Kanban é a ferramenta de acompanhamento do fluxo na execução.

- [x] Aceita como está
- [ ] Ajuste: ______

Justificativa para a defesa: combina previsibilidade contratual (marcos e preço fixos) com flexibilidade de priorização dentro do backlog vendido, adequada ao handoff com duas entregas incrementais.

## Decisão 2 — Fronteira do primeiro go-live

Base: Anexo B do PDF.

**Dentro (proposta):** cadastros (pacientes, profissionais, especialidades, unidades, perfis), agenda clínica, portal do paciente (pesquisar, agendar, ver compromissos, cancelar conforme regra), recepção (agenda do dia, check-in, fila), status administrativo do atendimento, notificações por canal suportado, indicadores operacionais, carga inicial essencial, treinamento, go-live assistido, evento de atendimento para o VidaFin.

**Fora (contrato):** app nativo, telemedicina, TISS/convênios, cobrança online, saneamento extenso de histórico, custos de cloud e mensageria (cliente).

**Zona cinzenta — o grupo precisa decidir cada item:**

| Item | Origem | Dentro | Fora | Depois / CR | Justificativa |
|---|---|---|---|---|---|
| Confirmação por WhatsApp (Z-01) | nota 01/09, P-03 | | | X | Canal e custo com o cliente; 5.5 exclui WhatsApp API. Baseline: e-mail. |
| Reagendamento pelo próprio paciente (Z-02) | nota 25/08, P-06 | | | X | P-06 sem regra fechada; contrato cobre cancelamento conforme política. Remarcação pela equipe dentro. |
| Regras de encaixe/bloqueio por médico (Z-03) | nota 03/09 | X | | | Parametrização por permissão no módulo Agenda; exceções novas via CR. |
| Pagamento antecipado no portal (Z-04) | nota 16/09 | | X | | Exclusão 5.5 e Anexo B (cobrança online). |
| Anos de histórico de pacientes (Z-05) | nota 14/09, P-02 | | X | | Carga essencial sim; migração ampla e saneamento extensivo fora. |
| Unidade Indaiatuba ativa no go-live (Z-06) | seção 3 e 10 | | X | | Cadastro de unidade pode existir; operação, agenda, carga e treinamento da 5ª unidade ficam fora de 03/03/2027. |
| Dashboard executivo além dos indicadores macro (Z-07) | nota 08/09 | | | X | Indicadores macro e exportação dentro (Gestão); painel executivo adicional sem data. |

## Decisão 3 — Quem decide

Proposta:

| Decisão | Quem decide |
|---|---|
| Trade-off executivo (prazo, escopo grande, custo) | Ricardo Salles (sponsor) |
| Condução do projeto e integração dos planos | Camila Rocha (GP) |
| Prioridade do backlog no dia a dia (papel de Product Owner do lado Goofy Jello) | Bruno Ferraz, validando com Paula e Dra. Helena |
| Regras clínicas de agenda | Dra. Helena Moraes |
| Aceite operacional da recepção | Paula Ribeiro |
| Acessos, integrações, ambiente | Marcelo Viana |
| Integração VidaFin | Fernanda Lopes + Marcelo |
| Templates de mensagem | Juliana Reis |

Regra: mudança que mexe em escopo, prazo, custo ou integração passa pelo Fluxo de Mudanças (artefato 10), e conversa de WhatsApp não aprova nada.

- [x] Aceita como está
- [ ] Ajuste: ______

## Decisão 4 — Marcos (já vendidos, seção 9)

| Marco | Data |
|---|---|
| Kick-off | 26/11/2026 |
| Descoberta e desenho funcional | 26/11 a 16/12/2026 |
| Protótipo | 17 a 23/12/2026 |
| Recesso | **24/12/2026 a 06/01/2027** (sem construção comprometida) |
| Entrega 1 — cadastros, configuração, agenda | 07 a 13/01/2027 |
| Entrega 2 — portal, recepção, notificações, indicadores | 28/01 a 03/02/2027 |
| Homologação integrada | 04 a 17/02/2027 |
| Preparação de produção | 18 a 24/02/2027 |
| Go-live | 03/03/2027 |

Ponto a discutir: entre 13/01 e 28/01 há só duas semanas para construir toda a Entrega 2.

## Alerta para a Pessoa 3 levar à reunião

Conta indicativa (confirmar no artefato 05):

- Toda a equipe na disponibilidade máxima custa cerca de R$ 14.040 por semana. Em 14 semanas, isso dá cerca de R$ 196.560, acima do teto de R$ 158.000.
- As 1.180 h da pré-venda, distribuídas no profissional mais provável de cada frente, ficam perto de R$ 163.000 a R$ 167.000. Isso também passa do teto.
- Backend tem 330 h para um só sênior a 24 h/semana: cerca de 14 semanas, ou seja, o projeto inteiro. Isso é caminho crítico.

Conclusão: o grupo vai ter que priorizar escopo ou realocar horas. Esse é exatamente o tipo de decisão que a defesa vai cobrar.

## Ordem de trabalho depois da reunião

1. Pessoa 2 publica Escopo e Backlog (rascunho).
2. Pessoa 1 trabalha em paralelo em Stakeholders, RACI e Comunicação.
3. Pessoa 3 parte do Backlog para Cronograma e Custos.
4. Pessoa 4 parte das Premissas, do Cronograma e do RACI para Riscos, Mudanças, Qualidade e Go-live.
5. Revisão cruzada: cada funcionalidade do go-live aparece em Escopo → Backlog → Roadmap → Cronograma → Custos → Riscos → Qualidade → Go-live.

## Kick-off fictício — registros assumidos (case acadêmico)

Registrado em **26/11/2026** para fechar coerência dos artefatos sem cliente real:

1. **P-08 — LGPD:** função **Encarregado(a) de Dados e Privacidade (Vida+)** formalmente designada no kick-off (sem nome individual no handoff). **Ricardo Salles** arquiva a decisão; **contato técnico inicial: Marcelo Viana** até a Vida+ publicar o titular da função.
2. **Recepção:** **quatro líderes de recepção** (um por **unidade em operação 1–4**), roster mantido por **Paula Ribeiro**, indicados no kick-off para homologação e treinamento (nomes não constam no handoff público).
3. **Premissas P-01 a P-07:** permanecem como condições contratuais com datas-limite no planejamento (não são “fechadas” no kick-off).

**Contingências ainda relevantes na defesa:** se **P-01** não for atendida até 16/12/2026, **PB-15** sai da baseline.

## Registro

Data da reunião: **26/11/2026** (kick-off + revisão cruzada do grupo)  
Decisões em aberto (documentação): **nenhuma** — ver bloco acima e [revisao-cruzada-status.md](revisao-cruzada-status.md). **Fechado:** governança Ricardo/Camila, VidaFin/mensageria (papéis internos), ferramentas CR-LOG/Teams, fronteira Z-01–Z-07, P-08 (função) e líderes de recepção por unidade.
