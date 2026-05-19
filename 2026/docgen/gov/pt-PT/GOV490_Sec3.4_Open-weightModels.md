##########
>white|orangered|left|14|30|hr Seção 3.4
### 3.4. Modelos de código aberto
>white|orangered|left|24|30|hb Modelos de pesos abertos

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informação-chave
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ O nível de acesso que as empresas de IA fornecem às “pesos” de seus modelos afeta os riscos que esses modelos apresentam. Pesos são os parâmetros matemáticos que permitem que modelos de IA processem entradas e gerem saídas. Para qualquer modelo específico, as empresas podem optar por manter os pesos totalmente privados, fornecer a alguns usuários algum acesso limitado ou permitir que qualquer pessoa os faça download na íntegra. Modelos cujos pesos estão publicamente disponíveis são chamados de “modelos de pesos abertos”.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Modelos de pesos abertos facilitam a pesquisa e a inovação, mas suas salvaguardas podem ser removidas com mais facilidade. Em todo o mundo, diversos atores – especialmente aqueles com menos recursos – podem usar modelos de pesos abertos para fins de pesquisa e comerciais. No entanto, em comparação com os modelos de pesos fechados, os modelos de pesos abertos são mais facilmente modificados para exibir comportamentos potencialmente prejudiciais, e  s mais difícil.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ As disponibilizações de modelos de código aberto não podem ser revertidas. Uma vez disponibilizados, os pesos do modelo não podem ser recuperados. Isso torna mais difícil mitigar possíveis danos decorrentes da disponibilização de um modelo com capacidades perigosas.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Desde a publicação do último Relatório (janeiro 2025), grandes lançamentos com pesos abertos reduziram a lacuna de capacidade em relação aos principais modelos fechados. Os desenvolvedores chineses DeepSeek e Alibaba lançaram, respectivamente, seus modelos R1 e Qwen, que alcançaram desempenho comparável ao dos principais modelos fechados, enquanto a OpenAI lançou seus primeiros modelos com pesos abertos desde 2019. As capacidades dos principais modelos fechados agora são estimadas como estando em menos de um ano à frente dos principais modelos com pesos abertos em benchmarks proeminentes de IA.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Um desafio-chave de políticas públicas é acessar os benefícios que os modelos open-weight oferecem, ao mesmo tempo em que se gerenciam seus riscos distintos. Uma abordagem é avaliar os modelos open-weight em termos de seu «risco marginal»: a medida em que sua disponibilização aumenta, de forma contrafactual, o risco social além daquele já imposto por modelos existentes ou outras tecnologias. No entanto, isso é complexo na prática. Pequenos aumentos no risco marginal ao longo do tempo também podem se somar a aumentos substanciais no risco geral.
>oldlace|black||11|15|br      


Modelos de código aberto com parâmetros disponibilizados publicamente para download têm implicações distintas para muitos dos desafios discutidos nas seções anteriores. Os ‘pesos’ de um modelo de IA contêm as informações cruciais que lhe permitem gerar respostas úteis para os usuários. Uma vez disponibilizados, esses pesos não podem ser recolhidos: qualquer pessoa pode baixá-los, estudá-los, modificá-los, compartilhá-los e usá-los em seus próprios computadores ou contas na nuvem. Quando os pesos estão abertamente disponíveis, outras pessoas podem construir e modificar o modelo com mais facilidade, atendendo a necessidades diversas e impulsionando a inovação (‡1317). Contudo, pelo mesmo mecanismo, usuários com intenções maliciosas também podem remover proteções com mais facilidade e modificar modelos de código aberto para usos nocivos (‡1122, ‡1160). Isso levantou a questão de se alguns modelos de código aberto devem ser submetidos a requisitos específicos (por exemplo, testes mais rigorosos antes do lançamento) ou, inversamente, receber isenções específicas (por exemplo, de exigências de reporte regulatório) (‡1033).

###@ Contexto sobre modelos de código aberto

>white|orangered||14|15.5|bb Modelos de código aberto podem ser, mas não necessariamente, modelos “open source”

Embora sejam frequentemente referidos como ‘open source’, a maior parte dos modelos disponibilizados publicamente é descrita de forma mais precisa como ‘open-weight’. Isso ocorre porque, embora os desenvolvedores forneçam os pesos do modelo, eles não disponibilizam o código de treinamento associado nem os conjuntos de dados. Além disso, o software open source geralmente é caracterizado por licenças permissivas que impõem requisitos mínimos aos agentes a jusante que usam ou modificam o software (‡1318). Por exemplo, os modelos Llama da Meta têm condições de licença restritivas e incluem apenas código de inferência, não código de treinamento, e portanto normalmente não são considerados open source (‡1319, ‡1320). As opções de disponibilização de modelos existem em um espectro que vai de totalmente fechado a totalmente open source, com diferentes compromissos entre risco e benefício em cada ponto (‡1086*, ‡1320, ‡1321). A Tabela 3.9 descreve essas opções.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Totalmente fechado
  Os utilizadores não podem interagir diretamente com o modelo de forma alguma
  Exemplos: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Acesso hospedado
  Os usuários só podem interagir por meio de uma aplicação ou interface específica, como uma aplicação móvel de chatbot
  Exemplos: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Acesso à API ao modelo
  Os usuários podem enviar solicitações ao modelo por meio de código, permitindo o uso em aplicativos externos
  Exemplos: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb Acesso à API para ajuste fino
  Os usuários podem ajustar o modelo para suas necessidades específicas
  Exemplos: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Pesos de código aberto: pesos disponíveis para download
  Os usuários podem baixar e executar o modelo nos próprios computadores.
  Exemplos: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Pesos, dados e código disponíveis para download com restrições de uso
  Os utilizadores podem transferir e executar o modelo, bem como o código de inferência e de treino, mas existem certas restrições de licença quanto ao seu uso
  Exemplos: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Totalmente aberto: pesos, dados e código disponíveis para download sem restrições de uso
  Os usuários têm liberdade total para baixar, usar e modificar o modelo, o código completo e os dados
  Exemplos: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 3.9: Opções de compartilhamento de modelo variando de totalmente fechado a totalmente aberto
>white|black||9|11|br Uma seleção ilustrativa de opções de compartilhamento de modelos, variando de modelos totalmente fechados (os modelos são privados e mantidos apenas para uso proprietário) a modelos totalmente abertos e open source (pesos do modelo, dados e código estão livre e publicamente disponíveis sem restrições de uso, modificação e compartilhamento). Os modelos que se enquadram nas quatro primeiras categorias são frequentemente chamados de ‘fechados’. Esta seção se concentra nas três linhas inferiores. Fonte: adaptado de Bommasani, 2024 (‡1317).


###@ Benefícios e riscos

>white|orangered|left|14|15.5|bb Modelos de código aberto podem ser mais facilmente personalizados e avaliados

Modelos de código aberto oferecem benefícios significativos para pesquisa, inovação e acesso. Conforme discutido em §1.1. O que é IA de propósito geral?, treinar modelos de IA de propósito geral é extremamente caro – os modelos de ponta custam centenas de milhões de dólares para serem desenvolvidos. Ao disponibilizar abertamente os pesos do modelo, atores com menos recursos podem replicar, estudar e construir sobre sistemas existentes. Sem esse acesso, comunidades em regiões de baixa capacidade de recursos correm o risco de serem excluídas dos benefícios da IA, tornando os pesos abertos críticos para permitir a participação da maioria global no desenvolvimento de IA (‡1322). Desenvolvedores a jusante podem ajustar finamente os modelos para aplicações diversas, por exemplo, adaptando-os para idiomas minoritários com poucos recursos ou otimizando desempenho para tarefas específicas como redação jurídica ou anotações médicas (‡1323, ‡1324*). Dessa forma, modelos com pesos abertos podem permitir que mais pessoas e comunidades usem e se beneficiem de IA do que seria possível de outro modo (‡1325). No caso de modelos que não sejam suficientemente capazes a ponto de serem perigosos, esses benefícios podem superar o risco adicional de liberar os pesos abertamente, embora isso dependa da tolerância ao risco dos tomadores de decisão relevantes.

O lançamento de pesos abertos também amplia o grupo de desenvolvedores e pesquisadores capazes de estudar o modelo, avaliar suas capacidades, testar vulnerabilidades e iterar sobre melhorias (‡1326, ‡1327). Isso torna mais provável que aplicações benéficas e falhas prejudiciais sejam identificadas, embora isso não seja garantido (‡1328, ‡1329). Os usuários também podem executar modelos de pesos abertos em seus próprios dispositivos, permitindo que mantenham o controle sobre dados sensíveis e evitem enviá-los para servidores de terceiros.

Há benefícios adicionais quando os desenvolvedores compartilham informações como dados de treinamento, código, ferramentas de avaliação e documentação, bem como pesos do modelo (‡1320, ‡1330, ‡1331, ‡1332*). Com mais informações, os desenvolvedores a jusante e outros pesquisadores podem compreender melhor os modelos de pesos abertos e adaptá-los a novas aplicações.

>white|orangered|left|14|15.5|bb As salvaguardas de modelos de código aberto são mais fáceis de remover, o que possibilita um uso malicioso potencial

Modelos de código aberto também apresentam riscos adicionais porque suas salvaguardas são mais fáceis de remover. Embora tanto modelos de código aberto quanto modelos fechados possam ter salvaguardas para recusar solicitações prejudiciais do usuário, essas salvaguardas são muito mais fáceis de remover em modelos de código aberto. Agentes maliciosos podem fazer fine-tuning de um modelo para otimizar seu desempenho para aplicações prejudiciais, remover partes do código projetadas para impedir usos nocivos, ou desfazer um fine-tuning de segurança anterior (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Como resultado, pesos de modelos abertos podem agravar os riscos de uso indevido discutidos em §2.1. Riscos de uso malicioso ao permitir que mais atores aproveitem e aprimorem capacidades existentes para fins maliciosos sem supervisão (‡1122, ‡1315). Embora muitos usuários não terão a habilidade ou o incentivo para remover salvaguardas em modelos de código aberto, agentes maliciosos altamente motivados são uma preocupação. Além disso, agentes maliciosos também podem conseguir usar modelos de código aberto para identificar vulnerabilidades em modelos fechados semelhantes (‡1055*). Essas falhas são mais difíceis de encontrar executando apenas modelos fechados, devido ao maior controle e às medidas de monitoramento que os provedores de modelo fechado conseguem implementar.

>white|orangered|left|14|15.5|bb Compartilhar os pesos do modelo é irreversível

Uma vez que os pesos do modelo estejam disponíveis para download público, não há como implementar um rollback em massa de todas as cópias existentes. Plataformas de hospedagem na Internet, como GitHub e Hugging Face, podem remover modelos de suas plataformas, dificultando que alguns agentes encontrem cópias baixáveis, e criando uma barreira significativa para muitos usuários maliciosos ocasionais (‡1339). No entanto, agentes determinados ainda podem obter cópias se o modelo tiver sido baixado e rehospedado em outro lugar ou armazenado localmente. Além disso, desenvolvedores a jusante que integram modelos de pesos abertos em seus sistemas também herdam quaisquer falhas, como vulnerabilidades a ataques adversariais (‡1055) ou capacidades do modelo para contornar sistemas de monitoramento (ver §2.2.2. Perda de controle) (‡1315). Diferentemente de modelos fechados, nos quais os provedores podem universalmente implementar correções, os desenvolvedores de modelos de pesos abertos não podem garantir que as atualizações serão adotadas pelos usuários.

###@ Atualizações

Desde a publicação do último Relatório (janeiro de 2025), a lacuna de capacidade entre os modelos open-weight líderes e os modelos closed diminuiu. Os desenvolvedores chineses tornaram-se, em particular, provedores importantes de modelos open-weight. Em janeiro de 2025, a DeepSeek lançou seu modelo R1, que atingiu desempenho comparável ao da o1 da OpenAI em diversos benchmarks (‡1340). Os modelos Qwen da Alibaba também ganharam tração, ocupando a primeira posição para um modelo open-weight no Chatbot Arena, um benchmark de desempenho amplamente usado, em agosto de 2025 (‡1341, ‡1342*). Em agosto de 2025, a OpenAI lançou seus primeiros modelos open-weight desde a disponibilização do GPT-2 em 2019, gpt-oss-120b e gpt-oss-20b. A Meta continuou lançando modelos Llama com pesos abertos. As capacidades dos modelos closed líderes agora são estimadas como sendo inferiores a um ano em relação aos modelos open-weight líderes em benchmarks proeminentes de IA (Figura 3.10).

###@ Lacunas de evidência

Uma lacuna fundamental de evidências diz respeito à eficácia no mundo real de soluções técnicas para impedir o uso indevido de modelos com pesos abertos. Pesquisadores têm proposto diversas abordagens para tornar os modelos resistentes a adulterações. Isso inclui novas técnicas de treinamento projetadas para fazer os modelos resistirem a modificações nocivas (‡1276), filtragem de conteúdo nocivo dos dados de treinamento (‡55) e defesas contra jailbreaks (‡675, ‡676). Essas técnicas agora estão sendo adotadas em lançamentos no mundo real de grandes desenvolvedores. Por exemplo, a OpenAI empregou algumas dessas técnicas em seus modelos gpt-oss, reportando que versões ajustadas adversarialmente não atingiram limiares altos de capacidade (‡1344*). No entanto, a pesquisa mostrou que agentes mal-intencionados podem desativar salvaguardas re-treinando os modelos com exemplos nocivos (‡1345, ‡1346). Além disso, ainda é desafiador avaliar de forma confiável a robustez das salvaguardas, tornando incerta sua eficácia contra ataques no mundo real (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Figura 3.10: Lacuna de capacidade entre os modelos de IA abertos e os modelos de IA fechados de ponta
>white|black||9|11|br Pontuações do Epoch Capabilities Index (ECI) dos modelos abertos (azul escuro) com melhor desempenho e dos modelos fechados (azul claro) ao longo do tempo. O ECI combina pontuações de 39 benchmarks em uma única escala geral de capacidade. Os melhores modelos abertos ficam cerca de 1 ano atrás dos modelos fechados. Fonte: Epoch AI, 2025 (‡1343).


###@ Mitigações

Mitigações técnicas para riscos de modelos de código aberto operam ao longo de todo o processo de desenvolvimento e implantação de IA (‡1141, ‡1195, ‡1347). Por exemplo, quando os modelos estão sendo desenvolvidos, desenvolvedores e adaptadores de terceiros podem filtrar conteúdo sensível dos dados de treinamento para minimizar capacidades prejudiciais. Remover exemplos prejudiciais dos dados de treinamento de um modelo pode impedir o fine-tuning adversarial com 10 vezes mais eficácia do que defesas adicionadas após o treinamento, embora também possa afetar capacidades benéficas (‡55). Provedores de aplicações de IA também podem implementar mecanismos de relato de incidentes e resposta (‡1348).

Além disso, plataformas de hospedagem como HuggingFace e GitHub podem estabelecer termos de serviço da plataforma para remover modelos modificados com finalidades prejudiciais (‡1141, ‡1324). Os desenvolvedores de modelos podem fornecer acesso total aos auditores antes do lançamento, ou optar por uma estratégia de lançamento “faseado” — disponibilizando modelos para grupos progressivamente maiores (‡1086). Isso pode ajudar a identificar possíveis falhas ou vulnerabilidades antes de um modelo ficar amplamente disponível (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Observação 3.1: Segurança dos pesos do modelo
>oldlace|black|left|13|15|hb Observação 3.1: Segurança do peso do modelo
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  Os riscos discutidos nesta seção pressupõem que os pesos do modelo sejam disponibilizados intencionalmente. No entanto, os pesos de modelos fechados também podem se tornar acessíveis por meio de roubo ou vazamento. Modelos fechados custam centenas de milhões de dólares para serem desenvolvidos (§1.1. O que é IA de propósito geral?) e, em média, são mais capazes do que modelos com pesos abertos (‡1343). Isso os torna alvos atraentes para agentes que vão de hackers amadores a estados-nação que buscam obter modelos de IA líderes.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Os pesos do modelo fechados e furtados representariam riscos semelhantes aos descritos acima para modelos com acesso aberto, mas potencialmente sem quaisquer das mitigações. Agentes maliciosos poderiam remover salvaguardas dos modelos mais capazes. Ao contrário de desenvolvedores legítimos, esses agentes não enfrentariam as restrições de reputação, legais ou comerciais que atualmente incentivam as empresas de IA de ponta a implantar seus modelos com segurança.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Os níveis de segurança atuais variam entre a indústria e podem ser insuficientes contra atacantes sofisticados. Alguns desenvolvedores se comprometem em proteger os pesos do modelo contra sindicatos de cibercrime e ameaças internas (‡582), enquanto outros não fizeram compromissos públicos de segurança (‡1109, ‡1349). A pesquisa indica que os data centres de IA podem não ser capazes de resistir a ataques dos atores mais sofisticados e bem providos de recursos (‡582, ‡1350, ‡1351). Em dezembro de 2025, não há instâncias confirmadas e documentadas publicamente de roubo de pesos do modelo. No entanto, outros incidentes de violação de segurança em empresas líderes de IA foram relatados, incluindo uma infiltração nos sistemas de email da Microsoft (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Fechar essas lacunas de segurança exigiria investimentos substanciais em hardware, software, pessoal e segurança da instalação. Algumas melhorias de segurança poderiam ser implementadas relativamente rapidamente com esforço coordenado (‡1122). Outras medidas críticas, no entanto, como proteger as cadeias de suprimento de hardware e as instalações, provavelmente levariam anos (‡1122). Empresas privadas também podem não ter os recursos ou a informação necessários para desenvolver proteções adequadas por conta própria. Por exemplo, desenvolvedores de IA não têm acesso à inteligência de ameaças classificada que os governos têm (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Desafios para formuladores de políticas

Um desafio fundamental para os formuladores de políticas é garantir os benefícios da partilha de modelos com pesos abertos sem aumentar significativamente o risco. Para evitar danos catastróficos, os desenvolvedores de modelos com pesos abertos não devem disponibilizar modelos sem avaliar os riscos, tanto utilizando métodos de avaliação estabelecidos usados para modelos fechados quanto por meio de testes adicionais, dado que agentes mal-intencionados podem fazer fine-tuning em modelos e remover proteções de segurança. Na prática, isso pode ser difícil porque o desenvolvimento de capacidades pode ser imprevisível, os lançamentos com pesos abertos são irreversíveis e os esforços de avaliação são necessários para prever quando um lançamento representaria um potencial de dano significativo. Uma abordagem é avaliar o “risco marginal” das divulgações abertas: até que ponto o lançamento contrafactualmente aumenta o risco social além daquele já imposto por modelos existentes ou por outras tecnologias (‡556, ‡1033, ‡1354, ‡1355) (ver §3.2. Práticas de gestão de risco). Contudo, estimar como um sistema irá aumentar ou diminuir o risco a jusante após ter sido implantado é complexo e depende do contexto. Aumentos incrementais no risco com lançamentos sucessivos podem se acumular ao longo do tempo, levando a aumentos substanciais no risco total, mesmo que o risco marginal associado a cada lançamento pareça aceitável (‡1356, ‡1357). A natureza de uso duplo das capacidades de IA ainda complica a governança: recursos que habilitam aplicações benéficas na medicina ou na pesquisa podem ser repropurados para causar danos e, uma vez que os pesos sejam públicos, pode ser difícil distinguir usos legítimos de usos maliciosos. Também não está claro quem deve ser responsabilizado quando modelos com pesos abertos são modificados para fins prejudiciais.

