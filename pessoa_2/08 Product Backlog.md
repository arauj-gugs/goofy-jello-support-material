# 08 — Product Backlog

**Projeto:** Vida+ — Sistema de Gestão e Agendamento de Clínica  
**Responsável pelo artefato:** Pessoa 2 — Escopo e produto  
**Status:** Rascunho inicial para validação na reunião do grupo  
**Base:** handoff `VidaMais - KT Projetos - Goofy Jello.pdf` (seções 6.2, 6.3, 6.4, 6.5 e 9; Anexo C), [02 Escopo, Premissas e Restrições](02%20Escopo%20Premissas%20e%20Restricoes.md), [Decisão 2](../planejamento/00-reuniao-de-decisoes.md) e definições das Aulas 18, 19 e 20.

## 1. Objetivo

Registrar a lista priorizada do que entra no primeiro go-live (**03/03/2027**), na mesma fronteira do artefato 02, para a Pessoa 3 estimar horas e montar cronograma e custos. A ordem permite que a Entrega funcional 1 exista **sem** portal e recepção digital.

**Responsável pela ordenação no dia a dia (Decisão 3):** Bruno Ferraz, validando com Paula Ribeiro e Dra. Helena Moraes.

## 2. Critérios adotados

Conceitos aplicados conforme o material das aulas e o guia da Pessoa 2:

| Conceito | Definição aplicada | Fonte |
|---|---|---|
| **Product Backlog** | Lista ordenada e viva do trabalho necessário para gerar valor no produto; transparência do que está dentro da linha de base do go-live. | Aula 20 |
| **Cartão de trabalho** | `Como [papel], quero [resultado].` Critérios observáveis; prioridade; responsável; dependências; evidências. Item grande vira histórias menores verificáveis (fatiamento). | Aula 19 |
| **Item de trabalho** | Funcionalidade ou habilitador com resultado verificável, critérios de aceitação e dependências explícitas. | Aula 19 |
| **Prioridade** | Posição na lista: itens acima podem ser iniciados antes; reordenação do que ainda não iniciou considera valor, risco e dependência. | Aula 19 + Decisão 3 |
| **Critério de aceite** | Verificações observáveis que definem quando o item está concluído no ambiente acordado. | Aula 19 + PDF 6.5 |
| **Incremento** | Software utilizável nas Entregas funcionais 1 e 2 vendidas (seção 9); não confundir com Sprint Backlog (aula futura — Aula 20). | Aula 18 + Aula 20 |
| **Sprint / eventos Scrum** | **Não** definidos neste artefato; Sprint, Sprint Backlog, eventos e Incremento operacional serão aprofundados em aula futura (Aula 20, plano de ensino Etapa 3). | Aula 20 |
| **Bloqueio** | Impedimento externo ou pendência do cliente que impede verificar o critério; permanece visível com causa, data e responsável. | Aula 19 |
| **Habilitador** | Item necessário para outros critérios serem testáveis (perfis, auditoria, carga, integração). | Guia Pessoa 2 + issue #12 |
| **Depois / CR** | Itens da zona cinzenta adiados; entram só por [Fluxo de Mudança](../pessoa_4/Fluxo%20de%20Mudança.md). | Aula 07 + artefato 02 |

Itens **fora** da seção 3 do artefato 02 **não** entram nesta lista. Reordenar o backlog não substitui aprovação formal de mudança de escopo.

## 3. Valor da Entrega 1 sem portal

Na janela **07 a 13/01/2027** (seção 9), usuários internos com perfil adequado cadastram pacientes, profissionais e estrutura da clínica e operam a agenda clínica nas **quatro unidades em operação**, com bloqueio, duração, agendamento, cancelamento, remarcação pela equipe e encaixe parametrizado (Z-03). A recepção e o coordenador deixam de depender de planilhas paralelas para conflitos de horário entre unidades. O paciente **ainda** agenda por telefone ou balcão; portal, check-in digital, notificações automáticas e indicadores consolidados vêm na Entrega 2. Isso atende ao princípio de entregar software utilizável cedo (Aula 18) dentro do contrato fechado.

## 4. Índice (prioridade = ordem)

| Ordem | ID | Módulo (artefato 02) | Entrega | Dependências principais | Habilitador |
|---:|---|---|---|---|---|
| 1 | PB-01 | Administração | 1 | — | Sim |
| 2 | PB-02 | Administração / 6.4 | 1 | PB-01 | Sim |
| 3 | PB-03a | Administração | 1 | PB-01 | — |
| 4 | PB-03b | Administração | 1 | PB-03a; **P-07** | — |
| 5 | PB-03c | Administração | 1 | PB-03b | — |
| 6 | PB-04 | Administração | 1 | PB-03a, PB-03b | — |
| 7 | PB-05a | Pacientes | 1 | PB-01 | — |
| 8 | PB-05b | Pacientes | 1 | PB-05a | — |
| 9 | PB-06 | Agenda | 1 | PB-03b, PB-03c, PB-04; **P-07** | — |
| 10 | PB-07 | Agenda | 1 | PB-05a, PB-06 | — |
| 11 | PB-08 | Agenda | 1 | PB-06, PB-07; Z-03 | — |
| 12 | PB-09 | Dados | 1 | PB-05a, PB-04; **P-02** | Sim |
| 13 | PB-10a | Recepção | 2 | PB-05a, PB-07 | — |
| 14 | PB-10b | Recepção | 2 | PB-10a, PB-05b | — |
| 15 | PB-10c | Recepção | 2 | PB-10b | — |
| 16 | PB-11 | Atendimento | 2 | PB-10a, PB-10b | — |
| 17 | PB-12a | Portal do paciente | 2 | PB-06, PB-07 | — |
| 18 | PB-12b | Portal do paciente | 2 | PB-12a, PB-07 | — |
| 19 | PB-12c | Portal do paciente | 2 | PB-12b | — |
| 20 | PB-12d | Portal do paciente | 2 | PB-12c; **P-06** | — |
| 21 | PB-13 | Notificações | 2 | PB-07, PB-12b; P-03 (canal) | — |
| 22 | PB-14 | Gestão | 2 | PB-07, PB-10a | — |
| 23 | PB-15 | Integração VidaFin | 2 | PB-11; **P-01** | Sim |

## 5. Cartões — itens dentro do go-live

### Entrega 1 · 07 a 13/01/2027

---

#### PB-01 · Perfis de acesso e usuários

**Módulo:** Administração (artefato 02 §3; PDF 5.2, 6.2) · **Entrega:** 1 · **Habilitador**

Como **administrador da Vida+**, quero **cadastrar perfis e usuários com permissões por unidade** para **garantir que cada papel acesse só o que o contrato prevê**.

**Critérios:**

- Criar e editar perfil com conjunto de permissões por módulo e por unidade.
- Associar usuário a um ou mais perfis e a unidades autorizadas; impedir acesso a unidade não vinculada.
- Usuário-chave do cliente (P-04) consegue autenticar e executar ao menos uma ação permitida e uma negada, conforme matriz acordada.
- Sem defeito **bloqueador** nos fluxos de cadastro de perfil/usuário (PDF 6.5 — funcional).

**Dependência:** nenhum item anterior. Bloqueio possível se **P-04** (lista de perfis e usuários-chave) não estiver aprovada até **09/12/2026** — causa: desenho de acesso incompleto; próxima ação: Paula Ribeiro + Marcelo Viana formalizarem matriz.

**Prioridade:** 1 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-02 · Auditoria de acesso e alteração

**Módulo:** Administração — diretriz 6.4 (artefato 02 §3) · **Entrega:** 1 · **Habilitador**

Como **gestor de projetos / segurança da informação**, quero **registrar eventos relevantes de acesso e de alteração de dados** para **rastrear quem fez o quê em homologação e produção**.

**Critérios:**

- Registrar login bem-sucedido e tentativa negada para usuário cadastrado.
- Registrar criação, alteração e exclusão (lógica ou física, conforme desenho) em entidades prioritárias: paciente, agenda e perfil/usuário.
- Consultar trilha por período, usuário e tipo de evento em ambiente de homologação.
- Perfis e acessos básicos validados por usuários-chave (PDF 6.5 — segurança).

**Dependência:** PB-01.

**Prioridade:** 2 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-03a · Cadastro de unidades

**Módulo:** Administração (artefato 02 §3; PDF 6.2) · **Entrega:** 1

Como **coordenador administrativo**, quero **cadastrar e manter unidades ativas** para **identificar as quatro unidades em operação e preparar a estrutura da clínica**.

**Critérios:**

- Criar e editar unidade com identificação e status ativo/inativo.
- Permitir cadastro da unidade Indaiatuba **sem** exigir agenda ou carga operacional (Z-06).
- Cenário Anexo C — Cadastros: criar/editar unidade sem defeito bloqueador.

**Dependência:** PB-01.

**Prioridade:** 3 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-03b · Especialidades, salas e tipos de atendimento

**Módulo:** Administração (artefato 02 §3; PDF 6.2) · **Entrega:** 1

Como **coordenador administrativo**, quero **cadastrar especialidades, salas/recursos e tipos de atendimento por unidade** para **vincular corretamente a estrutura física e clínica de cada unidade**.

**Critérios:**

- Cadastrar especialidade vinculada à unidade correta.
- Cadastrar sala/recurso por unidade conforme desenho funcional.
- Cadastrar tipo de atendimento vinculado à unidade e à especialidade acordada.
- Cenário Anexo C — Cadastros: criar/editar especialidade sem defeito bloqueador.

**Dependência:** PB-03a; **P-07** (dados de salas e recursos) até **16/12/2026**. Bloqueio: planilha de salas incompleta — Paula Ribeiro entrega layout padronizado.

**Prioridade:** 4 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-03c · Parâmetro geral de administração

**Módulo:** Administração (artefato 02 §3; PDF 6.2) · **Entrega:** 1

Como **coordenador administrativo**, quero **parametrizar ao menos um parâmetro geral acordado no desenho** para **padronizar comportamento do sistema nas unidades**.

**Critérios:**

- Definir e persistir ao menos um parâmetro geral acordado (ex.: tolerância de agenda ou identificação padrão).
- Alteração do parâmetro reflete nas telas de agenda ou cadastro que o desenho associar ao parâmetro.
- Verificação em homologação com perfil administrativo (PDF 6.5 — funcional).

**Dependência:** PB-03b.

**Prioridade:** 5 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-04 · Profissionais

**Módulo:** Administração (artefato 02 §3; PDF 6.2) · **Entrega:** 1

Como **coordenador administrativo**, quero **cadastrar profissionais vinculados a especialidades e unidades** para **montar grades de agenda por profissional**.

**Critérios:**

- Criar e editar profissional com vínculo a uma ou mais especialidades e unidades de atuação.
- Impedir profissional ativo em agenda sem especialidade vinculada (regra mínima acordada).
- Listar e filtrar profissionais por unidade e especialidade.
- Cenário Anexo C — Cadastros: criar/editar profissional.

**Dependência:** PB-03a, PB-03b.

**Prioridade:** 6 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-05a · Cadastrar paciente administrativo

**Módulo:** Pacientes (artefato 02 §3; PDF 6.2; Anexo B) · **Entrega:** 1

Como **recepcionista**, quero **registrar um novo paciente com dados administrativos** para **agendar e localizar o paciente sem prontuário clínico no escopo**.

**Critérios:**

- Registrar paciente com contatos, documentos, responsável (quando aplicável), convênio **informado** (sem TISS/autorização) e observações administrativas.
- **Não** exibir conteúdo clínico detalhado nem prontuário completo (fora do escopo, Anexo B).
- Cenário Anexo C — Cadastros: criar paciente.

**Dependência:** PB-01. Carga via PB-09 depende de **P-02** (layout e amostra até **16/12/2026**).

**Prioridade:** 7 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-05b · Atualizar cadastro administrativo do paciente

**Módulo:** Pacientes (artefato 02 §3; PDF 6.2; Anexo B) · **Entrega:** 1

Como **recepcionista**, quero **editar dados administrativos do paciente já cadastrado** para **manter cadastros corretos sem perder vínculo com agendamentos**.

**Critérios:**

- Editar dados cadastrais permitidos pelo perfil preservando histórico de agendamentos quando PB-07 existir (consulta somente leitura de compromissos passados).
- **Não** exibir conteúdo clínico detalhado nem prontuário completo (fora do escopo, Anexo B).
- Cenário Anexo C — Cadastros: editar paciente.

**Dependência:** PB-05a.

**Prioridade:** 8 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-06 · Grade, disponibilidade, bloqueio e duração da agenda

**Módulo:** Agenda (artefato 02 §3; PDF 6.2) · **Entrega:** 1

Como **coordenador de agenda / recepção**, quero **definir grade, disponibilidade, bloqueios e duração por profissional e unidade** para **oferecer horários consistentes ao agendar**.

**Critérios:**

- Abrir grade por profissional/unidade com intervalo e duração default configuráveis.
- Bloquear período (ex.: férias, manutenção de sala) impedindo novo agendamento no intervalo.
- Consultar disponibilidade considerando bloqueios e duração do tipo de atendimento.
- Cenários Anexo C — Agenda: abrir agenda, bloquear período, consultar disponibilidade.

**Dependência:** PB-03b, PB-03c, PB-04; **P-07**.

**Prioridade:** 9 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-07 · Agendar, cancelar e remarcar pela equipe

**Módulo:** Agenda (artefato 02 §3; PDF 6.2) · **Entrega:** 1

Como **recepcionista**, quero **agendar, cancelar e remarcar consultas pela equipe** para **substituir o controle manual de compromissos nas quatro unidades**.

**Critérios:**

- Agendar paciente em horário disponível; **impedir sobreposição** de dois agendamentos no mesmo recurso/profissional no mesmo instante.
- Cancelar agendamento futuro registrando motivo administrativo (campo acordado).
- Remarcar pela equipe para outro horário disponível, preservando rastro do compromisso anterior.
- Fluxos da Entrega 1 executados sem defeito bloqueador (PDF 6.5); homologação da entrega conforme cenários prioritários de Agenda (Anexo C).

**Dependência:** PB-05a, PB-06. Regras de cancelamento/remarcação pela equipe alinhadas a **P-06** quando fechadas até **16/12/2026**.

**Prioridade:** 10 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-08 · Encaixe com permissão parametrizada

**Módulo:** Agenda (artefato 02 §3; PDF 6.2; Z-03) · **Entrega:** 1

Como **usuário com permissão de encaixe**, quero **incluir encaixe em agenda cheia dentro dos limites parametrizados** para **atender urgências operacionais sem abrir exceções fora do contrato**.

**Critérios:**

- Permitir encaixe somente para perfil com permissão explícita; usuário sem permissão recebe bloqueio claro.
- Registrar encaixe distinguindo-o visualmente de slot regular na consulta de agenda.
- Respeitar regra mínima de bloqueio/duração já configurada em PB-06 (não anular bloqueio de indisponibilidade).
- Validação com Dra. Helena / Paula nos limites acordados (Z-03 **dentro**).

**Dependência:** PB-06, PB-07.

**Prioridade:** 11 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-09 · Carga inicial essencial de pacientes e profissionais

**Módulo:** Dados (artefato 02 §3; PDF 6.3 base legada; 6.5 dados) · **Entrega:** 1 · **Habilitador**

Como **coordenador de implantação**, quero **importar cadastros essenciais no layout acordado** para **não digitar manualmente a base mínima das quatro unidades**.

**Critérios:**

- Importar arquivo no layout fornecido pela Goofy Jello após **P-02** (amostra e layout até **16/12/2026**).
- Rejeitar ou sinalizar registros fora do layout com relatório de erros.
- Após importação, paciente e profissional importados aparecem nas telas de PB-05a e PB-04 e podem ser usados em PB-07.
- Carga conferida por **amostragem** pelo cliente (PDF 6.5 — dados); sem promessa de migração ampla nem saneamento extenso (Z-05 **fora**).

**Dependência:** PB-04, PB-05a. **Bloqueio possível:** P-02 não atendida — item sai da linha de base ou reduz escopo validável (premissa artefato 02). A carga final de produção na semana 13 é atividade de projeto, não um segundo item de produto neste backlog.

**Prioridade:** 12 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

### Entrega 2 · 28/01 a 03/02/2027

---

#### PB-10a · Agenda do dia na recepção

**Módulo:** Recepção (artefato 02 §3; PDF 6.2) · **Entrega:** 2

Como **recepcionista**, quero **consultar a agenda do dia por unidade** para **localizar compromissos e organizar o balcão**.

**Critérios:**

- Exibir agenda do dia por unidade com filtros mínimos (profissional/especialidade, conforme desenho).
- Cenário Anexo C — Recepção: fluxo de localização do agendamento do dia.

**Dependência:** PB-05a, PB-07 (agenda populada).

**Prioridade:** 13 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-10b · Check-in e cadastro na recepção

**Módulo:** Recepção (artefato 02 §3; PDF 6.2) · **Entrega:** 2

Como **recepcionista**, quero **confirmar a chegada do paciente e atualizar o cadastro administrativo permitido** para **registrar presença e corrigir dados no balcão**.

**Critérios:**

- Buscar paciente e registrar check-in vinculado ao agendamento do dia.
- Atualizar cadastro administrativo a partir da recepção sem violar permissão do perfil.
- Cenários Anexo C — Recepção: localizar paciente, confirmar chegada, atualizar cadastro.

**Dependência:** PB-10a; PB-05b.

**Prioridade:** 14 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-10c · Fila de atendimento na recepção

**Módulo:** Recepção (artefato 02 §3; PDF 6.2) · **Entrega:** 2

Como **recepcionista**, quero **alterar o status de chegada e visualizar a fila ordenada** para **acompanhar o fluxo de atendimento do dia**.

**Critérios:**

- Alterar status de chegada conforme regra acordada.
- Visualizar fila ordenada conforme regra acordada.
- Cenário Anexo C — Recepção: acompanhar fila.

**Dependência:** PB-10b.

**Prioridade:** 15 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-11 · Atendimento administrativo

**Módulo:** Atendimento (artefato 02 §3; PDF 6.2; Anexo B) · **Entrega:** 2

Como **profissional ou equipe de apoio autorizada**, quero **iniciar e encerrar atendimento com status e informações administrativas permitidas** para **acompanhar o fluxo da consulta sem prontuário clínico**.

**Critérios:**

- Iniciar e encerrar atendimento vinculado a agendamento em andamento.
- Registrar observações **administrativas** permitidas e classificar status conforme lista acordada.
- Anexar apenas tipos de arquivo permitidos no desenho; rejeitar tipo não permitido.
- **Não** permitir registro de conteúdo clínico detalhado (Anexo B — fora).
- Cenário Anexo C — Atendimento: alterar status e registrar informações permitidas.

**Dependência:** PB-10a, PB-10b.

**Prioridade:** 16 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-12a · Identificação do paciente no portal

**Módulo:** Portal do paciente (artefato 02 §3; PDF 6.2) · **Entrega:** 2

Como **paciente**, quero **identificar-me no portal** para **acessar apenas minhas informações e agendamentos permitidos**.

**Critérios:**

- Identificar paciente pelo mecanismo acordado (ex.: CPF + validação combinada).
- Bloquear acesso quando a identificação falhar, com mensagem clara ao usuário.
- Cenário Anexo C — Portal: fluxo de acesso após identificação.

**Dependência:** PB-06, PB-07.

**Prioridade:** 17 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-12b · Pesquisar horário e agendar pelo portal

**Módulo:** Portal do paciente (artefato 02 §3; PDF 6.2) · **Entrega:** 2

Como **paciente**, quero **pesquisar horários disponíveis e concluir um agendamento** para **marcar consulta sem depender exclusivamente do telefone**.

**Critérios:**

- Pesquisar horários disponíveis conforme regras de PB-06 e PB-07.
- Concluir agendamento respeitando as mesmas regras de **sobreposição** de PB-07.
- **Não** oferecer pagamento antecipado (Z-04 — fora).
- Cenários Anexo C — Portal: localizar horário, agendar.

**Dependência:** PB-12a, PB-07.

**Prioridade:** 18 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-12c · Consultar próximos compromissos no portal

**Módulo:** Portal do paciente (artefato 02 §3; PDF 6.2) · **Entrega:** 2

Como **paciente**, quero **listar meus próximos compromissos** para **saber quando devo comparecer**.

**Critérios:**

- Listar compromissos futuros do paciente autenticado.
- Exibir data, horário, unidade e profissional/especialidade conforme desenho.
- Cenário Anexo C — Portal: consultar compromisso.

**Dependência:** PB-12b.

**Prioridade:** 19 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-12d · Cancelar compromisso futuro no portal

**Módulo:** Portal do paciente (artefato 02 §3; PDF 6.2; Z-02) · **Entrega:** 2

Como **paciente**, quero **cancelar compromissos futuros conforme a política aprovada** para **desistir da consulta dentro das regras da clínica**.

**Critérios:**

- Cancelar compromissos futuros **somente** dentro da política aprovada em **P-06** (prazo e regra escritos).
- **Não** oferecer reagendamento autônomo pelo paciente (Z-02 — Depois / CR).
- Cenário Anexo C — Portal: cancelar conforme regra.

**Dependência:** PB-12c; **P-06** até **16/12/2026** para fechar regra de cancelamento no portal.

**Prioridade:** 20 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-13 · Notificações por canal suportado

**Módulo:** Notificações (artefato 02 §3; PDF 6.2, 6.3 mensageria; Z-01) · **Entrega:** 2

Como **paciente e recepção**, quero **receber confirmação, lembrete, cancelamento e alteração de horário com templates parametrizáveis** para **reduzir faltas e ligações de confirmação**.

**Critérios:**

- Disparar eventos de confirmação, lembrete, cancelamento e alteração de horário ao ocorrer transição correspondente na agenda (PB-07, PB-12b, PB-12d).
- Editar templates parametrizáveis com conteúdo mínimo validado com Juliana Reis (Decisão 3).
- **Baseline de aceite:** canal **e-mail** operacional em homologação; validar conteúdo e disparo (Anexo C — Notificações).
- WhatsApp permanece **fora** deste critério até CR formal (Z-01, P-03).

**Dependência:** PB-07, PB-12b. Se **P-03** não fechar até **16/12/2026**, a Entrega 2 aceita notificações por e-mail sem obrigação de outro canal.

**Prioridade:** 21 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-14 · Indicadores operacionais macro e exportação

**Módulo:** Gestão (artefato 02 §3; PDF 6.2; Z-07) · **Entrega:** 2

Como **gestor operacional (Paula / sponsor)**, quero **consultar indicadores macro de ocupação, faltas, cancelamentos e volume com exportação** para **enxergar desempenho das quatro unidades sem painel executivo adicional**.

**Critérios:**

- Exibir indicadores de ocupação, faltas, cancelamentos e volume filtráveis por unidade, profissional e especialidade (macros do contrato).
- Exportar relatório nos formatos acordados no desenho (ex.: planilha ou CSV).
- Conferir filtros prioritários com usuários-chave (Anexo C — Gestão).
- **Não** incluir dashboard executivo com metas/formulas adicionais (Z-07 — Depois / CR).

**Dependência:** PB-07, PB-10a (dados operacionais mínimos).

**Prioridade:** 22 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

#### PB-15 · Integração VidaFin — evento de atendimento particular

**Módulo:** Integração VidaFin (artefato 02 §3; PDF 6.3; **P-01**) · **Entrega:** 2 · **Habilitador** (faturamento)

Como **área financeira da Vida+**, quero **enviar evento de atendimento particular ao VidaFin após atendimento administrativo** para **permitir faturamento posterior sem digitação dupla**.

**Critérios:**

- Ao encerrar atendimento marcado como particular (regra acordada com Fernanda Lopes), enviar payload do evento definido na documentação da API.
- Tratar retorno esperado (sucesso e erro de negócio documentado) com registro consultável para suporte.
- Validar troca de dados em **ambiente de homologação** com credenciais e API disponibilizadas pelo cliente (PDF 6.5 — integração).
- Falha ou indisponibilidade da API **não** impede go-live dos demais módulos; integração sai da linha de base se **P-01** não se confirmar (premissa artefato 02).

**Dependência:** PB-11. **Bloqueio possível:** P-01 — Marcelo Viana entrega documentação, credenciais e ambiente de teste até **16/12/2026**.

**Prioridade:** 23 (ordenação acordada com Bruno Ferraz — Decisão 3).  
**Responsável e colaboradores:** A definir na execução.  
**Datas:** Entrada em fluxo: — · Conclusão: —  
**Evidências:** Homologação na entrega; registro para Natália (QA), conforme §6.

---

## 6. Políticas de fluxo (Aula 19)

Estas regras valem para todos os cartões deste backlog (PB-01 a PB-15, incluindo sub-IDs) quando o grupo operar a lista no quadro Kanban (Decisão 1):

| Transição | Política |
|---|---|
| **Backlog → em desenvolvimento** | Ordem respeitada ou reordenação acordada com Bruno Ferraz; critérios de aceite claros; dependências tratadas ou bloqueio registrado; capacidade da equipe disponível. |
| **Desenvolvimento → validação** | Código revisado conforme prática da equipe; testes previstos executados; evidências registradas para Natália (QA). |
| **Validação → concluído** | Todos os critérios do cartão atendidos no ambiente acordado (homologação na entrega); sem defeito bloqueador na dimensão funcional (PDF 6.5). |
| **Bloqueio** | Marcar cartão com causa, data e próxima ação com responsável; não remover o item da lista nem da ordem sem decisão formal se isso alterar escopo ou marco. |
| **Urgência** | Reordenar itens ainda não iniciados por valor, risco e dependência; exceção que altere escopo, prazo ou custo passa pelo [Fluxo de Mudança](../pessoa_4/Fluxo%20de%20Mudança.md). |

Este artefato **não** define limites de WIP, vazão nem tempo de ciclo: essas métricas dependem do histórico do fluxo na execução (Aula 19).

## 7. Depois / Change Request

Itens da zona cinzenta **adiados** para após **03/03/2027** ou até aprovação formal. **Sem data prometida** no roadmap comercial.

| ID | Zona (artefato 02) | Usuário principal | Por que não está no go-live | Entrada futura |
|---|---|---|---|---|
| CR-01 | Z-01 WhatsApp | Paciente / recepção | Canal e custo com o cliente; exclusão 5.5; baseline e-mail em PB-13 | Change Request após contratação P-03 |
| CR-02 | Z-02 Reagendamento pelo paciente | Paciente | Regra não fechada em P-06; remarcação pela equipe permanece em PB-07 | Change Request após política escrita |
| CR-03 | Z-07 Dashboard executivo | Sponsor / diretoria | Indicadores macro e exportação em PB-14; painel adicional fora da linha de base | Change Request sem compromisso de data |

Exclusões comerciais permanentes (app nativo, TISS, telemedicina, pagamento online, migração ampla, operação Indaiatuba no go-live, etc.) **não** viram cartão; ver seção 5 do [artefato 02](02%20Escopo%20Premissas%20e%20Restricoes.md).

## 8. Coerência e pendências

- **Pessoa 3:** transformar cada cartão em atividades, horas e marcos das Entregas 1 e 2 (seção 9 do PDF).
- **Pessoa 4:** critérios de aceite alimentam plano de qualidade (6.5, Anexo C); bloqueios P-01/P-02 ligam-se à matriz de riscos.
- **Pessoa 1:** validações clínicas e operacionais nas dependências P-05, P-06 e perfis P-04.
- **Artefato 09 Roadmap:** [09 Roadmap](09%20Roadmap.md) — cartões nas janelas Descoberta, Protótipo, Entrega 1, Entrega 2, Homologação, Preparação, Go-live e Estabilização.

**Pronto quando (issue #14):** cada item estiver no **formato de história/cartão** ensinado na Aula 19, com critérios de aceite revisados, fatiamento aplicado nos antigos PB-03/05/10/12 **sem** alterar fronteira do go-live, e o roadmap refletir os sub-IDs.