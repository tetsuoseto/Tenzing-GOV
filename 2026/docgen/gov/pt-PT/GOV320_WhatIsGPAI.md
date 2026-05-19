###@ Quais são os sistemas de IA de propósito geral?

Sistemas de IA de propósito geral são programas de software que aprendem padrões a partir de grandes quantidades de dados, permitindo que realizem uma variedade de tarefas em vez de serem especializados para uma única função ou domínio (ver Mesa 1.1). Para criar esses sistemas, desenvolvedores de IA realizam um processo em múltiplas etapas que exige recursos computacionais substanciais, grandes conjuntos de dados e especialização especializada (ver Mesa 1.2). Recursos computacionais (frequentemente abreviados como ‘compute’) são necessários tanto para desenvolver quanto para implantar sistemas de IA, e incluem chips de computador especializados, além do software e da infraestrutura necessários para executá-los.† Como são treinados em conjuntos de dados grandes e diversos, sistemas de IA de propósito geral podem realizar muitas tarefas diferentes, como resumir texto, gerar imagens ou escrever código de computador. Esta seção explica como os sistemas de IA de propósito geral são feitos, o que são modelos de ‘raciocínio’ e como decisões de política moldam o desenvolvimento de sistemas de IA de propósito geral.

    Nota † -- O termo ‘compute’ também pode se referir a uma medição do número de cálculos que um processador pode executar (normalmente medida em operações de ponto flutuante por segundo) ou especificamente ao hardware (como unidades de processamento gráfico) que realiza esses cálculos.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Sistemas de linguagem
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Command A (‡3*)
- EXAONE 4.0 (‡4*)
- Gemini 3 Pro (‡5*)
- GLM-4.5 (‡6*)
- GPT-5(‡7*)
- Hunyuan-Large (‡8*)
- Kimi K2 (‡9*)
- Mistral 3.1 (‡10*)
- Qwen3 (‡11*)
- DeepSeek-V3.2 (‡12*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Geradores de imagens
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Geradores de vídeo
- Cosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Vejo 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Sistemas de robótica e de navegação
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Preditores de diversas classes de estruturas biomoleculares
- AlphaFold 3 (‡27)
- Amplify (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Agentes de IA
- AlphaEvolve (‡31*)
- Agente do ChatGPT (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- O AI Scientist-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 1.1: Tipos de IA de uso geral
>white|black||9|11|br Existem vários tipos diferentes de IA de propósito geral. Neste Relatório, são considerados como “IA de propósito geral” os modelos capazes de prever informações estruturais para classes diversas de moléculas, pois podem ser adaptados para uma variedade de tarefas. Por exemplo, modelos treinados para prever a estrutura de proteínas são aplicáveis a uma variedade de outras tarefas, como prever interações de proteínas, prever sítios de ligação de pequenas moléculas, e prever e projetar peptídeos cíclicos (‡40).


>white|orangered|left|13|15|bb O deep learning é fundamental para a IA de propósito geral

Pesquisadores constroem modelos de IA de propósito geral usando um processo chamado ‘deep learning’, que treina modelos para aprender com exemplos (‡41). Diferentemente da engenharia de software, modelos de deep learning aprendem a realizar tarefas a partir de dados em vez de depender de instruções escritas à mão. Ao processar grandes quantidades de dados, como imagens, texto ou áudio, esses modelos descobrem maneiras de representar esses dados, criando representações internas de padrões (como formas, associações de palavras ou estruturas de sons) que ajudam o modelo a reconhecer relações e gerar saídas alinhadas ao seu objetivo de treinamento. Em seguida, eles usam essas representações internas aprendidas como características abstratas para analisar novos dados semelhantes e gerar saídas no mesmo estilo. Por exemplo, um modelo de IA de propósito geral treinado com exemplos suficientes de poesia inglesa romântica do século 19 pode reconhecer novos poemas nesse estilo e produzir novo material em um estilo semelhante.

Em um nível mais granular, o aprendizado profundo funciona processando dados por meio de camadas de nós interconectados de processamento de informações. Esses nós são frequentemente chamados de ‘neurônios’ porque são inspirados de forma imprecisa por neurônios em cérebros biológicos (‘redes neurais’) (Figura 1.1) (‡42). À medida que a informação flui de uma camada de neurônios para a próxima, o modelo transforma progressivamente os dados em representações mais abstratas, como grupos de características aprendidas – padrões que o modelo descobriu automaticamente nos dados, em vez de padrões codificados manualmente. Por exemplo, em um modelo de processamento de imagens, as primeiras camadas podem aprender a detectar características simples como bordas ou formas básicas, enquanto camadas mais profundas combinam essas características para identificar padrões mais complexos, como rostos ou objetos.

As caracteristicas em todas as camadas sao descobertas por meio do processo de otimizacao que define o procedimento de treinamento. Durante o treinamento, quando o modelo comete erros, algoritmos de deep learning ajustam a forca de varias conexoes entre neuronios para melhorar o desempenho do modelo. A forca de cada conexao entre nos e frequentemente chamada de ‘peso’. Essa abordagem em camadas da o nome ao deep learning.

O deep learning provou ser muito eficaz ao permitir que sistemas de IA realizem tarefas que antes eram consideradas difíceis para sistemas computacionais tradicionais programados à mão e para outros métodos anteriores de IA simbólica ou baseados em regras. A maior parte dos modelos gerais de IA de ponta atualmente é baseada em uma arquitetura específica de rede neural conhecida como 'transformer' (‡43, ‡44). Transformers usam um mecanismo de 'attention' (‡45) que ajuda o modelo a se concentrar nas partes mais relevantes dos dados de entrada ao processar informações, como determinar quais palavras em uma frase são mais importantes para compreender seu significado. Essa forma específica de construir modelos levou a melhorias significativas em tradução (‡43), processamento de linguagem natural (‡46), reconhecimento de imagens (‡47) e reconhecimento de fala (‡48, ‡49), culminando no desenvolvimento dos modelos mais avançados da atualidade.

![fig1.1](images/fig1.1_neural_network.png)

##### Figura 1.1: Uma representação ilustrativa de uma ‘rede neural’
>white|black||9|11|br Os modelos de IA de uso geral atuais são baseados nessas redes, que são inspiradas de forma ampla por cérebros biológicos. Diferentes redes têm tamanhos e arquiteturas diferentes. No entanto, todas são compostas por unidades de processamento de informações conectadas chamadas ‘neurônios’, em que as forças das conexões entre os neurônios são chamadas ‘pesos’. Os pesos são atualizados durante o treinamento com grandes quantidades de dados. Fonte: International AI Safety Report 2025 (‡50) (modificado).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Figura 1.2: Uma representação esquemática das etapas do desenvolvimento de IA de propósito geral
>white|black|left|9|11|br Relatório Internacional de Segurança em Inteligência Artificial 2026.


>white|orangered|left|13|15|bb A IA de uso geral é desenvolvida em etapas

Desenvolver um sistema de IA de propósito geral envolve múltiplas etapas, desde o treinamento inicial do modelo até o monitoramento e as atualizações pós-deploy (Figura 1.2). Na prática, esses passos frequentemente se sobrepõem de forma iterativa. Cada etapa requer diferentes insumos de recursos (por exemplo, dados, mão de obra, computação) e diferentes técnicas, e às vezes são conduzidas por diferentes desenvolvedores (Figura 1.2 e Mesa 1.2).

Por exemplo, o pré-treinamento de modelos geralmente requer grandes quantidades de computação e dados, tornando essa etapa particularmente sensível a políticas que afetam o acesso a recursos computacionais ou a dados de treinamento (‡51, ‡52). De maneira semelhante, a curadoria de dados e alguns métodos de ajuste fino de modelos atualmente envolvem grandes quantidades de trabalho humano para a rotulagem inicial de dados (‡53). Portanto, essa etapa é sensível a mudanças nos custos de mão de obra, políticas de plataforma ou regulações que afetam arranjos de contratação transfronteiriços.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Coleta e curadoria de dados
> 
  Antes de treinar um modelo de IA de propósito geral, desenvolvedores e profissionais de dados coletam, limpam, selecionam e padronizam dados brutos de treino em um formato a partir do qual o modelo possa aprender. Isso pode ser um processo trabalhoso. Os conjuntos de dados de treino por trás dos modelos de ponta incluem um número imenso de exemplos provenientes de toda a internet.
  As equipes frequentemente desenvolvem métodos de filtragem sofisticados para reduzir conteúdo prejudicial, eliminar dados duplicados e melhorar a representação entre diferentes tópicos e fontes (‡54, ‡55). A curadoria de dados também pode ajudar a reduzir violações de direitos autorais e de privacidade, remover exemplos que contenham conhecimento perigoso, lidar com vários idiomas e melhorar a documentação para proveniência dos dados (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Treinamento prévio (primeira fase do treinamento)

  Durante o pré-treinamento, os desenvolvedores alimentam os modelos com quantidades massivas de dados diversos para incutir uma base ampla de informações e entendimento contextual. Esse processo produz um “modelo base”. Trata-se de um processo altamente intensivo em dados e em computação.

  Durante o pré-treinamento, os modelos são expostos a bilhões ou trilhões de exemplos de conteúdo, como imagens, textos ou áudio. Por meio dessa exposição, o modelo gradualmente descobre características abstratas para representar os dados e aprende como essas características se relacionam, o que permite que ele faça sentido de novas entradas no contexto. Esse processo de pré-treinamento leva semanas ou meses (‡59) e utiliza dezenas ou centenas de milhares de unidades de processamento gráfico (GPUs) ou unidades de processamento de tensores (TPUs) (‡60) – chips especializados de computador projetados para processar rapidamente muitas dessas computações. Alguns desenvolvedores realizam o pré-treinamento com seu próprio poder de computação, enquanto outros usam recursos fornecidos por provedores especializados de computação.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Pós-treinamento e ajuste fino (segunda etapa do treinamento)

  ‘Pós-treinamento’ refina ainda mais o modelo base para otimizá-lo para uma aplicação específica. É um processo moderadamente intensivo em computação e altamente intensivo em mão de obra. Uma mudança para o uso de ‘dados sintéticos’ – informações geradas artificialmente que imitam dados do mundo real, mas são criadas usando algoritmos ou simulações – está ajudando a tornar esta fase menos intensiva em mão de obra.
  O pós-treinamento inclui várias técnicas de ajuste fino e outras modificações. ‘Ajuste fino supervisionado’ envolve treinar novamente um modelo previamente treinado em conjuntos de dados específicos para melhorar o desempenho do modelo naquele domínio (‡61, ‡62). Por exemplo, um modelo de propósito geral poderia ser treinado novamente em um grande conjunto de imagens radiológicas. ‘Aprendizagem por reforço’ (RL) envolve melhorar o desempenho do modelo ao ‘recompensar’ um modelo (fornecendo feedback positivo) por saídas desejáveis e ‘penalizar’ um modelo (fornecendo feedback negativo) por saídas indesejáveis. Ela tem duas subcategorias de destaque. ‘Aprendizagem por reforço a partir de feedback humano’ envolve recompensar saídas que se alinham às preferências humanas e penalizar aquelas que não se alinham, com base em feedback humano (‡63, ‡64*). ‘Aprendizagem por reforço com recompensas verificáveis’ (RLVR) é usada para melhorar o desempenho do modelo em tarefas que exigem correção factual, como geração de matemática ou código. Os desenvolvedores tipicamente alternam entre aplicar técnicas de pós-treinamento e executar testes até que os resultados mostrem que o modelo atende às especificações desejadas.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Integração de sistema

  Os desenvolvedores combinam um ou mais modelos de IA de propósito geral com outros componentes para criar um “sistema de IA” pronto para uso. O GPT-5 (por exemplo) é um modelo de IA de propósito geral que processa texto, imagens e áudio, enquanto o ChatGPT é um sistema de IA de propósito geral que combina vários modelos de diferentes tamanhos e capacidades com uma interface de chat, processamento de conteúdo, acesso à Web e integração com aplicações para criar um produto funcional.
  Além de tornar os modelos de IA operacionais, os componentes adicionais em um sistema de IA também buscam aprimorar a capacidade, a utilidade e a segurança. Por exemplo, um sistema pode vir com um filtro que detecta e bloqueia entradas ou saídas do modelo que contenham conteúdo prejudicial (‡65*). Os desenvolvedores também estão cada vez mais usando “scaffolding” — software adicional construído em torno de modelos de IA de propósito geral que permite que eles se planejem com antecedência, perseguam objetivos e interajam com o mundo (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Implantação e lançamento
  A implantação é o processo de tornar o sistema de IA integrado disponível para o uso pretendido. Desenvolvedores e implantadores implementam sistemas de IA em aplicações, produtos ou serviços do mundo real. Desenvolvedores podem implantar sistemas de IA internamente (para uso próprio) ou externamente (para clientes privados ou uso público). Ao implantar sistemas de IA externamente, as empresas muitas vezes oferecem aos usuários acesso por meio de interfaces de usuário online ou interfaces de programação de aplicações (APIs) que permitem que os usuários acessem e executem o sistema. Por exemplo, uma empresa pode projetar um chatbot personalizado de atendimento ao cliente que é alimentado por um sistema de IA de propósito geral de outra empresa.
  ‘implantação de sistemas de IA’ refere-se a disponibilizar um modelo para uso no mundo real com ferramentas e interfaces integradas, enquanto ‘lançamento de modelo’ envolve disponibilizar o modelo base para outras pessoas — seja como open-weight (parâmetros baixáveis) ou closed-weight (acesso apenas por API). Veja §3.4. Modelos open-weight.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Monitoramento pós-implantação e atualizações

  Os desenvolvedores frequentemente coletam e analisam feedback dos usuários, acompanham métricas de impacto e desempenho e fazem melhorias iterativas para lidar com problemas identificados durante o uso no mundo real (‡67). As melhorias são feitas atualizando as integrações do sistema, muitas vezes por meio de ajuste fino contínuo e fornecendo modelos com acesso a bancos de dados externos de (fatos) (recentes). Isso mantém grandes modelos de IA atualizados sem repetir todo o processo de pré-treinamento (‡68*). Isso permite que as capacidades se acumulem em rodadas sucessivas de treinamento, mantendo a estabilidade e reduzindo os custos computacionais.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 1.2: Estágios de desenvolvimento de IA de propósito geral
>white|black||9|11|br Em cada etapa de desenvolvimento de IA de uso geral, o modelo de IA é aprimorado para uso a jusante e, eventualmente, é implantado como um sistema de IA totalmente integrado, monitorado e atualizado.


>white|orangered|left|13|15|bb Os sistemas de raciocínio geram “cadeias de pensamento” durante a inferência para melhorar o desempenho

A inferência acontece quando alguém utiliza o modelo de IA depois que ele é treinado. Por exemplo, a inferência ocorre quando uma pessoa pede que um sistema de IA planeje uma viagem e o modelo por trás disso recorre a aspectos relevantes do que aprendeu sobre geografia, transporte e culinária para gerar um itinerário.

Na última década, os avanços nas capacidades de IA têm vindo, em grande parte, de execuções de treinamento maiores; isto é, aumentando a quantidade de computação usada para treinar um modelo de IA. Recentemente, porém, pesquisadores obtiveram mais ganhos ao permitir que os modelos processem informações por mais tempo e ao treiná-los para produzir etapas de raciocínio explícitas enquanto realizam uma tarefa (‡69*, ‡70). Sistemas de IA que funcionam dessa forma são chamados de ‘sistemas de raciocínio’, e as explicações intermediárias pelas quais eles passam ao resolver um problema ou responder a uma pergunta são chamadas de ‘cadeias de pensamento’. Sistemas de raciocínio exigem mais recursos computacionais no momento do uso para gerar essas cadeias de pensamento sofisticadas (‡71, ‡72, ‡73, ‡74), e mais recursos durante o treinamento para que aprendam a raciocinar melhor. Na prática, essas capacidades de raciocínio permitem que sistemas de IA resolvam problemas mais complexos decompondo iterativamente uma tarefa em etapas menores. A Mesa 1.3 mostra um exemplo de um sistema não orientado a raciocínio e um sistema de raciocínio resolvendo o mesmo problema.

Os sistemas de raciocínio alcançaram avanços importantes nas suas capacidades em problemas desafiadores. Por exemplo, em 2025, sistemas de raciocínio especializados em resolução de problemas matemáticos, como o Gemini Deep Think da Google e um modelo ainda não lançado, experimental, da OpenAI, resolveram problemas da Olimpíada Internacional de Matemática (em um ambiente de teste estruturado) em um nível equivalente ao desempenho humano de medalha de ouro (‡75, ‡76). Os sistemas de raciocínio demonstraram progresso significativo em domínios formais como matemática, quebra-cabeças de lógica e questões científicas estruturadas, nos quais o raciocínio passo a passo pode ser verificado explicitamente (‡77). No entanto, os sistemas de raciocínio também podem falhar ao produzir cadeias de pensamento irrelevantes, improdutivas ou repetitivas (‡78, ‡79).

###@ Atualizações sobre métodos de treinamento

Desde a publicação do último Relatório (January 2025), um método de treinamento chamado ‘distillation’ aumentou muito a eficiência com que alguns modelos podem ser ajustados. A distillation envolve treinar um modelo ‘student’ a partir das saídas de um modelo ‘teacher’ mais poderoso (e geralmente maior), permitindo que o modelo student imite diretamente as saídas do teacher (‡80). Por exemplo, a DeepSeek desenvolveu um modelo grande chamado DeepSeek-R1, que se destaca em raciocínio do tipo chain-of-thought. O R1 gerou saídas de raciocínio que, em seguida, foram usadas para ajustar modelos student menores, incluindo DeepSeek-V3. O DeepSeek-V3 mantém grande parte das capacidades matemáticas, de codificação e de análise de documentos do R1 e foi reportado como tendo sido ajustado para aproximadamente $10,000 USD (embora seus custos de pré-treinamento não tenham sido reportados) (‡81). Isso provavelmente é de ordens de magnitude menor do que o custo de ajustar modelos maiores e igualmente capazes.

![table1.3](images/table1.3_example_reasoning.png)

##### Mesa 1.3: Um exemplo de um sistema que não faz inferência (esquerda) versus um sistema que faz inferência (direita)
>white|black||9|11|br Resolvendo o mesmo enigma, estes exemplos foram adaptados de respostas reais de IA. O sistema de raciocínio gasta mais tempo e poder computacional com 'pensar' ao construir uma 'cadeia de raciocínio' antes de fornecer sua resposta final.

![figure.3](images/fig1.3_AI_agent.png)

##### Figura 1.3: Uma representação ilustrativa de um agente de IA
>white|black||9|11|br Um modelo de IA (centro) configurado para planejar iterativamente, raciocinar e usar ferramentas para realizar tarefas do mundo real. Fonte: International AI Safety Report 2026.


A destilação pode, assim, ser uma forma barata e eficiente de modelos adquirirem capacidades mais poderosas (‡82). Alguns pesquisadores têm usado destilação para fazer o ajuste fino de modelos altamente capazes, usando apenas 1,000 exemplos gerados a partir de modelos de ponta (‡83). Como a destilação exige um modelo professor previamente existente, ela não pode ser usada diretamente para avançar as capacidades de modelos de ponta. No entanto, ela pode acelerar a disseminação de capacidades avançadas de IA, mesmo a partir de modelos de código fechado (‡84*).

Juntamente com os avanços tecnológicos em “computação distribuída” e no treinamento descentralizado (abordagens em que os desenvolvedores usam vários processadores, servidores ou centros de dados trabalhando em conjunto para realizar o treinamento ou a inferência de IA (‡85, ‡86, ‡87)), o grau em que muitos projetos de desenvolvimento de IA dependem de infraestrutura computacional centralizada em larga escala foi reduzido. Isso cada vez mais permite que atores com menos recursos desenvolvam e implantem sistemas poderosos.

###@ Atualizações sobre agentes de IA

Desde o último Relatório (janeiro 2025), avanços na forma como os desenvolvedores combinam modelos de IA com ferramentas possibilitaram o desenvolvimento de agentes de IA cada vez mais poderosos. Agentes de IA são projetados para perseguir objetivos, que muitas vezes são especificados pelos usuários em linguagem natural. Para atingir esses objetivos, eles recebem acesso a ferramentas, como memória, uma interface de computador e navegadores da web. Essas ferramentas e o código usado para combiná-las com o modelo são chamados de ‘scaffolding’ (andaimes), e ajudam os agentes de IA a interagir autonomamente com o mundo, fazer planos, lembrar detalhes importantes e perseguir objetivos (‡88*, ‡89) com muito menos supervisão ou assistência de seres humanos. Por exemplo, Manus AI é um agente de IA popular que pode automatizar várias tarefas, incluindo pesquisa na Web, desenvolvimento de software e compras online (‡90). A Figura 1.3 ilustra um exemplo simples de um agente de IA composto por um modelo de IA de uso geral ‘brain’ que pode planejar, raciocinar e usar ferramentas iterativamente para memória, navegação na web e uso do computador.

A infraestrutura digital para agentes de IA está se expandindo (‡91) e eles se tornaram cada vez mais comuns em diversos setores (‡92, ‡93, ‡94). Agentes de IA foram desenvolvidos para tarefas como pesquisa (‡37), engenharia de software (‡95), controle robótico (‡96) e atendimento ao cliente (‡97). Pesquisas e desenvolvimento em andamento resultaram em agentes de IA ou sistemas multiagente cada vez mais capazes e mais autônomos. Pesquisadores estimaram que a complexidade das tarefas de benchmark de software que agentes de IA podem realizar dobra aproximadamente a cada sete meses (ver também §1.2. Capacidades atuais) (‡98). Especialistas argumentam que agentes de IA cada vez mais capazes darão origem tanto a grandes oportunidades quanto a riscos (‡99, ‡100*) (ver §2.2.1. Desafios de confiabilidade).

###@ Lacunas de evidência

As principais lacunas de evidência em torno do processo de desenvolvimento de sistemas de IA de propósito geral decorrem da falta de informações publicamente disponíveis sobre como eles são desenvolvidos. Alguns desenvolvedores são altamente transparentes sobre como desenvolvem sistemas de IA de propósito geral (‡1, ‡101). No entanto, em geral, há um grau limitado de conhecimento público e de formuladores de políticas sobre como a maioria dos modelos avançados é desenvolvida, protegida, avaliada e implantada. Isso é particularmente verdadeiro para sistemas de IA implantados internamente que são usados dentro de empresas de IA, mas não são usados nem compreendidos por partes interessadas externas (‡102, ‡103). Essa visibilidade externa limitada cria desafios para a transparência e a supervisão. Vários pesquisadores apontaram para a existência de transparência limitada e inconsistente em torno dos dados de treinamento (‡104, ‡105, ‡106), dos modelos de IA de propósito geral (‡107, ‡108), de agentes de IA (‡92), de avaliações (‡109), de pipelines de desenvolvimento (‡110) e de segurança (‡111). As limitações à divulgação externa às vezes são necessárias para proteger segredos comerciais das empresas e propriedade intelectual. Ao mesmo tempo, a baixa transparência torna mais difícil para pesquisadores independentes e formuladores de políticas estudarem modelos e sistemas de IA de propósito geral.


