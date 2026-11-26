# 11 — Plano de Qualidade

**Projeto:** Vida+ — Sistema de Gestão e Agendamento de Clínica  
**Responsável pelo artefato:** Luís Gabriel (Pessoa 4 — Controle e go-live)  
**Status:** Revisão cruzada alinhada ao escopo, backlog, cronograma, RACI e comunicação; janelas de QA

## 1. Objetivo

Definir **como** o grupo verifica que o produto atende aos critérios contratados antes de cada aceite e do go-live, integrando escopo, prazo e custo (Aula 04 / PMBOK).

## 2. Dimensões de qualidade (PDF §6.5)

| Dimensão | O que verificar | Evidência mínima | Responsável testes internos |
|---|---|---|---|
| **Funcional** | Fluxos PB do go-live executam conforme critérios do backlog | Roteiros Natália + build em homologação | Natália Campos (R) |
| **Segurança** | Perfis, permissões por unidade, trilha de auditoria (PB-02) | Matriz P-04 + casos por perfil | Natália + Marcelo (acessos) |
| **Integração** | Evento VidaFin quando P-01 atendida (PB-15) | Log de chamada API em homologação | Rafael + Fernanda (validação negócio) |
| **Dados** | Carga inicial essencial (PB-09) sem perda crítica | Amostra conferida com Paula | Rafael/Diego + Paula |
| **Performance** | Tempos aceitáveis em operações de agenda/recepção em homologação | Registro de teste de carga leve | Natália |
| **Homologação** | Cenários Anexo C cobertos nas quatro unidades representadas | Protocolo de disponibilização, evidências de teste e aceite/inconformidade | Ricardo Salles (A* provisório); Paula Ribeiro e Fernanda Lopes (R por área); Camila e Natália apoiam |

## 3. Cenários de homologação por área (Anexo C — síntese)

| Área | Cenários prioritários | Validador cliente |
|---|---|---|
| Cadastros e perfis | Criar/editar usuário; permissão por unidade; bloqueio de acesso indevido | Paula / Marcelo |
| Agenda clínica | Grade, bloqueio, encaixe parametrizado (Z-03); agendar/cancelar pela equipe | Dra. Helena + Paula |
| Recepção | Agenda do dia; check-in; fila | Paula |
| Portal paciente | Pesquisar, agendar, cancelar conforme P-06 | Paula |
| Notificações | E-mail baseline (P-03); templates Juliana | Juliana + Paula |
| VidaFin | Disparo de evento pós-atendimento (se P-01 ok) | Fernanda |
| Indicadores macro | Exportação/indicadores contratados (sem Z-07) | Bruno + Paula |

Homologação **integrada** (semanas 11–12 do [cronograma](../pessoa_3/04%20Cronograma.md)): validação ponta a ponta do conjunto PB-01 a PB-15 já aceito incrementalmente; PB-15 só integra a baseline se P-01 for atendida, caso contrário aplica-se a decisão do artefato 02 de retirá-lo da linha de base e informar a limitação.

## 4. Testes internos antes de cada entrega

| Momento | Escopo do teste interno | Janela (plano) | Responsável |
|---|---|---|---|
| Pré–Entrega 1 | PB-01 a PB-09; smoke de regressão | Semanas 4 e 7, antes da liberação de E1; data exata na semana 7 a confirmar; sem atividade no recesso 24/12–06/01 | Natália; Camila coordena e responde pela conclusão (A* provisório) |
| Pré–Entrega 2 | PB-10a a PB-15 + regressão E1 | Até 27/01/2027, antes da janela de disponibilização 28/01–03/02 | Natália; Camila coordena (A* provisório) |
| Pré–go-live | Regressão completa + dados carga amostra | Semana 13 (18–24/02) | Natália + Igor (ambiente); Camila coordena |

Natália reserva capacidade no cronograma **antes** de cada disponibilização ao cliente (alinhado à capacidade planejada e à conciliação com sustentação — ver [04](../pessoa_3/04%20Cronograma.md)). Pelo RACI, Camila é A provisório pela conclusão dos testes internos; Natália é R pela execução, registro de defeitos e evidências. A janela da E1 deve ser reconciliada com o recesso e a alocação semanal da Pessoa 3.

## 5. Classificação de defeitos e liberação

| Classe | Definição | Liberação para homologação/aceite |
|---|---|---|
| **Bloqueador** | Impede fluxo crítico contratado ou exposição grave de segurança/dados | **Não** disponibilizar até corrigir |
| **Alto** | Funcionalidade importante degradada sem contorno aceito | Corrigir antes de liberar; qualquer aceitação de risco/plano excepcional deve ser registrada e aprovada pela autoridade definida no RACI (Ricardo A* provisório), com recomendação de Camila e validação da área afetada |
| **Médio** | Desvio com contorno operacional documentado | Liberar com registro; corrigir antes go-live se afetar PB do go-live |
| **Baixo** | Cosmético / menor | Registrar; pode ir para pós go-live se não afetar aceite |

## 6. Aceite do cliente (PDF §7.4)

- **5 dias úteis** após cada disponibilização para aceite ou inconformidade **fundamentada**.  
- **Aceite tácito** se não houver manifestação no prazo — a [comunicação](../pessoa_1/07%20Plano%20de%20Comunicação.md) deve registrar a data de início.  
- **Defeito** (requisito aprovado) × **mudança** (nova expectativa) conforme [Fluxo de Mudanças](Fluxo%20de%20Mudança.md).  
- **Garantia 30 dias** após go-live: apenas defeitos do escopo entregue, não melhorias.

## 7. Carga inicial — conferência por amostragem

1. Importar layout acordado (P-02).  
2. Conferir amostra (% por unidade definida com Paula) para duplicidade e campos obrigatórios.  
3. Bloquear uso de dados reais de pacientes em dev sem controles LGPD (P-08).  
4. Registrar resultado na homologação de dados. Se a P-02 (amostra/layout até 16/12/2026) não se confirmar, aplicar a decisão do artefato 02: retirar ou reduzir a carga da baseline por decisão formal; não improvisar saneamento extenso.

## 8. Coerência e pendências

- Alimentado por [02 Escopo](../pessoa_2/02%20Escopo%20Premissas%20e%20Restricoes.md) e critérios nos cartões do [08 Backlog](../pessoa_2/08%20Product%20Backlog.md).  
- Revisar após aulas da Etapa 4 (#24) se o professor exigir ajuste de formato.  
- Confirmar lista final de cenários Anexo C na mobilização com Paula.
- Confirmar com Pessoa 3 a janela exata de QA E1: A09 está nas semanas 4 e 7, mas o recesso vai até 06/01. Não liberar E1 sem concluir testes internos; se a capacidade de QA não couber antes da disponibilização, replanejar a janela de entrega formalmente.
- Ricardo consta como A* provisório para homologação e aceite no RACI; obter confirmação formal ou delegação por tipo de entrega.
