# 07 — Plano de Comunicação

**Projeto:** Vida+ — Sistema de Gestão e Agendamento de Clínica  
**Responsável pelo artefato:** Jenifer Gomes (Pessoa 1 — Pessoas e governança)  
**Status:** Rascunho alinhado ao [RACI](Matriz%20RACI%20Vida%20Mais.md), [Decisão 3](../planejamento/00-reuniao-de-decisoes.md) e [cronograma](../pessoa_3/04%20Cronograma.md)

## 1. Objetivo

Garantir **informação certa, pessoa certa, momento certo e canal adequado** (Aula 11), com registro formal quando a decisão alterar escopo, prazo, custo ou integração — inclusive impedindo que conversas informais (ex.: WhatsApp) virem compromisso sem o [Fluxo de Mudanças](../pessoa_4/Fluxo%20de%20Mudança.md).

## 2. Princípios

| Princípio | Aplicação no Vida+ |
|---|---|
| Formal × informal | Decisões de baseline → canal formal + registro (CR/log). Dúvidas operacionais → e-mail ou reunião, sempre com ata curta na ferramenta do projeto. |
| Push / pull / interativa | Status semanal (push); repositório de artefatos e backlog (pull); workshops e homologação (interativa). |
| Recesso | **24/12/2026–06/01/2027:** sem entregas de build; GP envia **um** resumo assíncrono de premissas P-01 a P-08 e riscos abertos (se houver). |
| Aceite contratual | Cada disponibilização para aceite **inicia contagem de 5 dias úteis** (PDF 7.4); comunicação deve explicitar data de início e canal de manifestação. |

## 3. Matriz de comunicação por público

| Público | O quê | Quando | Canal | Formato | Quem comunica | Registro |
|---|---|---|---|---|---|---|
| **Ricardo Salles** (sponsor) | Status executivo; desvios de prazo/custo; decisões de trade-off; mudanças a aprovar; início de janelas de aceite | Quinzenal + sob demanda + antes de cada aceite de entrega | Reunião (Teams) + e-mail resumo | Push / interativa | Camila Rocha (GP) | Ata + planilha de status; IDs de mudança aprovados |
| **Paula Ribeiro** e **Dra. Helena** | Convocação para validações; regras P-05/P-06; homologação E1/E2 com antecedência mínima **3 dias úteis** | Conforme marcos do [Roadmap](../pessoa_2/09%20Roadmap.md); janelas 07–13/01 e 28/01–03/02 | E-mail + sessão guiada | Interativa | Camila (convocação); Bruno (conteúdo funcional) | Lista de presença + evidências de homologação |
| **Marcelo Viana** (TI Vida+) | Acessos; API VidaFin (P-01); ambientes homologação/produção; credenciais | Kick-off; até **16/12/2026** para P-01/P-02 críticos; antes E1/E2 | E-mail técnico + call se bloqueio | Push / interativa | Camila + Rafael Nunes (conteúdo técnico) | Ticket/e-mail arquivado; checklist P-01 |
| **Fernanda Lopes / Juliana Reis** | Eventos VidaFin; templates e canal de notificação (P-03) | Descoberta e pré-E2 | Reunião + e-mail | Interativa | Bruno + Camila | Versão aprovada de template/canal |
| **Equipe Goofy Jello** | Prioridades da semana; impedimentos; decisões de backlog | Diário assíncrono (Slack/Teams) + planning semanal | Slack/Teams + planning | Pull + push | Camila (facilita); Bruno (prioridades) | Board Kanban; impedimentos com dono |
| **Usuários-chave (homologação)** | Pacote de testes; critérios 6.5; prazo de **5 dias úteis** para aceite ou inconformidade fundada | Ao liberar E1, E2 e homologação integrada | E-mail formal com link/ambiente | Push | Camila + Natália (roteiro de testes) | Protocolo de disponibilização datado |
| **Quatro unidades / recepção** | Treinamento; go-live **03/03/2027**; plano de ondas | Semana 13–14 | Presencial/remoto + material | Push / interativa | Paula (coordenação cliente); Bruno (conteúdo) | Lista de treinamento; [12 Go-live](../pessoa_4/12%20Plano%20de%20Go-live.md) |
| **Diretoria Goofy Jello** | Margem, risco e capacidade | Mensal ou se R vermelho (matriz riscos) | E-mail executivo | Push | Camila + Gustavo Vieira (prazo/custo se impacto) | Referência a risco ID |

## 4. Comunicações ligadas a marcos (Decisão 4)

| Marco | Comunicação obrigatória | Responsável |
|---|---|---|
| Kick-off 26/11/2026 | Contexto, equipe, governança, premissas P-01 a P-08 | GP + grupo (P1 abertura) |
| Entrega funcional 1 (07–13/01/2027) | Disponibilização + início **5 dias úteis** aceite | Camila |
| Entrega funcional 2 (28/01–03/02/2027) | Idem | Camila |
| Homologação integrada (fev.) | Cenários Anexo C + prazo cliente | Camila + Paula |
| Go-live 03/03/2027 | Comunicação às unidades; plantão | Ver plano go-live |
| Recesso 24/12–06/01 | Aviso de pausa de build; canal para premissas urgentes | Camila |

## 5. Mudanças, escopo e “WhatsApp não aprova”

1. Pedido informal (WhatsApp, balcão, e-mail sem CR) → GP **responde** pedindo registro no fluxo ou e-mail com ID.  
2. Se alterar baseline → somente após decisão de **Ricardo Salles** (RACI + Fluxo 10) e atualização de artefatos.  
3. GP comunica decisão a solicitante, equipe e, se custo/prazo, sponsor (modelo Z-01 no [05 Custos](../pessoa_3/05%20Planejamento%20de%20Custos.md)).

## 6. Coerência com os demais artefatos

- **[03 RACI](Matriz%20RACI%20Vida%20Mais.md):** emissores por atividade (homologação, aceite, mudança).  
- **[04 Cronograma](../pessoa_3/04%20Cronograma.md):** datas das convocações.  
- **[06 Riscos](../pessoa_4/Matriz%20de%20Riscos.md):** escalonamento quando comunicação falhar (ex.: R09 homologação).  
- **[10 Fluxo de Mudanças](../pessoa_4/Fluxo%20de%20Mudança.md):** canal oficial de solicitação e comunicação pós-decisão.

## 7. Pendências do grupo

- Confirmar ferramenta única de registro (log de mudanças + atas).  
- Confirmar se aceite por entrega será centralizado em Ricardo ou delegado por área (RACI P-RACI-04).