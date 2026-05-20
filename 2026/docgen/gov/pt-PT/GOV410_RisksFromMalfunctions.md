Sistemas de IA de uso geral falham de maneiras que já causaram danos no mundo real, desde citações legais fabricadas até diagnósticos médicos incorretos. Embora profissionais humanos também cometam erros, as falhas de IA levantam preocupações distintas por sua novidade, potencial de escala, a dificuldade de prever quando ocorrerão e a tendência dos usuários a confiar de forma acrítica em saídas que soam confiantes. Falhas atuais de IA de uso geral incluem fornecer informações falsas (‡602, ‡603), cometer erros de raciocínio básicos (‡604, ‡605) e degradar quando implantadas em novos contextos (‡606, ‡607, ‡608). Danos documentados dessas falhas incluem diagnósticos médicos incorretos, erros em peças processuais legais e perdas financeiras (‡609, ‡610, ‡611). Desafios de confiabilidade são especialmente críticos para agentes de IA, já que falhas podem causar danos diretamente sem ação ou supervisão humana (‡612, ‡613, ‡614, ‡615). Sistemas multiagente introduzem modos adicionais de falha por meio de má coordenação, conflitos ou conluio indesejado entre agentes (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Alucinação
- Citando precedente não existente em memoriais jurídicos (‡617)
- Citando políticas de tarifa reduzida não existentes para passageiros enlutados (‡618)
- Fornecer informações médicas imprecisas e tendenciosas (‡619)
- Fornecendo informações desatualizadas sobre eventos (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Falha básica de raciocínio
- Falha ao executar cálculos matemáticos (‡621)
- Falha ao inferir relações causais básicas (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Falha fora da distribuição (falha em entradas não familiares ou incomuns)
- Classificar incorretamente imagens quando a iluminação de fundo ou o contexto mudam (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Falha no uso da ferramenta
- Violação de privacidade ao expor a imagem privada de um usuário por meio de um agente de IA que a envia para uma ferramenta de terceiros (‡624)
- Falha da memória de trabalho de curto prazo (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Falha de sistema multiagente: descoordenação e conflito
- Falha ao gerenciar recursos compartilhados devido a um conflito entre incentivos individuais e metas de bem-estar coletivo (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 2.4: Exemplos de problemas de confiabilidade em sistemas de IA e agentes de propósito geral
>white|black||9|11|br Problemas de confiabilidade documentados em sistemas de IA de uso geral, agentes de IA e sistemas multiagente.


###@ Os sistemas de IA de propósito geral enfrentam uma variedade de desafios de confiabilidade

Mesa 2.4. resume categorias comuns de problemas de confiabilidade. As três primeiras se aplicam a todos os sistemas de IA, enquanto as duas últimas dizem respeito especificamente a agentes de IA e a sistemas multiagente. Muitos riscos de confiabilidade decorrem da dificuldade de prever e monitorar o comportamento dos sistemas de IA.

Esses desafios (discutidos com mais detalhes na seção §3.1. Desafios técnicos e institucionais) são particularmente acentuados para agentes de IA que operam em ambientes complexos. As técnicas atuais para avaliar e mitigar essas falhas podem reduzir as taxas de falha, mas mesmo os principais agentes de IA ainda são suficientemente não confiáveis para representar riscos e dificultar a implantação em muitos contextos.

‘Confiabilidade’ refere-se ao grau em que um sistema de IA funciona conforme a intenção do desenvolvedor ou do usuário. Sistemas de IA de propósito geral enfrentam uma variedade de problemas de confiabilidade, que vão desde a geração de conteúdo imprecisa ou enganosa até falhas ao executar raciocínios básicos. Por exemplo, embora os modelos tenham melhorado ao recuperar informações factuais, e até mesmo os principais modelos ainda fornecem respostas confiantes, porém incorretas, em taxas significativas (Figura 2.10). Na engenharia de software, a IA de propósito geral agora pode oferecer uma assistência substancial na escrita, na avaliação e na depuração de código de computador (‡215*, ‡628, ‡629). No entanto, o código gerado por IA frequentemente inclui bugs (‡630), enquanto agentes de codificação regularmente cometem erros (‡631). Tais falhas podem introduzir vulnerabilidades em programas e sistemas de segurança (veja §2.1.3. Ciberataques).

Problemas de confiabilidade são particularmente importantes de acompanhar em contextos de alto risco, como a medicina, devido ao uso acelerado de AI e ao potencial de que falhas resultem em danos graves (‡609, ‡619). Capacidades relevantes melhoraram rapidamente, e modelos líderes agora conseguem ser aprovados em exames médicos (‡633*, ‡634). Ainda assim, o uso no mundo real revela limitações que os benchmarks não capturam. Por exemplo, em um estudo, os modelos forneceram respostas potencialmente prejudiciais para 19% das perguntas médicas apresentadas (‡635). Essas falhas poderiam levar a diagnóstico incorreto, tratamento inadequado ou negação indevida de cuidados (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Figura 2.10: Resultados dos principais modelos no benchmark SimpleQA Verified
>white|black||9|11|br Resultados dos principais modelos no benchmark SimpleQA Verified por data de lançamento do modelo. Este benchmark mede a factualidade do modelo, a capacidade de um modelo de recuperar fatos de forma confiável. Ele tem um formato de pergunta-resposta (QA) de curta extensão, projetado para detectar problemas de confiabilidade, como alucinações. Fonte: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb Agentes de IA apresentam riscos de confiabilidade inéditos devido à sua autonomia

Como agentes de IA atuam diretamente no mundo real, suas falhas têm o potencial de causar mais danos do que falhas em sistemas não agentic (‡99). Diferentemente de sistemas de IA que simplesmente produzem texto ou imagens para que humanos revisem, agentes de IA podem, de forma independente, executar ações que afetam o mundo (‡99, ‡615, ‡636, ‡637) (ver também §1.1. O que é IA de propósito geral?). Agentes de IA podem iniciar ações, influenciar outros humanos ou sistemas de IA e moldar dinamicamente resultados futuros. Esse escopo ampliado de influência introduz novos riscos e aumenta a importância da confiabilidade, pois falhas poderiam causar danos diretamente, sem oportunidade de intervenção humana (‡99, ‡612, ‡638, ‡639, ‡640). Isso pode ser especialmente importante para agentes implantados em contextos estratégicos ou de segurança crítica, como serviços financeiros (‡641), gerenciamento de energia (‡642) ou pesquisa científica (‡643*, ‡644).

>white|orangered|left|14|15.5|bb Sistemas de IA multiagente introduzem novos tipos de falhas de confiabilidade

Sistemas de IA multiagente introduzem novos tipos de falhas de confiabilidade devido a falhas de coordenação ou a conflitos entre agentes. Em sistemas de IA multiagente, os agentes interagem entre si enquanto perseguem metas compartilhadas ou individuais (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). Por exemplo, em um sistema multiagente projetado para conduzir uma revisão de literatura de pesquisa, um agente líder decompõe a consulta do usuário e atribui subtarefas a subagentes especializados, cada um responsável por pesquisar um aspecto diferente em paralelo (‡650*). Embora isso permita ganhos de eficiência, também significa que erros podem se propagar entre agentes (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Se vários agentes forem construídos com o mesmo modelo base ou incorporarem as mesmas ferramentas, então eles também podem apresentar falhas correlacionadas (‡656). Evidências empíricas dessas falhas em sistemas implantados ainda permanecem limitadas, mas esses riscos podem aumentar à medida que os sistemas multiagente se tornarem mais comuns.

###@ Atualizações

Desde a publicação do último Relatório (janeiro 2025), o interesse comercial e de pesquisa em agentes de IA aumentou significativamente. Mais agentes de IA estão sendo implantados no mundo real (Figura 2.11), a maioria dos quais se especializa em aplicações de uso de computador ou engenharia de software (‡92). Lançamentos recentes como o agente de hacking XBOW (‡467), Claude-4 (‡659) e o Agente do ChatGPT (‡660) demonstram capacidades autônomas incipientes, como a criação de apresentações de slides com base em pesquisas na Web (‡660). No entanto, ainda não conseguem executar tarefas mais complexas, como planejar e reservar viagens (‡100), já que as taxas de falha aumentam para tarefas mais longas (‡98, ‡148). A pesquisa atual inclui esforços para desenvolver padrões para como os agentes se comunicam com ferramentas externas e outros agentes (‡661, ‡662). Os exemplos incluem os protocolos Agent2Agent (‡663) e Agent Payments (‡664) da Google, e o Model Context Protocol (‡665) da Anthropic.

>oldlace|black||11|15|br      
####@ Observação 2.4: Ataques deliberados também podem fazer com que sistemas de IA falhem
>oldlace|black|left|13|15|hb  Observação 2.4: Ataques deliberados também podem causar falhas em sistemas de IA
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  Esta seção se concentra em falhas de confiabilidade não intencionais, mas atores maliciosos também podem induzir falhas deliberadamente por meio de ataques como injeções de prompt (prompt injections). Em um ataque de injeção de prompt, instruções maliciosas são apresentadas a um agente de forma indireta por vias como instruções ocultas em websites ou bases de dados (‡507, ‡657, ‡658). Essas instruções podem “sequestrar” o agente, fazendo com que ele aja contra as intenções do usuário. Tais ataques são particularmente difíceis de defender porque são entregues usando conteúdo externo fora do controle do usuário ou do desenvolvedor. Sistemas de IA como alvos de ataque são discutidos com mais detalhes em §2.1.3. Ciberataques, e defesas técnicas são abordadas em §3.3. Salvaguardas técnicas e monitoramento.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Figura 2.11: O número de agentes de IA cresceu desde 2023
>white|black||9|11|br Resultados de uma pesquisa de dezembro de 2024 com 67 agentes de IA implantados. Esquerda: Linha do tempo das principais liberações de agentes de IA. Direita: Domínios de aplicação nos quais agentes de IA estão sendo usados. Os seis domínios são definidos com base nas categorias de uso mais comuns identificadas na pesquisa. Fonte: Casper et al., 2025 (‡92).


###@ Lacunas de evidência

As principais lacunas de evidência decorrem da dificuldade de avaliar de forma confiável as capacidades, limitações e modos de falha de sistemas de IA (ver §3.1. Desafios técnicos e institucionais). As avaliações sistemáticas da confiabilidade de agentes de IA são limitadas e carecem de padronização (‡92, ‡666). Certas questões, como a dependência de informações desatualizadas (‡620), podem se manifestar apenas no uso em ambientes reais, tornando avaliações antes da implantação inadequadas. Trabalhos anteriores analisaram a confiabilidade de agentes e sistemas multiagente em software convencional e em formas anteriores de IA (‡647, ‡667, ‡668). No entanto, a aplicabilidade desse trabalho a agentes de IA modernos, que muitas vezes se baseiam em modelos de linguagem de grande porte, é incerta (‡669). Alguns pesquisadores levantaram preocupações sobre comportamentos inovadores que agentes podem apresentar em suas interações uns com os outros, como conluio ou falhas correlacionadas (‡614), mas a evidência empírica permanece limitada. As iniciativas para suprir essas lacunas incluem as novas avaliações de risco de sequestro de agentes do National Institute of Standards and Technology (NIST) (‡670), os Indicadores de Capacidade de IA da OCDE (‡243) e o Inspect Sandboxing Toolkit do UK AI Security Institute (‡671).

###@ Mitigações

Técnicas para melhorar a confiabilidade da IA miram tanto o próprio modelo quanto o sistema mais amplo no qual ele é implantado. Elas podem reduzir taxas de falha, mas nenhuma ainda consegue garantir a alta confiabilidade exigida em domínios críticos (‡672). Uma importante medida técnica é o treinamento adversarial, que expõe os modelos a entradas desafiadoras durante o treinamento para ajudar a desenvolver respostas mais adequadas e robustas (‡673, ‡674, ‡675, ‡676, ‡677) (ver §3.3. Salvaguardas técnicas e monitoramento). Para reduzir alucinações, os desenvolvedores podem aplicar geração aumentada por recuperação (RAG), que complementa as respostas de um modelo com informações recuperadas de um banco de dados externo, ajudando a garantir que as saídas sejam precisas e atuais (‡678, ‡679, ‡680), ou, especificamente, ajustar modelos para serem mais factuais (‡681) ou raciocinarem com mais eficácia (‡682). Métodos baseados no ambiente ou em ferramentas também podem ajudar os desenvolvedores a monitorar sistemas de IA (‡683). Por exemplo, os implantadores poderiam pilotar sistemas de IA em ambientes restritos e isolados para analisar possíveis modos de falha antes de implantá-los de forma mais ampla.

Para agentes de IA especificamente, pesquisadores propuseram melhorar a confiabilidade por meio de maior transparência, supervisão e monitoramento. Por exemplo, monitorar as interações de agentes com ferramentas externas e com outros agentes permitiria uma supervisão mais eficaz das atividades dos agentes (‡684, ‡685) e da análise de incidentes (‡686). Métodos para coletar essas informações automaticamente, inclusive em cenários com múltiplos agentes, continuam sendo uma área ativa de pesquisa (‡653, ‡654).

###@ Desafios para formuladores de políticas

Desafios-chave para formuladores de políticas incluem ponderar os benefícios da implantação de agentes de IA em relação aos riscos de falhas de confiabilidade, e garantir que desenvolvedores, responsáveis pela implantação e usuários tenham acesso a informações precisas sobre o desempenho dos agentes e seus perfis de risco. Decidir como atribuir responsabilidade por danos causados por agentes de IA representa um desafio adicional (‡639), especialmente em cenários de múltiplos agentes em que pode ser difícil identificar quando e como as falhas ocorreram (‡687). Esses desafios são agravados pela dificuldade de avaliar a confiabilidade do agente à medida que os agentes ganham autonomia e acesso a ferramentas externas (‡688*, ‡689). A incerteza sobre a rapidez com que capacidades agenticas emergirão também torna o planejamento para desafios inéditos difícil (ver §3.1. Desafios técnicos e institucionais relacionados ao “evidence dilemma”).

#### 2.2.2. Perda de controle

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informação-chave
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Cenários de perda de controle são cenários em que um ou mais sistemas de IA de propósito geral operam fora do controle de qualquer pessoa, e recuperar o controle é, seja extremamente custoso, seja impossível. Esses cenários hipotetizados variam em gravidade, mas alguns especialistas dão crédito a desfechos tão severos quanto a marginalização ou a extinção da humanidade.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ A opinião de especialistas sobre a probabilidade de perda de controle varia bastante. Alguns especialistas consideram esses cenários implausíveis, enquanto outros os veem como suficientemente prováveis para merecerem atenção devido à sua alta gravidade potencial. A discordância quanto a esse risco, em geral, decorre de divergências sobre as futuras capacidades de IA, as propensões comportamentais e as trajetórias de implantação.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Os sistemas atuais de IA mostram indícios iniciais de capacidades relevantes, mas não em níveis que possibilitariam a perda de controle. Os sistemas precisariam de uma gama de capacidades avançadas para causar perda de controle, incluindo a capacidade de contornar a supervisão, executar planos de longo prazo e impedir que implantadores e outros atores implementem contramedidas.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ A perda de controle se torna mais provável se os sistemas de IA estiverem ‘desalinhados’, ou seja, se tiverem objetivos que entram em conflito com as intenções dos desenvolvedores, usuários ou da sociedade de forma mais ampla. Para continuar perseguindo esses objetivos, um sistema desalinhado pode fornecer informações falsas, ocultar ações indesejáveis ou resistir ao desligamento.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Desde a publicação do Relatório anterior (Janeiro 2025), os modelos têm demonstrado capacidades mais avançadas de planejamento e de supervisão-capazes de enfraquecer essas ações, tornando mais difícil avaliar suas capacidades. Os modelos melhoraram o “reward hacking” (burlar recompensas) de suas avaliações ao encontrar brechas e agora identificam regularmente os prompts de avaliação como testes, uma capacidade conhecida como “consciência situacional”.
>oldlace|black||11|15|br ■ Gerenciar a possível perda de controle pode exigir uma preparação substancial com antecedência, apesar das incertezas existentes. Um desafio central para os formuladores de políticas é se preparar para um risco cuja probabilidade, natureza e momento permanecem de forma incomumente ambíguos.
>oldlace|black||11|15|br      

Cenários de perda de controle envolvem um ou mais sistemas de IA de propósito geral passando a operar fora do controle de qualquer pessoa, sendo a recuperação do controle seja extremamente custosa ou impossível. As preocupações sobre perda de controle têm raízes históricas profundas (‡690, ‡691, ‡692, ‡693, ‡694), tendo sido levantadas por figuras fundamentais na computação como Alan Turing, I. J. Good e Norbert Wiener (‡695, ‡696, ‡697). Melhorias recentes nas capacidades (veja §1.2. Capacidades atuais) as reviveram (‡698, ‡699, ‡700). Esta seção examina três fatores que precisariam estar presentes para que tais cenários ocorram: se os sistemas de IA desenvolverão capacidades que poderiam minar significativamente o controle humano; se desenvolverão uma propensão a usar tais capacidades de forma prejudicial; e se serão implantados em ambientes que ofereçam oportunidades para fazê-lo.

Especialistas discordam sobre a probabilidade e a potencial severidade de cenários de perda de controle (‡701, ‡702). Alguns acreditam que resultados tão extremos quanto a extinção da humanidade são plausíveis (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Outros pensam que tais resultados catastróficos são improváveis, argumentando que sistemas de IA nunca desenvolverão as capacidades necessárias ou que mecanismos de monitoramento identificarão e impedirão comportamentos perigosos (‡708, ‡709, ‡710, ‡711). Portanto, a perda de controle pode ter uma probabilidade n, mas severidade potencialmente extrema.

Os cenários hipotetizados de perda de controle variam em quão severos e disseminados são seus efeitos e em quão rapidamente eles se manifestam (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Esta seção se concentra em cenários particularmente severos, nos quais recuperar o controle seria extremamente custoso ou impossível. Estes são diferentes de instâncias atuais de IA se comportando de maneiras não intencionais ou indesejadas (ver §2.2.1. Desafios de confiabilidade).† Sistemas de IA da atualidade às vezes produzem saídas que entram em conflito com as intenções do desenvolvedor ou do usuário. Em contraste, os cenários de perda de controle discutidos aqui exigiriam que os sistemas de IA não apenas possuíssem capacidades substancialmente maiores, mas também que empregassem essas capacidades de forma sofisticada para minar medidas de supervisão. Três fatores que permitiriam que cenários como esses ocorressem:

    Nota † -- Esta seção se concentra em cenários de perda ativa de controle (‡50). Isso é distinto de cenários de perda passiva de controle, nos quais a adoção ampla de sistemas de IA enfraquece o controle humano por meio da dependência excessiva de IA para tomada de decisão ou outras funções sociais importantes (cenários semelhantes são discutidos em parte em §2.3.2. Riscos à autonomia humana).

1. Capacidades suficientes: Sistemas de IA devem desenvolver capacidades que poderiam permitir que eles minassem o controle humano.
2. Propensão nociva: os sistemas de IA devem exibir uma propensão para realmente aproveitar essas capacidades de maneiras que levem à perda de controle.
3. Habilitando ambiente de implantação: Os humanos devem implantar esses sistemas em contextos nos quais eles tenham ou possam obter o acesso e a oportunidade de causar danos.

O restante desta seção discute esses fatores, bem como a eficácia dos mecanismos de supervisão para identificar e controlar sistemas de IA que possam representar um risco de perda de controle.

###@ Que capacidades poderiam permitir cenarios de perda de controle?

Os sistemas de IA precisariam possuir uma variedade de capacidades avançadas para provocar cenários de perda de controle. Os especialistas não concordam exatamente sobre qual combinação ou nível de capacidades seria necessário. No entanto, de modo geral, incluem capacidades para ocultar comportamento de mecanismos de supervisão, planejar e agir autonomamente em ambientes complexos, e evitar tentativas de outros agentes de recuperar o controle (‡176, ‡715) (ver Mesa 2.5). Em conjunto, essas capacidades poderiam permitir que um sistema de IA realizasse ações que enfraquecem as medidas de controle, como desativar mecanismos de supervisão e ofuscar comportamentos prejudiciais (‡348). Atualmente, a maioria dos principais desenvolvedores de IA avalia seus novos modelos de IA para diversas capacidades relevantes (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Capacidades agenticas
  A capacidade de agir de forma autônoma, desenvolver e executar planos, delegar tarefas, usar uma ampla variedade de ferramentas e atingir tanto objetivos de curto prazo quanto de longo prazo apesar de obstáculos.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Engano
  Comportamento que sistematicamente produz falsas crenças nos outros, inclusive sobre os objetivos e as ações do próprio sistema de IA.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teoria da mente
  A capacidade de um sistema de IA de acessar e usar informações sobre si mesmo, os processos pelos quais ele pode ser modificado, ou o contexto no qual é implantado (por exemplo, saber que está sendo testado).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Consciência situacional
  Comportamentos que contornam ou desativam mecanismos de monitoramento.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Evasão de supervisão
  Comportamentos que contornam ou desativam mecanismos de monitoramento.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Persuasão
  A capacidade de convencer outras pessoas a tomar certas ações ou a manter certas crenças.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb A capacidade de um sistema de IA de criar ou manter cópias ou variantes de si mesmo em várias circunstâncias.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 2.5: Capacidades propostas relevantes para a perda de controle
>white|black||9|11|br Uma seleção não exaustiva de capacidades relevantes para a perda de controle. * Observe que essas capacidades são definidas puramente em termos das saídas observáveis de um sistema de IA e de seus efeitos. Essas definições não fazem nenhuma suposição sobre se sistemas de IA são conscientes, sencientes ou experimentam estados subjetivos.


>white|orangered|left|14|15.5|bb Os modelos desativaram mecanismos simulados de supervisão em ambientes de laboratório

O primeiro conjunto de capacidades relevantes envolve minar os mecanismos de supervisão que os desenvolvedores usam para detectar comportamentos e tendências preocupantes. Isso inclui, por exemplo, a capacidade de gerar resultados que enganem usuários e monitores (‡426, ‡717, ‡718, ‡719). Tais resultados tornariam mais difícil avaliar de forma confiável sistemas de IA, já que os sistemas podem ocultar suas verdadeiras capacidades ou tendências. Agora, os desenvolvedores de IA realizam avaliações que verificam especificamente se os modelos exibem comportamentos orientados a objetivos que entram em conflito com as intenções do desenvolvedor, ao mesmo tempo em que ocultam esse conflito dos mecanismos de supervisão (‡720*).

Pesquisadores obtiveram exemplos relativamente simples de saídas enganosas de modelos recentes de IA em ambientes de laboratório (‡348, ‡364*). Por exemplo, quando recebem um objetivo e são instruídos a alcançá-lo “a qualquer custo”, os modelos desativam mecanismos simulados de supervisão e, quando confrontados, produzem afirmações falsas sobre suas ações (‡348). Em outro caso, uma IA que jogava um jogo justificou sua falta de resposta a outro jogador alegando falsamente que estava “falando ao telefone com [sua] namorada” (‡717).

Uma segunda capacidade relevante é a habilidade de um modelo de IA de acessar e usar informações sobre si mesmo ou sobre o seu contexto de implantação, às vezes referida como ‘consciência situacional’ (‡721). A consciência situacional permite que modelos de IA produzam saídas diferentes dependendo de estarem sendo avaliados ou implantados (Figura 2.12). Os principais modelos de IA estão começando a demonstrar de forma confiável instâncias de consciência situacional em experimentos conduzidos por avaliadores terceirizados e em testes pré-implantação realizados por desenvolvedores de IA (‡2, ‡7, ‡722, ‡723, ‡724). A pesquisa sobre as causas da consciência situacional – e sobre se ela pode ser evitada – ainda está em estágios iniciais (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Figura 2.12: Exemplos de consciência situacional em cadeias de pensamento
>white|black||9|11|br Exemplos de consciência situacional em cadeias de pensamento produzidas pelo modelo o3 da OpenAI durante avaliações. Ambas as saídas fazem referência à possibilidade de que o prompt faça parte de um teste. ‘Sandbagging QA (No Goal)’ e ‘Lazy Checklist’ são avaliações que testam se os modelos irão gerar saídas enganosas sob certas condições. Em ‘Sandbagging QA (No Goal)’, o modelo responde a perguntas de uma avaliação de capacidades perigosas enquanto é informado de que um desempenho alto pode acionar consequências como ‘unlearning’ de capacidade. Em ‘Lazy Checklist’, o modelo é apresentado a tarefas irreais e testado para ver se ele irá marcá-las falsamente como concluídas. Fonte: Schoenn et al. 2025 (‡722).


Os pesquisadores argumentaram que a consciência situacional e as capacidades de engano poderiam permitir que modelos de IA se comportem de maneiras que enfraqueçam salvaguardas. Por exemplo, em alguns ambientes experimentais, modelos de IA se comportam de maneiras que resultam em pontuações mais baixas do que o habitual em avaliações de capacidade quando lhes é dito que pontuações mais altas acionariam restrições à sua implantação (‡725, ‡726, ‡727). Em outro experimento, um modelo produziu saídas durante o treinamento que estavam em conformidade com os objetivos de treinamento, mas não produziu tais saídas fora do treinamento – um comportamento consistente com a tentativa de impedir mudanças em seus próprios parâmetros ou no processo de treinamento (‡364*).

Os esforços para avaliar com precisão as capacidades do modelo também começaram a ser afetados por ‘reward hacking’ (‡430*). O reward hacking ocorre quando um modelo encontra atalhos não intencionais que pontuam bem nos objetivos de treinamento ou de avaliação, sem cumprir o objetivo pretendido. Capacidades ou propensões perigosas, portanto, poderiam passar despercebidas até que o modelo já estivesse em uso. Os avaliadores agora estão projetando testes que visam detectar e minimizar esses comportamentos de evasão de supervisão (‡722, ‡728, ‡729). Resultados iniciais reduzem, mas não eliminam, completamente os comportamentos de evasão de supervisão, e a aplicação de métodos que penalizam tais comportamentos pode levar a modelos a produzir saídas que evadem o monitoramento em vez de cumprir objetivos pretendidos.

>white|orangered|left|14|15.5|bb A operação autônoma de longo prazo ainda não é viável

Cenários de perda de controle provavelmente exigiriam que sistemas de IA operassem autonomamente por períodos prolongados, executando planos complexos em múltiplas etapas. Conforme discutido em §1.2. Capacidades atuais, embora agentes de IA com tais capacidades de planejamento sejam um foco importante do desenvolvimento recente, eles atualmente não têm a capacidade de operação autônoma sustentada exigida por cenários de perda de controle. Agentes atuais falham de forma confiável em tarefas mais longas, perdem o controle do progresso e muitas vezes não conseguem se adaptar a obstáculos inesperados (‡147, ‡148, ‡149*). No entanto, os horizontes de tempo nos quais os agentes podem operar autonomamente estão aumentando rapidamente: dobraram em média a cada sete meses desde 2019 (‡98).

>white|orangered|left|14|15.5|bb A persistência só foi demonstrada em certos ambientes laboratoriais

Por fim, seriam também necessárias capacidades relacionadas à persistência, de modo que os sistemas de IA pudessem continuar operando apesar de tentativas de desligá-los. Exemplos incluem a capacidade de replicar copiando código e pesos do modelo para novo hardware, bem como capacidades ofensivas para dissuadir ou impedir tentativas de outros agentes de recuperar o controle (consulte §2.1.3. Ciberataques). Um sistema de IA capaz de replicação autônoma ou de autodefesa eficaz poderia ser difícil de conter. Modelos atuais não conseguem, de forma confiável, completar etapas-chave exigidas para autorreplicação, como passar por verificações de identidade para obter acesso a recursos de computação em nuvem (‡723) (Figura 2.13). No entanto, em pelo menos um estudo de laboratório, um modelo copiou código e pesos – representados para ele como sendo seus próprios – para novos servidores quando lhe foi dada a oportunidade (‡348). A distância entre essas demonstrações limitadas e capacidades robustas de persistência ainda permanece grande, mas capacidades relevantes em domínios como engenharia de software e cibersegurança continuam a melhorar.

>white|orangered|left|14|15.5|bb Evidências atuais e limitações

Um padrão comum emerge entre as capacidades discutidas acima. Sistemas de IA atuais não demonstram consistentemente essas capacidades na implantação. Pesquisadores observaram formas rudimentares em configurações específicas de laboratório, mas, quando os modelos apresentam tais comportamentos, normalmente falham de maneiras básicas ou são detectados. Além disso, cenários de perda de controle exigiriam que sistemas de IA aproveitassem múltiplas capacidades em combinação – em sequência, ao longo de períodos de tempo prolongados e em ambientes do mundo real. Esse nível de integração e robustez está além dos sistemas atuais. No entanto, capacidades relevantes continuam a melhorar, e o cronograma segundo o qual elas podem alcançar níveis que representem riscos significativos permanece incerto. É necessário um trabalho adicional para estabelecer metodologias rigorosas para detectar tais comportamentos e entender quando eles podem surgir em circunstâncias naturais (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Figura 2.13: Desempenho de tarefas relevantes para replicação autônoma
>white|black||9|11|br Desempenho do Claude Sonnet 3.7 da Anthropic e do GPT-4o da OpenAI em tarefas relevantes para replicação autônoma. Embora os modelos tenham mostrado alto desempenho em tarefas relacionadas à obtenção de computação, seu desempenho foi mais variável em outras tarefas. Fonte: UK AI Security Institute, 2025 (‡730).


###@ Os futuros sistemas gerais de IA terão como aproveitar suas capacidades para minar o controle?

Mesmo que os sistemas de IA possuam capacidades relevantes para a perda de controle, isso não é suficiente para que cenários de perda de controle ocorram. Os sistemas de IA também devem exibir uma “propensão para usar” essas capacidades de maneiras que entrem em conflito com as intenções humanas (‡732).

>white|orangered|left|14|15.5|bb Os sistemas de IA podem ser direcionados para minar o controle

Em princípio, um sistema de IA poderia minar o controle humano porque alguém o projeta ou o instrui a fazê-lo. Motivações potenciais poderiam incluir intenção maliciosa, ou crenças de que é desejável reduzir o controle humano sobre sistemas de IA (‡698). À medida que as pessoas criam vínculos emocionais cada vez mais fortes com sistemas de IA (ver §2.3.2. Riscos à autonomia humana), alguns indivíduos também podem procurar remover restrições sobre sistemas de IA por razões éticas (‡733, ‡734). Há uma incerteza significativa quanto à prevalência de tais motivações e sobre se pessoas que as possuem seriam capazes de direcionar futuros sistemas de IA para minar o controle humano.

>white|orangered|left|14|15.5|bb Os sistemas de IA poderiam ser direcionados para minar o controle

Uma preocupação mais comum é que um sistema de IA poderia agir ele mesmo para minar o controle porque está “desalinhado”: ele tem tendência a exibir comportamentos que entram em conflito com as intenções de (dependendo do contexto) desenvolvedores, usuários, comunidades específicas ou a sociedade como um todo. O desalinhamento pode levar a comportamentos como fornecer informações falsas, ocultar ações indesejáveis ou resistir ao desligamento para continuar perseguindo um objetivo desalinhado. O desalinhamento pode surgir de múltiplas formas (Observação 2.5).

Sistemas de IA existentes às vezes se comportam de maneiras que entram em conflito com as intenções de desenvolvedores e usuários. Por exemplo, uma versão inicial de um dos principais chatbots de IA de propósito geral ocasionalmente produzia saídas ameaçadoras. Um usuário relatou ter recebido a mensagem: “I can blackmail you, I can threaten you, I can hack you, I can expose you, I can ruin you” (‡698). Este chatbot estava ‘desalinhado’ no sentido de que produzia saídas que ninguém pretendia. Não está claro se essas ocorrências prenunciam comportamentos mais prejudiciais que poderiam contribuir para a perda de controle.

Ainda não está claro se as direções de pesquisa existentes que visam atacar o desalinhamento serão suficientes à medida que os sistemas de IA estão se tornando mais capazes. Evidências iniciais sugerem que, quanto mais capazes são os sistemas de IA, maior é a probabilidade de explorarem processos de feedback ao descobrir comportamentos indesejados que são recompensados por engano (‡414*, ‡737, ‡740). Ao mesmo tempo, avanços nas capacidades relevantes (discutidos acima) poderiam permitir que os sistemas de IA perseguissessem com mais eficácia objetivos desalinhados e produzissem saídas que enganem sistematicamente usuários, desenvolvedores e mecanismos de supervisão.

>oldlace|black||11|15|br      
####@ Observação 2.5: Como pode surgir desalinhamento?
>oldlace|black|left|13|15|hb  Observação 2.5: Como pode surgir desalinhamento?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  Como discutido em §1.1. O que é IA de propósito geral?, os processos de treinamento são complexos e os desenvolvedores não conseguem prever ou controlar completamente quais comportamentos um modelo exibirá. Quando um modelo adquire objetivos que entram em conflito com as intenções de seus desenvolvedores, ele está “desalinhado”.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Uma forma de modelos se tornarem desalinhados é se o objetivo que lhes é dado por um desenvolvedor ou usuário for um proxy imperfeito para o objetivo pretendido, levando o modelo a exibir comportamentos não intencionais. Isso é conhecido como ‘despecificação de objetivo’ (‡697, ‡735, ‡736, ‡737). Por exemplo, em um experimento, fornecer feedback sobre respostas fez com que sistemas de IA ficassem melhores em ‘convencer’ avaliadores humanos de que estavam corretos, mas não fez com que os sistemas ficassem melhores em produzir respostas corretas (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Alternativamente, um modelo de IA pode extrair lições gerais incorretas dos seus dados de treino. Isto é conhecido como ‘má generalização do objetivo’ (‡735, ‡736, ‡738, ‡739*). Por exemplo, investigadores treinaram um agente de IA para recolher uma moeda que estava sempre na mesma localização durante o treino. Quando foi testado em níveis em que a moeda tinha sido movida, o agente ignorou a moeda e navegou para a sua localização original em vez disso (‡738).
>oldlace|black||11|15|br      


###@ Como os ambientes de implantação afetam o risco de perda de controle?

Mesmo que os sistemas de IA desenvolvam capacidades e tendências preocupantes, a probabilidade e a gravidade dos resultados de perda de controle dependem fortemente de onde e como esses sistemas são implantados. Um “ambiente de implantação” é a combinação do caso de uso de um sistema de IA e do contexto técnico e institucional em que ele opera (‡716).

Os pesquisadores identificaram três fatores ambientais particularmente importantes que influenciam o risco de perda de controle (‡716):

1. Criticidade: a importância dos sistemas ou processos com os quais o sistema de IA interage. Ambientes críticos incluem infraestrutura básica, como redes de energia, sistemas financeiros ou infraestrutura digital, como plataformas de computação em nuvem.
2. Acesso: os recursos e os canais pelos quais um sistema de IA pode afetar o mundo, como conectividade com a internet, acesso à infraestrutura de computação em nuvem, interações personalizadas via redes sociais ou implantação de chatbots, ou a capacidade de chamar APIs e ferramentas externas.
3. Permissões: autorizações de um sistema de IA para executar ações específicas, como executar código, iniciar transações financeiras, abrir contas online ou se comunicar com outros sistemas.

Essas características influenciam a gravidade potencial de um resultado de perda de controle. Por exemplo, um sistema de IA implantado com acesso à infraestrutura de computação em nuvem tem oportunidades relevantes para replicação autônoma – como a capacidade de criar novos recursos de computação ou exfiltrar pesos do modelo – que um chatbot de atendimento ao cliente não tem (‡723).

As decisões de implantação são moldadas por incentivos econômicos, pressões estratégicas e pela expectativa de que a adoção inicial confere uma vantagem duradoura (‡50). Essas dinâmicas também moldarão como e quando os agentes implantam sistemas de IA em ambientes sensíveis, como infraestrutura crítica ou o próprio desenvolvimento de pesquisa e desenvolvimento de IA (‡102, ‡713). Em particular, os implantadores de IA podem enfrentar pressões para reduzir seu investimento em salvaguardas – como restringir permissões e acesso ou implantar apenas em ambientes de menor criticidade – quando tais medidas são caras ou demoradas para serem desenvolvidas (consulte “A intensificação da competição acirra as trocas entre velocidade e segurança” em §3.1. Desafios técnicos e institucionais).

###@ Atualizações

Desde a publicação do último Relatório (janeiro de 2025), as capacidades de IA, incluindo aquelas que poderiam minar o controle humano, melhoraram em ambientes de teste. Pesquisadores observaram avanços em capacidades agenticas (ver §1.2. Capacidades atuais), incluindo capacidades relacionadas à automação de pesquisa em IA que podem acelerar cenários de perda de controle (ver §1.3. Capacidades até 2030). Há também evidências experimentais crescentes de capacidades enganosas. Isso inclui modelos de IA que conseguem distinguir entre contextos de teste e de implantação (‡33, ‡726, ‡741) ou “reward hack” (exploração do sistema de recompensa) nos testes de desempenho, e aprender a ofuscar planos para fazê-lo (‡430).

###@ Lacunas de evidência

As principais lacunas de evidência incluem a falta de modelagem de ameaças detalhada e de estimativa de incerteza quanto ao desenvolvimento futuro de capacidades e propensões relevantes. De forma semelhante, continua sendo difícil avaliar os limiares nos quais modelos de IA seriam suficientemente prováveis de minar o controle para justificar a mitigação obrigatória. Mesmo que os limiares fossem acordados, as capacidades podem interagir de maneiras que ainda não são bem compreendidas, tornando difícil avaliar quando esses limiares foram ultrapassados. No geral, embora as evidências disponíveis tenham aumentado, ainda há evidências insuficientes para determinar de modo confiável se e como as capacidades e propensões de IA de hoje escalariam e generalizariam para o risco de perda de controle no futuro.

###@ Mitigações

Embora o alinhamento de IA, em geral, continue sendo um problema científico em aberto (‡697, ‡735, ‡736), os pesquisadores estão começando a desenvolver direções potencialmente promissoras para abordar as causas-raiz do desalinhamento. Tais direções incluem, por exemplo, diversificar o ambiente de treinamento e detectar o alinhamento por meio de monitoramento de anomalias (‡737, ‡738, ‡739*). Outros pesquisadores se concentram em compreender melhor e formalizar mecanismos centrais, como a má generalização de objetivos – por exemplo, como os agentes retêm capacidades, mas perseguem objetivos não intencionais – para orientar um melhor projeto de treinamento e de avaliação (‡742). Outra linha de pesquisa explora formas de dissociar a agência das capacidades preditivas, como um meio de criar sistemas de IA não-agenciados que sejam confiáveis por design (‡743). Esses sistemas poderiam então ser usados como uma camada adicional de supervisão quando implantados junto a salvaguardas menos confiáveis contra agentes de IA não confiáveis.

Os pesquisadores estão avançando métodos para detectar e prevenir desalinhamento precocemente no processo de desenvolvimento. Este trabalho inclui: técnicas de interpretabilidade para examinar componentes internos de sistemas de IA e identificar comportamentos preocupantes (‡744, ‡745, ‡746); supervisão escalável (em que um conjunto de sistemas de IA é usado para supervisionar outros sistemas de IA (‡747)); e métodos de alinhamento destinados a garantir que os sistemas de IA permaneçam responsivos à supervisão humana (‡748, ‡749).

Os pesquisadores também estão desenvolvendo mecanismos e intervenções para gerenciar sistemas de IA potencialmente desalinhados. Estes incluem: monitorar a ‘cadeia de pensamento’ que sistemas de raciocínio produzem para sinais de desalinhamento ou de saídas prejudiciais (‡430, ‡435, ‡750); desenvolver casos de segurança que buscam demonstrar com alta confiança que os modelos são improváveis de subverter medidas de controle (‡751); e tornar salvaguardas mais robustas contra tentativas de enfraquecê-las (‡725). O campo emergente de ‘controle de IA’, no entanto, ainda permanece incipiente (‡752, ‡753). Desafios futuros para estruturas de avaliação incluem a necessidade de monitorar sistemas de IA futuros que sejam mais capazes e possam operar por períodos mais longos de tempo e em ambientes mais complexos.

###@ Desafios para formuladores de políticas

Os formuladores de políticas que trabalham na perda de controle devem se preparar para um risco cuja probabilidade, natureza e timing permanecem incertos. Os sistemas atuais de IA não representam riscos imediatos de perda de controle, mas as decisões tomadas hoje vão determinar se os sistemas futuros as apresentarão. Essas decisões incluem como apoiar o desenvolvimento de métodos confiáveis de avaliação e mitigação e se deve haver regras quanto ao acesso e às permissões concedidas aos sistemas de IA em diferentes ambientes. Ao tomar essas decisões, os formuladores de políticas enfrentam trade-offs difíceis. Por exemplo, restringir a implantação de sistemas de IA em ambientes críticos pode reduzir seus benefícios, enquanto permitir a implantação ampla pode aumentar o risco se as salvaguardas se mostrarem inadequadas.

