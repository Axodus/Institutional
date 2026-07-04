

Axodus paper v0.3.2 pt br · MD
---
título: "Axodus: Uma Arquitetura Conceitual em Estágio de Protótipo para Rastreabilidade e Accountability em Instituições Digitais Assistidas por Humano-IA"
autor:
  - "Mauricio Z. Filho"
afiliação: "Pesquisador Independente, Axodus"
correspondência: "mzfshark@gmail.com"
fórum_de_discussão_do_projeto: "Telegram @thinkincoin"
handle_social_do_autor: "@mzfshark"
versão: "Draft v0.3.2"
status: "Pronto para revisão interna por pares após revisão pontual; não pronto para circulação externa ou publicação"
licença: "CC BY 4.0"
tipo_de_documento: "Arquitetura conceitual em estágio de protótipo e paper de agenda de pesquisa focado"
---
 
> **Nota do tradutor:** Esta é uma tradução para português brasileiro do documento original em inglês, mantida para uso interno e revisão do Coordenador Geral do Axodus. Em caso de divergência de interpretação, a versão original em inglês (`paper.md` / `paper.tex`) é a fonte de verdade.
 
# Resumo
 
Instituições digitais dependem cada vez mais de assistência automatizada, ao mesmo tempo em que continuam exigindo autoridade identificável, evidência revisável e supervisão humana responsabilizável (*accountable*). As literaturas existentes abordam design sociotécnico, governança descentralizada, interação humano-IA e padrões de credenciamento, mas não produzem, por si só, uma arquitetura conceitual focada em rastreabilidade e *accountability* para tomada de decisão institucional assistida por humano-IA. Este paper apresenta o Axodus como uma arquitetura conceitual em estágio de protótipo e uma agenda de pesquisa focada nesse problema. Sua contribuição central é um modelo em camadas para conectar autoridade de decisão, evidência, assistência de IA delimitada, justificativa (*rationale*) e caminhos de revisão em instituições digitais. A discussão de apoio aborda prontidão de participação, restrições de risco delimitadas e redução de complexidade. O Axodus é descrito apenas como um modelo conceitual em estágio de protótipo; o paper não relata sistema implantado, validação empírica ou prontidão operacional.
 
**Palavras-chave:** sistemas sociotécnicos; instituições digitais; coordenação humano-IA; rastreabilidade; *accountability*; governança; contestabilidade
 
# 1. Introdução
 
Instituições digitais podem combinar governança distribuída, documentação pública, assistência automatizada e requisitos de participação dentro do mesmo ambiente de decisão. Essas capacidades não determinam, por si só, quem pode decidir, qual evidência sustenta uma decisão, como uma análise automatizada deve ser revisada, ou como uma parte afetada pode contestar um resultado. A pesquisa em sistemas sociotécnicos, portanto, trata o design organizacional e o design técnico como interdependentes, em vez de assumir que um pode ser derivado do outro [@baxter2011sociotechnical].
 
Literaturas relevantes esclarecem partes desse problema, mas ainda não produzem um único modelo institucional focado em rastreabilidade e *accountability* sob tomada de decisão assistida por humano-IA. A pesquisa em governança descentralizada destaca a importância contínua de interpretação, mudança e coordenação social em torno de regras autoexecutáveis [@hassan2021dao; @hsieh2018bitcoin]. As diretrizes de interação humano-IA enfatizam o estabelecimento de expectativas, correção e revisão, em vez de uma transferência indiferenciada de autoridade [@amershi2019guidelines]. Os padrões de credenciamento ajudam a separar a verificação de máquina do julgamento institucional [@w3c2025vcdm]. O que permanece menos claramente especificado é como autoridade, evidência, assistência de IA delimitada, contestabilidade e caminhos de revisão devem ser organizados em conjunto em uma arquitetura conceitual inspecionável.
 
Este paper aborda essa lacuna introduzindo o Axodus como uma arquitetura conceitual em estágio de protótipo e agenda de pesquisa focada. O projeto tem origem em um esforço de pesquisa e design independente de vários anos. A presente contribuição limita-se a um modelo: não relata uma plataforma funcional, implantação em produção, usuários, resultados de avaliação, controles validados ou autoridade operacional.
 
A contribuição central é uma arquitetura em camadas para rastreabilidade e *accountability* em instituições digitais assistidas por humano-IA. Ela conecta autoridade institucional, evidência, assistência de IA delimitada, justificativa de decisão, contestabilidade e caminhos de revisão. A contribuição reside nesse arranjo específico, não em qualquer camada considerada isoladamente. Prontidão de participação, separação de maturidade e limites de risco permanecem como componentes de apoio necessários para enquadrar como o arranjo poderia ser inspecionado e eventualmente avaliado.
 
Implementação, implantação, adoção institucional e validação empírica estão fora do escopo do paper. O manuscrito também não avalia efeitos educacionais, propriedades de segurança, mecanismos financeiros ou conformidade legal.
 
# 2. Contexto e Trabalhos Relacionados
 
## 2.1 Sistemas sociotécnicos e instituições digitais
 
Uma perspectiva sociotécnica pergunta como papéis, incentivos, práticas de trabalho, informação e tecnologia moldam conjuntamente os resultados. Baxter e Sommerville defendem a integração de preocupações organizacionais com engenharia de sistemas, em vez de tratá-las como um problema de adoção tardia [@baxter2011sociotechnical]. O Axodus adota essa perspectiva ao modelar governança e *accountability* como elementos arquitetônicos, não como documentos de política externos anexados após a implementação.
 
O termo *instituição digital* é usado aqui para um sistema organizado de papéis, regras, registros e capacidades técnicas por meio do qual participantes perseguem atividade coletiva. Não exige que toda regra seja executável ou que toda interação ocorra em blockchain.
 
## 2.2 Governança descentralizada, rastreabilidade e revisão
 
Hassan e De Filippi descrevem uma DAO como um sistema baseado em blockchain no qual pessoas coordenam por meio de governança descentralizada e regras autoexecutáveis [@hassan2021dao]. Hsieh et al. distinguem consenso de máquina do consenso social necessário para alterar protocolos e arranjos organizacionais [@hsieh2018bitcoin]. Essas distinções alertam contra equiparar distribuição técnica com governança responsabilizável.
 
As finanças descentralizadas oferecem um exemplo específico de domínio no qual a composabilidade pode propagar dependências entre protocolos conectados [@schar2021defi]. A pesquisa de segurança sistêmico-teórica trata acidentes em sistemas sociotécnicos complexos como produtos de interações e controle inadequado em todo o sistema, e não apenas falhas isoladas de componentes [@leveson2012engineering]. Esse enquadramento mais amplo evita que o exemplo específico de DeFi carregue a afirmação arquitetônica geral.
 
## 2.3 Supervisão humano-IA, confiança calibrada e governança
 
As diretrizes de interação humano-IA enfatizam comunicar as capacidades do sistema, apoiar correção e aprender com o comportamento ao longo do tempo [@amershi2019guidelines]. No nível organizacional, o NIST AI Risk Management Framework trata governança, mapeamento, medição e gestão como funções de risco conectadas [@tabassi2023airmf]. Essas fontes motivam uma arquitetura na qual as saídas de IA são insumos atribuíveis a decisões, e não decisões soberanas, e na qual as condições de revisão humana permanecem visíveis.
 
A IA Constitucional usa princípios escritos para guiar o comportamento do modelo por meio de aprendizado supervisionado e *feedback* de IA [@bai2022constitutional]. O Axodus usa *constitucional* de forma diferente: refere-se a regras institucionais sobre autoridade, proibições, emendas, revisão e apelação. O modelo proposto não afirma treinar ou alinhar um modelo de IA por meio de IA Constitucional.
 
## 2.4 Credenciais, prontidão de participação e julgamento institucional
 
O W3C Verifiable Credentials Data Model separa a verificação criptográfica de uma credencial da validação de se suas alegações são adequadas ao propósito de um verificador [@w3c2025vcdm]. Isso importa aqui porque um registro tecnicamente verificável não estabeleceria, por si só, avaliação justa, aprendizado ou restrição de governança legítima.
 
## 2.5 Proveniência de dados e reconstrução responsabilizável
 
O W3C PROV Data Model descreve proveniência por meio de entidades, atividades, agentes, derivações, atribuição e relações de responsabilidade [@w3c2013provdm]. Esse vocabulário é útil para distinguir artefatos de origem, transformações, assistência automatizada e papéis responsáveis em um registro de decisão. Ele apoia a reconstrução de como uma saída foi produzida, mas não estabelece, por si só, que a decisão foi legítima, contestável ou responsabilizável. Trabalhos sobre algoritmos responsabilizáveis argumentam de forma semelhante que processos de decisão automatizados devem ser avaliáveis em relação a padrões legais ou de política externos, e que a transparência por si só é insuficiente [@kroll2017accountable]. A proveniência é, portanto, um insumo para a *accountability*, não seu substituto.
 
# 3. Declaração do Problema
 
A arquitetura aborda um problema de design, e não um efeito empírico estabelecido:
 
> Como uma instituição digital pode tornar decisões assistidas por humano-IA mais rastreáveis, contestáveis e responsabilizáveis, conectando autoridade, evidência, justificativa e caminhos de revisão, sem confundir documentação com implementação, ou automação com governança legítima?
 
Cinco tensões estruturam o problema.
 
1. **Modularidade versus coerência.** Componentes independentes podem limitar o acoplamento, mas decisões compartilhadas exigem identidade, evidência e regras de revisão comuns.
2. **Participação versus prontidão.** A participação aberta pode sustentar legitimidade, enquanto decisões consequentes podem exigir compreensão demonstrada.
3. **Automação versus *accountability*.** A assistência de IA pode reduzir a carga analítica, mas a responsabilidade pode se tornar pouco clara quando suas saídas influenciam a ação.
4. **Transparência versus privacidade e segurança.** Decisões rastreáveis precisam de registros, enquanto a divulgação indiscriminada pode prejudicar participantes ou expor sistemas.
5. **Documentação versus verdade operacional.** Uma especificação detalhada pode melhorar a revisão, ao mesmo tempo em que cria uma impressão enganosa de conclusão.
O Axodus é proposto como uma arquitetura para tornar essas tensões explícitas. Não é apresentado como sua solução.
 
# 4. Arquitetura Conceitual
 
O modelo compreende seis camadas lógicas. Elas descrevem responsabilidades e interfaces, não uma topologia de implementação.
 
Conceitualmente, as camadas formam um caminho de decisão direcional:
 
1. a governança constitucional define os papéis aplicáveis, direitos de decisão, proibições e regras de apelação;
2. um componente institucional delimitado recebe uma solicitação de decisão e, quando justificado, verifica condições de prontidão de participação;
3. a camada de evidência reúne material de origem, conflitos declarados e a base de autoridade da solicitação;
4. a assistência humano-IA pode transformar ou analisar esse material, com sua tarefa, insumos, saída e revisor responsável registrados como proveniência;
5. os limites de risco restringem as ações disponíveis ao tomador de decisão humano autorizado; e
6. a decisão resultante e sua justificativa entram em um caminho de revisão por meio do qual um papel independente pode inspecionar, corrigir, escalar ou ouvir uma apelação.
A informação, portanto, se move das regras, solicitações e evidências, passando por qualquer assistência, até um registro de decisão. O controle permanece com papéis humanos autorizados, restringidos pela governança e pelos limites de risco. O fluxo de revisão pode devolver evidência ou justificativa em disputa para correção, sem tratar o registro original como uma interpretação imutável.
 
**Cenário sintético ilustrativo — revisão de exceção de política.** Uma solicitação simulada de exceção de política inclui uma declaração de autoridade, a regra aplicável e um pacote de evidências controlado. Um resumo de IA simulado omite uma fonte citada. O revisor responsável registra a omissão, retém a decisão até a correção e escala a solicitação porque um limite de risco é acionado. Um papel de apelação independente pode então reconstruir quais evidências foram fornecidas, o que a assistência simulada alterou e por que a escalada ocorreu. Este cenário é uma ilustração analítica, não evidência de uma implementação ou processo institucional do Axodus.
 
## 4.1 Governança constitucional
 
A camada de governança declara papéis, direitos de decisão, proibições, regras de emenda, caminhos de escalada e mecanismos de apelação. Seu propósito é tornar visível a autoridade de ordem superior. Uma ação válida precisaria tanto de autorização técnica quanto de justificativa institucional; nenhuma das duas isoladamente estabeleceria legitimidade.
 
## 4.2 Evidência e *accountability*
 
A camada de evidência conecta propostas, material de apoio, conflitos declarados, análises geradas por IA, decisões, papéis responsáveis e revisões subsequentes. O objetivo de design é a reconstrutibilidade: um revisor deve conseguir perguntar o que era conhecido, quem estava autorizado, qual assistência foi usada e por que um resultado se seguiu. A proposta não assume que mais dados produzam automaticamente *accountability*.
 
No nível conceitual, documentos de origem e saídas podem ser tratados como entidades, etapas de análise e revisão como atividades, e participantes humanos ou automatizados como agentes. Relações de derivação e atribuição podem então conectar uma saída a seus insumos e papéis responsáveis [@w3c2013provdm]. Esses conceitos especificam o que um registro revisável deve expressar; não prescrevem um sistema de armazenamento ou mecanismo de integridade.
 
## 4.3 Componentes institucionais modulares
 
Componentes delimitados representam capacidades institucionais. Uma taxonomia conceitual mínima inclui as seguintes classes funcionais:
 
- um **registro de autoridade e papéis** para direitos de decisão e delegações;
- um **registro de evidências** e uma **camada de proveniência de assistência de IA** para fontes, transformações e insumos automatizados atribuíveis;
- um **registro de justificativa de decisão** e um **registro de conflitos e divulgações** para a base e as condições de uma decisão;
- um **caminho de revisão e apelação** e um **controlador de limites de risco** para contestação, escalada e ação delimitada; e
- **apoio à prontidão de participação** para preparação educacional antes de atividades consequentes selecionadas.
Esses são tipos de componentes, não um inventário definitivo de módulos do Axodus nem afirmações de implementação. Cada tipo deve declarar seu propósito, insumos, saídas, autoridade, dependências, requisitos de evidência e comportamento de falha. Em conjunto, fornecem um caminho conceitual desde a ação autorizada e a evidência de origem, passando pela assistência de IA e justificativa, até a revisão ou apelação.
 
## 4.4 Apoio à prontidão de participação
 
Uma camada educacional e um mecanismo de prontidão de participação são propostos como interfaces de apoio para aprendizado e avaliação. Seu propósito seria ajudar os participantes a compreender riscos específicos do domínio e deveres de governança antes de realizar ações consequentes selecionadas. Neste paper, são elementos de apoio, não contribuições coequivalentes. Não devem se tornar um sistema geral de classificação social.
 
## 4.5 Assistência humano-IA
 
Serviços de IA podem apoiar tarefas delimitadas, como comparação de documentos, resumo de propostas, detecção de inconsistências, sinalização de risco e preparação de material de revisão. Cada uso deve declarar a tarefa, o material de origem, a saída, a incerteza (quando disponível), o revisor humano e a decisão. Os humanos retêm autoridade de decisão e responsabilidade.
 
## 4.6 Limites de risco e revisão
 
A camada de risco expressa restrições sobre autoridade, exposição, tempo, conflitos e escalada. Um limite deve identificar o papel responsável, a condição de acionamento, a evidência exigida, a exceção permitida e o caminho de escalada. Isso conecta a ação delimitada aos registros de decisão e revisão usados para *accountability*.
 
# 5. Modularidade, Maturidade e Redução de Escopo
 
O processo de governança interna do Axodus distingue duas dimensões de maturidade ortogonais. O **Nível-L** refere-se à maturidade organizacional, de documentação, governança e autoridade. O **Nível-D** refere-se à maturidade de desenvolvimento, implementação, validação técnica e operacional. O Nível-L não mede código, e o Nível-D não mede governança. Nenhuma das dimensões autoriza produção ou ação sensível; o status de produção e a autoridade de ação exigem portões (*gates*) separados.
 
A rubrica L0–L5 e D0–D5 é uma taxonomia operacional interna, não um instrumento de medição empiricamente validado. Este paper não atribui níveis a componentes. Sua relevância aqui limita-se a evitar que a documentação seja confundida com implementação, que a implementação local seja confundida com produção, ou que a maturidade seja confundida com autoridade. A rubrica completa é mantida separadamente na documentação de governança do projeto.
 
A modularidade é, da mesma forma, uma hipótese de apoio, não uma propriedade assegurada. Os limites de componentes podem auxiliar a revisão, mas também podem deslocar complexidade para as interfaces e dificultar a avaliação da governabilidade.
 
A arquitetura deve, portanto, ser reduzida antes de ser expandida. Protótipos iniciais devem:
 
- começar com decisões para as quais a reconstrução e a apelação sejam materiais;
- usar um registro mínimo suficiente de evidência e justificativa;
- separar saídas de IA consultivas de decisões humanas com autoridade;
- exigir um pacote de evidências antes de introduzir assistência automatizada;
- escalonar os requisitos de revisão de acordo com a consequência da decisão; e
- remover um componente quando a avaliação não mostrar que ele melhora a reconstrutibilidade ou a contestabilidade.
# 6. Mecanismo de Prontidão de Participação
 
O mecanismo conectaria objetivos de aprendizado definidos, avaliação, resultados revisáveis, elegibilidade delimitada e um caminho de apelação para atividades selecionadas.
 
O modelo de credenciais do W3C poderia informar representações portáveis, mas a verificação de um emissor e de uma credencial não valida a qualidade educacional nem justifica a autorização [@w3c2025vcdm]. O problema de governança, portanto, inclui quem define os critérios, como as adaptações são fornecidas e como um participante pode contestar um resultado.
 
A hipótese central é que a prontidão educacional pode melhorar a qualidade da participação delimitada em contextos selecionados de alta consequência. Hipóteses concorrentes permanecem igualmente importantes: o mecanismo pode excluir participantes, centralizar o poder curricular, incentivar a manipulação de testes ou criar riscos de privacidade. Deve ser rejeitado ou redesenhado se esses danos não puderem ser controlados.
 
Os critérios de avaliação propostos incluem exclusão falsa e inclusão falsa, acessibilidade e adaptação, disponibilidade e conclusão de apelações, concentração curricular, ônus de privacidade e evidência de melhoria no contexto específico de decisão. As salvaguardas candidatas incluem separar o design curricular das decisões de autorização, divulgar conflitos de avaliação e submeter os critérios a revisão independente. Os portões de prontidão de participação devem se limitar a contextos nos quais sua necessidade e proporcionalidade possam ser testadas.
 
# 7. Governança, *Accountability* e Supervisão Humana
 
O registro mínimo conceitual de decisão possui sete campos: escopo da decisão, papéis autorizados, evidência considerada, conflitos divulgados, assistência automatizada usada, decisão e justificativa, e caminho de revisão ou apelação.
 
A assistência de IA é regida por limites específicos de tarefa. Redações de baixa consequência podem permitir revisão leve; classificação de risco ou análise de propostas exigiria proveniência mais forte, verificação independente e decisão humana explícita. Uma saída de IA não pode aprovar seu próprio uso, resolver uma apelação sobre si mesma, ou se tornar a portadora final da responsabilidade.
 
O modelo deve apoiar a contestabilidade. Participantes afetados por uma decisão precisam de uma forma de identificar as regras aplicáveis, contestar evidências, corrigir registros e solicitar revisão por um papel apropriadamente independente. Registros imutáveis, quando usados, não devem ser tratados como interpretações imutáveis.
 
Dentro desta proposta, a independência do revisor significa separação da decisão original, divulgação de conflitos e recusa quando um revisor participou da análise contestada. Os caminhos de escalada devem identificar para onde uma revisão se move quando a autoridade, a expertise ou a capacidade são insuficientes. A escalabilidade do processo pode ser examinada por meio do tamanho da fila, tempo de revisão, taxa de casos não resolvidos e amostragem para revisão secundária.
 
A supervisão humana torna-se nominal quando um revisor carece de autoridade, tempo, acesso à evidência ou capacidade prática de alterar o resultado. Esses requisitos se alinham com a orientação de governança orientada a risco e de interação humano-IA [@tabassi2023airmf; @amershi2019guidelines]. A literatura sobre contestabilidade por design identifica de forma semelhante salvaguardas, revisão e intervenção humana, e escrutínio de terceiros como características de design [@alfrink2023contestable]. Rotação de papéis e revisão multi-papel permanecem hipóteses candidatas de resistência à captura cujos efeitos exigem teste.
 
# 8. Limites de Risco como Restrições de Apoio
 
Os limites de risco restringem ação, exposição, processo e escalada. Para cada decisão consequente, a arquitetura conecta o limite aplicável à sua base de autoridade, evidência de apoio, registro de exceção e caminho de revisão. Registros visíveis são insuficientes quando premissas ou justificativas permanecem implícitas. As dependências entre componentes devem, portanto, ser declaradas na interface onde evidência, autoridade ou escalada cruzam um limite de componente. Se a dependência não puder ser revisada ou delimitada proporcionalmente, o design deve reduzir o escopo em vez de adicionar mais uma camada de controle.
 
# 9. Status do Protótipo
 
O Axodus é apresentado neste paper como um modelo conceitual em estágio de protótipo. O repositório público atualmente sustenta artefatos editoriais e documentação de pesquisa. Não fornece evidência de uma implementação integrada, operação em produção, adoção de usuários, desempenho empírico ou controles efetivos.
 
A ausência dessas afirmações é substantiva. A consistência arquitetônica pode ser revisada antes da implementação, mas não pode substituir o comportamento observado. Versões futuras devem manter uma tabela de evidências componente a componente, distinguindo estados projetado, prototipado, testado, implantado e avaliado independentemente.
 
# 10. Plano de Avaliação
 
O programa de avaliação é intencionalmente priorizado, não amplo.
 
Antes de qualquer um dos estudos iniciais, o estágio empírico inicial exige um ambiente controlado, e não um sistema institucional implantado. O ambiente deve combinar cenários de decisão sintéticos, pacotes de evidência controlados, registros de assistência de IA simulados, erros plantados e uma interface de revisão de alta fidelidade (*mock-up*) ou *wizard-of-oz*. Um protocolo pré-registrado deve definir as tarefas do revisor e os critérios de medição propostos. Esses critérios são desenhos de estudo, não resultados relatados.
 
**Estudo inicial primário — RQ1: Rastreabilidade.** O modelo de evidência proposto ajuda revisores independentes a reconstruir decisões com mais precisão e eficiência do que uma linha de base apenas documental? O ambiente controlado apoiaria cenários de governança pareados e revisão cega. As medidas propostas são completude de reconstrução, detecção de evidência ausente, tempo para reconstruir a justificativa, discordância entre revisores, detecção de conflito de autoridade, detecção de erro de proveniência e classificação correta de se uma apelação pode prosseguir. Esta é a prioridade primária de avaliação do paper, porque testa mais diretamente a alegação central sobre rastreabilidade e *accountability*.
 
**Estudo inicial secundário — RQ3: Confiança em humano-IA.** Para tarefas delimitadas de análise de propostas, como a proveniência e a decisão humana obrigatória afetam a detecção de erros, a confiança calibrada, o comportamento de anulação (*override*) e a qualidade da revisão? Os registros de IA simulados devem incluir erros plantados e casos ambíguos. As medidas propostas são detecção de erro plantado, detecção de saída não sustentada, comportamento de anulação ou aceitação por condição, qualidade da justificativa, discordância entre revisores e correção após a exibição de informações de proveniência. Esta é uma prioridade secundária porque a arquitetura depende da assistência de IA delimitada ser revisável, e não apenas disponível.
 
**Avaliação futura em estágios.** A avaliação deve progredir da inspeção de artefatos controlados para estudos de revisores delimitados usando cenários sintéticos, e então para avaliação de protótipo controlado sob um protocolo aprovado separadamente. Qualquer estudo institucionalmente situado posterior exigiria portões adicionais de governança, ética, jurídicos, de privacidade e de evidência. Participação educacional, confiabilidade de maturidade e governança de risco mais ampla permanecem tópicos de pesquisa futuros.
 
# 11. Limitações e Ameaças à Validade
 
Este paper é conceitual e ainda mais amplo do que um artigo externo maduro idealmente seria. A arquitetura pode parecer coerente porque ainda não encontrou restrições de implementação, conflito institucional ou condições de campo que testariam se seus caminhos de revisão propostos são viáveis.
 
A base de evidências públicas para o Axodus está atualmente limitada à documentação de design. Não há resultados com os quais avaliar viabilidade, usabilidade, legitimidade de governança, segurança, confiança calibrada, apelações contestáveis ou impacto social. A supervisão humana pode se tornar nominal quando os revisores carecem de tempo, autoridade ou expertise. A assistência de IA pode ser não confiável, difícil de calibrar ou difícil de auditar sob carga de trabalho e pressão de tempo realistas. Contestabilidade fraca ou caminhos de apelação mal projetados poderiam tornar a rastreabilidade visível sem tornar a *accountability* significativa.
 
Os mecanismos de prontidão de participação apresentam riscos particulares de exclusão, vigilância, captura curricular e falsa confiança. A modularidade pode ocultar acoplamento sistêmico. Regras explícitas podem formalizar arranjos injustos em vez de corrigi-los. A arquitetura proposta também pode ser complexa demais para governar na prática sem redução substancial de escopo.
 
O cenário sintético é explicativo, não empírico. O vocabulário de proveniência não estabelece integridade de registro ou *accountability*, e as medidas propostas não demonstram desempenho. A avaliação institucionalmente situada também pode expor conflitos, incentivos e efeitos de carga de trabalho que um artefato controlado não consegue reproduzir.
 
Designs de governança voltados para Web3 também podem encontrar incerteza regulatória, fragilidade operacional e encargos de conformidade específicos de jurisdição.
 
O paper não fornece aconselhamento jurídico, financeiro, de segurança ou de investimento. Sua terminologia pode não se mapear de forma limpa em toda jurisdição ou comunidade de pesquisa.
 
# 12. Agenda de Pesquisa
 
O trabalho de curto prazo deve priorizar um modelo mínimo de decisão-e-evidência e tarefas de assistência de IA delimitadas adequadas para estudos iniciais de rastreabilidade, junto com a verificação da literatura sobre proveniência, *accountability* algorítmica, contestabilidade e acoplamento sociotécnico. O design de prontidão de participação, a especificação de maturidade e cenários de governança mais amplos pertencem a papers ou notas técnicas posteriores, junto com questões de validade educacional.
 
# 13. Conclusão
 
O Axodus é proposto como uma arquitetura conceitual para tornar decisões institucionais assistidas por humano-IA mais rastreáveis e responsabilizáveis, por meio de autoridade, evidência, assistência atribuível, justificativa, contestabilidade e caminhos de revisão conectados. A contribuição imediata do modelo é um arranjo inspecionável de responsabilidades funcionais e interfaces, por meio do qual premissas de *accountability* podem ser examinadas.
 
O próximo passo de pesquisa é instanciar o modelo mínimo de decisão-e-evidência em um ambiente experimental controlado e testar se revisores independentes conseguem reconstruir e contestar decisões sob a estrutura de registro proposta.
 
# Referências
 
As referências são mantidas em `references.bib`. Todas as entradas citadas neste rascunho possuem registros de verificação internos correspondentes em `../../research/bibliography-verified.md`; a rechecagem final de metadados é necessária antes de qualquer submissão, divulgação pública ou circulação externa.
