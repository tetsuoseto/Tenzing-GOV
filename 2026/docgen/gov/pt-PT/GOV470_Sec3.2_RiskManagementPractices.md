##########
>white|orangered|left|14|30|hr Seção 3.2
### 3.2. Práticas de gerenciamento de riscos
>white|orangered|left|24|30|hb Práticas de gerenciamento de riscos

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informação-chave
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ A gestão de riscos de IA de propósito geral abrange uma variedade de práticas usadas para identificar, avaliar e reduzir riscos decorrentes de IA de propósito geral. Isso inclui testes e avaliações no nível do modelo (como “red-teaming”), processos organizacionais que orientam decisões de desenvolvimento e de liberação, salvaguardas condicionais (como compromissos “if-then”) e relatórios de incidentes.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Vários desenvolvedores de IA produziram Estruturas de Segurança de IA de Nível de Fronteira. Essas estruturas incluem informações sobre avaliações de risco e especificam medidas condicionais, como restrições de acesso que as empresas planejam implementar para modelos mais capazes. Elas variam nos riscos que abrangem, em como definem limites de capacidade e em quais ações são acionadas quando esses limites são atingidos.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ A evidência sobre a eficácia no mundo real das práticas de gestão de risco de IA ainda é limitada. A falta de notificação de incidentes e de monitoramento dificulta avaliar o desempenho das práticas atuais na redução de riscos ou o quanto elas são implementadas de forma consistente.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Desde a publicação do último Relatório (janeiro 2025), a gestão de riscos tornou-se mais estruturada por meio de novas iniciativas da indústria e de governança. Novos instrumentos como o Código de Prática para IA de Finalidade Geral da UE, o Quadro de Governança de Segurança de IA 2.0 da China e o Quadro de Relato do Processo de IA de Hiroshima do G7, em conjunto com iniciativas lideradas por empresas, ilustram a tendência em direção a abordagens mais padronizadas para transparência, avaliação e relato de incidentes.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ As dinâmicas de mercado e o ritmo do desenvolvimento de IA criam desafios adicionais. Devido às pressões competitivas, empresas de IA podem enfrentar trade-offs entre lançamentos de produtos mais rápidos e investimentos em esforços de redução de riscos. Muitos danos relacionados a IA também são externalizados, e a responsabilidade legal por eles permanece pouco clara, enquanto os processos de governança podem ser lentos para se adaptar às mudanças no cenário de IA.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Principais desafios para os formuladores de políticas incluem priorizar entre os diversos riscos apresentados pela IA de propósito geral e esclarecer quais atores ao longo da cadeia de valor da IA estão melhor posicionados para mitigá-los. Esses desafios são agravados pela visibilidade limitada sobre como os riscos são identificados, avaliados e gerenciados na prática, bem como pelo compartilhamento fragmentado de informações entre desenvolvedores, implantadores e provedores de infraestrutura.
>oldlace|black||11|15|br      


A gestão de riscos de IA abrange uma variedade de práticas que visam identificar, avaliar e reduzir a probabilidade e a gravidade dos riscos associados a sistemas de IA. Essas práticas podem ser implementadas por desenvolvedores de IA, implantadores, avaliadores e reguladores. Exemplos incluem modelagem de ameaças, classificação de riscos, red-teaming, auditoria e comunicação de incidentes. Esta seção descreve as práticas atuais de gestão de riscos, novos desenvolvimentos e limitações remanescentes.

Desde o início de 2025, várias novas iniciativas internacionais para a gestão de riscos de IA de propósito geral foram desenvolvidas, incluindo quadros de transparência organizacional e de reporte de riscos, bem como quadros regulatórios e de governança.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Figura 3.4: Quatro componentes da gestão de riscos
>white|black||9|11|br As quatro categorias de métodos para a gestão de riscos de IA de propósito geral: identificação de risco; análise e avaliação de risco; mitigação de risco; e governança de risco. Elas constituem um processo iterativo e cíclico. A governança de risco, mostrada no centro, facilita o sucesso dos outros componentes. Fonte: International AI Safety Report 2026.


Os desafios remanescentes incluem a padronização limitada, o que dificulta a conformidade e a avaliação, e a evidência limitada quanto à eficácia no mundo real. Além disso, os contextos institucionais, culturais e políticos diferem globalmente, o que implica que as abordagens para identificar e gerenciar riscos, incluindo limites de risco aceitáveis, podem variar entre regiões. A discussão desta seção sobre abordagens de gerenciamento de riscos é descritiva: tem como objetivo informar os atores do ecossistema de IA sobre as abordagens globais atuais para gerenciamento de riscos. Quando disponíveis, evidências sobre a eficácia e as limitações dessas abordagens são discutidas, mas recomendações de política não estão no escopo deste trabalho.

###@ Componentes da gestão de riscos

A gestão de riscos é um processo iterativo com práticas e métodos que abrangem todo o ciclo de desenvolvimento e implantação de IA, mas que funcionam juntos de forma coerente (‡969). A gestão de riscos para IA de uso geral pode incluir funções para uma ampla variedade de atores, incluindo cientistas de dados, engenheiros de modelos, auditores, especialistas de domínio, executivos, usuários finais, comunidades afetadas, fornecedores terceirizados, formuladores de políticas, governos, organizações de padrões e organizações da sociedade civil (‡970, ‡971, ‡972). As principais normas de gestão de riscos são frequentemente interoperáveis, mas usam terminologias diferentes para descrever os elementos da gestão de riscos (‡973, ‡974). Elas normalmente têm quatro componentes interconectados (Figura 3.4): identificar; analisar e avaliar; mitigar; e governar o risco (‡970, ‡973, ‡975, ‡976). As tabelas abaixo fornecem exemplos ilustrativos de métodos, técnicas e ferramentas relevantes. As práticas continuam a evoluir, portanto as tabelas não são exaustivas, e a aplicabilidade variará entre os contextos.

###@ Identificação de riscos

A identificação de riscos é o processo de encontrar, reconhecer e descrever riscos. Uma identificação de riscos abrangente normalmente inclui avaliações orientadas por capacidade, que testam se modelos possuem capacidades perigosas específicas (‡977), bem como modelagem de risco (‡978) e previsão (‡715*), que são usadas para explorar riscos existentes e emergentes. A Tabela 3.1 fornece vários exemplos de práticas de identificação de riscos. A identificação de riscos também se baseia na interação com especialistas e comunidades relevantes para entender o contexto mais amplo de como os riscos surgem (‡979, ‡980). Mecanismos como programas de bug bounty podem apoiar esse processo ao incentivar a identificação de vulnerabilidades anteriormente desconhecidas (‡981) (Tabela 3.1). Um objetivo-chave da identificação de riscos é considerar tanto riscos bem conhecidos e bem compreendidos quanto riscos futuros potenciais que permanecem incertos ou mal caracterizados (‡982). Isso é particularmente importante para IA de propósito geral, em que muitos riscos ainda podem não estar totalmente compreendidos ou observáveis (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Programas de bug bounty
  Programas de recompensa por bugs ou programas de divulgação responsável de vulnerabilidades incentivam as pessoas a encontrar e reportar vulnerabilidades em sistemas de IA. Vários desenvolvedores implementaram programas de recompensa por bugs (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Consulta especializada
  Especialistas do domínio, usuários e comunidades afetadas fornecem insights sobre riscos prováveis. Existem diretrizes emergentes para IA participativa e inclusiva (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Diagrama de Ishikawa (fishbone)
  Os diagramas de espinha de peixe são ferramentas bem estabelecidas de análise de causa raiz, e os pesquisadores propuseram utilizá-los para a análise estruturada de incidentes de risco de IA (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Previsão
  Previsão é o processo de prever eventos ou tendências futuras com base na análise de dados passados e atuais. Ela tem sido usada para comparar a probabilidade relativa de, por exemplo, diferentes resultados econômicos devido à IA avançada (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Taxonomia de riscos
  As taxonomias de risco são uma forma de categorizar e organizar riscos em múltiplas dimensões. Existem várias que descrevem riscos de IA de propósito geral (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Planejamento de cenários
  O planejamento de cenários envolve desenvolver cenários futuros plausíveis e analisar como os riscos se materializam. Isso tem sido usado para explorar os riscos e os impactos de modelos de IA (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modelagem de ameaças
  Modelagem de ameaças é um processo para identificar ameaças e vulnerabilidades para um sistema. Muitos desenvolvedores de IA destacam seu uso de modelagem de ameaças para antecipar cenários potenciais de uso indevido de sistemas de IA (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 3.1: Exemplos de identificação de riscos na gestão de riscos de IA de propósito geral
>white|black||9|11|br Exemplos de métodos para identificação de riscos de IA listados em ordem alfabética. Os métodos incluídos
são projetados para apoiar a identificação de riscos para muitos tipos diferentes de risco, incluindo riscos decorrentes de uso malicioso, riscos decorrentes de mau funcionamento e riscos sistêmicos. Dada a natureza ainda incipiente da gestão de riscos de IA de propósito geral, nem todos os métodos serão adequados para todo desenvolvedor ou implantador de IA.


>white|orangered|left|14|15.5|bb Modelagem de ameaças e taxonomias de risco são métodos proeminentes de identificação de riscos

Dois métodos de destaque para identificar os riscos de IA de propósito geral são a modelagem de ameaças do International AI Safety Report 2026 (um processo estruturado para mapear como os riscos relacionados a IA podem se materializar) e taxonomias de risco. A Meta, por exemplo, usa exercícios de modelagem de ameaças para antecipar cenários potenciais de uso indevido de seus modelos de IA (‡990), e a Anthropic inclui modelagem de ameaças como parte de seu ASL-3 Deployment Standard (‡991). Taxonomias de risco e de perigos em IA, que listam categorias de risco e exemplos, podem igualmente servir como ponto de partida para conceituar, identificar e especificar os riscos relevantes associados à IA de propósito geral em domínios de aplicação específicos (‡906, ‡988, ‡992, ‡993).

###@ Análise e avaliação de riscos

A análise e avaliação de risco é o processo de determinar o nível de risco de um modelo ou sistema de IA e compará-lo com critérios estabelecidos para avaliar a aceitabilidade ou a necessidade de mitigação (‡994, ‡995, ‡996, ‡997). Ela inclui práticas como medir o desempenho do modelo em benchmarks (‡998) e avaliações (‡176, ‡715), realizar exercícios de red-teaming (‡999*), avaliações de impacto (‡1000) e auditorias (‡1001, ‡1002). Veja a Mesa 3.2 para exemplos de análise e avaliação de risco de IA de propósito geral. Os métodos são projetados para apoiar análise e avaliação simultâneas para muitos tipos diferentes de risco.

Os principais objetivos da análise e avaliação de risco são realizar avaliações das capacidades e vulnerabilidades do modelo (‡1003), aproveitar uma modelagem de risco robusta para orientar decisões sobre limiares de risco (‡1004, ‡1005) e compreender como os sistemas de IA são usados na prática, a fim de avaliar impactos sociais a jusante (‡869, ‡904, ‡905, ‡1006). Os processos de análise e avaliação de risco frequentemente são considerados mais propensos a identificar riscos quando incorporam revisão independente (‡1001, ‡1007), recorrem a expertise intersetorial (‡1008) e incluem perspectivas diversas de múltiplos domínios e disciplinas, bem como de comunidades afetadas (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Auditorias
  As auditorias são avaliações formais do desempenho e dos impactos dos modelos de IA e/ ou da conformidade de uma organização com padrões, políticas e procedimentos, realizadas internamente ou por uma parte externa. A auditoria de IA é um campo em crescimento, e existem inúmeras ferramentas e práticas para auditar modelos de IA e as práticas dos desenvolvedores de modelos de IA (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Benchmarks
  Os benchmarks são testes ou métricas quantitativos e padronizados, frequentemente, usados para avaliar e comparar o desempenho de sistemas de IA em um conjunto fixo de tarefas projetadas para representar o uso no mundo real (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Método Bowtie
  O método do laço-borboleta é um método bem conhecido para visualizar onde controles podem ser adicionados para mitigar eventos de risco. Ele fornece uma diferenciação clara entre a gestão de risco proativa e reativa (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Método de Delphi
  O método Delphi é uma técnica de tomada de decisão em grupo que utiliza uma série de questionários para reunir consenso a partir de um painel de especialistas (‡1020, ‡1021). Ele tem sido usado para ajudar a explorar futuros possíveis com IA avançada (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Testes de campo
  A validação em campo avalia o desempenho e o impacto de um sistema de IA em um ambiente operacional real. Algumas pesquisas enfatizam a validação em campo como um complemento à avaliação do modelo para avaliar resultados e consequências no mundo real (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Avaliação de impacto
  As avaliações de impacto avaliam os potenciais impactos de uma tecnologia ou projeto. Isso pode incluir quantificar, agregar e priorizar impactos. O EU AI Act, por exemplo, exige que os desenvolvedores de sistemas de IA de alto risco realizem Avaliações de Impacto sobre Direitos Fundamentais (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Avaliação do modelo
  As avaliações de modelos incluem processos e testes para avaliar e medir o desempenho de um modelo de IA em uma tarefa específica. Há inúmeras avaliações de IA para avaliar diferentes capacidades e riscos, incluindo para segurança, segurança da informação e impacto social (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Avaliação probabilística de riscos
  A avaliação de risco probabilística é uma metodologia para avaliar riscos associados a sistemas ou processos complexos que incorpora incerteza. Ela foi adaptada para sistemas avançados de IA (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Red teaming
  Red-teaming é um exercício em que um grupo de pessoas ou sistemas automatizados fingem ser um adversário e atacam os sistemas tecnológicos de uma organização para identificar vulnerabilidades. Numerosas empresas de IA têm práticas internas para red-teaming de sistemas de IA (‡458, ‡1028). O red-teaming também pode ser conduzido por agentes fora das empresas. Essas equipes enfrentam desafios como acesso limitado, mas também podem revelar percepções distintas (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Matrizes de risco
  As matrizes de risco são uma ferramenta visual para ajudar a priorizar riscos de acordo com a sua probabilidade de ocorrência e o seu potencial impacto (‡1027). Alguns desenvolvedores de IA incluem matrizes de risco básicas nos seus Frameworks de Segurança para IA Frontier (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Limiares de risco/ níveis de risco
  Os limiares ou níveis de risco são limites quantitativos ou qualitativos que distinguem riscos aceitáveis de inaceitáveis e acionam ações específicas de gestão de risco quando são excedidos. Para IA de propósito geral, eles são determinados por uma combinação de capacidades, impacto, computação, alcance e outros fatores (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tolerância ao risco
  A tolerancia ao risco refere-se ao nível de risco que uma organização está disposta a aceitar. Em IA, as tolerâncias ao risco são frequentemente definidas de forma implícita por meio de políticas e práticas da empresa, enquanto alguns regimes regulatórios definem explicitamente riscos inaceitáveis e impõem consequências legais (‡1032). Algumas empresas descrevem sua tolerância ao risco em termos do risco marginal de um novo modelo; isto é, a extensão em que um modelo aumenta contrafactualmente o risco além do já imposto por modelos existentes ou outras tecnologias (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Casos de segurança
  Um safety case é uma argumentação estruturada, suportada por evidências, de que um sistema é suficientemente seguro para operar em um contexto específico. A literatura recente (‡1037, ‡1038, ‡1039) explorou safety cases para sistemas de IA de fronteira, e certos Frontier AI Safety Frameworks os referenciam (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Análise de segurança do sistema
  A análise de segurança do sistema destaca dependências entre componentes e o sistema do qual fazem parte, a fim de antecipar como perigos em nível de sistema podem surgir a partir de falhas de componentes ou processos, ou de interações entre subsistemas, fatores humanos e condições ambientais. Abordagens aplicadas para sistemas de IA na literatura incluem análise de processos baseada em teoria de sistemas (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 3.2: Análise/avaliação de riscos na gestão de riscos de IA de propósito geral
>white|black||9|11|br Exemplos de métodos para análise/avaliação de risco de IA, listados em ordem alfabética. Dada a natureza incipiente da gestão de riscos de IA de propósito geral, nem todos os métodos serão adequados para todo desenvolvedor ou implantador de IA.


>white|orangered|left|14|15.5|bb As ferramentas comuns de análise de riscos incluem benchmarks e avaliações de modelos

Benchmarks e avaliações de modelo são testes padronizados para avaliar o desempenho de sistemas de IA de propósito geral em tarefas específicas. Pesquisadores desenvolveram uma ampla variedade de benchmarks e avaliações, incluindo conjuntos de perguntas de múltipla escolha desafiadoras, problemas de engenharia de software e tarefas relacionadas ao trabalho em ambientes de escritório simulados (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Avaliações de capacidades prejudiciais (‡715) são usadas para avaliar se um modelo ou sistema de IA de propósito geral possui conhecimentos ou habilidades particularmente perigosos, como a capacidade de ajudar em ciberataques (ver §2.1.3. Ciberataques).

Decisões de alta relevância por empresas e governos sobre liberações de modelos baseiam-se parcialmente nessas avaliações (‡1050, ‡1051, ‡1052). No entanto, os benchmarks variam significativamente em qualidade e escopo (‡998, ‡1003), e pode ser difícil julgar sua validade devido a inúmeras deficiências nas práticas de benchmarking (‡902, ‡909, ‡1003, ‡1053*). Por exemplo, benchmarks podem se tornar ‘saturados’ – quando as pontuações de muitos modelos se aproximam da pontuação mais alta – o que significa que eles já não distinguem com força os modelos. Os modelos também têm maior probabilidade de identificar certas tarefas como avaliações e exibir comportamentos diferentes do que exibiriam em tarefas semelhantes em contextos de implantação devido à ‘consciência situacional’ (veja §2.2.2. Perda de controle). Por fim, benchmarks e avaliações têm limitações amplamente documentadas: notadamente, eles não conseguem capturar riscos associados ao uso de IA de propósito geral em domínios novos e para tarefas inéditas, já que as condições de teste diferem do uso no mundo real em graus variados (‡913) (veja §1.2. Capacidades atuais e §3.1. Desafios técnicos e institucionais).

>white|orangered|left|14|15.5|bb Red teaming permite avaliações de risco mais específicas do domínio

Outro método comum para avaliar riscos é o red-teaming. Uma ‘equipe vermelha’ é um grupo de avaliadores encarregado de procurar vulnerabilidades, limitações ou potencial de uso indevido. O red-teaming pode ser específico de um domínio e realizado por especialistas do domínio, ou aberto para explorar novos fatores de risco. Por exemplo, uma equipe vermelha pode explorar ataques de ‘jailbreaking’ que subvertem as restrições de segurança do modelo (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). Em contraste com benchmarks, uma vantagem importante do red-teaming é que as equipes vermelhas podem adaptar suas avaliações ao sistema específico que está sendo testado. Por exemplo, as equipes vermelhas podem projetar entradas personalizadas para identificar comportamentos no pior caso, oportunidades de uso malicioso e falhas inesperadas. No entanto, pode exigir acesso especial aos modelos e pode falhar ao evidenciar classes importantes de riscos (‡999, ‡1028).

Importantly, a ausência de riscos identificados não implica que esses riscos sejam baixos: trabalhos anteriores mostram que bugs frequentemente escapam à detecção, especialmente quando as equipes de red teaming têm acesso ou recursos limitados (‡1060). A pesquisa também tem questionado se o red teaming pode produzir resultados confiáveis e reproduzíveis (‡1061). A composição da equipe de red teaming e as instruções fornecidas aos red-teamers (‡1062), o número de rodadas de ataque (‡1063) e o acesso do modelo a ferramentas (‡1064, ‡1065) podem influenciar significativamente os resultados, incluindo a superfície de risco coberta. Diretrizes abrangentes sobre red teaming buscam abordar alguns desses desafios (‡1066).

###@ Mitigação de riscos

A mitigação de riscos é o processo de priorizar, avaliar e implementar controles e contramedidas para reduzir os riscos identificados. Exemplos incluem controles de acesso (‡991), monitoramento contínuo (‡986) e compromissos if-then (‡700). Mitigar o risco levanta uma questão-chave: qual é o nível de risco aceitável? Frameworks recentes e políticas da empresa começaram a formalizar critérios de “aceitação de risco” (‡965, ‡1040). No entanto, definir limites apropriados continua sendo desafiador, especialmente para riscos com amplos impactos sociais (‡986, ‡1067). Atualmente, não existe nenhum mecanismo estabelecido para validar decisões de aceitação de risco feitas por desenvolvedores antes do lançamento (‡1005).

Os métodos de mitigação de risco descritos na Tabela 3.3 abaixo são adaptáveis e podem mitigar uma variedade de riscos, incluindo alguns riscos inesperados. A tabela não inclui métodos técnicos de mitigação, como treinamento adversarial, filtros de conteúdo e monitoramento de chain-of-thought. Estes são abordados em §3.3. Proteções técnicas e monitoramento, bem como ao longo do Relatório nos parágrafos de ‘Mitigações’ para cada risco em §2. Riscos.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Políticas de uso aceitável
  Uma política de uso aceitável é um conjunto de regras e diretrizes para o uso responsável, ético e legal de modelos de IA. É comum que desenvolvedores de IA publiquem políticas de uso aceitável, bem como políticas de uso proibido, com novos lançamentos de modelo (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Controle de acesso/validação de usuários
  Os controles de acesso incluem o uso de políticas e regras para restringir o acesso a modelos de IA, dados e sistemas com base em funções do usuário, atributos e outras condições, a fim de impedir o uso não autorizado, a manipulação ou violações de dados. As empresas de IA frequentemente desabilitam contas encontradas como envolvidas em atividade criminal (‡486) e incluem verificações de diligência do usuário e triagens de Conheça-Seu-Cliente para garantir que os modelos sejam usados apenas por atores confiáveis (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Especificação de comportamento/modelo
  Uma especificação de comportamento de IA é um documento que define como um modelo de IA deve se comportar em diversas situações. Ela serve como um modelo para alinhamento e segurança de IA, orientando o desenvolvimento do modelo, treinamento, avaliação e saídas. Várias empresas de IA usam documentos de especificação de modelos e tornam pelo menos partes deles públicas (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitoramento contínuo
  O monitoramento contínuo é o processo contínuo, automatizado, de observar, analisar e controlar sistemas de IA em uso, acompanhando seu desempenho e limitando seu comportamento para garantir confiabilidade, eficácia e segurança. Há inúmeras ferramentas disponíveis para monitoramento contínuo (‡1073*) bem como técnicas para apoiar
observabilidade de IA (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Defesa em profundidade
  Defesa em profundidade é a ideia de que várias camadas de defesa independentes e sobrepostas podem ser implementadas de modo que, se uma falhar, as outras ainda serão eficazes (‡1075, ‡1076). Múltiplos Frameworks de Segurança de IA para a Fronteira fazem referência a isso (por exemplo, (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitoramento de ecossistema
  Este é o processo de monitoramento do ecossistema mais amplo de IA, incluindo rastreamento de computação e hardware, proveniência do modelo, proveniência dos dados e padrões de uso. A literatura de pesquisa discute tal monitoramento em relação a riscos provenientes de IA de propósito geral (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Compromissos condicionais (se-entao)
  Os compromissos condicionais (if-then) são um conjunto de protocolos técnicos e organizacionais, bem como de compromissos para gerenciar riscos à medida que os modelos de IA se tornam mais capazes. Vários desenvolvedores de IA empregam esses tipos de compromissos como parte de seus Frameworks de Segurança de IA de Fronteira (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Linhas vermelhas ou proibições
  As linhas vermelhas são limites específicos expressos como capacidades, impacto ou tipos de uso. O conceito aparece em declarações públicas e iniciativas, bem como em proibições regulatórias (‡1079, ‡1080, ‡1081). A literatura também observa limitações de abordagens baseadas em linhas vermelhas, incluindo desafios em torno de consenso e exequibilidade.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Estratégias de lançamento e implantação
  As estratégias de lançamento e implantação para IA de propósito geral podem incluir o uso de lançamentos em etapas ou acesso via API para que haja mais opções de mitigação disponíveis no caso de uso indevido ou dano inesperado (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 3.3: Mitigação de riscos na gestão de riscos de IA de uso geral
>white|black||9|11|br Exemplos de métodos para mitigação de risco de IA listados em ordem alfabética. Os métodos incluídos são projetados para apoiar a mitigação de riscos para muitos tipos diferentes de risco simultaneamente, incluindo riscos de uso malicioso, riscos de mau funcionamento e riscos sistêmicos. Dada a natureza incipiente da gestão de risco de IA de propósito geral, nem todos os métodos serão adequados para todo desenvolvedor ou implantador de IA.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Figura 3.5: Um diagrama de “queijo suíco” ilustrando a abordagem de defesa em profundidade
>white|black||9|11|br Múltiplas camadas de defesas podem compensar falhas em camadas individuais. As técnicas atuais de gerenciamento de risco para IA têm falhas, mas colocá-las em camadas pode oferecer uma proteção muito mais forte contra riscos. Fonte: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Estratégias de defesa em profundidade e de liberação são ferramentas importantes de mitigação

Um modelo de “defesa em profundidade” pode apoiar a gestão de riscos de IA de propósito geral. Neste contexto, “defesa em profundidade” refere-se a uma combinação de medidas técnicas, organizacionais e societais aplicadas em diferentes etapas do desenvolvimento e da implantação (Figura 3.5). Isso significa criar camadas de salvaguardas independentes, de modo que, se uma camada falhar, as demais camadas ainda possam prevenir danos. Um exemplo frequentemente citado de um modelo de defesa em profundidade é o conjunto de medidas preventivas implantadas para prevenir doenças infecciosas. Vacinas, máscaras e lavagem das mãos, entre outras medidas, podem reduzir substancialmente o risco de infecção em conjunto, mesmo que nenhum desses métodos seja 100% eficaz por si só (‡1083*). Para IA de propósito geral, a defesa em profundidade incluirá controles que não estão no próprio modelo de IA, mas sim no ecossistema mais amplo. Isso inclui (por exemplo) controles sobre os materiais necessários para executar um ataque biológico, como reagentes (‡1084, ‡1085). No entanto, as medidas de defesa em profundidade abordam principalmente riscos relacionados a acidentes, mau funcionamento e uso malicioso, e podem ter um papel menor na gestão de riscos sistêmicos (ver §3.5. Construindo resiliência societal).

A estratégia de lançamento e implantação de uma empresa é um componente importante da mitigação de riscos. As decisões sobre como os modelos são disponibilizados aos usuários podem afetar substancialmente a exposição a riscos (‡1082). Diferentes opções de lançamento e implantação incluem lançamento em etapas para grupos limitados de usuários, acesso por meio de serviços online controlados (como APIs) e o uso de acordos de licenciamento e políticas de uso aceitável que, legalmente, proíbem certas aplicações prejudiciais (‡176, ‡1086, ‡1087). §3.4. Modelos de pesos abertos discute com mais detalhes como a disponibilização dos pesos do modelo afeta os riscos.

###@ Governança de riscos

A governança de riscos é o processo pelo qual as avaliações, decisões e ações de gestão de riscos são conectadas à estratégia e aos objetivos de uma organização ou de outra entidade (‡1088, ‡1089). A Tabela 3.4 fornece uma visão geral de técnicas comuns de governança de riscos. Conforme mostrado na Figura 3.4, a governança de riscos pode ser entendida como o núcleo da gestão de riscos, pois facilita a operação eficaz de outros componentes da gestão de riscos. Ela proporciona responsabilização, transparência e clareza que apoiam decisões informadas de gestão de riscos. A governança de riscos pode incluir práticas como comunicação de incidentes (‡1090), alocação de responsabilidades de risco (‡965) e proteção a denunciantes (‡1091). De forma mais ampla, a governança de riscos pode incluir orientações, estruturas, legislação, regulamentação, padrões nacionais e internacionais, bem como iniciativas de treinamento e educação. Um propósito-chave da governança de riscos é estabelecer políticas e mecanismos organizacionais que esclareçam como as responsabilidades pela gestão de riscos são alocadas em toda a organização ou em outra entidade, a fim de apoiar a supervisão e a responsabilização apropriadas (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Documentação
  As práticas de documentação ajudam a rastrear informações-chave sobre sistemas de IA, como dados de treinamento, escolhas de design, usos pretendidos, limitações e riscos. ‘Model cards’ e ‘system cards’, que fornecem informações sobre como um modelo ou sistema de IA foi treinado e avaliado, são exemplos de práticas recomendadas proeminentes de documentação de IA (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Relato de incidentes
  A comunicação de incidentes é o processo de documentar e compartilhar sistematicamente casos nos quais a criação ou a implantação de IA causou dano direto ou indireto. Existem várias plataformas que facilitam a comunicação de incidentes para IA (‡1096, ‡1097) e frameworks para facilitar uma comunicação de incidentes de IA mais eficaz (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Estruturas de gerenciamento de riscos
  As estruturas de gestão de riscos são planos organizacionais para reduzir lacunas na cobertura de riscos, coordenar várias atividades de gestão de riscos e implementar verificações e contrapesos. Estruturas específicas para IA de uso geral (‡986, ‡1098) frequentemente fazem referência a outras medidas mencionadas nesta seção.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Matriz de riscos
  Um registro de riscos é um repositório de vários riscos, sua priorização, responsáveis e planos de mitigação. Esses itens são relativamente comuns em muitas indústrias, incluindo segurança cibernética (‡1099), e às vezes são usados para atender a requisitos de conformidade regulatória.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Alocação de responsabilidade pelos riscos
  A alocação de funções e responsabilidades para a gestão de riscos dentro de uma organização pode estruturar a supervisão interna da tomada de decisões (‡1002, ‡1093). Esses arranjos são refletidos em alguns frameworks de governança, incluindo o Código de Prática de IA de Finalidade Geral da UE (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Relatórios de transparência
  Os relatórios de transparência descrevem as práticas de gerenciamento de risco de uma empresa de IA ao divulgar publicamente certas informações ou ao compartilhar documentação com grupos da indústria ou órgãos governamentais. Por exemplo, diversas empresas de IA enviam relatórios de transparência Hiroshima AI Process (HAIP) (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Proteção ao denunciante
  Como grande parte do desenvolvimento de IA ocorre em portas fechadas, alguns frameworks de governança incluem proteções a denunciantes para permitir a divulgação de potenciais riscos às autoridades (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 3.4: Governança de riscos na gestão de riscos de IA de propósito geral
>white|black||9|11|br Exemplos de métodos para governança de riscos de IA listados em ordem alfabética. Os métodos incluídos foram projetados para apoiar a governança de riscos para muitos tipos diferentes de risco simultaneamente, incluindo riscos de uso malicioso, riscos de mau funcionamento e riscos sistêmicos. Dada a natureza incipiente da gestão de riscos de IA de uso geral, nem todos os métodos serão adequados para todo desenvolvedor ou implantador de IA.


>white|orangered|left|14|15.5|bb A documentação e a transparência são componentes da governança de riscos

Mecanismos de documentação e de transparência institucional, juntamente com práticas de compartilhamento de informações, facilitam a fiscalização externa e apoiam esforços para gerenciar riscos associados à IA de propósito geral (‡1101, ‡1102). Tornou-se prática comum publicar os resultados de testes pré-implantação em um “model card” ou “system card”, juntamente com detalhes básicos sobre o modelo ou sistema, incluindo como ele foi treinado e quais são suas limitações potenciais (‡1094, ‡1095). Alguns desenvolvedores também publicam relatórios de transparência que incluem detalhes sobre suas práticas de gerenciamento de riscos de forma mais ampla (‡1103). Outros elementos de documentação e transparência incluem monitoramento e comunicação de incidentes (‡176, ‡1083*, ‡1103) e compartilhamento de informações, que podem ser viabilizados por terceiros, como o Frontier Model Forum. Alguns marcos regulatórios, como o EU AI Act ou a California’s Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), em certos casos exigem o compartilhamento de informações sobre riscos de IA de propósito geral.

>white|orangered|left|14|15.5|bb O comprometimento da liderança e os incentivos moldam as práticas de gerenciamento de riscos

A cultura organizacional, a estrutura de liderança e os incentivos afetam os esforços de gestão de riscos de diversas maneiras (‡1105). O compromisso da liderança e as estruturas de incentivos são frequentemente relevantes para o modo como as políticas de gestão de riscos operam na prática. Alguns desenvolvedores têm painéis internos de tomada de decisão que deliberam sobre como projetar, desenvolver e revisar novos sistemas de IA de forma segura e responsável. Comitês de supervisão e assessoria, trusts, ou conselhos de ética em IA também podem servir como mecanismos para orientação de gestão de riscos e supervisão organizacional (‡1092*, ‡1106, ‡1107, ‡1108). Pesquisadores argumentaram que desafios associados à autogovernança voluntária significam que auditorias, verificação e padronização por terceiros poderiam ajudar a fortalecer a gestão de riscos de IA de propósito geral (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Gestão de riscos organizacionais, transparência e estruturas de reporte de riscos

Várias novas iniciativas concentram-se em processos de gestão de risco, documentação e transparência. Na sua forma atual, o Código de Prática da UE para IA de Fins Gerais funciona como um quadro voluntário para orientar práticas de transparência, direitos autorais e segurança e segurança de software, a fim de apoiar a conformidade com as disposições do AI Act da UE para IA de fins gerais (‡965). Em dezembro de 2025, mais de duas dezenas de empresas† assinaram. O Quadro de Relato do Processo de IA de Hiroshima do G7 (HAIP) (‡1100) é o primeiro quadro internacional para relato público voluntário de práticas organizacionais de gestão de risco para sistemas avançados de IA. Pelo menos 20 desenvolvedores publicaram relatórios públicos de transparência que abrangem identificação de riscos, métricas de avaliação, estratégias de mitigação e processos de segurança de dados.

Os desenvolvedores de IA adotaram compromissos voluntários de transparência. Na China, compromissos de 17 empresas chinesas de IA, coordenados pela AI Industry Alliance of China, foram divulgados em dezembro de 2024 (‡1113) e atualizados em 2025 (‡1114). Na Cúpula de IA de Seul de maio de 2024, na Coreia do Sul, 16 desenvolvedores de IA de vários países assinaram compromissos voluntários para publicar Frontier AI Safety Frameworks para seus modelos e sistemas mais capazes e para adotar práticas de gerenciamento de risco em todas as etapas de desenvolvimento e implantação de modelos (‡1052).

    Nota † -- Os signatários em  dezembro de 2025 incluem: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing e WRITER.

>white|orangered|left|14|15.5|bb As estruturas de segurança de IA da Frontier tornaram-se uma abordagem organizacional proeminente para a gestão de riscos de IA

Desde 2023, vários desenvolvedores de IA de fronteira publicaram voluntariamente documentos descrevendo como planejam identificar e responder a riscos sérios provenientes de seus sistemas mais avançados. Essas Estruturas de Segurança de IA de Fronteira descrevem como um desenvolvedor de IA planeja avaliar, monitorar e controlar seus modelos e sistemas de IA mais avançados antes e durante a implantação. Essas estruturas compartilham muitas semelhanças, mas diferem em aspectos-chave (‡1115, ‡1116). A maioria se concentra em riscos associados a ameaças químicas, biológicas, radiológicas e nucleares (CBRN), capacidades cibernéticas avançadas e comportamento autônomo avançado (‡1115, ‡1117). Uma minoria das estruturas aborda domínios adicionais de risco, como discriminação ilícita em escala e exploração sexual de crianças.

Vários desenvolvedores atualizaram seus frameworks em 2025, adicionando novas seções sobre manipulação nociva, risco de desalinhamento e replicação e adaptação autônomas (‡1078, ‡1118). Embora muitos frameworks descrevam abordagens de gerenciamento de risco semelhantes – incluindo modelagem de ameaças, red-teaming e avaliações de capacidades perigosas – eles variam em suas definições de níveis e limiares de risco, a frequência das avaliações, as margens entre as avaliações e os limiares e a abrangência de seus compromissos de mitigação (por exemplo, se incluem excluir pesos do modelo versus apenas pausar o desenvolvimento) (‡1115, ‡1119). Veja a Mesa 3.5 para mais informações.

>white|orangered|left|14|15.5|bb Muitas ações nos Frameworks de Segurança de IA da Frontier se baseiam em compromissos do tipo se-então

Uma parte fundamental dos Frameworks de Segurança da Frontier AI são os “compromissos if-then”. Estes são protocolos condicionais que acionam respostas específicas quando modelos e sistemas de IA atingem limiares de capacidade predefinidos (‡1120). Por exemplo, um compromisso if-then poderia afirmar que, se for constatado que um modelo tem a capacidade de auxiliar de forma significativa iniciantes na criação e no emprego de armas de CBRN, então o desenvolvedor implementará medidas de segurança aprimoradas, controles de implantação e monitoramento em tempo real (‡991*).

Em 2025, vários desenvolvedores de IA anunciaram que novos modelos acionaram alertas antecipados de aviso, ou que não podiam descartar a possibilidade de que, após uma avaliação adicional, ficasse demonstrado que os modelos haviam ultrapassado limites de capacidade. Isso os levou a aplicar salvaguardas reforçadas como medida de precaução (‡7, ‡33, ‡1121*). Frameworks de Segurança de IA de ponta comumente exigem uma avaliação inicial de capacidades antes da mitigação de riscos, bem como uma análise de risco residual ou um caso de segurança, frequentemente informado por red teaming, após a mitigação. Veja a Mesa 3.5 para informações detalhadas.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Estrutura de Preparação 2 (‡1078*)
  Riscos cobertos:
1. Capacidades biológicas e químicas
2. Capacidades de cibersegurança
3. Capacidades de autoaperfeiçoamento da IA
  Níveis de risco ou equivalente e salvaguardas associadas:
- Alto: poderia ampliar os caminhos existentes para causar danos graves (exige controles de segurança e salvaguardas)
- Crítico: Poderia introduzir caminhos novos e sem precedentes para causar danos graves (Interromper o desenvolvimento adicional até que as salvaguardas especificadas e os padrões de controles de segurança atendam a um padrão Crítico)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Política de Escalonamento Responsável 2.2 (‡991*)
  Riscos cobertos:
1. Armas CBRN
2. Pesquisa e desenvolvimento (P&D) autônomos de IA (IA P&D)
3. Operações cibernéticas (em avaliação)
  Níveis de risco ou equivalente e salvaguardas associadas:
  Níveis de Segurança de IA (ASL)
- ASL-1: Sem risco catastrófico significativo
- ASL-2: Sinais iniciais de capacidades perigosas (Os modelos devem atender aos Padrões de Implantação e Segurança ASL-2)
- ASL-3: Risco substancialmente aumentado de uso catastrófico indevido (Os Modelos devem atender aos Padrões de Implantação e/ ou Segurança ASL-3)
- ASL-4+: Futuras classificações (ainda não definidas)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Riscos cobertos:
1. Uso indevido
    a. CBRN
    b. Cyber
    c. Manipulação prejudicial
2. Pesquisa e Desenvolvimento em Aprendizado de Máquina
3. Desalinhamento/ raciocínio instrumental
  Níveis de risco ou equivalente e salvaguardas associadas:
  Níveis de Capacidade Crítica
    Níveis de capacidade nos quais, na ausência de medidas de mitigação (casos de segurança para implantações e mitigações de segurança alinhadas com os níveis de segurança 2, 3 ou 4 da RAND (‡1122)), modelos ou sistemas de IA podem representar risco elevado de causar dano grave. Os níveis de capacidade incluem “avaliações de alerta precoce”, com “limiares de alerta” específicos
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Framework de IA de Vanguarda 1.1 (‡990*)
  Riscos cobertos:
1. Cibersegurança
2. Riscos químicos e biológicos
  Níveis de risco ou equivalente e salvaguardas associadas:
  Níveis de Limite de Risco
- Moderado (liberação com medidas de segurança e mitigações apropriadas)
- igh (não liberar)
- Crítico (parar o desenvolvimento)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Estrutura de Segurança do Modelo de Fronteira (‡1123*)
  Riscos cobertos:
1. Proliferação de armas CBRN
2. Operações cibernéticas ofensivas
3. Pesquisa e Desenvolvimento (P&D) Automatizada em IA
  Níveis de risco ou equivalente e salvaguardas associadas:
  Limiar de Capacidades Críticas
    Capacidades do modelo que têm potencial para causar danos significativos ao público se forem utilizadas de forma inadequada. (Se os limiares forem atingidos ou excedidos, o modelo não será disponibilizado publicamente sem as medidas de mitigação de risco adequadas)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Estrutura de Governança do Frontier (‡1124*)
  Riscos cobertos:
1. Armas CBRN
2. Operações cibernéticas ofensivas
3. Autonomia avançada (incluindo P&D de IA)
  Níveis de risco ou equivalente e salvaguardas associadas:
  Níveis de Risco
- Baixo ou Médio (implantação permitida de acordo com os requisitos do Programa de IA Responsável)
- Alto ou Crítico (Revisão adicional e mitigação
(necessário)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Avaliação de Risco de IA da Frontier (‡1029*)
  Riscos cobertos:
1. crime cibernético
2. CBRN
3. Persuasão e manipulação
4. Discriminação ilícita em escala
  Níveis de risco ou equivalente e medidas de salvaguarda associadas:
  Limiar de risco – pontuações de risco do modelo (MR)
- MR1 ou MR2 (Os resultados de avaliação são documentados pelas equipes de engenharia)
- MR3 (As medidas de mitigação de riscos e os resultados da avaliação são documentados pelas equipes de engenharia e revisados periodicamente)
- MR4 (Uma avaliação de risco detalhada deve ser concluída e a aprovação do líder da unidade de negócio é necessária)
- MR5 (Uma avaliação de risco detalhada deve ser concluída e aprovada por um comitê independente, por exemplo, o comitê de ética em IA da NVIDIA)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Framework de Modelo de Fronteira de IA Segura (‡1125*)
  Riscos cobertos:
1. Uso malicioso (por exemplo, malware, exploração sexual infantil)
2. Dano no uso ordinário e não malicioso, por exemplo, resultados que levem a uma discriminação ilegal ou à geração de código inseguro
  Níveis de risco ou equivalente e salvaguardas associadas:
  Probabilidade e Severidade do Dano no Contexto
- Baixo
- Médio
- Alto
- Muito Alto
    (Mitigação de riscos e controles de segurança estão implementados para todos os sistemas e processos; são necessárias mitigação adicionais para serem adaptadas ao sistema de IA e ao caso de uso em que um modelo é implantado)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: Política de prontidão para AGI (‡1127*)
  Riscos cobertos:
1. crime cibernético
2. Pesquisa e Desenvolvimento (P&D) Automatizada em IA
3. Replicação e adaptação autônomas
4. Assistência a armas biológicas
  Níveis de risco ou equivalente e salvaguardas associadas:
  Limiar de Capacidades Críticas
    Limiares quantitativos em benchmarks de capacidade (se ultrapassados, conduza avaliações de capacidade perigosas, medidas de segurança da informação e mitigações de implantação, ou interrompa o desenvolvimento)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Política de Prontidão para AGI da Magic (‡1127*)
  Riscos cobertos:
1. crime cibernético
2. Pesquisa e Desenvolvimento (P&D) Automatizada em IA
3. Replicação e adaptação autônomas
4. Assistência a armas biológicas
  Níveis de risco ou equivalente e salvaguardas associadas:
  Limiar de Capacidades Críticas
    Limiares quantitativos em benchmarks de capacidade (Se forem excedidos, conduza avaliações perigosas de capacidade, medidas de segurança da informação e mitigações de implantação, ou suspenda o desenvolvimento)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: Estrutura de Segurança de IA (‡1128*)
  Riscos cobertos:
1. Perda de controle
2. Uso indevido (por exemplo, armazenamento bioquímico
  Níveis de risco ou equivalente e salvaguardas associadas:
  Níveis de Risco
- Baixo risco (Implantar sistemas de IA, mas realizar monitoramento posteriormente para gerenciar riscos)
- Risco identificado (ou expor apenas sistemas de IA da OpenAI a utilizadores autorizados para mitigar riscos, ou adiar a implementação até serem tomadas medidas adicionais de segurança, dependendo do caso de uso)
- Alto risco (Não implemente sistemas de IA)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Estrutura de Segurança de IA da Frontier (‡1129*)
  Riscos cobertos:
1. Ameaças biológicas
2. Cibersegurança ofensiva
3. Operação autônoma e manipulação avançada
  Níveis de risco ou equivalente e salvaguardas associadas:
  Níveis de Risco
- Nível 1 (Garantias básicas para riscos mínimos e possibilidade de liberação em código aberto)
- Nível 2 (monitoramento em tempo real, filtragem de prompts, detecção de anomalias comportamentais, controles de acesso, red-teaming e simulações adversariais)
- Nível 3 (Salvaguardas avançadas, incluindo red-teaming, implementações faseadas, testes adversariais, criptografia, controles de acesso multiparte e arquitetura de zero-trust)
- Nível 4 (protocolos de segurança máximos para modelos de alto risco e medidas máximas de segurança)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 3.5: Frameworks de Frontier AI Safety
>white|black||9|11|br O primeiro conjunto de Marcos de Segurança para IA de Fronteira que foi publicado por um subconjunto dos desenvolvedores de IA que assinaram os Compromissos de Segurança para IA de Fronteira. Os marcos cobrem riscos semelhantes (com variações sutis) e empregam diferentes níveis de risco e abordagens de gerenciamento de risco.


>white|orangered|left|14|15.5|bb A eficácia dos Frameworks de Segurança de IA da Frontier é incerta

Os Frameworks de Segurança da Frontier AI podem servir como ferramentas de gestão de risco sob condições específicas e para certas categorias de risco que tenham um caminho plausível para causar dano (‡1117). Ao mesmo tempo, várias análises discutem questões relacionadas à sua clareza e escopo (‡111, ‡986) e sobre a robustez das capacidades da IA e dos limiares de risco (‡1031, ‡1130). Frameworks existentes tendem a focar em um subconjunto de domínios de risco. Como resultado, alguns riscos de destaque, como vigilância ilegal (‡1131, ‡1132) e imagens íntimas sem consentimento (‡287), recebem menos ênfase. Diferentemente de abordagens de gestão de risco de outros setores, como aviação ou energia nuclear (‡1133*), os Frameworks de Segurança da Frontier AI tipicamente não usam limiares de risco quantitativos explícitos (‡1134).

As avaliações externas da conformidade dos desenvolvedores com seus Frontier AI Safety Frameworks até agora permanecem limitadas, em parte porque a maioria dos frameworks é recente, as informações publicamente disponíveis são escassas e não há auditorias externas padronizadas. A eficácia deles também será determinada por quão bem – e em que medida – os compromissos são implementados na prática. Por si só, esses frameworks podem não garantir um gerenciamento de riscos eficaz, já que seu impacto prático depende de quão bem e em que medida eles são implementados. Até o momento, eles não se alinham totalmente com padrões internacionais de gerenciamento de riscos (‡1135). Um estudo sobre compromissos voluntários anteriores encontrou cumprimento desigual entre as medidas, sugerindo que a adesão a compromissos voluntários provavelmente varia entre empresas e domínios (‡1109).

Tomados em conjunto, os Frontier AI Safety Frameworks representam a forma mais detalhada de gestão voluntária de riscos organizacionais atualmente em uso, mas variam substancialmente em escopo, limiares e exequibilidade.

###@ Iniciativas regulatórias e de governança

>white|orangered|left|14|15.5|bb Várias jurisdições introduziram leis com requisitos de transparência

Várias abordagens regulatórias iniciais introduzem requisitos legais destinados a aumentar a padronização e a transparência na gestão de riscos. O Ato sobre IA da UE, que entrou em vigor em 2024, estabelece requisitos relacionados com transparência, direitos autorais e segurança para modelos de IA de finalidade geral. Em 2025, foi publicado o Código de Prática para IA de Finalidade Geral da UE, para apoiar a conformidade com essas obrigações, fornecendo orientações sobre documentação do modelo e direitos autorais, bem como – para os modelos mais avançados – práticas de gestão de riscos, como avaliações, avaliação e mitigação de riscos, segurança da informação e comunicação de incidentes graves (‡965).

Outros exemplos de novos requisitos regulatórios incluem a Lei-Quadro sul-coreana sobre o Desenvolvimento da Inteligência Artificial e o Estabelecimento de Confiança, que introduz requisitos para sistemas de IA de “alto impacto” em setores críticos (‡1136), e a SB 53 da Califórnia, que estabelece requisitos de transparência sobre estruturas de segurança e de comunicação de incidentes (‡1104). Dado o quão recentemente esses requisitos foram estabelecidos, ainda é cedo para avaliar em detalhe como eles afetarão as práticas de gestão de risco ou os resultados reais de risco.

>white|orangered|left|14|15.5|bb Iniciativas mais amplas de governança oferecem orientação voluntária

Vários quadros de governança regionais e interregionais agora articulam expectativas comuns para o gerenciamento de riscos provenientes de IA de propósito geral, fornecendo orientações não vinculativas para formuladores de políticas e organizações. O China’s AI Safety Governance Framework 2.0, publicado em 2025, oferece orientações estruturadas sobre a categorização de riscos e contramedidas ao longo do processo de desenvolvimento e implantação de IA (‡1137). Os Estados-Membros da ASEAN publicaram o ‘ASEAN Expanded Guide on AI Governance and Ethics (Generative AI)’, que fornece orientações sobre a governança e a ética de IA de propósito geral e tem como objetivo apoiar uma maior harmonização de políticas entre os Estados-Membros da ASEAN (‡1138). Além disso, iniciativas lideradas por especialistas, como o Singapore Consensus, desenvolvido por cientistas de IA de múltiplos países, delineiam prioridades de pesquisa para a segurança de IA de propósito geral em avaliação de riscos, desenvolvimento e controle (‡690).

###@ Atualizações

Desde a publicação do último Relatório (janeiro de 2025), o panorama de gestão de riscos para IA de finalidade geral evoluiu, com a publicação de novos recursos como o Código de Prática para IA de Finalidade Geral da UE, o G7 HAIP Reporting Framework, o Framework Nacional de Governança de Segurança de IA da China 2.0 e vários Frontier AI Safety Frameworks de desenvolvedores de IA. Essas iniciativas descrevem abordagens e práticas usadas por desenvolvedores de IA para gerenciar os riscos associados a sistemas de IA de finalidade geral (‡1115). Há uma variação significativa entre os Frontier AI Safety Frameworks e entre os relatórios de transparência do HAIP (‡1103), refletindo diferenças nas práticas organizacionais, na priorização de riscos e no estágio inicial do ecossistema de gestão de riscos da IA de finalidade geral. Um ecossistema confiável em que diferentes agentes de IA contribuam com práticas complementares de gestão de riscos ao longo do ciclo de vida pode contribuir para uma gestão eficaz de riscos (‡690).

###@ Lacunas de evidência

Há uma falta de evidências sobre: como medir a gravidade, a prevalência e o horizonte temporal de riscos emergentes; em que medida esses riscos podem ser mitigados em contextos do mundo real; e como incentivar ou exigir, de forma eficaz, a adoção da mitigação por diversos atores. É necessária mais pesquisa para entender quão prevalentes são diferentes riscos e o quanto eles variam entre diferentes regiões do mundo, especialmente para regiões como Ásia, África e América Latina, que estão se digitalizando rapidamente. À medida que modelos de IA recebem agência e autoridade cada vez maiores e o estado da arte no campo dos riscos de IA de propósito geral avança, as abordagens de gerenciamento de riscos também precisarão evoluir (‡639, ‡1139).

Algumas mitigacoes de risco estao crescendo em popularidade (‡690, ‡956), mas ainda e necessario mais pesquisa para entender o quao robustas sao, na pratica, as mitigacoes de risco e salvaguardas para diferentes comunidades e agentes de IA (incluindo pequenas e medias empresas). Maior acesso a dados sobre implantacao e uso em situacoes reais de modelos e relevante para essas avaliacaes. Alem disso, os esforcos de gerenciamento de risco atualmente variam de forma muito acentuada entre as principais empresas de IA. Argumentou-se que os incentivos dos desenvolvedores nao estao bem alinhados com a avaliacao e a gestao minuciosas de riscos (‡934). Ainda existe uma lacuna de evidencias quanto ao grau em que diferentes compromissos voluntarios estao sendo atendidos, quais obstaculos as empresas enfrentam para cumprir plenamente os compromissos e como estao integrando os Frontier AI Safety Frameworks nas praticas mais amplas de gerenciamento de riscos de IA.

###@ Desafios para formuladores de políticas

Os principais desafios incluem determinar como priorizar os riscos diversos impostos pela IA de propósito geral, esclarecer quais atores estão melhor posicionados para mitigá-los e compreender os incentivos e restrições que moldam suas ações. As evidências indicam que os formuladores de políticas atualmente têm acesso limitado a informações sobre como os desenvolvedores e implantadores de IA estão testando, avaliando e monitorando riscos emergentes, e sobre a eficácia de diferentes práticas de mitigação (‡1140). Pesquisadores e formuladores de políticas discutiram iniciativas de transparência e relatos de incidentes mais sistemáticos como possíveis formas de informar a priorização de riscos, promover a confiança e incentivar o desenvolvimento responsável (‡957). Na prática, a gestão de riscos envolve múltiplos atores ao longo da cadeia de valor da IA – como provedores de dados e de computação em nuvem, desenvolvedores de modelos e plataformas de hospedagem de modelos – cada um com oportunidades distintas para avaliar e gerenciar diferentes riscos (‡1141). A partilha limitada de informações entre esses atores dificulta determinar quais riscos são mais prováveis ou impactantes, especialmente quando são considerados efeitos sociais a jusante.

