# ART-10 — Academy, BBA, and institutional workflows

Status: Annotated source material — not approved copy

This file preserves the editorial annotation for Academy, BBA, and institutional workflows. It is an input to
claims review and bounded rewriting, not a publication-ready manuscript.

## Theme

Learning, building blocks, institutional process

## Intended conceptual direction

Describe Academy as learning/standards, BBA as modular building blocks, and institutional workflows as proposed review/decision processes.

## Claims requiring reclassification or removal

Do not assert certification, compliance-as-code, production deployment, recertification, or active workflows. Keep BBA expansion explicitly under definition if unresolved.

## Annotated thread directions

Qualification-to-component flow; regulatory-change feedback loop.

## Mandatory transformation

Classify every material statement as fact, design proposal, hypothesis, or
future work. Check the claims register and evidence boundaries. Preserve the
concept only after rewriting it with explicit status and limitations. Do not
infer implementation, adoption, users, partners, performance, security,
revenue, certification, regulatory approval, or production readiness.

## Review record

- Claims worksheet: [../../../plans/institutional/claims-review-worksheet.md](../../../plans/institutional/claims-review-worksheet.md)
- Directive index: [../editorial-annotation-directives.md](../editorial-annotation-directives.md)
- Reviewer: [TBD]
- Decision: [Pending]

## Original context

# Artigo 10 — Academy, BBA and Institutional Workflows

## 1. Funções Conceituais

O encerramento do ecossistema Axodus consolida a ponte entre a capacidade técnica, a validação estrutural e a execução operacional através de três pilares fundamentais:

* **Academy:** O braço de **capacitação, certificação e padronização do conhecimento**. Sua função conceitual é garantir que desenvolvedores, agentes de IA, auditores e parceiros compreendam as diretrizes de arquitetura e governança, transformando o conhecimento teórico em prática alinhada às normas do ecossistema.
* **BBA (*Business & Building Architecture* / *Building Block Architecture*):** A camada de **estruturação de ativos e componentes operacionais**. Atua como o arcabouço modular que traduz requisitos de negócio e especificações de governança em blocos reutilizáveis, padronizados e interoperáveis.
* **Workflows Institucionais (*Institutional Workflows*):** O conjunto de **processos formais e orquestrados de tomada de decisão, auditoria e execução**. Definem os rituais de governança, aprovações humanas, validações de conformidade e fluxos de trabalho que mantêm a integridade institucional do ecossistema.

---

## 2. Relações Entre os Componentes

A interação entre Academy, BBA e Workflows Institucionais cria um ciclo fechado de qualificação, construção e governança diária dentro da plataforma.

```
+-----------------------------------------------------------------------+
|                                ACADEMY                                |
|          (Capacitação, Certificação & Validação do Conhecimento)     |
+-----------------------------------------------------------------------+
                                   |
                                   v Credenciamento & Padrões
+-----------------------------------------------------------------------+
|                                  BBA                                  |
|         (Construção de Bloco Modulares & Ativos do Ecossistema)        |
+-----------------------------------------------------------------------+
                                   |
                                   v Submissão de Artefatos
+-----------------------------------------------------------------------+
|                       WORKFLOWS INSTITUCIONAIS                        |
|        (Aprovação Humana, Execução de Governança & Compliance)        |
+-----------------------------------------------------------------------+

```

### Dinâmica das Relações:

* **Academy ➔ BBA:** A Academy estabelece as diretrizes de código, padrões de segurança e modelos de arquitetura que orientam o desenvolvimento dos componentes no BBA. Um agente ou módulo só pode ser construído sob os padrões BBA se o seu criador (humano ou sistema) possuir a certificação emitida pela Academy.
* **BBA ➔ Workflows Institucionais:** Os blocos de construção desenvolvidos na BBA não entram em execução automaticamente; eles alimentam os Workflows Institucionais como propostas, atualizações de serviços ou novos ativos a serem submetidos às instâncias de aprovação e auditoria.
* **Workflows Institucionais ➔ Academy:** A execução dos workflows institucionais identifica novas necessidades regulatórias, lacunas operacionais ou falhas de conformidade, gerando insumos para atualização contínua do currículo e das certificações da Academy.

---

## 3. Duas Threads

Para ilustrar a operacionalização conjunta desses três elementos, definem-se duas **threads de execução**:

---

### Thread 1: O Ciclo de Habilitação e Implantação de um Bloco de Negócio

Esta thread descreve o percurso que uma nova funcionalidade percorre desde o treinamento inicial até sua entrada em produção.

1. **Certificação na Academy:** Uma equipe de desenvolvimento realiza o programa de capacitação da **Academy**, obtendo as credenciais de conformidade arquitetural e constitucional da plataforma.
2. **Modelagem via BBA:** A equipe utiliza as especificações e *templates* da **BBA** para estruturar um novo módulo de liquidação financeira altamente desacoplado e padronizado.
3. **Ingresso no Workflow Institucional:** O módulo BBA finalizado é submetido como uma proposta de alteração dentro do **Workflow Institucional** de governança.
4. **Validação e Promulgação:** O workflow aciona verificações automáticas de conformidade e a aprovação final do comitê humano, liberando o bloco BBA para implantação no ecossistema operacional.

> **Pontos de Contato Chave:** `Academy (Certificação)` ➔ `BBA (Modelagem de Bloco)` ➔ `Workflow Institucional (Submissão/Aprovação)` ➔ `Deploy em Produção`.

---

### Thread 2: A Auditoria e Atualização de Conformidade por Mudança Regulatória

Esta thread ilustra como uma mudança nas regras do ecossistema reconfigura os processos institucionais, os blocos de construção e o currículo educacional.

1. **Disparo do Workflow Institucional:** Diante de uma nova exigência legal ou regulatória externa, um **Workflow Institucional** de revisão de conformidade é iniciado pela equipe de governança.
2. **Atualização das Especificações na BBA:** A deliberação institucional resulta em novas diretrizes para os componentes BBA, exigindo que todos os blocos de dados incorporem novas travas de privacidade.
3. **Revisão Pedagógica na Academy:** A **Academy** atualiza suas trilhas de aprendizado e simuladores para refletir os novos padrões BBA e os procedimentos do workflow atualizado.
4. **Recertificação de Atores:** Os atores do ecossistema passam pelo processo de recertificação na Academy para manter suas permissões de publicação no BBA ativas.

> **Pontos de Contato Chave:** `Workflow Institucional (Nova Regra)` ➔ `BBA (Ajuste de Padrões)` ➔ `Academy (Atualização de Trilhas)` ➔ `Recertificação Operacional`.
