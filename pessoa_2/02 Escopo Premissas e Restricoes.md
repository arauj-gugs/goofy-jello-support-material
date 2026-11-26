# 02 — Escopo, Premissas e Restrições

**Projeto:** Vida+ — Sistema de Gestão e Agendamento de Clínica  
**Responsável pelo artefato:** Pessoa 2 — Escopo e produto  
**Status:** Rascunho inicial para validação na reunião do grupo  
**Base:** handoff `VidaMais - KT Projetos - Goofy Jello.pdf`, [Decisão 2](planejamento/00-reuniao-de-decisoes.md) da reunião de decisões e definições das Aulas 02, 03 e 07.

## 1. Objetivo

Registrar a linha de base de escopo, premissas e restrições do Vida+ para que backlog, cronograma, custos, riscos e qualidade usem a mesma fronteira do primeiro go-live.

**Objetivo do projeto (uma frase):** disponibilizar em **03/03/2027** uma plataforma única de cadastro, agenda, atendimento administrativo e indicadores operacionais para as **quatro unidades em operação**, reduzindo conflitos de agenda, faltas e retrabalho da recepção, antes da abertura da unidade de Indaiatuba.

Fonte principal: memorando e resumo executivo do handoff (seções 2 e 3).

## 2. Critérios adotados

Conceitos aplicados conforme o material das aulas e do guia da Pessoa 2:

| Conceito | Definição aplicada | Fonte |
|---|---|---|
| **Escopo do produto** | Características e funcionalidades da solução entregue ao cliente (o que o sistema faz). | Aula 07 |
| **Escopo do projeto** | Trabalho necessário para produzir e entregar essa solução (atividades e marcos). | Aula 07 |
| **Fora do escopo** | Itens explicitamente excluídos ou não caracterizados no pacote vendido; definir limites reduz expectativa e expansão descontrolada. | Aula 07 |
| **Premissa** | Condição assumida como verdadeira para o planejamento, ainda que não totalmente confirmada (“estamos planejando considerando que…”). Se não se confirmar, gera risco e impacto. | Aula 07 |
| **Restrição** | Limite que restringe opções do projeto e precisa ser respeitado (prazo, orçamento, tecnologia, recursos, políticas). | Aula 07 |
| **Abordagem** | Linha de base preditiva para escopo, prazo e preço contratados; execução com backlog priorizado, duas entregas incrementais vendidas e mudanças formais quando necessário. | Aula 03 + [Fluxo de Mudança](pessoa_4/Fluxo de Mudança.md) |

Regras de negócio detalhadas (cancelamento, encaixe, indicadores) integram o **escopo do produto**, não a lista de restrições. Itens informais da seção 4 do handoff não viram compromisso até decisão registrada ou Change Request.

## 3. Escopo do produto (dentro)

Pacote comercial (seção 5.2) e módulos do anexo técnico (seção 6.2), incluindo a integração citada em 6.3 quando as dependências do cliente forem atendidas.

| Módulo | Funcionalidades macro incluídas no primeiro go-live |
|---|---|
| **Administração** | Unidades; especialidades; profissionais; salas; tipos de atendimento; perfis; usuários; parâmetros gerais. |
| **Pacientes** | Cadastro; contatos; documentos; responsável; convênio informado; observações administrativas; histórico de agendamentos. |
| **Agenda** | Grade por profissional/unidade; disponibilidade; bloqueios; duração; agendamento; cancelamento; remarcação pela equipe; encaixe mediante permissão parametrizada. |
| **Portal do paciente** | Identificação; pesquisa de horários; agendamento; visualização de próximos compromissos; cancelamento conforme regra aprovada (P-06). |
| **Recepção** | Agenda diária; busca de paciente; check-in; status de chegada; atualização cadastral; fila de atendimento. |
| **Atendimento** | Início/fim; registro de observações permitidas; classificação de status; anexos permitidos. |
| **Notificações** | Confirmação, lembrete, cancelamento e alteração de horário; templates parametrizáveis; disparo pelo canal contratado e suportado (e-mail como baseline se P-03 não fechar a tempo). |
| **Gestão** | Indicadores macro de ocupação, faltas, cancelamentos e volume por unidade/profissional/especialidade; exportação de relatórios. |
| **Integração VidaFin** | Envio de evento de atendimento particular para posterior faturamento, sujeito à API e ambiente de homologação (P-01). |
| **Dados** | Carga inicial de cadastros essenciais em layout acordado pelo cliente (não migração ampla de histórico). |

**Incluído com limites acordados na zona cinzenta (ver seção 5):** encaixe e bloqueio parametrizados por perfil; indicadores operacionais macro, sem dashboard executivo adicional.

## 4. Escopo do projeto (trabalho a realizar)

Atividades para entregar o produto acima, conforme objeto da contratação (seção 5.1) e marcos comerciais (seção 9):

1. Descoberta e desenho funcional  
2. UX/UI e protótipo da experiência principal  
3. Desenvolvimento (Entrega funcional 1 e Entrega funcional 2)  
4. Testes internos e apoio à homologação integrada  
5. Carga inicial essencial  
6. Treinamento de usuários-chave  
7. Go-live assistido em 03/03/2027  
8. Estabilização inicial e correções no período de garantia  

O projeto é **temporário** (Aula 02): encerra-se com aceite do go-live e término da garantia contratual de 30 dias. **Sustentação mensal, operação 24x7 e evoluções** após esse período são operação contínua ou novos projetos, não parte deste escopo de projeto.

## 5. Fora do escopo e zona cinzenta

### 5.1 Exclusões comerciais (seção 5.5)

- Aquisição de licenças de terceiros, serviços de mensageria, WhatsApp Business/API, certificados ou meios de pagamento (custos com o cliente).  
- Infraestrutura cloud, sustentação mensal e operação 24x7 após estabilização.  
- Integrações não descritas expressamente na proposta técnica.  
- Faturamento TISS, autorização de convênios e integração direta com operadoras.  
- Telemedicina, videochamada e gravação de consultas.  
- Aplicativo mobile nativo iOS/Android.  
- Saneamento extensivo de base histórica ou digitação manual de dados em larga escala.  
- Customizações após aprovação do escopo detalhado, salvo gestão formal de mudanças.  

### 5.2 Fronteiras do Anexo B (coluna “Não caracterizado / depende de validação”)

Registrado como **fora** ou **adiado** para o primeiro go-live:

| Tema | Decisão para 03/03/2027 |
|---|---|
| Profundidade de histórico clínico e deduplicação ampla | **Fora** — apenas carga essencial e histórico de agendamentos no layout acordado. |
| Regras específicas por especialidade/profissional além do parametrizado | **Dentro com limite** — bloqueio, duração e encaixe por permissão; exceções novas via CR. |
| Reagendamento autônomo pelo paciente | **Depois / CR** — remarcação pela equipe permanece dentro. |
| Pagamento no portal | **Fora** (seção 5.5 e nota 16/09). |
| Conteúdo clínico detalhado e prontuário completo | **Fora**. |
| Fornecedor/canal WhatsApp e custos transacionais | **Depois / CR** até contratação formal (P-03). |
| Cobrança online, conciliação e contas a receber | **Fora**. |
| Migração ampla de histórico e saneamento | **Fora**. |
| Dashboard executivo além dos indicadores macro | **Depois / CR**. |

### 5.3 Zona cinzenta — decisões do grupo (rastreio)

Identificadores estáveis para backlog, roadmap e riscos (Aula 15 — coerência entre artefatos):

| ID | Item | Origem | Decisão | Justificativa |
|---|---|---|---|---|
| Z-01 | Confirmação por WhatsApp | nota 01/09; P-03 | **Depois / CR** | Canal e custo são do cliente; WhatsApp na seção 5.5. Baseline: e-mail. |
| Z-02 | Reagendamento pelo próprio paciente | nota 25/08; P-06 | **Depois / CR** | Regra não fechada; portal no contrato cobre cancelamento conforme política aprovada. |
| Z-03 | Encaixe e bloqueio por médico | nota 03/09 | **Dentro** | Parametrização por permissão no módulo Agenda; detalhes excepcionais via CR. |
| Z-04 | Pagamento antecipado no portal | nota 16/09 | **Fora** | Exclusão comercial e Anexo B. |
| Z-05 | Anos de histórico de pacientes | nota 14/09; P-02 | **Fora** (amplo) | Carga essencial sim; saneamento extenso e profundidade histórica fora. |
| Z-06 | Unidade Indaiatuba ativa no go-live | seções 3 e 10 | **Fora** (operação) | Cadastro da unidade pode existir; sem agenda, carga, treinamento e operação em 03/03/2027. |
| Z-07 | Dashboard executivo além dos indicadores macro | nota 08/09 | **Depois / CR** | Indicadores macro e exportação dentro (Gestão). |

Mudanças que alterem esta fronteira seguem o [Fluxo de Mudanças (artefato 10)](pessoa_4/Fluxo de Mudança.md): solicitar, analisar impacto, decidir formalmente e atualizar artefatos.

## 6. Premissas

Premissas derivadas das pendências P-01 a P-08 (seção 11). Cada linha regista dono do lado **Vida+**, data-limite para o planejamento e impacto se não se confirmar (base para Matriz de Riscos da Pessoa 4).

| ID | Estamos planejando considerando que… | Dono (cliente) | Data-limite | Se não se confirmar |
|---|---|---|---|---|
| P-01 | a documentação técnica, credenciais e ambiente de teste da API do **VidaFin** estarão disponíveis para homologação. | Marcelo Viana | 16/12/2026 | Integração não entra na linha de base; go-live sem promessa de faturamento automático até nova decisão. |
| P-02 | o cliente entrega **amostra e layout** da base de pacientes compatíveis com a carga inicial acordada. | Paula Ribeiro (exportação com Marcelo Viana / TI) | 16/12/2026 | Carga inicial essencial sai da linha de base ou reduz escopo validável. |
| P-03 | o **canal de mensageria** em produção, fornecedor e responsável pelos custos estão definidos. | Juliana Reis (com Marcelo Viana) | 16/12/2026 | Entrega 2 valida notificações por **e-mail**; WhatsApp permanece fora (Z-01). |
| P-04 | a **lista final de perfis e usuários-chave** para homologação está aprovada. | Paula Ribeiro | 09/12/2026 | Desenho de acessos e cenários de teste não fecha; risco de retrabalho em segurança. |
| P-05 | a **disponibilidade da Dra. Helena Moraes** para validações clínicas está formalizada. | Ricardo Salles | 02/12/2026 | GP escala ao sponsor; validações clínicas não podem atrasar o cronograma em silêncio. |
| P-06 | a **política de cancelamento** e as regras de **remarcação pela equipe** estão escritas e aceitas. | Dra. Helena Moraes (validação operacional: Paula Ribeiro) | 16/12/2026 | Portal só implementa cancelamento já aprovado; reagendamento autônomo do paciente não entra (Z-02). |
| P-07 | os **dados de salas e recursos por unidade** estão na planilha padronizada. | Paula Ribeiro | 16/12/2026 | Configuração da agenda da Entrega 1 não cobre as quatro unidades em cenário real. |
| P-08 | a Vida+ **indica formalmente** o responsável pelo tratamento de dados/LGPD (Ricardo providencia a indicação, não sendo ele o encarregado por presunção). | Ricardo Salles | 02/12/2026 | Sem validação de acesso, retenção e uso de dados reais em homologação/aceite. |

## 7. Restrições

Limites do projeto classificados conforme Aula 07. Alteração de escopo macro, prazo ou custo exige negociação na **tripla restrição** (Aula 02).

### 7.1 Prazo

- Kick-off: **26/11/2026**.  
- Primeira operação produtiva: **03/03/2027** (14 semanas comerciais, marcos da seção 9).  
- Ordem de Serviço: até **100 dias corridos**, observadas dependências da Contratante.  
- Homologação: até **5 dias úteis** após cada disponibilização para aceite ou inconformidade fundamentada; **aceite tácito** se não houver manifestação no prazo (seção 7.4).  
- Garantia: **30 dias corridos** após aceite do go-live, apenas para **defeitos** do escopo entregue.  

### 7.2 Orçamento

- Receita comercial do projeto: **R$ 248.000,00** (preço vendido ao cliente).  
- Teto interno de custo direto de equipe: **R$ 158.000,00** (seção 8.2).  
- Margem bruta-alvo antes de overhead: **R$ 90.000,00**.  
- Reserva gerencial explicitamente separada: **não informada** no handoff.  
- Custos de cloud, mensageria, licenças, certificados e meios de pagamento: **responsabilidade da Vida+**.  

### 7.3 Tecnologia

- Aplicação **web responsiva** (seções 6.1 e 6.4).  
- Compatibilidade-alvo: versões atuais de **Chrome** e **Edge** em desktops corporativos e navegadores móveis modernos.  
- Ambientes separados: desenvolvimento, homologação e produção (cliente provê condições de produção conforme contrato).  

### 7.4 Recursos

- Equipe fixa da seção 8 (Camila, Bruno, Lívia, Rafael, Diego, Natália, Igor), sem profissional adicional reservado para picos.  
- Atividades previstas **prioritariamente remotas**; deslocamentos presenciais só com aprovação prévia (seção 5.3).  

### 7.5 Políticas e contrato

- Escopo macro **fechado**; evoluções e itens adiados (Z-01, Z-02, Z-07) entram por **Change Request**.  
- Notas informais da negociação (seção 4) **não** são compromisso isolado.  
- Melhorias e novas funcionalidades **não** são cobertas pela garantia.  

## 8. Coerência com os demais artefatos

- **Pessoa 3:** escopo do projeto e marcos alimentam cronograma e custos; premissas com data alimentam dependências do cliente.  
- **Pessoa 4:** premissas P-01 a P-08 e decisões Z-01 a Z-07 alimentam riscos, qualidade e go-live.  
- **Pessoa 1:** validações de regras clínicas e operacionais (Dra. Helena, Paula) ligam-se a P-05 e P-06.  
- **08 Backlog** ([08 Product Backlog](08%20Product%20Backlog.md)) / **09 Roadmap:** apenas itens **dentro** e habilitadores; lista “Depois / CR” com Z-01, Z-02 e Z-07.  

## 9. Pendências para validação do grupo

- Confirmar este rascunho na reunião e alinhar com [Decisão 2](planejamento/00-reuniao-de-decisoes.md) preenchida.  
- Decisão 1 (abordagem híbrida) permanece para confirmação formal na reunião.  
- Revisão cruzada após publicação do backlog: cada funcionalidade do go-live deve aparecer em Escopo → Backlog → Roadmap → Cronograma → Riscos.