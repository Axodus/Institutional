# Plano de mídia orgânica da Axodus

## Resumo

Construir uma presença editorial consistente e gratuita para explicar a Axodus, seus conceitos e suas plataformas, usando apenas canais próprios ou de publicação aberta. O site permanece como fonte canônica; Medium, Substack e GitHub funcionam como canais de distribuição, discussão e descoberta.

O plano não promete aumento de tráfego, indexação, reputação, seguidores ou alteração de resultados de busca.

## Canais prioritários

### 1. Site `axodus.country`

Função: fonte primária e canônica.

Publicar:

- `/what-is-axodus/`;
- `/platforms/`;
- artigos de arquitetura;
- notas de governança;
- páginas de pesquisa;
- changelog institucional;
- índice de publicações.

Todo artigo externo deve apontar para uma página correspondente no site.

### 2. Medium — `https://axodus.medium.com/`

Função: distribuição de artigos e descoberta orgânica.

Usar inicialmente o perfil/publicação já existente. Criar uma publicação Medium própria somente se houver assinatura/recursos aprovados, pois a criação de uma publicação exige membership ativo.[^1]

Publicar:

- artigos completos;
- versões editoriais simplificadas de textos do site;
- ensaios sobre arquitetura e governança;
- explicações de conceitos.

A distribuição do Medium pode ocorrer pelo perfil, seguidores, recomendações e publicações, mas não é garantida.[^2]

### 3. Substack — `https://axodus.substack.com/`

Função: newsletter, arquivo editorial e relacionamento recorrente.

Publicar:

- resumo quinzenal ou mensal;
- artigos originais;
- notas de evolução;
- explicações de conceitos;
- links para novas páginas do site.

O Substack permite publicar na web e, por padrão, enviar para e-mail e para o aplicativo; cada publicação deve escolher conscientemente se usará esses canais.[^3]

### 4. GitHub — organização e repositório Institutional

Função: evidência documental, transparência de processo e discussão técnica.

Usar:

- README;
- Discussions, se habilitado;
- Releases ou changelog documental;
- Issues para questões de documentação;
- links para o site e a documentação oficial.

O GitHub não deve ser usado para sugerir que um módulo está implementado, operacional ou pronto para produção.

### 5. Canais comunitários opcionais

Avaliar apenas depois de estabelecer consistência nos canais próprios:

- DEV Community;
- Hashnode;
- Reddit técnico;
- Hacker News;
- LinkedIn ou X, se já houver contas oficiais.

Esses canais devem receber excertos ou links para a fonte canônica, não cópias descontroladas do mesmo artigo.

## Pilares editoriais

Manter cinco pilares fixos:

1. **Identity** — o que é Axodus, o que não é e qual é seu estágio.
2. **Architecture** — modularidade, plataformas interoperáveis, governança constitucional e limites.
3. **Governance** — accountability, revisão, contestação, evidência e supervisão humana.
4. **Platforms** — Academy, Marketplace, BBA, ACS e Governance como domínios propostos ou protótipos autor-reportados, sempre qualificados.
5. **Research and practice** — hipóteses, decisões arquiteturais, aprendizados, limitações e agenda de pesquisa.

DeFi, Mining, Lotto, DEX, Trading e temas financeiros devem receber tratamento conceitual e cauteloso, sem estratégia, rendimento, preço, adoção ou promessa operacional.

## Formato editorial semanal

Com a capacidade escolhida de uma publicação longa e duas threads por semana:

- **1 artigo semanal:** 900–1.600 palavras, publicado primeiro no site.
- **Thread 1:** resumo conceitual com 5–8 pontos.
- **Thread 2:** pergunta, diagrama, decisão arquitetural ou trecho comentado.
- **1 adaptação quinzenal:** versão resumida para Medium ou Substack.
- **1 compilação mensal:** índice dos artigos, decisões e atualizações.

Cada peça deve conter:

- definição do tema;
- status da afirmação: fato, proposta, hipótese ou futuro trabalho;
- link para a fonte canônica;
- limitações relevantes;
- data de publicação;
- autor/editor responsável.

## Cronograma de 12 semanas

| Semana | Artigo principal | Threads e distribuição |
|---|---|---|
| 1 | What is Axodus? | Identidade canônica; diferença entre Axodus e outras entidades |
| 2 | Why governed knowledge matters | Problema da fragmentação documental; link para `/research/` |
| 3 | Axodus platform ecosystem | Visão geral da taxonomia e das relações |
| 4 | How constitutional governance is framed | Restrições, revisão e autoridade humana |
| 5 | What makes a platform a proposed nucleus? | ACS, Academy e Marketplace |
| 6 | Governance as a standalone platform context | Governance e seu contexto Harmony, sem alegar adoção |
| 7 | Designing for evidence and traceability | Provenance, accountability e limites |
| 8 | AI assistance under human oversight | O que a IA pode apoiar e o que não pode decidir |
| 9 | From research to reference platform | Lifecycle proposto, sem afirmar etapas concluídas |
| 10 | Academy, BBA and institutional workflows | Funções conceituais e limites de implementação |
| 11 | DeFi, Mining and Lotto as bounded domains | Domínios conceituais, sem linguagem financeira promocional |
| 12 | Axodus research agenda and open questions | Síntese, limitações e próximos temas de pesquisa |

## Fluxo de publicação

```text
Ideia
  ↓
Classificação da afirmação
  ↓
Rascunho no site
  ↓
Revisão de evidência e linguagem
  ↓
Publicação canônica
  ↓
Adaptação para Medium/Substack
  ↓
Threads e discussões
  ↓
Medição e registro
```

A ordem deve ser sempre: site primeiro, canais externos depois. Medium e Substack não devem se tornar fontes divergentes da identidade oficial.

## Artefatos de controle E0

O pacote de produção controlada está versionado em:

- [inventário editorial](editorial-inventory.md), com 12 artigos e 24 threads;
- [worksheet de claims](claims-review-worksheet.md), vinculado ao registro de
  claims;
- [fluxo de adaptação canônica](editorial-adaptation-flow.md) e templates;
- [log mensal de observações](observation-log.md);
- [prontidão e autorização de canais](channel-readiness.md).

Esses registros são planejamento e revisão; não autorizam publicação,
outreach, edição de perfis ou qualquer ação em serviço externo.

## Regras de distribuição

- Não publicar o mesmo artigo integral em vários locais sem estratégia de canonicalização ou indicação clara da fonte original.
- Preferir no Medium e no Substack um resumo editorial com link para o artigo canônico quando a duplicação puder confundir a origem.
- Usar títulos informativos, não títulos de choque.
- Não comprar backlinks, seguidores, anúncios, publieditoriais ou cobertura.
- Não fazer spam em comunidades.
- Não solicitar avaliações favoráveis.
- Não usar “first”, “unique”, “revolutionary”, “guaranteed”, “scam-proof” ou equivalentes.
- Não repetir defensivamente “Axodus não é scam” como tema de SEO.
- Corrigir erros factuais publicamente apenas com evidência verificável e linguagem neutra.

## Revisão e controle

Antes de publicar cada peça:

- conferir a identidade canônica;
- conferir o claims register;
- classificar cada afirmação;
- remover alegações de adoção, usuários, parceiros, receita, performance, segurança ou prontidão;
- confirmar links oficiais;
- verificar imagens e direitos de uso;
- revisar título, description e Open Graph;
- registrar a URL publicada e a data.

O planejamento editorial orgânico está ativo nesta fase. Publicação externa,
submissão a terceiros, contato dirigido, imprensa, divulgação comercial e
qualquer ação paga continuam sujeitos a revisão humana e autorização
específica para o canal correspondente.

## Métricas observáveis

Acompanhar mensalmente:

- artigos publicados;
- páginas canônicas criadas;
- links internos adicionados;
- visualizações por canal;
- inscrições no Substack;
- referências ao site;
- consultas de marca;
- erros de rastreamento;
- consistência de snippets e previews;
- perguntas recorrentes dos leitores;
- correções editoriais realizadas.

Interpretar essas métricas como observações, não como prova de crescimento, autoridade ou melhoria causal nos resultados de busca.

## Critérios de sucesso da primeira fase

Ao final de 12 semanas:

- 12 artigos canônicos publicados ou revisados;
- 24 threads publicadas;
- páginas de identidade, plataformas e pesquisa interligadas;
- perfis Medium, Substack e GitHub com descrição consistente;
- todos os canais apontando para `axodus.country`, `docs.axodus.country` e o repositório Institutional;
- nenhuma peça contendo claims bloqueados;
- calendário e registro editorial mantidos;
- relatório mensal de observações produzido.

## Assumptions

- O inglês será o idioma principal nesta fase.
- A cadência será de 1 artigo e 2 threads por semana.
- Site, Medium, Substack e GitHub serão os canais principais.
- Produtos sem site próprio receberão conteúdo conceitual, sem CTA inventado.
- Nenhuma ação paga ou contato externo será executado.
- A publicação efetiva exigirá revisão humana antes de cada lote.

[^1]: [Medium Help — Getting started with a Medium publication](https://help.medium.com/hc/en-us/articles/115004681607-Getting-started-with-a-Medium-publication)
[^2]: [Medium Help — What happens to your story when you publish](https://help.medium.com/hc/en-us/articles/360018677974-What-happens-to-your-story-when-you-publish)
[^3]: [Substack Help — How do I publish a new post?](https://support.substack.com/hc/en-us/articles/360037831771-How-do-I-publish-a-new-post-on-Substack)
