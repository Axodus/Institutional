# Validação V-01 a V-08 — revisão autoral direcionada

Estado: TARGETED_AUTHORIAL_REVISION_COMPLETE / CRO_REVIEW_PENDING. PASS é verificação do executor no escopo documental, não aceite pelo CRO nem aprovação do autor. Os números à esquerda são da fonte anterior e os números à direita são da candidata.

| Gate | Resultado verificável |
|---|---|
| V-01 PASS | Abstract 25 e §10 629 → 25 e 633: de exemplo ilustrativo e utilidade potencial para contribuição representacional apoiada, hipótese contextual federativa, ausência de diagnóstico exclusivo e desempenho em aberto. §2.4, 84–86 → 84–86 conserva síntese delimitada. Conferido contra assessment E–I e adjudicação I/V. |
| V-02 PASS | §2.4, 84–86 → 84–86 diferencia configuração HAIG, processo revisável e desenho de intervenção, sem presumir incapacidade. §8, 432 → 434–436 e A.4, após 741 → 747 registram equivalência possível de R/C no dossiê federativo. Assessment A, C–E; referências preexistentes e copiada byte a byte a bibliografia. |
| V-03 PASS | §8, após 432 → 436 traz convergência procurement, leitura equivalente em alta cadência, ganho de decomposição sem exclusividade federativa. §8.7 484 → 488 explicita custo não medido e nega que granularidade baste para acurácia/eficiência/valor. Assessment D–G. |
| V-04 PASS | A.3 e linhas da tabela 734–739 → 738–743 preservadas. A.4, após 741 → 747 distingue intervenção provisória, elegibilidade e reconsideração local; admite a mesma leitura por R/C e não confunde decisão de elegibilidade com desfecho da impugnação, término ou remédio da medida. Assessment B–F; adjudicação II. |
| V-05 PASS | §2.5, 88–94 → 88–94 idêntica; §8, após 432 → 434 registra trabalho posterior, casos hipotéticos, um analista informado, sem cegamento/codificação independente, dossiê com interpretações IDE, sem validação de desempenho. §9.5 583 → 587 é prospectiva. Protocolo/dossiê e adjudicação III. |
| V-06 PASS | §3.1, 98–104 → mesmas linhas, intocado. §8.10 506 → 510 distingue validade interna de legitimidade moral, democrática, política e efeitos legais. §1 52 → 52 e §8.2 448 → 452 qualificam influência sem vestígios. |
| V-07 PASS | §6.1–6.4, 274–357 → mesmas linhas, byte a byte. Notação matemática, as três tabelas e hierarquia de títulos conferidas em sequência. Apêndice A.1–A.3 mantido; a inserção de A.4 é posterior aos fatos e à tabela. Nenhum campo, episódio ou construto novo. |
| V-08 PASS | Abstract 25, §8 432 e §10 629 → 25, 434–436 e 633 mantêm distinção hipótese/resultado e negam exclusividade; reconstrução melhor, reprodutibilidade, eficácia e superioridade permanecem não demonstradas. §9.5 conserva hipótese e condição contrária, sem relatar estudo. |

## Evidência de integridade

- O diff foi aplicado em uma cópia temporária do paper.md histórico com git apply --check e git apply; cmp reproduziu a candidata. Aplicação reversa reconstituiu a origem byte a byte. Nenhum staging.
- Preflight e depois do trabalho: git diff no diretório da candidata protegida vazio; fonte e bibliografia igualadas aos blobs do commit 92bd0b900bb4342a0006872271b367f594ef6fc5. Hashes de TeX/PDF históricos preservados. Git main, HEAD b20755af2d9b5968973728cf1c2e5981edda15bf; somente a nova candidata aparece como não rastreada em Institutional.
- SHA-256 da origem: paper.md 41616bffc80b5aa487ea1fae0b49099292fbb3af490dce5f6e860cb098eb28c6; references.bib a7ea77ac1a3d17e9957c4ba216f91f8fb45b79c22bea010654dff13a8fcaa26c; paper.tex 5648f220768e904474ff5d050e955db10f0eab1e85de62d85d3f9787a7f21eee; paper.pdf 82e7d2ecda5c99d3b33db068ff9530b6633e8e9c8cfcdfec9c3cda9640ec9258.
- SHA-256 derivados: paper.md bcc8e639f63d482565a97d692f6d21b8125cbe763ded1012f87e1b1f07735f79; references.bib a7ea77ac1a3d17e9957c4ba216f91f8fb45b79c22bea010654dff13a8fcaa26c; targeted-authorial-revision.diff 2d19d5e47d1ce4896e8c2448e989bd3793d7c2dab8dc95a53a42ec425c008051. O hash deste relatório é externo ao próprio arquivo. As fontes do assessment permanecem com os hashes registrados no registro conceitual.
- Não houve nova pesquisa, nova aplicação comparativa, execução ARS, revisão generalista, avaliação empírica, alteração do IDE, commit, push, contato editorial ou circulação.
