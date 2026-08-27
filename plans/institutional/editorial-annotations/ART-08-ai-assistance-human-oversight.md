# ART-08 — AI assistance under human oversight

Status: Annotated source material — not approved copy

This file preserves the editorial annotation for AI assistance under human oversight. It is an input to
claims review and bounded rewriting, not a publication-ready manuscript.

## Theme

Bounded AI and human authority

## Intended conceptual direction

Explain bounded tasks, human-in-the-loop approval, human-on-the-loop supervision, and final human responsibility.

## Claims requiring reclassification or removal

Confidence scores, policy interceptors, autonomous critical actions, kill switches, rollback, and live anomaly response are proposals/future work, not existing controls.

## Annotated thread directions

Recommendation-and-approval flow; supervision and intervention flow.

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

Abaixo está a proposta de redação e estrutura para o **Artigo 8 — AI Assistance Under Human Oversight**, encerrando a série conceitual com foco no equilíbrio entre automação inteligente e controle humano soberano.

---

# Artigo 8 — AI Assistance Under Human Oversight

## 1. Assistência de IA e Tarefas Delimitadas

No ecossistema Axodus, os modelos de Inteligência Artificial não operam como agentes totalmente autônomos sem amarras, mas sim sob o paradigma da **Assistência de IA em Tarefas Delimitadas (*Bounded AI Assistance*)**. A IA é projetada como uma ferramenta de amplificação de capacidade e eficiência, operando estritamente dentro de domínios funcionais claros e pré-aprovados.

Os pilares da delimitação funcional incluem:

* **Escopo Estrito de Atuação (*Bounded Scope*):** A IA só executa tarefas para as quais possui permissão explícita de domínio (ex.: análise preditiva de fraude, otimização de consultas de banco de dados, geração de rascunhos de relatórios ou triagem de chamados).
* **Ausência de Autonomia Decisória Crítica:** O sistema de IA é impedido de realizar mutações imutáveis de estado, transferências financeiras de grande porte ou alterações na infraestrutura sem a passagem por um ponto de controle humano.
* **Saídas Determinísticas e Auditáveis:** Toda recomendação ou código gerado por IA é acompanhado do grau de confiança (*confidence score*) e da justificativa explicável de suas saídas.

---

## 2. Autoridade Humana (*Human-in-the-Loop & Human-on-the-Loop*)

A **Autoridade Humana** é a garantia constitucional e operacional de que o controle final do ecossistema permanece, inegociavelmente, sob supervisão e responsabilidade de operadores, desenvolvedores e auditores humanos.

```
+-----------------------------------------------------------------------+
|                         AGENTE / ASSISTENTE DE IA                     |
|         (Processamento de Dados | Geração de Recomendações)           |
+-----------------------------------------------------------------------+
                                   |
                                   v
+-----------------------------------------------------------------------+
|                    GARGALO DE AUTORIZAÇÃO / LIMITES                   |
|          (Gatilhos de Risco | Interceptação de Ações Críticas)        |
+-----------------------------------------------------------------------+
                                   |
                  +----------------+----------------+
                  |                                 |
                  v                                 v
+-----------------------------------+ +---------------------------------+
|       HUMAN-IN-THE-LOOP           | |       HUMAN-ON-THE-LOOP         |
|  (Aprovação Prévia Mandatória)    | | (Monitoramento Contínuo & Stop) |
+-----------------------------------+ +---------------------------------+

```

### Princípios da Autoridade Humana:

* **Aprovação Prévia (*Human-in-the-Loop*):** Para decisões de alto impacto (alterações de política, autorizações financeiras relevantes, novos *deploys*), a IA atua apenas como conselheira. O ato executivo exige obrigatoriamente a assinatura digital de um humano responsável.
* **Supervisão em Tempo Real (*Human-on-the-Loop*):** Em tarefas automatizadas repetitivas de baixo risco, a IA pode agir autonomamente, mas o operador humano possui painéis de observabilidade e mecanismos de interrupção instantânea (*Kill Switches*) para assumir o controle a qualquer momento.
* **Atribuição Final de Responsabilidade:** Um assistente de IA nunca responde legal ou constitucionalmente por uma falha. A responsabilidade é sempre mapeada até o humano que aprovou a ação ou que falhou em supervisioná-la dentro dos limites estabelecidos.

---

## 3. Duas Threads

Para detalhar a dinâmica de interação entre a assistência de IA e a supervisão humana, definem-se duas **threads funcionais**:

---

### Thread 1: O Fluxo de Análise, Sugestão e Aprovação (Human-in-the-Loop)

Esta thread ilustra o ciclo operacional em que um assistente de IA apoia a tomada de decisão humana em um processo de alto impacto.

1. **Geração de Análise pela IA:** O assistente de IA varre o ambiente operando no Núcleo de Dados, identifica um risco de sobrecarga na infraestrutura e elabora um plano de otimização de recursos.
2. **Construção do Artefato de Sugestão:** Em vez de aplicar as mudanças diretamente, a IA gera um relatório detalhado contendo a alteração proposta, o nível de confiança, os riscos associados e a estimativa de custo.
3. **Revisão e Validação Humana:** O operador recebe a notificação no painel de governança, analisa os artefatos de justificativa apresentados pela IA e pode aceitar, modificar ou rejeitar a recomendação.
4. **Execução Autenticada:** Somente após o clique de aprovação e a verificação de identidade do operador humano, a **Plataforma de Operações** aplica a mudança sugerida na **Fundação**.

> **Pontos de Contato Chave:** `IA (Análise de Dados)` ➔ `Geração de Recomendação Explicável` ➔ `Revisão e Aprovação Humana` ➔ `Execução na Infraestrutura`.

---

### Thread 2: O Monitoramento e Intervenção de Emergência (Human-on-the-Loop)

Esta thread descreve o processo de monitoramento contínuo em que um operador humano intervém no comportamento de agentes de IA operando em escala.

1. **Execução Autônoma Delimitada:** Um conjunto de agentes de IA realiza a triagem automática de requisições de baixo risco, dentro de parâmetros rígidos definidos na política de governança.
2. **Detecção de Anomalia pela Observabilidade:** Durante a execução, a **Plataforma de Observabilidade** identifica que a taxa de decisões do agente começou a divergir do padrão esperado, aproximando-se de um limite de risco.
3. **Alerta e Intervenção Humana:** O operador de supervisão é alertado em tempo real e avalia o comportamento anômalo da IA no painel de controle.
4. **Acionamento do Circuit Breaker:** O operador dispara o comando de *override* humano, pausando o agente de IA e revertendo as operações recentes para um estado seguro até que o modelo seja reavaliado e corrigido.

> **Pontos de Contato Chave:** `Execução Autônoma de IA` ➔ `Monitoramento de Observabilidade` ➔ `Identificação de Anomalia pelo Humano` ➔ `Acionamento do Circuit Breaker / Retratação`.
