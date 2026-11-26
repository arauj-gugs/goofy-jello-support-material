# 03 — Matriz RACI

**Projeto:** Vida+ — Sistema de Gestão e Agendamento de Clínica  
**Responsável pelo artefato:** Jenifer Gomes (Pessoa 1 — Pessoas e governança)  
**Status:** Versão para validação na reunião do grupo (A\* = autoridade provisória até confirmação Vida+)

## 1. Objetivo

Definir as responsabilidades de execução, aprovação, consulta e
comunicação nas principais atividades do projeto Vida+, utilizando as
pessoas identificadas no handoff Comercial → Projetos, no documento de
identificação dos stakeholders e na equipe disponibilizada pela Goofy
Jello.

A matriz contempla as atividades solicitadas para a etapa de
planejamento e governança. As atribuições foram construídas a partir das
responsabilidades das seções 7.2 e 7.3, das pessoas e funções da seção 8
e dos stakeholders da seção 10.1.

A **Decisão 3** e o **Fluxo de Mudanças** (Pessoa 4) já estão publicados e orientam o mapeamento Scrum e a linha “Aprovação de mudança”. Pendências de formalização (GP, sponsor, LGPD) permanecem na seção 7.

## 2. Legenda e critérios

  -----------------------------------------------------------------------
  Sigla                   Significado             Aplicação
  ----------------------- ----------------------- -----------------------
  **R**                   Responsável pela        Pessoa que executa ou
                          execução                conduz diretamente o
                                                  trabalho. Pode haver
                                                  mais de um R por
                                                  atividade.

  **A**                   Aprovador / responsável Pessoa que responde
                          final                   pela aprovação ou pelo
                                                  resultado final da
                                                  atividade. Deve existir
                                                  exatamente um A em cada
                                                  linha.

  **C**                   Consultado              Pessoa que fornece
                                                  informações,
                                                  conhecimento
                                                  especializado ou
                                                  validação durante a
                                                  atividade.

  **I**                   Informado               Pessoa que recebe
                                                  informações sobre
                                                  andamento, decisões ou
                                                  resultados.

  **---**                 Sem participação direta Não há participação
                          prevista                direta atribuída à
                                                  pessoa naquela
                                                  atividade.
  -----------------------------------------------------------------------

**Regras adotadas:**

-   Cada atividade possui exatamente um **A**.
-   As pessoas das colunas são nomes identificados nos materiais
    fornecidos.
-   A Goofy Jello responde pelo planejamento, análise, desenvolvimento,
    testes internos, implantação e apoio à homologação.
-   A Vida+ responde pela disponibilização de regras, cadastros, dados,
    acessos e documentação de sistemas externos, participação nas
    reuniões e homologação funcional.
-   Atribuições específicas que não estejam formalizadas foram propostas
    conforme a função de cada pessoa e estão identificadas nas
    justificativas e pendências.
-   Não foram criados nomes para fornecedores, representantes das
    unidades ou responsáveis ainda não identificados.

## 3. Pessoas consideradas

  --------------------------------------------------------------------------
  Pessoa                  Organização / função       Participação
                          identificada               considerada
  ----------------------- -------------------------- -----------------------
  Ricardo Salles          Vida+ --- Diretor          Decisões executivas,
                          Administrativo / Sponsor   desbloqueios e
                                                     representação do
                                                     cliente.

  Dra. Helena Moraes      Vida+ --- Diretora Médica  Regras clínicas, agenda
                                                     e fluxo médico.

  Paula Ribeiro           Vida+ --- Coordenadora de  Requisitos e validações
                          Recepção / usuária-chave   operacionais, encaixes
                                                     e check-in.

  Marcelo Viana           Vida+ --- Coordenador de   Integrações, segurança,
                          TI / ponto focal técnico   acessos e dependências
                                                     técnicas.

  Fernanda Lopes          Vida+ --- Financeiro       Eventos financeiros e
                                                     validação da integração
                                                     VidaFin.

  Juliana Reis            Vida+ ---                  Comunicação com
                          Marketing/Relacionamento   pacientes, templates e
                                                     mensagens.

  Camila Rocha            Goofy Jello --- Gerente de Coordenação e
                          Projetos Sênior            acompanhamento do
                                                     projeto; designação
                                                     formal ainda a
                                                     confirmar.

  Bruno Ferraz            Goofy Jello --- Analista   Levantamento, análise e
                          de Negócios Pleno          documentação de
                                                     requisitos.

  Lívia Monteiro          Goofy Jello --- UX/UI      Jornadas, interfaces e
                          Designer Pleno             protótipos.

  Rafael Nunes            Goofy Jello ---            Desenvolvimento backend
                          Desenvolvedor Backend      e integrações.
                          Sênior                     

  Diego Prado             Goofy Jello ---            Desenvolvimento das
                          Desenvolvedor Full Stack   funcionalidades.
                          Pleno                      

  Natália Campos          Goofy Jello --- QA/Testes  Planejamento e execução
                          Pleno                      de testes, registro de
                                                     defeitos e evidências.

  Igor Mendes             Goofy Jello ---            Ambientes,
                          DevOps/Cloud Sênior        infraestrutura,
                                                     implantação e operação
                                                     técnica.

  Henrique Tavares        Goofy Jello --- Pré-vendas Esclarecimentos sobre
                          / Solution Consultant      premissas e informações
                                                     da negociação. Não é
                                                     considerado gerente
                                                     formal sem confirmação.

  Marina Couto            Goofy Jello --- Executiva  Esclarecimentos sobre
                          Comercial                  proposta, condições e
                                                     compromissos
                                                     comerciais.
  --------------------------------------------------------------------------

## 4. Matriz RACI

As atividades aparecem na ordem solicitada. A matriz utiliza todas as
pessoas nomeadas nos materiais como possíveis participantes; a ausência
de uma letra significa que não há participação direta prevista naquela
atividade.

  ------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Atividade           Ricardo     Dra.     Paula   Marcelo   Fernanda   Juliana   Camila    Bruno      Lívia   Rafael   Diego   Natália     Igor   Henrique   Marina
                       Salles   Helena   Ribeiro     Viana      Lopes      Reis    Rocha   Ferraz   Monteiro    Nunes   Prado    Campos   Mendes    Tavares    Couto
                                Moraes                                                                                                                      
  ----------------- --------- -------- --------- --------- ---------- --------- -------- -------- ---------- -------- ------- --------- -------- ---------- --------
  Descoberta                I        C         C         C          C         C        A        R          C        C       C         I        I          C        I

  Desenho funcional         I        C         A         C          C         C        I        R          C        C       C         C        I          I        I

  Protótipo                 I        C         A         C          I         C        I        C          R        I       I         C        I          I        I

  Desenvolvimento           I        C         C         C          C         I        A        C          C        R       R         C        R          I        I

  Testes internos           I        I         C         C          C         I        A        C          C        R       R         R        C          I        I

  Homologação             A\*        C         R         C          R         C        C        C          C        I       I         C        I          I        I

  Carga de dados            I        I         C       A\*          I         I        C        C          I        R       R         C        C          I        I

  Integração                I        I         I       A\*          R         I        C        C          I        R       C         R        C          I        I
  VidaFin                                                                                                                                                   

  Treinamento               I        C         A         C          C         C        C        R          C        I       I         C        I          I        I

  Go-live                 A\*        C         R         R          C         I        R        I          I        R       R         R        R          I        I

  Aprovação de            A\*        C         C         C          C         C        R        C          C        C       C         C        C          I        I
  mudança                                                                                                                                                   

  Aceite de entrega       A\*        C         R         C          C         C        R        I          I        I       I         C        I          I        I
  ------------------------------------------------------------------------------------------------------------------------------------------------------------------

\*\*Atenção aos A marcados com asterisco (\*):\*\* são atribuições
provisórias de planejamento, utilizadas para manter um único A em cada
linha nesta versão. Não substituem uma aprovação formal nem resolvem
pendências de governança. Os motivos e as confirmações necessárias estão
detalhados na seção 6.

## 5. Justificativa das atribuições

### 5.1. Descoberta

-   **A --- Camila Rocha:** coordena a atividade de planejamento e
    organização do trabalho pela Goofy Jello, conforme sua função de
    Gerente de Projetos Sênior. A designação formal ainda precisa ser
    confirmada pela Diretoria de Operações.
-   **R --- Bruno Ferraz:** conduz o levantamento, a análise e a
    documentação de requisitos e regras de negócio.
-   **C --- Paula Ribeiro, Dra. Helena Moraes, Marcelo Viana, Fernanda
    Lopes e Juliana Reis:** fornecem informações operacionais, clínicas,
    técnicas, financeiras e de relacionamento.
-   **C --- Henrique Tavares:** pode esclarecer premissas e informações
    transmitidas durante a passagem de bastão Comercial → Projetos.
-   **I --- Ricardo Salles, Natália Campos e Igor Mendes:** recebem
    informações sobre a atividade e seus resultados.

### 5.2. Desenho funcional

-   **A --- Paula Ribeiro:** representa a operação de recepção e valida
    a aderência dos fluxos às necessidades operacionais, como
    usuária-chave.
-   **R --- Bruno Ferraz:** consolida os requisitos e documenta o
    desenho funcional.
-   **C --- Dra. Helena Moraes, Marcelo Viana, Fernanda Lopes, Juliana
    Reis e Lívia Monteiro:** contribuem com regras clínicas, restrições
    técnicas, processos financeiros, comunicação e experiência do
    usuário.
-   **I --- Ricardo Salles, Camila Rocha, Natália Campos, Igor Mendes,
    Henrique Tavares e Marina Couto:** recebem as informações
    pertinentes ao desenho.

### 5.3. Protótipo

-   **A --- Paula Ribeiro:** valida se os fluxos e as telas representam
    as necessidades da operação.
-   **R --- Lívia Monteiro:** desenvolve os protótipos e conduz as
    definições de UX/UI.
-   **C --- Dra. Helena Moraes, Marcelo Viana, Bruno Ferraz, Juliana
    Reis e Natália Campos:** contribuem com regras clínicas, restrições
    técnicas, requisitos, comunicação e critérios de teste.

### 5.4. Desenvolvimento

-   **A --- Camila Rocha:** responde pela coordenação da entrega de
    desenvolvimento pela Goofy Jello, de forma provisória até a
    confirmação da gerência do projeto.
-   **R --- Rafael Nunes e Diego Prado:** implementam as funcionalidades
    conforme suas funções de desenvolvimento backend e full stack.
-   **R --- Igor Mendes:** executa as atividades de DevOps/Cloud
    necessárias aos ambientes e à operação técnica.
-   **C --- Bruno Ferraz, Lívia Monteiro, Dra. Helena Moraes, Paula
    Ribeiro, Marcelo Viana e Fernanda Lopes:** apoiam com requisitos,
    experiência, regras de negócio e dependências do cliente.

### 5.5. Testes internos

-   **A --- Camila Rocha:** responde pela coordenação da conclusão dos
    testes internos antes da disponibilização da versão para
    homologação.
-   **R --- Natália Campos:** planeja e executa os testes, registra
    defeitos e mantém evidências.
-   **R --- Rafael Nunes e Diego Prado:** apoiam a reprodução e a
    correção de defeitos nas funcionalidades desenvolvidas.
-   **C --- Bruno Ferraz, Lívia Monteiro, Marcelo Viana e Fernanda
    Lopes:** apoiam a análise de requisitos, experiência, dependências
    técnicas e regras financeiras.

### 5.6. Homologação

-   **A --- Ricardo Salles (provisório):** indicado nesta versão como
    responsável final do cliente pela aprovação executiva da
    homologação. A autoridade de aceite por tipo de entrega ainda
    precisa ser formalizada pela Vida+.
-   **R --- Paula Ribeiro:** participa da homologação dos processos
    operacionais de recepção.
-   **R --- Fernanda Lopes:** participa da validação funcional dos
    eventos financeiros e da integração VidaFin.
-   **C --- Dra. Helena Moraes:** valida regras e fluxos clínicos.
-   **C --- Marcelo Viana:** apoia a verificação técnica e as
    dependências de TI.
-   **C --- Camila Rocha, Bruno Ferraz, Lívia Monteiro e Natália
    Campos:** apoiam o acompanhamento, os esclarecimentos funcionais, a
    experiência e o registro das ocorrências.
-   A homologação funcional é executada pela Vida+, conforme a seção
    7.3. A Goofy Jello disponibiliza versões e presta apoio, conforme a
    seção 7.2.

### 5.7. Carga de dados

-   **A --- Marcelo Viana (provisório):** indicado como responsável pela
    coordenação técnica do lado da Vida+, por ser o ponto focal de TI. A
    aprovação da qualidade e da completude da base ainda precisa ser
    confirmada.
-   **R --- Rafael Nunes e Diego Prado:** executam as atividades
    técnicas de carga e tratamento dos dados.
-   **C --- Paula Ribeiro:** apoia a conferência dos dados relacionados
    à operação.
-   **C --- Bruno Ferraz:** apoia a validação das regras e dos
    requisitos de dados.
-   **C --- Natália Campos e Igor Mendes:** apoiam testes, ambiente e
    condições técnicas.

### 5.8. Integração VidaFin

-   **A --- Marcelo Viana (provisório):** indicado como responsável pela
    coordenação técnica da integração pelo lado da Vida+, como ponto
    focal de TI. A autoridade final de aprovação técnica precisa ser
    confirmada.
-   **R --- Rafael Nunes:** conduz a implementação backend da
    integração.
-   **R --- Fernanda Lopes:** valida os eventos e resultados
    financeiros.
-   **R --- Natália Campos:** executa testes e registra resultados.
-   **C --- Bruno Ferraz, Camila Rocha, Diego Prado e Igor Mendes:**
    apoiam requisitos, coordenação, implementação complementar e
    ambiente.
-   O fornecedor do VidaFin não foi identificado nos materiais e, por
    isso, não foi incluído como pessoa na matriz.

### 5.9. Treinamento

-   **A --- Paula Ribeiro:** responde pela validação da preparação
    operacional da recepção, como usuária-chave.
-   **R --- Bruno Ferraz:** conduz a orientação funcional e a
    transferência de conhecimento sobre os processos e requisitos.
-   **C --- Dra. Helena Moraes, Marcelo Viana, Fernanda Lopes, Juliana
    Reis, Lívia Monteiro, Camila Rocha e Natália Campos:** contribuem
    conforme os processos clínicos, técnicos, financeiros, comunicação,
    usabilidade, coordenação e dúvidas de testes.
-   Os representantes das equipes de recepção das quatro unidades ainda
    precisam ser confirmados.

### 5.10. Go-live

-   **A --- Ricardo Salles (provisório):** indicado como responsável
    pela autorização executiva da entrada em operação pelo cliente. A
    governança da Vida+ deve confirmar formalmente essa autoridade.
-   **R --- Camila Rocha:** coordena a implantação e a preparação da
    entrada em produção, sujeita à confirmação de sua designação como
    Gerente de Projetos.
-   **R --- Marcelo Viana:** coordena as condições técnicas, os acessos
    e as dependências pelo lado da Vida+.
-   **R --- Paula Ribeiro:** acompanha a preparação operacional.
-   **R --- Rafael Nunes, Diego Prado, Natália Campos e Igor Mendes:**
    apoiam implantação, correções, testes finais, ambiente e operação
    técnica.
-   **C --- Dra. Helena Moraes e Fernanda Lopes:** validam a prontidão
    dos processos clínicos e financeiros.

### 5.11. Aprovação de mudança

-   **A --- Ricardo Salles (provisório):** utilizado somente para manter
    a matriz preenchida enquanto o Fluxo de Mudanças da Pessoa 4 não foi
    publicado. **Não é possível confirmar que Ricardo seja o aprovador
    correto sem consultar esse fluxo.**
-   **R --- Camila Rocha:** recebe e registra a solicitação, coordena a
    análise de impacto e acompanha a decisão.
-   **C --- Bruno Ferraz, Lívia Monteiro, Rafael Nunes, Diego Prado,
    Natália Campos e Igor Mendes:** avaliam impactos funcionais, de
    experiência, técnicos, de qualidade e infraestrutura.
-   **C --- Paula Ribeiro, Dra. Helena Moraes, Marcelo Viana, Fernanda
    Lopes e Juliana Reis:** são consultados conforme a área afetada.
-   **I --- Henrique Tavares e Marina Couto:** podem receber informação
    ou ser acionados para esclarecer premissas da negociação e
    compromissos comerciais.
-   **Regra obrigatória:** assim que o Fluxo de Mudanças for publicado,
    o A desta linha deverá ser ajustado para corresponder exatamente à
    autoridade de aprovação definida nele. A matriz não deve manter um
    aprovador diferente do fluxo.

### 5.12. Aceite de entrega

-   **A --- Ricardo Salles (provisório):** representa a aprovação final
    do cliente nesta versão. A Vida+ precisa confirmar se o aceite será
    centralizado no sponsor ou delegado por tipo de entrega.
-   **R --- Paula Ribeiro:** coordena a validação operacional e
    consolida as evidências da área usuária.
-   **R --- Camila Rocha:** organiza a disponibilização da entrega,
    acompanha o prazo de validação e registra o resultado junto à equipe
    do projeto.
-   **C --- Dra. Helena Moraes, Marcelo Viana, Fernanda Lopes e Natália
    Campos:** participam das validações clínicas, técnicas, financeiras
    e de qualidade.
-   O aceite de entrega não se confunde com os testes internos. A Vida+
    executa a homologação funcional e registra evidências de aceite ou
    rejeição, conforme a seção 7.3.

## 6. Mapeamento dos papéis Scrum

Papéis Scrum (Aula 20) mapeados em pessoas do handoff, **sem organograma paralelo**, conforme [Decisão 3](../planejamento/00-reuniao-de-decisoes.md) registrada na reunião do grupo.

| Papel Scrum | Pessoa(s) | Papel no Vida+ / na Decisão 3 |
|---|---|---|
| **Product Owner** (prioridade do backlog — lado Goofy Jello) | **Bruno Ferraz** | Prioriza e refina o backlog no dia a dia; **valida** com **Paula Ribeiro** (aceite operacional da recepção) e **Dra. Helena Moraes** (regras clínicas de agenda). Paula e a Dra. Helena **não** substituem Bruno como PO contratado — são consultas obrigatórias para decisões de produto. |
| **Scrum Master** (facilitação e impedimentos) | **Camila Rocha** | GP sênior: condução do projeto, integração dos planos, cadência e escalonamento. Designação formal pela Diretoria de Operações ainda a confirmar no cliente (ver P-RACI-03). |
| **Developers** | **Lívia Monteiro**, **Rafael Nunes**, **Diego Prado**, **Natália Campos**, **Igor Mendes** (e **Bruno** na frente de negócio quando não está na priorização) | Construção multidisciplinar alinhada ao [cronograma](../pessoa_3/04%20Cronograma.md) e [backlog](../pessoa_2/08%20Product%20Backlog.md). |

**Governança além do Scrum (Decisão 3):** trade-off executivo (prazo, escopo grande, custo) → **Ricardo Salles**; acessos/API/ambiente → **Marcelo Viana**; VidaFin → **Fernanda Lopes + Marcelo**; templates de mensagem → **Juliana Reis**.

**Aprovação de mudança (coerência com artefato 10):** na linha “Aprovação de mudança” desta matriz, **Ricardo Salles** permanece **A\*** (autoridade de trade-off / baseline contratual). **Camila Rocha** é **R** (registro, coordenação da análise de impacto). O [Fluxo de Mudanças](../pessoa_4/Fluxo%20de%20Mudança.md) usa o mesmo par — não há aprovador alternativo por nível de impacto até a Vida+ formalizar delegação.

Henrique Tavares e Marina Couto permanecem como contatos de Pré-vendas e
Comercial para esclarecimentos sobre premissas e compromissos da
passagem de bastão. Não foram adicionados ao Scrum Team, pois as
informações disponíveis não indicam que integrem a equipe de
desenvolvimento do produto.

## 7. Pendências para validação

  -------------------------------------------------------------------------
  ID                Pendência         Impacto na matriz   Ação necessária
  ----------------- ----------------- ------------------- -----------------
  P-RACI-02         Autoridade formal O A de "Aprovação    Ricardo Salles
                    de Ricardo como   de mudança" está    ratifica com a
                    aprovador de      alinhado ao Fluxo   Vida+ na
                    mudanças na Vida+ 10; A* indica       mobilização, se
                                      provisório até      necessário.
                                      confirmação do      
                                      sponsor.            

  P-RACI-03         Gerente de        A coordenação       Formalizar a
                    Projetos          atribuída a Camila  designação pela
                    formalmente       e seu mapeamento    Diretoria de
                    designado ainda   como Scrum Master   Operações e
                    não confirmado    são provisórios. O  atualizar a
                                      handoff menciona    matriz.
                                      Henrique, mas       
                                      também registra que 
                                      a designação        
                                      depende da          
                                      Diretoria de        
                                      Operações.          

  P-RACI-04         Autoridade de     Ricardo foi         Confirmar se o
                    aceite por tipo   indicado            sponsor
                    de entrega não    provisoriamente     centraliza o
                    formalizada       como A em           aceite ou se
                                      homologação,        haverá
                                      go-live e aceite.   aprovadores
                                                          delegados por
                                                          área ou tipo de
                                                          entrega.

  P-RACI-05         Alocação efetiva  As horas semanais   Confirmar a
                    da equipe não     da seção 8 são      disponibilidade e
                    confirmada        capacidades         a distribuição
                                      iniciais, não       das atividades no
                                      alocações           planejamento.
                                      definitivas.        

  P-RACI-06         Fornecedor        Não há contatos     Identificar
                    VidaFin e demais  externos nomeados   fornecedores e
                    terceiros não     para assumir        contatos técnicos
                    identificados     responsabilidades   quando definidos.
                                      na matriz.          

  P-RACI-07         Responsável por   Decisões sobre      Formalizar o
                    dados/LGPD na     dados pessoais,     responsável do
                    Vida+ não         acessos e           lado da Vida+ e
                    designado         privacidade podem   incluí-lo nas
                                      exigir participação atividades
                                      específica.         pertinentes,
                                                          conforme sua
                                                          autoridade.

  P-RACI-08         Responsáveis      Treinamento e       Confirmar
                    locais e          validação           representantes
                    representantes    operacional podem   das unidades,
                    das quatro        exigir participação médicos e equipes
                    unidades não      de pessoas ainda    de recepção.
                    confirmados       não identificadas.  
  -------------------------------------------------------------------------

## 8. Premissas e limitações

-   A matriz utiliza os nomes e funções disponíveis nos materiais
    fornecidos: seções 7.2, 7.3, 8 e 10.1 do handoff e documento de
    identificação e classificação dos stakeholders.
-   As responsabilidades organizacionais seguem o que está descrito no
    handoff: a Goofy Jello conduz planejamento, análise,
    desenvolvimento, testes internos, implantação e apoio à homologação;
    a Vida+ disponibiliza informações e recursos do cliente, participa
    das reuniões e executa a homologação funcional.
-   Atribuições individuais que não estão expressamente formalizadas
    foram propostas com base nas funções e devem ser validadas pelos
    responsáveis.
-   A matriz contém exatamente um A por atividade. Os A marcados com
    asterisco são provisórios e dependem das confirmações indicadas.
-   A capacidade semanal da equipe da Goofy Jello é inicial e precisa
    ser confirmada no planejamento.
-   Fornecedores e representantes não identificados não foram inventados
    nem incluídos como pessoas.
-   A pendência P-08 do documento de stakeholders permanece válida:
    Ricardo Salles deve providenciar a definição do responsável por
    LGPD, mas não foi designado como responsável por LGPD por hora.
-   Decisão 3 e Fluxo de Mudanças (artefato 10) publicados em `main`; revisar apenas se a Vida+ alterar autoridades na mobilização.

## 9. Referências

-   Handoff Comercial → Projetos — Vida+, seções 7.2, 7.3, 8 e 10.1.
-   [Mapa de Stakeholders](Mapa%20de%20Stakeholders%20.md).
-   [Decisão 3 — Quem decide](../planejamento/00-reuniao-de-decisoes.md).
-   [Fluxo de Mudanças](../pessoa_4/Fluxo%20de%20Mudança.md) (Pessoa 4).
-   Aulas 06 e 20 — Governança e papéis Scrum.
