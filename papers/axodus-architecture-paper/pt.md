---
title: "Axodus: Uma Arquitetura Conceitual em Estágio de Protótipo para Rastreabilidade e Responsabilização em Instituições Digitais Modulares Federadas"
author:
   - "Mauricio Z. Filho"
affiliation: "Pesquisador Independente, Axodus"
correspondence: "mzfshark@gmail.com"
project_discussion_forum: "Telegram @thinkincoin"
author_social_handle: "@mzfshark"
version: "Rascunho v0.6"
status: "Rascunho acadêmico interno v0.6 baseado na linha de base interna fechada v0.5; não pronto para revisão externa controlada, circulação externa ou publicação"
license: "CC BY 4.0"
document_type: "Arquitetura conceitual em estágio de protótipo e artigo com agenda de pesquisa focada"
---

## Resumo

Instituições digitais assistidas por IA tornam-se difíceis de governar quando
restrições constitucionais, domínios de governança local delimitados,
capacidades modulares e obrigações de revisão precisam ser coordenadas dentro
do mesmo ambiente decisório. Literaturas adjacentes sobre sistemas
sociotécnicos, governança descentralizada, proveniência, algoritmos
responsáveis, contestabilidade e interação humano-IA fornecem componentes com
escopos diferentes para examinar esse problema. Este artigo apresenta Axodus
como uma integração proposta desses componentes: uma arquitetura conceitual em
estágio de protótipo para esse contexto. Sua contribuição central é um modelo
orientado à governança com seis camadas que relaciona um centro constitucional,
domínios de governança local delimitados, capacidades institucionais modulares,
evidências e proveniência, assistência de IA limitada e controles de risco ou
contestabilidade. As seis camadas são apresentadas como uma decomposição
conceitual defensável, não como uma estrutura necessária, mínima,
unicamente correta ou universalmente suficiente. Rastreabilidade e
reconstruibilidade podem apoiar responsabilização e contestabilidade, mas não
estabelecem nenhuma das propriedades de forma independente. Axodus é descrito
apenas como um modelo conceitual em estágio de protótipo; o artigo não relata
implantação, validação empírica, uso institucional observado ou prontidão
operacional.

**Palavras-chave:** sistemas sociotécnicos; instituições digitais federadas;
coordenação humano-IA; rastreabilidade; responsabilização; governança;
contestabilidade
## 1. Introdução

Instituições digitais vêm combinando cada vez mais autoridade distribuída,
capacidades modulares, registros públicos e assistência automatizada. A
governança torna-se mais difícil quando esses elementos precisam permanecer
passíveis de revisão tanto em um centro constitucional quanto em domínios de
governança local delimitados, em vez de estarem concentrados em uma única
cadeia de autoridade. Nesse cenário, o desafio institucional não é apenas
se uma decisão pode ser documentada, mas se revisores posteriores podem
reconstruir qual autoridade foi aplicada, qual capacidade delimitada foi
invocada, quais evidências foram consideradas, como a assistência de IA
influenciou o registro e como correção ou contestação poderiam prosseguir.
A pesquisa em sistemas sociotécnicos trata essas questões como simultaneamente
organizacionais e técnicas, e não redutíveis a um único domínio
[@baxter2011sociotechnical].

Literaturas relevantes abordam partes desse problema com diferentes escopos
e sobreposições parciais. Pesquisas sobre governança descentralizada mostram
que regras autoexecutáveis não eliminam interpretação, emenda ou coordenação
social [@hassan2021dao; @hsieh2018bitcoin]. Diretrizes de interação humano-IA
enfatizam revisão, correção e definição de expectativas em vez de uma
transferência indistinita de autoridade [@amershi2019guidelines]. Padrões de
proveniência e credenciamento ajudam a distinguir a linhagem de evidências e
verificação por máquina do juízo institucional [@w3c2013provdm; @w3c2025vcdm].
Este artigo não afirma uma demonstração exaustiva de que não exista arquitetura
comparável; desenvolve uma síntese integrativa delimitada para um problema
institucional específico.

Este artigo apresenta Axodus como uma arquitetura conceitual em estágio de
protótipo para instituições digitais assistidas por IA sob restrições de
governança delimitadas. O projeto tem origem em um esforço de pesquisa e
desenho independente de vários anos; essa declaração registra proveniência de
fundo em vez de evidência científica. A contribuição aqui permanece
conceitual: não relata uma plataforma em uso institucional real, um ambiente
institucional funcional, resultados de avaliação ou controles testados de
forma independente.

A contribuição é raciocínio de nível arquitetural em vez de uma reivindicação
de implementação. O artigo propõe um modelo em camadas para como um centro
constitucional, domínios locais de governança delimitados, capacidades
institucionais modulares, pacotes de evidência, assistência de IA
atribuível e caminhos de revisão podem ser organizados em uma estrutura de
decisão inspecionável. A estrutura de seis camadas é uma decomposição
conceitual defensável entre alternativas possíveis. A prontidão para
participação permanece uma preocupação de apoio delimitada, enquanto
distinções entre documentação, desenvolvimento, produção e autoridade
servem apenas como limites de escopo.

Implementação, implantação, uso institucional e validação empírica estão
fora do escopo do artigo. O manuscrito também exclui projeto de tokens,
operações financeiras, mecânicas de distribuição educacional, garantias de
segurança e conclusões legais.

## 2. Antecedentes e Trabalhos Relacionados

### 2.1 Sistemas sociotécnicos e instituições digitais federadas

Uma perspectiva sociotécnica pergunta como papéis, incentivos, práticas de
trabalho, informação e componentes técnicos moldam conjuntamente os
resultados. Baxter e Sommerville defendem integrar preocupações
organizacionais com engenharia de sistemas, em vez de tratá-las como um
problema de adoção tardia [@baxter2011sociotechnical]. Axodus adota essa
perspectiva ao modelar governança, responsabilização e revisão como elementos
arquitetônicos, em vez de políticas externas anexadas após a implementação.

O termo *instituição digital modular federada* é usado aqui para um sistema
organizado em que uma camada constitucional central define restrições
compartilhadas, enquanto domínios de governança local delimitados podem
configurar capacidades institucionais modulares. Esse uso é conceitual e não
implica uma federação implantada, status federal legal ou uma plataforma
multitenant em operação.

### 2.2 Governança descentralizada, acoplamento modular e revisão

Hassan e De Filippi descrevem um DAO como um sistema baseado em blockchain no
qual pessoas se coordenam por meio de governança descentralizada e regras
autoexecutáveis [@hassan2021dao]. Hsieh et al. distinguem consenso de
máquina de consenso social necessário para alterar protocolos e arranjos
organizacionais [@hsieh2018bitcoin]. Essas distinções alertam contra
igualar distribuição técnica com governança responsável.

Mercados financeiros baseados em contratos inteligentes fornecem um exemplo
específico no qual a composabilidade pode propagar dependências entre
protocolos conectados [@schar2021defi]. A pesquisa em segurança sob a ótica
da teoria de sistemas oferece uma afirmação mais ampla: falhas em sistemas
sociotécnicos complexos podem surgir de interações, desalinhamentos de
controle e acoplamento mal governado, em vez de defeitos isolados de
componentes [@leveson2012engineering]. O presente artigo trata esse domínio
apenas como um exemplo motivador de propagação de dependências, não como o
centro institucional do estudo.

### 2.3 Supervisão humano-IA e suporte decisório responsável

Diretrizes para interação humano-IA enfatizam comunicar as capacidades do
sistema, apoiar correções e aprender com o comportamento ao longo do tempo
[@amershi2019guidelines]. Em nível organizacional, o NIST AI Risk Management
Framework trata governança, mapeamento, mensuração e gestão como funções de
risco conectadas [@tabassi2023airmf]. Essas fontes motivam uma arquitetura na
qual as saídas de IA permanecem atribuíveis e passíveis de revisão como
insumos para decisões humanas, em vez de decisões soberanas por si só.

Constitutional AI usa princípios escritos para guiar o comportamento de modelos
por meio de aprendizado supervisionado e feedback de IA [@bai2022constitutional].
Axodus usa "constitucional" de forma diferente: refere-se a regras
institucionais sobre autoridade, proibições, emendas, revisão e contestação.
O modelo proposto não afirma treinar ou alinhar um modelo de IA via
Constitutional AI.

### 2.4 Proveniência, credenciais e julgamento institucional

O W3C PROV Data Model descreve proveniência por meio de entidades, atividades,
agentes, derivações, atribuição e relações de responsabilidade
[@w3c2013provdm]. Esse vocabulário é útil para distinguir artefatos de
origem, transformações, assistência automatizada e papéis responsáveis em um
registro decisório. Ele apoia a reconstrução de como uma saída foi produzida,
mas não estabelece por si só que a decisão foi legítima, contestável ou
responsável.

O W3C Verifiable Credentials Data Model separa a verificação criptográfica da
validação de se as alegações de uma credencial são adequadas ao propósito do
verificador [@w3c2025vcdm]. Isso é relevante porque artefatos de elegibilidade
verificáveis por máquina não estabelecem por si mesmos uma avaliação justa,
autorização legítima ou limites de participação responsáveis.

Trabalhos sobre algoritmos responsáveis também argumentam que processos de
decisão automatizados devem ser avaliáveis frente a normas legais ou políticas
externas e que transparência por si só é insuficiente [@kroll2017accountable].
Portanto, proveniência é um insumo para responsabilização, não seu
substituto.

### 2.5 Contestabilidade e governança passível de revisão

A literatura sobre contestabilidade por projeto identifica salvaguardas,
revisão e intervenção humanas e escrutínio por terceiros como características
de projeto para contestação e correção [@alfrink2023contestable]. Essa
estrutura é diretamente relevante para governança modular federada porque um
registro rastreável continua insuficiente se uma pessoa afetada por uma
decisão não puder identificar a regra aplicável, contestar evidências ou
atingir um revisor adequadamente independente.

### 2.6 Síntese conceitual e derivação da arquitetura

A arquitetura é derivada por meio de uma síntese conceitual narrativa e
não sistemática, em vez de uma revisão sistemática, prova formal ou método de
desenho empírico. A síntese trata as vertentes literárias nas Seções 2.1–2.5
como fundamentos conceituais, as cinco tensões na Seção 3 como problemas de
desenho e os requisitos resultantes como razões para separar responsabilidades
em seis camadas. As fronteiras das camadas são traçadas onde autoridade,
interpretação local, capacidade delimitada, reconstrução de registros,
análise consultiva e condições de contestação exigem responsabilidades distintas
ou poderes expressamente excluídos.

Esse procedimento não estabelece que seis camadas sejam necessárias, mínimas,
unicamente corretas ou universalmente suficientes. Ele apresenta uma
decomposição conceitual defensável cujas fronteiras podem ser inspecionadas,
comparadas com alternativas e revistas ou rejeitadas. A matriz de derivação
torna explícita a cadeia dos fundamentos aos construtos de avaliação; isso
não implica que a literatura citada valide o Axodus.

## 3. Enunciado do Problema

A arquitetura aborda um problema de desenho, não um efeito empírico
estabelecido:

> Como uma instituição digital modular federada, limitada por um conjunto de
> regras constitucionais, pode suportar rastreabilidade, reconstruibilidade
> e as condições institucionais para responsabilização e contestabilidade,
> quando domínios locais de governança delimitados configuram capacidades
> institucionais modulares por meio de processos decisórios assistidos por
> IA?

Cinqüenta tensões estruturam o problema.

1. **Restrições centrais versus autonomia local.** Uma camada constitucional
   pode preservar coerência, enquanto domínios locais de governança ainda
   exigem discrição significativa sobre decisões e configurações locais.
2. **Capacidades modulares versus governabilidade.** A separação de serviços
   pode limitar o acoplamento direto, enquanto a seleção modular pode criar
   cadeias de dependência ocultas, autoridade ambígua e caminhos de revisão
   fragmentados.
3. **Automação versus disposição responsável.** A assistência de IA pode
   reduzir o esforço analítico, mas a responsabilidade pode se tornar
   incerta quando suas saídas influenciam autorização, escalonamento ou
   revisão.
4. **Participação versus prontidão delimitada.** A participação aberta pode
   apoiar legitimidade, enquanto ações de governança de grande consequência
   podem exigir preparação, acomodações e contestação passíveis de revisão.
5. **Documentação versus realidade institucional.** Uma especificação detalhada
   pode melhorar a inspeção mas também criar uma impressão enganosa de
   completude de implementação ou autoridade legítima.

Axodus é proposto como uma decomposição conceitual defensável para tornar
essas tensões inspecionáveis e passíveis de revisão. Não é apresentado como
uma solução completa, ótima, unicamente correta ou testada empiricamente.

## 4. Arquitetura Conceitual

O modelo compreende seis camadas lógicas selecionadas pela derivação na
Seção 2.6. Elas são superfícies conceituais de projeto para alocar
autoridade, estruturar registros e preservar a passibilidade de revisão, não
uma topologia de implementação. Sua separação expressa responsabilidades
distintas e poderes excluídos; isso não afirma que toda instituição requeira
essa decomposição.

Informação e controle atravessam a arquitetura de maneiras diferentes.
O controle começa com restrições constitucionais que definem quais decisões
locais, seleções de capacidades e caminhos de escalonamento estão no escopo.
Pacotes de evidência, registros de proveniência, análises consultivas,
justificativas e registros de revisão tornam essas decisões reconstruíveis
para revisões posteriores. Limites de risco restringem transições de estado
permitidas, enquanto caminhos de contestabilidade preservam condições para
contestação, correção, escalonamento e revisão.

**Cenário sintético ilustrativo – revisão de exceção em governança
delimitada.** Um domínio fictício de governança local delimitada solicita uma
exceção temporária que afeta uma capacidade institucional modular. A
solicitação inclui a regra constitucional aplicável, a base de autoridade
local, conflitos declarados e um pacote de evidência controlado. Uma revisão
simulada por IA sinaliza um conflito mas omite uma dependência entre a
configuração solicitada e um requisito de revisão. O revisor humano designado
retém a disposição, registra a omissão e escala o assunto porque um limite de
risco foi acionado. Um papel de revisão independente pode então reconstruir
qual restrição constitucional foi aplicada, qual escolha local foi proposta,
o que a revisão simulada por IA alterou e por que o escalonamento ocorreu.
Esse cenário é uma ilustração analítica, não evidência de uma
implementação Axodus ou processo institucional.

1. a governança constitucional define os papéis aplicáveis, direitos de
   decisão, proibições, regras de emenda e condições de contestação;
2. domínios locais de governança delimitados interpretam esse escopo para um
   contexto decisório local e podem propor uma configuração ou exceção dentro
   dos limites constitucionais;
3. capacidades institucionais modulares expressam o que está sendo selecionado,
   revisado ou alterado;
4. a camada de evidência e proveniência vincula materiais de origem, declarações
   de autoridade, conflitos, transformações e papéis responsáveis;
5. a assistência humano-IA pode analisar esse material, mas apenas como insumo
   consultivo atribuível à disposição humana; e
6. controles de limite de risco e contestabilidade mantêm condições de
   contestação, correção, escalonamento e revisão disponíveis.

A tabela de interfaces entre camadas especifica responsabilidades conceituais
e pontos de passagem. Suas entradas e saídas são categorias de registro, não
APIs, componentes de software ou afirmações sobre infraestrutura implementada.

| Camada | Responsabilidade conceitual | Entrada principal | Saída ou registro principal | Dependência entre camadas | Limite ou invariante | Autoridade expressamente excluída |
| --- | --- | --- | --- | --- | --- | --- |
| Governança constitucional | Definir papéis de ordem superior, restrições, emenda, escalonamento e condições de contestação | Regras institucionais e base para emenda | Registro de restrição aplicável e autoridade | Restringe domínios locais, módulos e condições de revisão | Restrições não delegáveis não podem ser ampliadas localmente; regras permanecem inspecionáveis | Não é alegado efeito jurídico, implantação, infalibilidade ou execução automática |
| Domínio de governança local delimitado | Interpretar o escopo permitido para um contexto decisório local | Restrições constitucionais e proposta local | Decisão delimitada, configuração ou pedido de escalonamento | Depende do escopo constitucional e das declarações de módulo | Não pode anular restrições não delegáveis | Não possui autoridade soberana, ilimitada ou de produção |
| Módulo de serviço funcional | Expressar uma capacidade institucional delimitada e suas dependências | Escopo autorizado, tarefa, requisitos de evidência e declarações de dependência | Proposta específica do módulo, resultado ou registro de falha | Constrangido pela governança; inspecionado por meio das camadas de evidência e risco | Deve expor propósito, dependências, necessidades de evidência, escalonamento e condições de falha | Não detém autoridade constitucional, proveniência, disposição de IA ou contestabilidade |
| Evidência e proveniência | Atribuir fontes, transformações, agentes, assistência e disposições | Artefatos de origem, declarações de autoridade, análises, conflitos e decisões | Registro vinculado de decisão e evidência | Recebe registros de todas as camadas decisórias e suporta revisão posterior | A vinculação de registros não estabelece verdade, integridade, legitimidade ou responsabilização | Sem validação automática, julgamento ou garantia de integridade |
| Assistência de IA | Fornecer análise consultiva delimitada e atribuível | Tarefa declarada, material de origem e restrições | Saída de IA com proveniência e disposição humana | Depende de entradas de evidência e revisão humana; sujeita-se a limites de risco | Autoridade e responsabilidade humana permanecem explícitas | Não é decisão soberana, execução ou julgamento vinculante |
| Limite de risco e contestabilidade | Tornar visíveis gatilhos de revisão, condições de contestação, necessidades de independência e possíveis disposições | Ação proposta, limite aplicável, evidência contestada e conflitos | Registro de revisão, recusa, escalonamento, correção, reversão ou sem alteração | Depende do escopo constitucional e da evidência reconstruível | Um caminho de contestação deve ser identificável e separável da disposição original | Não afirma um procedimento em vigor, remédio efetivo ou responsabilização garantida |

### 4.1 Camada de governança constitucional

A camada de governança constitucional é uma superfície conceitual de
restrição que define regras de ordem superior: papéis, direitos de decisão,
proibições, procedimentos de emenda, caminhos de escalonamento e condições de
contestação. Seu propósito é tornar visíveis restrições institucionais
não delegáveis antes do início da configuração local e enquadrar como uma
revisão posterior pode distinguir uma ação permitida de uma fora do escopo.

Nesta proposta, a camada estrutura limites que apoiam responsabilização em
vez de servir como uma constituição implantada, instrumento legal, autoridade
ativa ou órgão de execução. Uma ação passível de revisão depende tanto da
justificação institucional quanto de qualquer autorização técnica que uma
implementação futura possa usar; nenhuma das duas, isoladamente, estabeleceria
legitimidade.

Como as restrições constitucionais podem ser incompletas, ambíguas ou excessivas,
elas devem permanecer como objetos de projeto inspecionáveis com revisão,
emenda e condições de contestação delimitadas. O modelo, portanto, não trata
a camada constitucional como infalível ou além da contestação.

### 4.2 Camada de domínio de governança local delimitado

Como referência conceitual em vez de equivalência de implementação,
governança policêntrica descreve múltiplos centros decisórios que podem ser
formalmente distintos, mas interdependentes, operando através de camadas de
governança aninhadas [@ostrom2010beyond]. A camada de domínio de governança
local delimitado representa um contexto decisório com escopo local que opera
sujeito às restrições constitucionais. Um domínio local delimitado pode
configurar processos locais, selecionar módulos de serviço funcional e
alocar tarefas decisórias apenas dentro do escopo permitido pela camada
constitucional. A documentação institucional Axodus pode usar o termo
`Tenant` para esses domínios; este artigo usa a expressão "domínio de
governança" para evitar insinuar locação SaaS implantada, entidades clientes
ativas, comunidades operantes ou infraestrutura de produção.

Um domínio de governança local delimitado não pode expandir ou anular
restrições constitucionais não delegáveis. Quando a interpretação local de
uma ação proposta conflita com um limite constitucional, a arquitetura trata
essa ambiguidade como condição de revisão exigindo documentação e, quando
necessário, escalonamento antes da disposição final.

### 4.3 Camada de módulo de serviço funcional

Como referência conceitual em vez de validação dessa taxonomia, a literatura
sobre modularidade descreve sistemas complexos construídos a partir de
subsystems menores que podem ser projetados separadamente e funcionar em
conjunto sob regras de projeto compartilhadas [@baldwin2000design]. Módulos de
serviço funcional são capacidades institucionais abstratas e delimitadas por
meio das quais funções selecionadas podem ser configuradas, limitadas e
governadas. O artigo não apresenta um catálogo de produtos. Em vez disso,
trata o módulo de serviço funcional como uma unidade conceitual que deve
declarar seu propósito, entradas, saídas, escopo autorizado e dependências de
decisão, requisitos de evidência, dependências, condições de escalonamento
e comportamento em caso de falha.

Um módulo de serviço funcional é, portanto, uma superfície de capacidade
delimitada, não o detentor da autoridade constitucional, proveniência de
evidência, assistência de IA ou contestabilidade. Essas continuam sendo
camadas transversais separadas que restringem, inspecionam e reconstróem
decisões específicas do módulo.

A documentação institucional Axodus pode usar o termo "service nuclei" em
contextos institucionais mais amplos; este artigo usa "módulos de serviço
funcionais" como a abstração voltada à arquitetura para evitar implicar um
catálogo de produtos, inventário de implementação ou decomposição de sistema
implantado.

Uma taxonomia funcional mínima pode incluir registros de autoridade e papéis,
registros de evidência, registros de justificativa de decisão, registros de
conflito e divulgação, caminhos de revisão e contestação, controladores de
limite de risco e suporte à prontidão para participação como tipos de
componentes associados a capacidades governadas por módulo. Estes são tipos
de componente, não afirmações sobre um inventário definitivo de módulos
Axodus ou estado de implementação.

### 4.4 Camada de evidência e proveniência

A camada de evidência e proveniência vincula propostas, materiais de apoio,
declarações de autoridade, conflitos declarados, análises geradas por IA,
decisões e revisões subsequentes. Seu objetivo de projeto é a
reconstruibilidade: um revisor deve ser capaz de perguntar o que era conhecido,
quem estava autorizado, qual configuração foi proposta, que assistência foi
utilizada e por que um determinado resultado ocorreu.

No nível conceitual, documentos-fonte e saídas podem ser tratados como
entidades, passos de análise e revisão como atividades, e participantes
humanos ou automatizados como agentes. Relações de derivação e atribuição
podem então conectar uma saída às suas entradas e aos papéis responsáveis
[@w3c2013provdm]. Esses conceitos especificam o que um registro passível de
revisão deve expressar para que um revisor posterior possa reconstruir o
caminho do material-fonte até a disposição. Eles não provam, por si só, que um
registro é verdadeiro, completo, resistente a adulteração ou responsável no
sentido normativo mais forte.

Consequentemente, a camada apoia a inspeção posterior em vez da validação
automática. Ela não prescreve um sistema de armazenamento, prova
criptográfica, infraestrutura de evidência implementada ou garantia de
integridade, e não converte vinculação de registros em um julgamento pleno
sobre se a decisão foi substancialmente justificada.

### 4.5 Camada de assistência de IA

A assistência de IA permanece consultiva. Ela pode apoiar tarefas delimitadas,
como comparação de documentos, sumarização de propostas, detecção de
inconsistências, suporte à análise constitucional, checagem adversarial e
apoio à revisão orientada ao planejamento. Cada uso deve declarar a tarefa,
o material-fonte, a saída, a incerteza quando disponível, o revisor humano e
a disposição, de forma que revisores posteriores possam inspecionar como a
análise consultiva entrou no registro. Humanos mantêm autoridade e
responsabilidade pela decisão.

Essa camada é intencionalmente abstrata quanto a papéis. O artigo não usa
rótulos de agentes nomeados, não afirma autoridade de execução autônoma e
não alega que a assistência de IA por si só imponha governança, emita julgamentos
vinculantes ou substitua a revisão institucional humana.

### 4.6 Camada de limite de risco e contestabilidade

A camada de limite de risco e contestabilidade é uma superfície conceitual
para tornar visível quando revisão adicional, recusa, documentação ou um
caminho de contestação podem ser necessários. Nesse modelo, um limite deve
identificar o papel relevante, o gatilho de revisão, a evidência necessária
para inspeção e a condição sob a qual uma ação proposta excede seu escopo
permitido. Contestabilidade, portanto, diz respeito a se uma decisão pode ser
reconstruída, questionada e reexaminada em princípio, não a se a arquitetura
já opera um mecanismo de contestação em vigor.

Um registro minimamente contestável deve identificar a decisão ou registro
contestados, a regra ou limite aplicável, a evidência ou justificativa em
disputa, a condição de independência de revisão esperada para reexame e a
categoria de disposição possível, como correção, condição de escalonamento,
recusa, reversão ou sem alteração. Esses são campos conceituais para
reconstruibilidade e contestabilidade, não um procedimento de contestação em
vigência.

Dentro desse enquadramento, a independência do revisor é uma preocupação de
projeto e não uma alegação sobre um corpo permanente ou um papel nomeado. A
arquitetura deve possibilitar distinguir o contexto decisório original das
condições de contestação ou reexame posteriores, incluindo conflitos
divulgados e situações nas quais o mesmo ator não deveria ser o único juiz de
um registro contestado. A supervisão humana torna-se nominal quando um
revisor não dispõe de tempo, autoridade, acesso às evidências ou capacidade
prática para alterar um resultado [@tabassi2023airmf; @amershi2019guidelines].
A literatura sobre contestabilidade por projeto trata visibilidade de revisão,
intervenção e escrutínio externo como requisitos de projeto para sistemas
contestáveis, e não como garantias de que resultados nocivos sejam evitados
[@alfrink2023contestable].

### 4.7 Limite de prontidão para participação

A prontidão para participação é mantida apenas como uma preocupação de
apoio delimitada para preparação, acomodação, revisão e contestação em
contextos selecionados e de consequência. Não é uma contribuição de igual
nível, um sistema geral de classificação social ou um filtro universal de
competência. Qualquer artefato de prontidão seria um insumo contestável e
passível de revisão, não uma fonte independente de legitimidade, justiça ou
autoridade. Os critérios precisariam permanecer proporcionais, com mecanismos
de acomodação e abertos à contestação; exclusão, vigilância, captura
interpretativa, manipulação de testes e riscos à privacidade são motivos para
reduzir, redesenhar ou rejeitar o mecanismo. Sua validade é tema de pesquisa
futura, e não uma reivindicação avaliada neste artigo.

## 5. Estado do Protótipo

Axodus é apresentado neste artigo como um modelo conceitual em estágio de
protótipo. O repositório público atualmente suporta artefatos editoriais,
registros de governança e documentação de pesquisa. Ele não fornece evidência
de uma implementação integrada, plataforma federada em funcionamento,
operação em produção, adoção de usuários, desempenho empírico ou controles
eficazes.

A ausência dessas alegações é substancial. A consistência arquitetônica pode
ser revisada antes da implementação, mas não pode substituir o comportamento
observado. Versões futuras devem manter uma tabela de evidências por
componente distinguindo estados projetados, prototipados, testados,
implantados e avaliados independentemente.

Maturidade da documentação, maturidade de desenvolvimento, prontidão para
produção e autoridade institucional são determinações separadas. Essa
distinção é usada apenas para evitar erro de categoria: documentação não
estabelece implementação, implementação não estabelece autorização de
produção e maturidade não estabelece autoridade legítima ou capacidade
operacional. O artigo não retém L-Level ou D-Level como construtos científicos
isolados, não atribui níveis a componentes nem apresenta uma taxonomia de
maturidade como instrumento validado.

A redução de escopo continua sendo um requisito de projeto. Protótipos
iniciais devem focar em decisões para as quais reconstrução e contestação são
materialmente importantes, usar um registro delimitado de decisão e evidência,
separar saídas consultivas de IA de disposições humanas e remover elementos
que não melhorem a inspecionabilidade.

## 6. Plano de Avaliação

O programa de avaliação é organizado em torno da arquitetura integrada, ao
mesmo tempo que permanece controlado, conceitual, sintético e baseado em
artefatos. Ele avalia se a decomposição proposta torna autoridade,
dependências, registros, assistência consultiva e condições de contestação
mais inspecionáveis. Não avalia uma instituição em operação nem estabelece
legitimidade, justiça, responsabilização, efetividade da contestabilidade ou
remédio.

A fase inicial do estudo usaria cenários sintéticos de governança local
delimitada, pacotes de evidência controlados, registros simulados de
assistência por IA, erros plantados e um mock-up de alta fidelidade ou
interface "wizard-of-oz" de revisão, em vez de um ambiente institucional
ativo. Um protocolo pré-registrado definiria tarefas dos revisores e critérios
do estudo. São projetos propostos, não resultados reportados.

**RQ1: Rastreabilidade e reconstrução.** A estrutura em camadas de decisão e
evidência proposta ajuda revisores independentes a reconstruir decisões de
governança local delimitada envolvendo módulos de serviço funcional de forma
mais precisa e eficiente do que uma linha de base apenas documental? Critérios
ilustrativos incluem precisão e completude da reconstrução, visibilidade da
proveniência, detecção de conflitos de autoridade, detecção de evidência
ausente, tempo para reconstruir a justificativa e desacordo entre revisores.

**RQ2: Coerência entre camadas e condições de revisão.** Revisores
independentes conseguem usar a representação de seis camadas para identificar
autoridade faltante ou conflitante, dependências não declaradas, transições
entre camadas sem suporte e se um caminho de contestação acessível e condição
de independência de revisão estão especificados? Critérios ilustrativos
incluem consistência entre camadas, completude de dependências, detecção de
transições sem suporte, acessibilidade do caminho de contestação e
classificação correta de categorias possíveis de disposição. Essas medidas
testam condições que apoiam inspectabilidade e responsabilização ou
contestabilidade; não demonstram resposta institucional, contestação efetiva,
correção, reversão ou remédio.

**RQ3: Dependência humano-IA na revisão consultiva.** Para tarefas delimitadas
de análise de propostas, como proveniência e disposição humana obrigatória
afetam detecção de erros, confiança calibrada, comportamento de substituição,
qualidade da justificativa e qualidade da revisão? Registros simulados de IA
incluiríam erros plantados, casos ambíguos e recomendações contestadas.

Critérios ilustrativos incluem detecção de erro plantado e saída não suportada,
comportamento de substituição ou aceitação por condição, qualidade da
justificativa, desacordo entre revisores e correção após exibição de
informações de proveniência.

Para este artigo, uma linha de base apenas documental usa política e
documentação de registros estáticos sem a arquitetura de revisão em camadas
proposta, estrutura explícita de proveniência ou enquadramento de caminho de
contestação delimitado. Resultados negativos são tão relevantes quanto os
positivos: a representação pode não melhorar a reconstrução, pode aumentar a
carga de trabalho sem melhorar a detecção de erros, pode deixar
inconsistências entre camadas sem detecção, pode produzir desacordo sobre
condições de contestação ou pode não melhorar a confiança calibrada.

**Avaliação futura em estágios.** A avaliação deve progredir da inspeção de
artefatos controlados para estudos com revisores delimitados usando cenários
sintéticos, e então para avaliação de protótipo controlada sob um protocolo
aprovado separadamente. Qualquer estudo posterior situado institucionalmente
exigiria etapas adicionais de governança, ética, jurídicas, privacidade e
controle de evidência. A validade da prontidão para participação e a
responsabilização institucional mais ampla permanecem tópicos de pesquisa
futuros.

## 7. Limitações e Ameaças à Validade

Este artigo é conceitual e ainda mais amplo do que um artigo externo maduro
idealmente seria. A arquitetura pode aparentar coerência porque ainda não
enfrentou restrições de implementação, conflitos institucionais, pressão de
carga de trabalho ou condições de campo que testariam se os caminhos de
revisão propostos são viáveis através de decisões constitucionais e decisões
em domínios locais de governança delimitados.

A base de evidências pública para Axodus está atualmente limitada à
documentação de projeto. Não há resultados para avaliar viabilidade,
usabilidade, legitimidade da governança, confiança calibrada, caminhos de
contestação efetivos ou impacto social. O artigo não relata validação de
campo, validação situada institucionalmente, uso em produção, reivindicações
de projeto ou distribuição de token, reivindicações sobre operação financeira,
garantias de segurança ou conclusões legais ou regulatórias.

A supervisão humana pode tornar-se nominal quando revisores não dispõem de
tempo, autoridade, acesso às evidências ou poder prático para alterar o
resultado. A assistência de IA pode ser não confiável, difícil de calibrar ou
difícil de auditar sob carga de trabalho realista e pressão temporal.
Contestabilidade fraca ou caminhos de contestação mal projetados podem tornar
a rastreabilidade visível sem produzir resposta, capacidade corretiva,
remédio efetivo ou responsabilização institucional significativa.

Mecanismos de prontidão para participação apresentam riscos particulares de
exclusão, vigilância, captura interpretativa e confiança ilusória. A
separação modular também pode ocultar acoplamento sistêmico, enquanto
restrições constitucionais podem ser excessivamente rígidas ou ambíguas para
uma governança local efetiva. A arquitetura proposta pode ser complexa demais
para ser governada na prática sem uma redução substantiva de escopo.

O cenário sintético é explanatório e não empírico. O vocabulário de
proveniência não estabelece integridade do registro ou responsabilização, e
as medidas propostas avaliam reconstruibilidade, inspecionabilidade entre
camadas, condições de revisão e dependência limitada, em vez de legitimidade,
justiça, contestabilidade efetiva, remédio ou responsabilização institucional
plena. Decomposições alternativas podem se mostrar mais claras ou úteis do
que o modelo de seis camadas. Avaliações situadas institucionalmente também
podem expor conflitos, incentivos e efeitos de carga de trabalho que um
artefato controlado não consegue reproduzir.

O artigo não fornece consultoria financeira, de segurança, investimento ou
legal. Sua terminologia pode não se mapear perfeitamente para todas as
jurisdições ou comunidades de pesquisa.

## 8. Agenda de Pesquisa

Trabalhos de curto prazo devem priorizar a derivação e os artefatos de
interface, cenários sintéticos envolvendo domínios locais de governança
delimitados e tarefas de revisão adequadas para estudos de reconstrução,
coerência entre camadas, condições de contestação e dependência limitada.
Fortalecimento adicional da literatura sobre qualidade de governança,
independência do revisor, caminhos de contestação institucionais empíricos
e validade da prontidão para participação permanece como requisito posterior
antes de qualquer revisão externa mais ampla ser considerada.

## 9. Conclusão

Axodus é proposto como uma arquitetura conceitual em estágio de protótipo para
examinar como a governança assistida por humano-IA pode tornar-se mais
rastreável, reconstruível, passível de revisão e favorável à responsabilização
e contestabilidade em instituições digitais modulares federadas. Sua
contribuição não é um catálogo de produtos, reivindicação de estado de
implementação ou afirmação de uma decomposição unicamente correta, mas uma
arranjo inspecionável de seis camadas que liga restrições constitucionais,
domínios de governança local delimitados, módulos de serviço funcionais,
evidência e proveniência, assistência consultiva de IA e caminhos de revisão.

O próximo passo de pesquisa é instanciar a representação conceitual em um
ambiente experimental controlado e testar se revisores independentes conseguem
reconstruir decisões, identificar inconsistências entre camadas, inspecionar
condições de contestação e avaliar dependência limitada de IA. Esses resultados
testariam as condições de apoio propostas pela arquitetura; eles não
estabeleceriam, por si sós, legitimidade, remédio efetivo ou responsabilidade
institucional.

### Referências

As referências são mantidas em `references.bib`. Registros de verificação para
todas as entradas citadas são mantidos nos registros de controle da
bibliografia do repositório; é necessária uma rechecagem final dos metadados
antes de qualquer submissão, liberação pública ou circulação externa.
