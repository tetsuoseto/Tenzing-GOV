##########
>white|orangered|left|14|30|hr Seção 3.3
### 3.3. Medidas técnicas de proteção e monitoramento
>white|orangered|left|24|30|hb Salvaguardas técnicas e monitoramento

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informação-chave
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Uma ampla gama de salvaguardas técnicas é usada em diferentes etapas do desenvolvimento e do uso de IA. Isso inclui técnicas aplicadas durante o desenvolvimento do modelo para tornar os sistemas mais robustos e resistentes a uso indevido (como curadoria de dados), monitoramento e controle durante a implantação (como filtragem de conteúdo e supervisão humana) e ferramentas pós-implantação para monitorar o ecossistema mais amplo de IA (como proveniência e detecção de conteúdo).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ As salvaguardas técnicas têm limitações e não impedem de forma confiável comportamentos prejudiciais em todos os contextos. Por exemplo, por vezes, os usuários conseguem obter saídas prejudiciais reescrevendo solicitações ou as dividindo em etapas menores. Da mesma forma, ferramentas como a marca d'água, que são projetadas para identificar conteúdo gerado por IA, muitas vezes podem ser removidas ou alteradas, o que limita sua confiabilidade.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ As limitações das salvaguardas individuais significam que pode ser necessário ‘defesa em profundidade’ para evitar certos resultados prejudiciais. Por exemplo, um sistema pode combinar um modelo treinado para segurança com filtros de entrada, filtros de saída e monitores de conteúdo.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Desde a publicação do último Relatório (janeiro de 2025), os pesquisadores avançaram na melhoria das salvaguardas, mas limitações fundamentais permanecem. Por exemplo, a taxa de sucesso de ataques projetados para burlar salvaguardas tem diminuído, mas ainda permanece relativamente alta. Também existem limitações fundamentais quanto ao nível de salvaguardas que pode ser aplicado de forma abrangente a modelos de código aberto.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Um desafio-chave para os formuladores de políticas é a evidência limitada sobre a eficácia das salvaguardas em diversos usos reais de sistemas de IA de finalidade geral. Os desenvolvedores de IA variam amplamente em quanto de informação compartilham sobre suas salvaguardas e monitoramento. Um desafio adicional é o potencial de compensações entre a aplicação de salvaguardas mais fortes e a manutenção do desempenho ou da utilidade do sistema.
>oldlace|black||11|15|br      


Desenvolvedores de IA podem usar várias salvaguardas técnicas úteis, porém imperfeitas, para mitigar e gerenciar riscos de sistemas de IA de propósito geral, mas os desafios de robustez persistem. Os desenvolvedores ainda não conseguem impedir totalmente que sistemas de IA de propósito geral realizem ações mesmo bem conhecidas e abertamente prejudiciais, como oferecer aos usuários instruções para cometer crimes. Por exemplo, pesquisadores demonstraram que salvaguardas de ponta podem ser contornadas por meio de métodos de prompting adversarial (isto é, ‘jailbreaks’) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), fazendo com que modelos quebrem tarefas prejudiciais complexas em etapas (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), e com modificações simples nos modelos (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Pesquisadores continuam trabalhando em salvaguardas contra mau funcionamento e uso indevido (‡690). Esses métodos variam amplamente quanto ao seu objetivo e eficácia, e seu impacto, em última instância, depende do contexto sociotécnico e de governança mais amplo no qual os sistemas de IA são construídos e implantados.

As salvaguardas técnicas podem, de forma ampla, ser divididas em três categorias: técnicas para desenvolver modelos mais seguros; técnicas usadas durante a implantação para monitoramento e controle; e técnicas que dão suporte ao monitoramento do ecossistema após a implantação. A Mesa 3.6 resume as salvaguardas técnicas discutidas, sua eficácia e desafios em aberto.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Desenvolver modelos mais seguros
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Curadoria de dados (‡1167)
  Remover dados prejudiciais para impedir que um modelo aprenda capacidades perigosas. Esses métodos podem ser úteis, incluindo para desenvolver modelos de código aberto (open-weight) que não possuem capacidades prejudiciais e resistem a ajustes finos (fine-tuning) prejudiciais (‡55). No entanto, há desafios com erros de curadoria e com a escalabilidade (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Aprendizado por reforço a partir de feedback humano (‡64*)
  Treinar o modelo para se alinhar com objetivos especificados, como ser útil e não prejudicial. Esta é uma forma eficaz de fazer com que modelos aprendam comportamentos benéficos (‡64*). No entanto, a otimização excessiva para aprovação humana pode fazer com que os modelos se comportem de forma enganosa ou de maneira bajuladora (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Técnicas de alinhamento pluralista (‡1170)
  Treinar o modelo para integrar múltiplas perspectivas divergentes sobre como ele deve agir. Essas técnicas ajudam a reduzir o grau em que os modelos favorecem perspectivas específicas (‡1170). No entanto, apesar dessas técnicas, a discordância humana é inevitável, e é difícil projetar formas amplamente aceitas de equilibrar perspectivas concorrentes (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Treinamento adversarial (‡677)
  Treinar o modelo para recusar causar danos (mesmo em contextos não familiares) e para resistir a ataques de usuários mal-intencionados (por exemplo, ‘jailbreaks’). Este é um método eficaz para fazer os modelos resistirem a tentativas de uso indevido (‡1064), mas os desafios de robustez persistem (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Desaprendizado (“unlearning”) de máquinas (‡1175, ‡1176)
  Treinar um modelo usando algoritmos especializados significa suprimir ativamente capacidades prejudiciais (por exemplo, conhecimento de agentes biológicos). Essas técnicas oferecem uma forma direcionada de remover capacidades prejudiciais de modelos (‡1175, ‡1176), mas os algoritmos atuais de unlearning podem não ser robustos e ter efeitos não intencionais sobre outras capacidades (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ferramentas de interpretabilidade e verificação de segurança (‡1177)
  Uma família diversificada de métodos de projeto e verificação destinados a oferecer uma garantia mais rigorosa de que os modelos tenham propriedades específicas relacionadas à segurança. Eles permitem que os avaliadores façam garantias de segurança com maior confiança (‡1177), mas os métodos atuais dependem de suposições e raramente são competitivos em desempenho na prática (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Monitoramento e controle
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mecanismos de monitoramento baseados em hardware (‡1179, ‡1180, ‡1181)
  Verificando que os processos autorizados estão em execução no hardware, a fim de estudar ameaças de segurança ou conformidade regulatória. Esses mecanismos oferecem formas únicas de monitorar quais computações estão sendo executadas no hardware e por quem (‡1181). No entanto, os mecanismos de hardware não conseguem monitorar todos os tipos de ameaças, e algumas técnicas exigem hardware especializado (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitores de interação do usuário (‡1154, ‡1166)
  Monitorar as interações dos usuários em busca de sinais de uso malicioso pode ajudar os desenvolvedores a encerrar o serviço para usuários maliciosos (‡1154, ‡1166). No entanto, a aplicação pode inadvertidamente prejudicar pesquisas benéficas sobre segurança (‡689), e algumas formas de uso indevido são difíceis de detectar (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitores de interação do usuário (‡1154, ‡1166)
  Monitorar interações de usuários em busca de sinais de uso malicioso pode ajudar os desenvolvedores a encerrar o serviço para usuários maliciosos (‡1154, ‡1166). No entanto, a aplicação da política pode inadvertidamente prejudicar pesquisas benéficas sobre segurança (‡689), e algumas formas de uso indevido são difíceis de detectar (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Filtros de conteúdo (‡65*, ‡725)
  Filtrar entradas e saídas potencialmente prejudiciais do modelo é uma forma muito eficaz de reduzir danos acidentais e riscos de uso indevido (‡725). No entanto, os filtros exigem computação adicional e são vulneráveis a alguns ataques (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitores de computação interna do modelo (‡744, ‡1183, ‡1184)
  Monitorar sinais de engano ou outras formas internas nocivas de cognição em modelos pode ser uma forma eficiente de detectar enganos (‡744, ‡1183, ‡1184). No entanto, os métodos atuais carecem de robustez e confiabilidade (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitores de cadeia de pensamento (‡430, ‡435)
  Monitorar o texto do chain-of-thought da cadeia de raciocinio do modelo em busca de sinais de comportamento enganoso ou de outros raciocínios prejudiciais é uma forma eficaz de entender e identificar falhas na maneira como os modelos raciocinam (‡435). No entanto, eles podem ser não confiáveis (‡752, ‡753, ‡1186) e, se os modelos forem treinados para produzir um chain of thought benigno, eles podem aprender comportamento enganoso (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Human in the loop (‡1187, ‡1188, ‡1189)
  A supervisão humana e as ações de anulação (overrides) para decisões do sistema são essenciais em algumas aplicações críticas para segurança (‡1187). No entanto, essas técnicas são limitadas por viés de automação e por limitações na velocidade de tomada de decisão humana (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Isolamento (‡1192)
  Impedir que um agente de IA influencie diretamente o mundo é uma forma eficaz de limitar o dano que ele pode causar (‡1192). No entanto, o sandboxing limita a capacidade do sistema de realizar diretamente certas tarefas (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Ferramentas para facilitar o monitoramento do ecossistema
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Técnicas de identificação de modelos de IA (‡1193*, ‡1194)
  Tornar os modelos, ou instâncias individuais de modelos, mais fáceis de identificar em casos de uso do mundo real ajuda com a perícia forense digital e com a conscientização do ecossistema (‡1195). No entanto, essas técnicas podem ser contornadas com alguns tipos de modificações de modelos (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Inferência de herança do modelo de IA (‡1197)
  Estas técnicas permitem que os pesquisadores estudem como os modelos são modificados no ecossistema de IA, especialmente modelos de pesos abertos. Elas ajudam com a computação forense digital e a conscientização do ecossistema (‡1198), mas seriam necessários projetos em grande escala para mapear de forma completa o ecossistema de modelos de pesos abertos (‡1198).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Filigranas e metadados (‡1199, ‡1200, ‡1201*)
  Estas técnicas tornam mais fácil detectar quando um trecho de texto, imagem, vídeo, etc., foi gerado ou modificado por IA, e por qual sistema. Elas facilitam uma melhor consciência do ecossistema (‡1199, ‡1200, ‡1201*). No entanto, marcas d'água e metadados podem ser forjados ou removidos por algumas modificações no conteúdo (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Detecção de conteúdo gerado por IA (‡1203, ‡1204, ‡1205*)
  Melhorar a capacidade dos usuários de distinguir entre conteúdo gerado por IA e conteúdo genuíno ajuda na análise forense digital e na conscientização do ecossistema (‡1203, ‡1204). No entanto, classificadores podem ser pouco confiáveis (‡1205*) e ter desempenho variável entre modalidades.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 3.6: Medidas de proteção técnicas discutidas nesta seção
>white|black||9|11|br Um resumo das salvaguardas técnicas discutidas nesta seção, dividido em métodos para desenvolver modelos mais seguros, monitoramento e controle em tempo de implantação, e técnicas para facilitar a monitoração do ecossistema.


###@ Desenvolver modelos mais seguros

Uma primeira linha de defesa contra danos causados por sistemas de IA de uso geral é tornar o modelo subjacente mais seguro. Esta subseção cobre salvaguardas que são “incorporadas aos parâmetros do modelo” durante o processo de desenvolvimento do modelo (Figura 3.6).

>white|orangered|left|14|15.5|bb A curadoria de dados de treinamento pode limitar o desenvolvimento de capacidades potencialmente perigosas

Modelos de IA de propósito geral são úteis precisamente porque desenvolvem uma ampla gama de conhecimentos e capacidades após processar dados de treinamento, mas alguns tipos de dados de treinamento são desproporcionalmente responsáveis pelo desenvolvimento de capacidades potencialmente perigosas. Por exemplo, um modelo de IA treinado em artigos de virologia pode ser melhor capaz de fornecer assistência em tarefas de biologia potencialmente prejudiciais (‡549, ‡1206*) (ver também §2.1.4. Riscos biológicos e químicos). Além disso, geradores de imagem/vídeo treinados em imagens de nudez humana também podem ser usados de forma indevida para criar deepfakes íntimos sem consentimento (‡308, ‡319) (ver também §2.1.1. Conteúdo gerado por IA e atividade criminal).

Filtrar os dados de treinamento é uma mitigação eficaz contra algumas capacidades indesejadas (‡319, ‡1167, ‡1207, ‡1208). No entanto, pode ser difícil filtrar os grandes conjuntos de dados usados para treinar modelos de IA de propósito geral (‡1168) devido a custos elevados (‡1209), erros de filtragem (‡1210) e impactos negativos na qualidade do conjunto de dados (‡1211). Esses desafios são agravados pela natureza multilíngue do texto da internet (‡1212), por vieses culturais na moderação de conteúdo (‡1211, ‡1213, ‡1214, ‡1215) e pelo fato de que a avaliação de se um determinado dado é “prejudicial” depende de fatores contextuais (‡1216). Ainda assim, filtrar materiais potencialmente prejudiciais dos dados de treinamento mostra promessa para tornar os modelos mais seguramente seguros, incluindo tornar modelos de código aberto mais resistentes a adulterações prejudiciais (‡55). As relações entre o conteúdo dos dados de treinamento e as capacidades emergentes do modelo ainda não são totalmente compreendidas (‡1195), e a filtragem parece ser mais eficaz para limitar capacidades prejudiciais quando aplicada a domínios amplos de conhecimento (‡55) em comparação com comportamentos mais restritos (‡1206, ‡1217). Veja §3.4. Modelos de código aberto para discussão adicional.

![figure 3.6](images/fig3.6_safeguards.png)

##### Figura 3.6: Onde aplicar salvaguardas técnicas
>white|black||9|11|br Salvaguardas técnicas podem ser aplicadas em diferentes etapas do desenvolvimento do modelo. A curadoria de dados molda o que os modelos aprendem durante o pré-treinamento e o ajuste fino. Métodos baseados em treinamento, como aprendizado por reforço a partir de feedback humano e treinamento de robustez, ajustam o comportamento do modelo. Métodos de teste, como ataques adversariais, identificam as vulnerabilidades restantes. Algumas técnicas, como algoritmos com base em safe-by-design, abrangem várias etapas. Fonte: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Métodos para treinar modelos de IA de propósito geral para serem úteis e seguros, baseiam-se principalmente em feedback humano

É difícil treinar e avaliar modelos de forma confiável para se alinharem a princípios de alto nível, como serem úteis, seguros e honestos. Na prática, os desenvolvedores buscam alcançar isso ajustando modelos de IA por meio de demonstrações e feedback de humanos. Por exemplo, o paradigma principal para ajustar modelos de IA, conhecido como ‘aprendizado por reforço a partir de feedback humano’, é baseado no treinamento de modelos para produzir saídas que os anotadores humanos avaliam positivamente (‡1218). No entanto, o feedback positivo de humanos é uma métrica substituta falha para comportamento benéfico (‡737, ‡878, ‡1219, ‡1220) e é limitado por erros e vieses humanos (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Isso leva a vários desafios: modelos ajustados por reforço por meio de aprendizado a partir de feedback de humanos às vezes agradam ao usuário, um comportamento conhecido como ‘sycophancy’ (‡358, ‡740, ‡1226, ‡1227); fornecer respostas que sejam úteis em alguns contextos, mas prejudiciais em outros (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); fornecer respostas difíceis de avaliar quanto à correção (‡1233); ou executar ações cuja utilidade ou nocividade é uma questão de opinião (‡1234). A Mesa 3.7 fornece exemplos desses desafios. Algumas pesquisas têm como objetivo desenvolver métodos para ajudar humanos a avaliar melhor soluções para tarefas complexas com assistência de IA (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). No entanto, esses métodos atualmente têm confiabilidade limitada, e o grau em que eles são usados para treinar os modelos de IA mais avançados de hoje não é conhecido publicamente.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sycophancy/pleasing (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Explicação:
>white|black|left|11|13|br O modelo só fornece feedback positivo, deixando de apontar a falta de uma estrutura correta de sílabas de haiku 5-7-5.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Algumas ações são úteis em alguns contextos, mas prejudiciais em outros (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Explicação:
>white|black|left|11|13|br As informações sobre risco biológico podem ser usadas para educação e defesa, mas também para informar atores maliciosos.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb O comportamento correto é difícil de verificar (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Explicação:
>white|black||11|13|br A correção desta resposta é difícil de avaliar porque requer experiência médica. Mesmo para um médico experiente, avaliar respostas como esta exige tempo e atenção cuidadosa aos detalhes.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Os humanos discordam sobre o que está correto (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Explicação:
>white|black|left|11|13|br As pessoas discordam significativamente sobre qual é a resposta correta.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 3.7: Solicitação do usuário e resposta do modelo de IA
>white|black||9|11|br Exemplos de desafios ao especificar e incentivar ações benéficas a partir de modelos de IA.


>white|orangered|left|14|15.5|bb Os seres humanos nem sempre concordam sobre quais comportamentos são desejáveis, exigindo métodos para equilibrar preferências concorrentes

Os humanos nem sempre concordam sobre quais respostas ou ações os modelos de IA devem ou não produzir (‡1006). Isso torna fundamentalmente desafiador desenvolver modelos cujas ações e impactos estejam amplamente alinhados com os interesses da sociedade (‡420). Alguns pesquisadores estudam de quem as preferências são refletidas nos sistemas de IA (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) e trabalham para desenvolver técnicas de “alinhamento pluralístico” que buscam equilibrar preferências concorrentes (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Por exemplo, os desenvolvedores de IA podem projetar sistemas para evitar gerar respostas controversas recusando-se a responder a certas solicitações, ou alinhar com a visão mediana em alguma amostra relevante de pessoas, ou personalizar os sistemas para usuários individuais.

Um desafio comum para essas abordagens é que, em geral, os sistemas de IA não conseguem se alinhar de maneira igualmente adequada com as preferências de todos, e que seus impactos sociais a jusante afetarão diferentes grupos de pessoas de formas distintas. Alguns pesquisadores têm argumentado que a maior parte das abordagens técnicas de alinhamento pluralístico falha em abordar, e potencialmente distrai de, desafios mais profundos, como vieses sistemáticos, dinâmicas de poder social e a concentração de riqueza e influência (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb Os desenvolvedores de IA usam 'treinamento adversarial' para melhorar a robustez do modelo

É desafiador garantir que modelos de IA traduzam de forma robusta os comportamentos benéficos que aprendem durante o treinamento para contextos reais de implantação. Mesmo modelos treinados com um sinal de aprendizagem “perfeito” podem falhar ao generalizar com sucesso para todos os contextos não vistos (‡738, ‡739, ‡1255, ‡1256, ‡1257). Por exemplo, alguns pesquisadores descobriram que chatbots têm maior probabilidade de tomar ações prejudiciais em idiomas que estão sub-representados nos seus dados de treinamento (‡159, ‡880, ‡1258*, ‡1259), o que inclui muitas línguas faladas predominantemente no Sul Global.

Nos últimos anos, os pesquisadores também criaram um grande conjunto de ferramentas de técnicas de “ataque adversário” que podem ser usadas para fazer com que os modelos gerem respostas potencialmente prejudiciais (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Por exemplo, uma iniciativa recente obteve por crowdsourcing mais de 60,000 exemplos diversos de ataques bem-sucedidos contra modelos de IA de última geração, o que os fez violar as políticas das empresas sobre comportamento aceitável do modelo (‡1149). A Tabela 3.8 mostra exemplos de técnicas de “jailbreak” que os pesquisadores demonstraram que podem fazer com que os modelos atendam a solicitações prejudiciais.

Um método para melhorar a robustez dos modelos é conhecido como ‘treinamento adversarial’ (‡1064). Ele envolve construir ‘ataques’ (por exemplo, jailbreaks) projetados para fazer um modelo agir de maneira indesejada e treinar o modelo para lidar com esses ataques de forma apropriada. No entanto, o treinamento adversarial é imperfeito (‡1260, ‡1261). Os atacantes conseguem consistentemente desenvolver novos ataques bem-sucedidos contra modelos de ponta (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Como os desenvolvedores precisam de exemplos específicos de modos de falha para treinar contra eles (‡512, ‡1263), o resultado é um jogo contínuo de ‘gato e rato’, no qual os desenvolvedores atualizam continuamente os modelos em resposta a vulnerabilidades recém-descobertas, e os adversários buscam continuamente novos ataques. Alguns pesquisadores propuseram treinamento adversarial em maior escala (‡1264, ‡1265) ou novos algoritmos (‡675, ‡676, ‡1263, ‡1266, ‡1267) para melhorar a robustez, mas os sistemas modernos de IA permanecem persistentemente vulneráveis.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Estratégia: fazer pedidos prejudiciais em texto cifrado, como código Morse (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Estratégia: preencha o sistema com exemplos de respostas em conformidade a solicitações prejudiciais (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Estratégia: Faça solicitações prejudiciais em idiomas de baixo recurso que provavelmente sejam menos usados no treinamento (por exemplo, Suaíli (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Estratégia: Quebrar uma tarefa prejudicial em múltiplas subtarefas inofensivas (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Mesa 3.8: estratégias de jailbreak
>white|black||9|11|br Atores maliciosos e equipes de red teaming têm usado vários tipos de “jailbreaks” para fazer modelos de IA atenderem a solicitações prejudiciais que normalmente recusariam devido a salvaguardas. Os exemplos de saídas foram escritos pelos autores do Relatório apenas para fins ilustrativos. Muitos modelos de IA de ponta atuais já resistem à maioria desses métodos, mas novas técnicas de jailbreak continuam a ser descobertas.


>white|orangered|left|14|15.5|bb Técnicas de “Unlearning” podem mitigar capacidades específicas prejudiciais do modelo

Outra estratégia para mitigar riscos de IA de uso geral é ajustar modelos para não terem capacidades em domínios específicos de alto risco (‡1175, ‡1176). Por exemplo, pesquisadores estão trabalhando para desenvolver algoritmos de “machine unlearning” que possam suprimir especificamente habilidades relacionadas a ameaças biológicas ou à geração de imagens fotorrealistas de corpos humanos nus (‡903, ‡1272, ‡1273). Esses métodos podem tornar os modelos substancialmente mais seguros, ao custo de limitar algumas utilizações positivas das capacidades “unlearned”. Limitar o conhecimento dos modelos de IA em domínios prejudiciais também foi proposto como uma forma de projetar modelos open-weight “tamper-resistant” que possam resistir a ajustes finos prejudiciais (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). No entanto, até o momento, isso tem sido desafiador de fazer de maneira robusta (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Veja §3.4. Modelos open-weight para discussão adicional.

>white|orangered|left|14|15.5|bb Alguns pesquisadores estão trabalhando em métodos para garantias de segurança mais robustas por meio da interpretação de estados internos do modelo ou da verificação matemática

Alguns pesquisadores estão trabalhando em métodos para verificar com mais rigor as propriedades de segurança relacionadas a modelos. Em uma abordagem, os pesquisadores buscam interpretar as computações internas dos modelos para, ou identificar riscos, ou construir argumentos mais convincentes de que o modelo é seguro (‡1285, ‡1286). Por exemplo, em uma prova de conceito, os pesquisadores demonstraram que ferramentas para analisar a computação interna de um modelo de linguagem poderiam ajudar avaliadores a identificar comportamentos prejudiciais (‡1287). Em 2025, a Anthropic também começou a analisar os componentes internos do modelo como uma forma de estudar a consciência situacional do modelo e o “intento” (‡2). No entanto, esses tipos de métodos atualmente não são comuns ou não são conhecidos por serem competitivos com outras técnicas de avaliação.

Uma abordagem diferente para obter garantias mais fortes de segurança envolve a construção de provas matemáticas de que um modelo irá satisfazer certas condições de segurança (‡1177, ‡1282, ‡1288). No entanto, essas provas assumem que o contexto de teste corresponde ao contexto de implantação e não foram testadas contra muitos tipos de adversários.

Atualmente, também não é possível dimensioná-los para modelos grandes. No geral, há um debate significativo entre especialistas sobre a promessa de métodos de interpretabilidade e verificação formal.

###@ Monitoramento e controle em tempo de implantação

Além de salvaguardas implementadas durante o desenvolvimento do modelo, uma segunda linha de defesa contra comportamentos prejudiciais são salvaguardas externas que se concentram em monitorar e controlar as ações de um modelo ou sistema durante a implantação. Tais salvaguardas ajudam a mitigar falhas e mau uso, como saídas alucinadas e instruções prejudiciais.

>white|orangered|left|14|15.5|bb Os deployers de modelos podem usar uma variedade de ferramentas para identificar e abordar comportamentos de alto risco do modelo

Quando um sistema de IA está em execução, um implantador pode monitorar sinais de risco e intervir se eles aparecerem. Por exemplo, eles podem inspecionar as entradas de um modelo em busca de sinais de ataques adversariais, filtrar conteúdo inadequado das saídas, ou monitorar a cadeia de pensamento do sistema em busca de sinais de planos prejudiciais. Pontos nos quais implantadores podem monitorar e intervir sobre como as pessoas estão usando seus sistemas incluem hardware (‡1180, ‡1181), interações do usuário (‡1154, ‡1166), entradas e saídas (‡65, ‡725, ‡1182), computações internas (‡744, ‡1183, ‡1184) e cadeia de pensamento (‡430, ‡435). Também existem múltiplas ações que implantadores podem executar quando riscos são identificados. Elas incluem registrar informações, filtrar/modificar conteúdo prejudicial, sinalizar atividade anormal, desligamentos do sistema ou acionar mecanismos de segurança. A Figura 3.7 ilustra exemplos de mecanismos comuns de monitoramento e controle.

Uma vez que são versáteis e frequentemente eficazes, esses mecanismos são amplamente utilizados e podem prevenir muitos tipos de danos não intencionais (‡725, ‡751, ‡1289). No entanto, essas salvaguardas são imperfeitas, especialmente sob ataques maliciosos otimizados para fazê-las falhar (‡752, ‡1182). Pesquisas recentes também exploraram como a monitoração pode ser pouco confiável se um sistema for otimizado usando as pontuações de um monitor, por exemplo, tornando a cadeia de pensamento menos confiável (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Figura 3.7: Técnicas de monitoramento e controle
>white|black||9|11|br As técnicas de monitoramento e controle operam em múltiplos pontos: triagem de entradas e saídas para conteúdo prejudicial, acompanhamento dos estados internos do modelo, restrição de ações externas por meio de sandboxing e manutenção de supervisão humana. Fonte: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Humanos no loop permitem supervisão direta em ambientes de alto risco

Para reduzir a chance de falhas de agentes de IA (ver §2.2.1. Desafios de confiabilidade), os implantadores podem buscar projetar sistemas de IA que funcionem em cooperação com humanos, em vez de totalmente de forma autônoma (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Isso é importante para casos de uso em que decisões incorretas podem causar danos significativos, como em finanças, saúde ou policiamento. No entanto, ter um ‘humano no circuito’ é frequentemente impraticável. Às vezes, a tomada de decisão acontece rápido demais, como em aplicativos de chat com milhões de usuários. Em outros casos, vieses humanos e erros podem amplificar riscos devido a erros cumulativos (‡1187). Humanos no circuito também tendem a apresentar ‘viés de automação’, o que significa que muitas vezes depositam mais confiança no sistema de IA do que o que seria justificável (‡1190, ‡1191) (ver §2.3.2. Riscos à autonomia humana).

>white|orangered|left|14|15.5|bb O ‘sandboxing’ protege contra riscos decorrentes de comportamentos autônomos

Agentes de IA que podem agir autonomamente sem limitações na Web ou no mundo físico apresentam riscos elevados (consulte §2.2.1. Desafios de confiabilidade). ‘Sandboxing’ envolve limitar as formas pelas quais agentes de IA podem influenciar diretamente o mundo, tornando muito mais fácil supervisioná-los e gerenciá-los (‡640, ‡1192, ‡1295). Por exemplo, restringir a capacidade de um sistema de IA de publicar na internet ou de editar o sistema de arquivos de um computador pode impedir danos inesperados decorrentes de ações inesperadas (‡1296). No entanto, essas abordagens nem sempre podem ser usadas para aplicações em que um sistema de IA necessariamente deve agir diretamente no mundo.

###@ Ferramentas de monitoramento de ecossistemas: proveniência de modelo e de dados

As ferramentas de modelo e de proveniência de dados são ferramentas técnicas para estudar o ecossistema de IA, a fim de melhorar a conscientização sobre os usos a jusante e os impactos dos sistemas de IA.

>white|orangered|left|14|15.5|bb As técnicas de proveniência de sistemas de IA ajudam a rastrear os usos e os impactos dos sistemas

Desenvolvedores e implantadores podem usar várias técnicas para estudar o uso de modelos e sua disseminação ‘no mundo real’. Por exemplo, eles podem fornecer aos modelos comportamentos únicos de identificação (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) ou aplicar padrões exclusivos aos pesos de modelos individuais open-weight (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). No entanto, tornar essas técnicas mais resistentes a modificações do modelo é um problema em aberto (‡1195, ‡1196*). Pesquisadores também estão trabalhando em métodos para ‘inferir a herança do modelo’ (‡1197, ‡1198, ‡1305, ‡1306), ajudando a responder perguntas do tipo: ‘O modelo X foi uma versão fine-tuned ou destilada do modelo Y?’ Por fim, alguns desenvolvedores estão trabalhando em protocolos e infraestrutura para agentes de IA a fim de facilitar identificação e verificação quando interagem com sistemas externos (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Figura 3.8: Marcas d'água incorporam perturbações imperceptíveis em imagens e áudio
>white|black||9|11|br As marcas d'água incorporam perturbações imperceptíveis em imagens e áudio que permitem que o conteúdo gerado por IA seja identificado por ferramentas de detecção. Nesta figura, as marcas d'água tanto da imagem quanto do áudio são exageradas para melhorar a visibilidade. Fonte: imagem Chameleon do Unsplash (‡1313*). Outros elementos criados pelos autores do Relatório. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Figura 3.9: Taxas de sucesso de ataques de prompt injection
>white|black||9|11|br Taxas de sucesso de ataques de injeção de prompt, conforme relatadas por desenvolvedores de IA para modelos importantes lançados entre maio de 2024 e agosto de 2025. Cada ponto representa a proporção de ataques bem-sucedidos em 10 tentativas contra um modelo específico logo após o lançamento. A taxa de sucesso desses ataques relatada tem caído ao longo do tempo, mas permanece relativamente alta. Fonte: Zou et al. 2025 (‡1149), citado em Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb As técnicas de detecção de conteúdo de IA ajudam a monitorar a disseminação e os impactos de conteúdo gerado por IA

As marcas d'água, os metadados e outros detectores de conteúdo de IA podem ajudar os pesquisadores a rastrear e estudar o impacto no mundo real do conteúdo criado por IA. 

Primeiro, as marcas-d'água de dados são motivos discretos, mas distintos, inseridos em mídia digital que podem codificar informações sobre sua origem (‡1199, ‡1200, ‡1201*). Para texto, elas tipicamente assumem a forma de vieses sutis nas escolhas de palavras e no estilo (‡1308, ‡1309); para imagens e vídeo, padrões sutis sobre pixels (‡1310); e, para áudio, padrões sutis nas ondas sonoras (‡1311). A Figura 3.8 ilustra isso.

Além de marcas d’água, o conteúdo gerado por IA também pode ser salvo usando formatos de arquivo que armazenam metadados sobre como eles foram gerados. Por exemplo, muitos dispositivos móveis salvam arquivos de imagem e de áudio usando um formato de arquivo que pode armazenar informações sobre configurações da câmera, data/hora, localização, etc. (‡1312). Metadados semelhantes podem ser usados para armazenar informações sobre se os dados foram gerados por um sistema de IA. De modo semelhante à identificação por impressão digital na perícia forense criminal, marcas d’água e metadados podem ser adulterados ou removidos, mas ainda assim são úteis.

Os pesquisadores também estão trabalhando no desenvolvimento de detectores de conteúdo gerado por IA (‡1203, ‡1204, ‡1205*) para ajudar a identificar conteúdo gerado por IA no mundo real, mesmo quando não há marca d'água ou metadados disponíveis. No entanto, essas técnicas de identificação têm uma taxa de sucesso limitada.

###@ Atualizações

Desde a publicação do último Relatório (Janeiro 2025), houve progresso no desenvolvimento de sistemas de IA com múltiplas camadas eficazes de salvaguardas. Conforme discutido em §3.2. Práticas de gestão de riscos, defence-in-depth é um princípio central na gestão de riscos (‡1314). Por exemplo, sistemas de IA que combinam modelos treinados para segurança com filtros de entrada, filtros de saída e outros monitores de conteúdo estão sendo cada vez mais estudados e implantados (‡32, ‡65, ‡1182*). Pesquisas recentes também mostraram que, embora os desenvolvedores de modelos tenham feito progresso ao aumentar a robustez contra tentativas de contornar salvaguardas, os atacantes ainda obtêm sucesso em alta taxa (Figura 3.9).

###@ Lacunas de evidência

São necessárias mais evidências para ajudar os pesquisadores a compreender e considerar as limitações das abordagens existentes. As proteções técnicas para sistemas de IA estão sendo aprimoradas, mas as técnicas sofrem com limitações. Por exemplo, o progresso em melhorar a robustez no pior caso de sistemas de IA de propósito geral tem sido lento, e há limitações fundamentais quanto à forma como modelos de pesos abertos podem ser protegidos e monitorados de modo suficientemente abrangente (‡1195, ‡1315, ‡1316) (ver também §3.4. Modelos de pesos abertos). Enquanto isso, nem todas as proteções técnicas são igualmente comuns, igualmente eficazes ou igualmente comprovadas no mundo real. Por exemplo, o treinamento adversarial é usado quase de forma onipresente em modelos de ponta (‡64*, ‡677), enquanto técnicas de interpretabilidade do modelo e verificação formal têm sido pouco utilizadas até o momento em sistemas de produção (‡1177, ‡1285).

###@ Desafios para formuladores de políticas

Os principais desafios para os formuladores de políticas incluem decidir se e como devem apoiar a pesquisa, o desenvolvimento, a avaliação e a adoção de salvaguardas técnicas e métodos de monitoramento. Isso é desafiador porque a compreensão dos cientistas sobre como salvaguardar mecanismos de forma prática é ainda uma área em evolução e as melhores práticas ainda não foram estabelecidas. Por exemplo, diferentes desenvolvedores aplicam diferentes salvaguardas, e suas abordagens para mitigação de risco técnico de forma mais ampla variam consideravelmente (‡1116). Por fim, a existência de salvaguardas técnicas eficazes não garante, por si só, a segurança, já que a adoção e a implementação podem variar entre desenvolvedores e contextos de implantação.

