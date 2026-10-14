# Reunião de decisões do grupo — Vida+

Fazer **antes** de qualquer pessoa escrever a versão final do seu artefato. Se cada um decidir sozinho, os 12 artefatos vão se contradizer, e coerência é o que o professor avalia (Aula 15).

Participantes: os 4 integrantes. Duração sugerida: 1h. Resultado: esta folha preenchida e compartilhada.

## Divisão

| Seat | Integrante | Artefatos |
|---|---|---|
| Pessoa 1 — Pessoas e governança | ______ | 01 Stakeholders, 03 RACI, 07 Comunicação |
| Pessoa 2 — Escopo e produto | ______ | 02 Escopo/Premissas/Restrições, 08 Backlog, 09 Roadmap |
| Pessoa 3 — Prazo e dinheiro | ______ | 04 Cronograma, 05 Custos |
| Pessoa 4 — Controle e go-live | ______ | 06 Riscos, 10 Mudanças, 11 Qualidade, 12 Go-live |

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

- [ ] Aceita como está
- [ ] Ajuste: ______

Justificativa para a defesa: ______

## Decisão 2 — Fronteira do primeiro go-live

Base: Anexo B do PDF.

**Dentro (proposta):** cadastros (pacientes, profissionais, especialidades, unidades, perfis), agenda clínica, portal do paciente (pesquisar, agendar, ver compromissos, cancelar conforme regra), recepção (agenda do dia, check-in, fila), status administrativo do atendimento, notificações por canal suportado, indicadores operacionais, carga inicial essencial, treinamento, go-live assistido, evento de atendimento para o VidaFin.

**Fora (contrato):** app nativo, telemedicina, TISS/convênios, cobrança online, saneamento extenso de histórico, custos de cloud e mensageria (cliente).

**Zona cinzenta — o grupo precisa decidir cada item:**

| Item | Origem | Dentro | Fora | Depois / CR | Justificativa |
|---|---|---|---|---|---|
| Confirmação por WhatsApp | nota 01/09, P-03 | | | | |
| Reagendamento pelo próprio paciente | nota 25/08, P-06 | | | | |
| Regras de encaixe/bloqueio por médico | nota 03/09 | | | | |
| Pagamento antecipado no portal | nota 16/09 | | | | |
| Anos de histórico de pacientes | nota 14/09, P-02 | | | | |
| Unidade Indaiatuba ativa no go-live | seção 3 e 10 | | | | |
| Dashboard executivo além dos indicadores macro | nota 08/09 | | | | |

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

- [ ] Aceita como está
- [ ] Ajuste: ______

## Decisão 4 — Marcos (já vendidos, seção 9)

| Marco | Data |
|---|---|
| Kick-off | 26/11/2026 |
| Descoberta e desenho funcional | 26/11 a 16/12/2026 |
| Protótipo | 17 a 23/12/2026 |
| Recesso | ______ (o grupo define) |
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

## Registro

Data da reunião: ______
Decisões que ainda ficaram abertas: ______
