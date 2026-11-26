# 11 — Plano de Qualidade

**Projeto:** Vida+ — Sistema de Gestão e Agendamento de Clínica  
**Responsável pelo artefato:** Luís Gabriel (Pessoa 4 — Controle e go-live)  
**Status:** Rascunho alinhado ao PDF §6.5, §7.4, Anexo C e [backlog](../pessoa_2/08%20Product%20Backlog.md)

## 1. Objetivo

Definir **como** o grupo verifica que o produto atende aos critérios contratados antes de cada aceite e do go-live, integrando escopo, prazo e custo (Aula 04 / PMBOK).

## 2. Dimensões de qualidade (PDF §6.5)

| Dimensão | O que verificar | Evidência mínima | Responsável testes internos |
|---|---|---|---|
| **Funcional** | Fluxos PB do go-live executam conforme critérios do backlog | Roteiros Natália + build em homologação | Natália Campos (R) |
| **Segurança** | Perfis, permissões por unidade, trilha de auditoria (PB-02) | Matriz P-04 + casos por perfil | Natália + Marcelo (acessos) |
| **Integração** | Evento VidaFin quando P-01 atendida (PB-15) | Log de chamada API em homologação | Rafael + Fernanda (validação negócio) |
| **Dados** | Carga inicial essencial (PB-08) sem perda crítica | Amostra conferida com Paula | Rafael/Diego + Paula |
| **Performance** | Tempos aceitáveis em operações de agenda/recepção em homologação | Registro de teste de carga leve | Natália |
| **Homologação** | Cenários Anexo C cobertos nas quatro unidades representadas | Protocolo assinado / e-mail aceite | Cliente (R) com apoio Camila |

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

Homologação **integrada** (semanas 11–12 do [cronograma](../pessoa_3/04%20Cronograma.md)): validação ponta a ponta do conjunto PB-01 a PB-15 já aceito incrementalmente.

## 4. Testes internos antes de cada entrega

| Momento | Escopo do teste interno | Janela (plano) | Responsável |
|---|---|---|---|
| Pré–Entrega 1 | PB-01 a PB-09; smoke de regressão | Até 06/01/2027 (retomada pós-recesso) | Natália |
| Pré–Entrega 2 | PB-10a a PB-15 + regressão E1 | 27/01/2027 | Natália |
| Pré–go-live | Regressão completa + dados carga amostra | Semana 13 | Natália + Igor (ambiente) |

Natália reserva capacidade no cronograma **antes** de cada disponibilização ao cliente (alinhado a 16 h/sem com conciliação sustentação — ver [04](../pessoa_3/04%20Cronograma.md)).

## 5. Classificação de defeitos e liberação

| Classe | Definição | Liberação para homologação/aceite |
|---|---|---|
| **Bloqueador** | Impede fluxo crítico contratado ou exposição grave de segurança/dados | **Não** disponibilizar até corrigir |
| **Alto** | Funcionalidade importante degradada sem contorno aceito | Corrigir ou plano datado aprovado por GP + sponsor |
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
4. Registrar resultado na homologação de dados.

## 8. Coerência e pendências

- Alimentado por [02 Escopo](../pessoa_2/02%20Escopo%20Premissas%20e%20Restricoes.md) e critérios nos cartões do [08 Backlog](../pessoa_2/08%20Product%20Backlog.md).  
- Revisar após aulas da Etapa 4 (#24) se o professor exigir ajuste de formato.  
- Confirmar lista final de cenários Anexo C na mobilização com Paula.