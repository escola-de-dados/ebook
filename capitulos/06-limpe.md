# Limpe

Você já checou como os dados foram coletados e divulgados e não encontrou nenhum problema. Também já entrou em contato com os responsáveis pelo levantamento e os números parecem responder aos mais rigorosos critérios de qualidade. Além disso, você verificou se os arquivos tinham alguns erros comuns e tudo parece estar conforme o esperado. Agora é só sucesso, certo? Nem sempre.

O maior risco de erro vem de onde menos prestamos atenção: nós mesmos. Nossos próprios vieses e eventuais falhas nas premissas que adotamos na hora de analisar um banco de dados são um estoque inesgotável de cascas de banana.

Philip Meyer, criador do jornalismo de dados, propõe uma reflexão que ajuda a entender esse problema.

Em seu livro de 1973, _Precision Journalism_, ele discute a maneira como repórteres encaram a missão de reportar fatos com objetividade. De acordo com Meyer, jornalistas gostam de se entender como pessoas de mente aberta, capazes de embarcar em investigações como &quot;tábulas rasas&quot;, sem qualquer prejulgamento.

O autor aponta, porém, que isso é impossível. Na prática, não dá para começar a pensar sobre qualquer problema sem partir de um enquadramento teórico ou de uma hipótese. Nós começamos a investigar um assunto porque achamos que pode existir algo de interesse ali, afinal.

Paul Bradshaw, professor da Birmingham City University, publicou recentemente [um artigo](https://onlinejournalismblog.com/2020/03/24/a-journalists-guide-to-cognitive-bias-and-how-to-avoid-it/) relacionado ao tema. O texto explora como diversos vieses cognitivos afetam o trabalho jornalístico. Sem jargão, isso significa o seguinte: existem vários mecanismos programados na mente humana que fazem com que nossa avaliação da realidade não seja tão isenta e objetiva como gostaríamos que fosse.

Um dos vieses listados é tão importante que mereceu um [texto só para ele](https://onlinejournalismblog.com/2020/04/07/how-to-prevent-confirmation-bias-affecting-your-journalism/): o viés de confirmação. Em resumo, humanos tendem a prestar mais atenção em informações que reafirmam suas próprias opiniões sobre um tema, enquanto ignoram informações que possam colocar essas perspectivas em xeque. O viés de confirmação também é frequentemente acionado nas crenças de fatos duvidosos, como ocorre no circuito da desinformação.

Essa questão não surge exclusivamente no jornalismo de dados, mas também pode ser observada nas reportagens que não se utilizam de quantificações. Muitas vezes, na ânsia de ver uma investigação se confirmar, repórteres direcionam a atenção apenas para os elementos que corroboram o resultado que querem alcançar e ignoram evidências contrárias.Isso acontece porque o repórter tem estímulos positivos para confirmar as próprias suposições, desde a satisfação de ver seu faro estar certo até a pressão que envolve apurar, escrever e entregar uma matéria relevante dentro de um prazo apertado.

Assim como acontece com as pessoas do outro lado do balcão, que produzem dados para nosso consumo, jornalistas de dados também podem falhar: erros de digitação, fórmulas malaplicadas, a mão que escorrega na hora de aplicar uma função na planilha… Tudo isso pode acontecer e passar despercebido.

Entretanto, o próprio Philip Meyer propõe uma saída para o problema que levantou - e ela funciona também para minimizar tanto os efeitos dos vieses cognitivos quanto dos deslizes mundanos.Para ele, o _jornalismo de precisão_ deveria adotar, na medida do possível, os ideais, os métodos e o conceito de objetividade dos cientistas.

A seguir, um exemplo de uma tabela fora do formato tidy data.


O que isso significa, porém?

De saída, significa formalizar, enunciar e tomar consciência das hipóteses, teorias e premissas que assumimos na hora de apurar uma matéria - ou, no nosso caso, de fazer uma análise de dados. Só assim é possível fazer uma análise mais criteriosa dos pressupostos que envolvem nossa forma de pensar e as conclusões que derivam dela.

Além disso, é importante adotar o **maior rigor metodológico possível.** Antes de mergulhar nos números, vale listar quais são os elementos que você procura, que evidências seriam necessárias para comprovar a hipótese que você investiga e, em contraste, o que seria necessário para admitir que não há nada ali. A ciência estatística pode ser aliada nesse processo, como veremos adiante.

Na tabela acima, o fenômeno capturado são notas de alunos. Mas repare que a variável &quot;disciplina&quot; ocupa diferentes colunas. No formato tidy data, essa planilha deveria ter uma coluna chamada &quot;disciplina&quot;, onde as matérias estivessem declaradas nas células abaixo dessa coluna.

Por fim, Meyer também destaca a importância de assumir uma postura de **transparência radical** , semelhante àquela que os bons cientistas adotam ao divulgar seus estudos de forma que possam ser meticulosamente avaliados e até reproduzidos pelos pares.

Explico melhor: cientistas estão acostumados a registrar todos os seus passos de forma detalhada. Junto com a conclusão de seus experimentos, publicam também uma descrição detalhada do método utilizado, os dados relacionados e um passo a passo de como os resultados foram obtidos.

Assim, um trabalho científico é também uma espécie de &quot;mapa&quot; que serve para que colegas (na revisão entre pares, por exemplo) e o público em geral possam verificar se tudo está como deveria estar ou se há alguma falha no estudo.

O jornalismo investigativo &quot;tradicional&quot; faz isso em certa medida, quando reúne documentos e registros concretos que podem ser verificados: atas de reunião, contratos, editais… Uma reportagem de impacto geralmente cita e mostra elementos como esses, o que ajuda a conferir credibilidade ao relato.

A coisa fica mais complicada, entretanto, quando o trabalho envolve informações confidenciais, fontes anônimas ou eventos que o repórter testemunhou em primeira pessoa. Algumas reportagens, pela própria natureza, não podem vir acompanhadas da demonstração de evidências.

O jornalismo de dados, por sua vez, apresenta condições de oferecer **transparência** ao leitor. Como o trabalho costuma ser mais metódico e controlado, é possível documentar cada passo de uma apuração ou análise.

Quando o repórter sabe programar, ele pode divulgar o **código-fonte** de uma matéria, ou seja, as linhas de instruções que foram executados pelo computador para chegar ao resultado. Assim, pessoas que também entendem de código podem revisar o processo de elaboração do material em busca de erros. Este processo já é adotado na redação de grandes jornais no Brasil e no mundo, como o Estadão ou New York Times.

Mesmo quando o trabalho não envolve programação, é possível fazer algo semelhante através do registro sistemático de todas as ações que foram tomadas no processo de produção.

Vale a pena anotar tudo o que você fizer, desde a origem dos arquivos que baixou até o passo a passo da limpeza de dados e das fórmulas e filtros que aplicou. Além de servir para organizar melhor o próprio fluxo de trabalho, esse tipo de material pode ser divulgado junto com a matéria.

Ao permitir que terceiros avaliem se seu métodos são sólidos, você também minimiza a chance de que um erro passe despercebido por todos. Mais do que isso, você demonstra que está trabalhando de boa fé e constrói uma relação de confiança com os leitores. O princípio é parecido com o processo de _revisão por pares_ no método científico: quanto mais gente prestar atenção e discutir os méritos e falhas do jornalismo, mais a qualidade dos conteúdos tende a crescer.

**Dicas para começar uma análise**
- **Desenvolva um método:** em vez de mergulhar na base de dados de forma livre, olhando para todos os lados em busca de algo que possa ser interessante, é importante elaborar um plano de ação. Assim, nos obrigamos a tomar consciência das hipóteses e premissas que envolvem o trabalho. O que exatamente você espera encontrar? De que maneira vai sistematizar essa busca? Que evidências seriam suficientes para corroborar suas hipóteses?

- **Reporte contra suas convicções:** quando começamos uma análise de dados, é natural que o esforço de investigação enfatize elementos que corroborem a história que queremos contar. Entretanto, precisamos pensar também naquilo que pode derrubar a matéria. Que evidências fariam você desistir da reportagem? Procure por elas também.

- **Seja transparente:** desenvolver um método claro de trabalho não é útil apenas para guiar nossos próprios esforços de apuração. Quando a metodologia é publicada junto com uma reportagem, você ajuda o público a entender quais foram os passos da investigação, o que aumenta a credibilidade do material e permite que interessados verifiquem se os resultados são mesmo sólidos. 

## Vieses e limitações

Agora, já sabemos que dados podem trazer erros e vieses e que esses problemas podem ter várias causas, desde falhas metodológicos até pequenos deslizes humanos.

Falta entender, entretanto, como esses dados ruins podem afetar a sociedade de forma negativa - e o que podemos fazer diante disso.

Em 2016, o veículo americano [ProPublica](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing) como um programa de inteligência artificial usado pelo sistema de justiça americano discriminava pessoas negras.

Essa inteligência artificial supostamente era capaz de dizer qual era a chance de um prisioneiro reincidir no crime caso fosse solto e, assim, ajudar juízes a tomarem decisões melhores. O programa avalia dados sobre o réu e emite uma nota, em uma escala de 1 a 10, para mensurar o risco. O juiz, depois de consultar o valor, decide o que fazer: concede liberdade condicional ou mantém o sujeito na prisão?

A promessa de um sistema como esse é reduzir a influência do preconceito inerente aos humanos no processo de decisão. Entretanto, a reportagem mostrou que isso não aconteceu.

De acordo com a análise, o programa sistematicamente classifica americanos negros como mais propensos a reincidir do que americanos brancos, ainda que tenham cometidos crimes menos violentos.

Por que isso acontece? Porque uma inteligência artificial precisa de dados para operar. Um sistema como esse funciona ao analisar quantidades enormes de números, buscando padrões neles. É com base em registros e métodos elaborados por humanos que o computador cospe seu veredito.

Agora o problema fica mais aparente: de acordo com um dos procurados citados na matéria, a sociedade americana, e o sistema prisional em especial, tem um histórico grave de racismo.

O programa não era alimentado com dados sobre a raça dos réus, mas se debruçava sobre dados sócio-econômicos e comportamentais, como renda e desemprego. Esses problemas não afetam pessoas de diferentes raças igualmente: negros sofrem mais com eles. Assim, a máquina passou a enxergar uma relação indireta - e inexistente, como a reportagem demonstra - entre raça e risco de reincidência.

Quando um sistema analisa automaticamente números produzidos por uma sociedade que discrimina, o resultado da análise vai trazer consigo o mesmo tipo de discriminação. Os dados são, em sua origem, essencialmente humanos.

A reportagem da ProPublica, além de revelar essa dinâmica que perpetua desigualdades, mostra como o jornalismo de dados pode agir diante de um contexto como esse.

O trabalho usou técnicas do jornalismo de dados não apenas para encontrar tendências em uma base, mas para entender melhor os efeitos que ela tem sobre o mundo. Aqui, o dado não é encarado como espelho da realidade, mas como uma construção que tanto reflete quanto afeta a sociedade.

Além disso, as melhores práticas foram seguidas e o resultado foi publicado junto com uma [descrição detalhada da metodologia](https://www.propublica.org/article/how-we-analyzed-the-compas-recidivism-algorithm). A matéria serve para ilustrar como é possível tratar os dados não apenas como uma fonte de informação, mas como um tema que merece ser investigado por si só.

Outro exemplo dessa postura vem do trabalho da Folha de São Paulo na cobertura da epidemia de Covid-19: a equipe do núcleo de dados do jornal (Delta Folha), ao analisar dados sobre mortalidade publicado pelos cartórios do Brasil, percebeu uma série de erros que impediam fazer uma análise sólida.

Em vez de simplesmente desistir da reportagem e começar outra matéria, o jornal [publicou um texto](https://www1.folha.uol.com.br/equilibrioesaude/2020/05/base-de-dados-de-cartorios-traz-falhas-que-impedem-calcular-efeito-real-do-coronavirus-no-brasil.shtml) em que expôs os diversos problemas daquelas estatísticas, que vinham sendo usadas cada vez mais por outros participantes do debate público.

O The New York Times também tem se destacado nesse aspecto, com [uma cobertura](https://www.nytimes.com/series/new-york-times-privacy-project) dedicada aos efeitos que a coleta em massa de dados pode ter para a privacidade dos cidadãos e suas consequências para a democracia.

Essa atitude inquisitiva é especialmente importante porque, cada vez mais, dados e programas de computador têm efeitos na vida das pessoas. O tema tem se tornado mais caro ao jornalismo, tanto que alguns repórteres já se propõem a fazer a **cobertura de algoritmos**. Em vez de se especializar em reportar sobre política, cultura ou saúde, eles se dedicam a entender melhor e discutir de forma crítica como esses mecanismos atuam. O tema não cabe no escopo do livro, mas vale registrar que técnicas do jornalismo de dados podem ser úteis para quem quer se aventurar por esse campo.

Agora que já dedicamos uma boa atenção às preocupações que precisamos ter durante a análise de uma base dados, vamos começar a parte mais prática deste capítulo. Como, afinal, fazemos para descobrir quais são as histórias que se escondem em uma série de números? Quais são as técnicas e saberes que eu preciso mobilizar para produzir uma boa reportagem guiada por dados?

A primeira recomendação é não esquecer daquilo que importa para todos os repórteres do universo: seu trabalho é encontrar e comunicar o que há de mais novo, relevante e interessante no mundo. O que muda é que um bom jornalista de dados precisa desenvolver habilidades para encontrar informações em um novo ambiente social.

Uma das melhores explicações sobre o que isso significa veio de Tim Berners Lee, pesquisador e criador da internet moderna (World Wide Web).

<<<<<<< HEAD
Em uma [entrevista](https://www.theguardian.com/technology/organgrinder/2010/nov/19/berners-lee-journalism-data) de 2010 para o jornal britânico The Guardian, Lee resumiu a questão: segundo ele, jornalistas estão acostumados a encontrar histórias conversando com pessoas, e vão continuar fazendo isso. Entretanto, em mundo cada vez mais digitalizado, eles também vão encontrar histórias em bancos de dados, e portanto precisam estar equipados para analisá-los.

Esse pensamento se materializa quando percebemos que, hoje, praticamente todas as ações humanas acabam se tornado um registro numérico, no final das contas. Quando um parlamentar compra uma refeição, o registro vai parar em uma planilha em algum canto do site da Câmara. Quando o Presidente da República publica um tweet, um banco de dados é atualizado. Quando alguém faz uma busca no Google, um algoritmo é posto para funcionar.

E qual é o equipamento que um jornalista de dados precisa ter em mãos para compreender e usar esses dados, afinal? O mais essencial é desenvolver uma maneira quantitativa de pensar. Em vez de enxergar anedotas e histórias individuais, um repórter treinado para trabalhar com informação quantitativa busca ver padrões, tendências, repetições.

Para deixar mais claro como essa mentalidade funciona, vamos pensar em um acontecimento frequente: um roubo de celular que aconteceu em uma rua movimentada de uma grande capital.

Um único roubo, por si só, provavelmente não seria noticiado por um jornal da cidade. É corriqueiro demais, comum demais. Entretanto, o bom repórter de dados não para em um roubo só. Ele percebe que esse fato singular está inserido dentro de vários outros. Quantos celulares são roubados por dia em São Paulo, por exemplo?

Além disso, ele percebe que o roubo é um fenômeno quantificável: a ação aconteceu em determinado dia da semana e em determinado horário, em um local que pode ser representado como coordenadas geográficas. A vítima tem uma idade, uma raça, uma profissão. O ladrão também. Tudo isso cabe muito bem em uma planilha, não acha?

Quando jornalistas e editores percebem essa possibilidade, a história sobre roubo de celular fica interessante. Vira até [capa de jornal](https://sao-paulo.estadao.com.br/noticias/geral,roubos-de-celular-atingem-metade-das-ruas-de-sao-paulo,70002022457): o exemplo é real, e resultou em uma matéria que foi publicada pelo Estadão em setembro de 2017. A planilha com todas essas informações sobre os roubos existe, de fato: é o registro dos boletins de ocorrência publicado pela Secretaria de Segurança Pública de São Paulo.

A matéria ecoa o[texto clássico sobre jornalismo de dados](http://www.holovaty.com/writing/fundamental-change/), publicado em 2006 por Adrian Holovaty e sobre o qual falamos na introdução deste livro. Depois que você aprende a enxergar números em todos os lugares, precisa aprender também a entender o que eles revelam. E é aí que entra no jogo algo que parece assustador: a matemática.

Dificilmente um jornalista entrou na profissão porque gosta de fazer contas. Na verdade, o que acontece com frequência é o contrário: muita gente escolhe virar repórter porque quer evitar os números, geralmente depois de passar anos sofrendo para superar provas de matemática.

O resultado dessa aversão generalizada à matemática é perceptível no ambiente de trabalho, visto que algumas pessoas entram em desespero ao precisar fazer uma simples conta de regra de três.

O fenômeno da ansiedade causada pela matemáticajá foi descrito em [pesquisas acadêmicas](https://journals.sagepub.com/doi/full/10.1177/1326365X18780418) e a conclusão assusta: muitos estudantes deixam de cursar disciplinas de jornalismo de dados porque acham que não gostam ou não sabem o suficiente de matemática.

Esse medo, entretanto, não faz muito sentido: quase tudo que um jornalista de dados faz envolve matemática básica. Além disso, ao contrário da escola, podemos usar calculadoras ou, como é mais frequente, programas como o Google Sheets e o Microsoft Excel.

Antes de aprender como mexer com essas ferramentas, porém, precisamos relembram algumas tarefas simples dos tempos de escola, como taxas, porcentagem, estatística básica e afins.

## Operações matemáticas básicas

Nesta seção, aprenderemos um pouco sobre como calcular porcentagem e taxas, além de ter algumas dicas relacionadas à correção de valores pela inflação e análise de séries temporais. Para uma descrição mais detalhada das operações matemáticas básicas importantes para o trabalho com dados vale conferir o livro de Sarah Cohen, Numbers In The Newsroom. Trata-se de um manual clássico escrito por uma ex-editora de jornalismo de dados do New York Times, que apresenta os conceitos da matemática que mais são usados nas redações de forma didática.

**Porcentagem**

Calcular a porcentagem é, provavelmente, a tarefa mais comum de um jornalista em redação. Manchetes como &quot;65% dos entrevistados se preocupam com o desemprego&quot; são extremamente comuns e não costumamos pensar muito no que elas significam. É óbvio, certo?

Pode até ser, mas vale a pena esmiuçar o conceito. Quando alguém menciona 65% dos entrevistados, na prática está dizendo que 65 de cada 100 deles demonstrou preocupação com o desemprego.

Entretanto, a descrição metodológica dessa pesquisa diz que foram entrevistados, na verdade, 6.734 brasileiros e não 100. Desses, 4.377 disseram que estavam preocupados, em vez de 65. Nesse contexto, por que estamos falando de &quot;65 de cada 100&quot; em vez de &quot;4.377 de cada 6.734&quot;?

A explicação é simples: é mais fácil entender o que significa &quot;65 de 100&quot; do que &quot;4.377 de 6.734&quot;. No primeiro caso, fica bem mais fácil entender que estamos falando de mais da metade do total. Ao falar em &quot;65%&quot;, a proporção dos preocupados fica mais clara.

É para isso que serve a porcentagem: o cálculo parte de um valor arbitrário e difícil de compreender e o transforma em algo mais palatável. O passo a passo é:

Figuras2, 3 e 4 - Como calcular percentuais

![](RackMultipart20200807-4-10x14ou_html_f944026a85b552ee.png) ![](RackMultipart20200807-4-10x14ou_html_14d33b825617923.png)

![](RackMultipart20200807-4-10x14ou_html_d3b35e2e7e54ee2a.png)

Agora que já entendemos o que é uma porcentagem, podemos dar um passo adiante e falar de variação percentual, outro tema que é comum em jornais. Veja este exemplo real de título: &quot;[Com Bolsonaro, liberação de agrotóxicos cresceu 42%, diz estudo](https://noticias.uol.com.br/meio-ambiente/ultimas-noticias/redacao/2019/05/17/com-bolsonaro-liberacao-de-agrotoxicos-cresceu-42-diz-estudo.htm)&quot;.

Vamos aos números: de acordo com a reportagem, até abril de 2019, o governo de Jair Bolsonaro havia aprovado o uso de 166 novos agrotóxicos. No mesmo período de 2018, sob outro presidente, haviam sido 117. Como fazemos para chegar nessa variação de 42%, então?

Primeiro, precisamos calcular a **diferença** entre a aprovação de agrotóxicos em 2019 e 2018. Depois, queremos saber quanto essa diferença representa do **valor original**. Na prática, é muito parecido com o cálculo simples de porcentagem, mas com um passo a mais.

Veja:

Figuras 5, 6, 7, 8 - Cálculo de diferença percentual

![](RackMultipart20200807-4-10x14ou_html_d388f07b626e2db3.png) ![](RackMultipart20200807-4-10x14ou_html_1e78d85f96c10d4.png) ![](RackMultipart20200807-4-10x14ou_html_ebd99b4ea5f8d5b4.png) ![](RackMultipart20200807-4-10x14ou_html_c6db6cc10b096922.png)

O que todas essas contas fazem, em sua essência, é descobrir **o quanto a mudança nos números brutos** representa do valor inicial. Discernir isso é importante para não cair em um erro comum: confundir variação percentual e diferença em pontos percentuais.

Esse último é mais fácil de entender: ele não envolve as transformações de números em percentuais que acabamos de fazer, mas sim a comparação já entre duas porcentagens.

O exemplo desta vez é a pesquisa Datafolha de 28 de maio de 2020, que mostrou que a reprovação do presidente Jair Bolsonaro cresceu de 38% para 43% desde o mês anterior.

Alguém desavisado poderia dizer que a variação foi de 5%, já que 43 menos 38 é igual a cinco. Entretanto, calcular a variação em porcentagem envolve os passos que acabamos de mostrar. Quando a conta é simples assim, comparando a diferença entre duas porcentagens com uma simples subtração, o correto é dizer que a queda foi de **cinco**** pontos percentuais**.

Calcular a **variação percentual** , por outro lado, envolveria pegar essa diferença de 5 pontos percentuais e dividir pelos 38 originais. O resultado seria uma queda de aproximadamente 13%.

**Taxas**

Ao entender como funciona o cálculo de uma porcentagem, você automaticamente aprende também a usar outra ferramenta importante no cinto de utilidades de um jornalista de dados: o cálculo de **taxas**.

Como vimos, uma porcentagem consiste em transformar um número absoluto, muitas vezes difícil de colocar em perspectiva, em algo mais palatável. Assim, é mais fácil entender o que aquele valor representa.

Calcular uma porcentagem nada mais é que calcular uma taxa. Lembre-se do passo final da operação, quando o resultado da divisão da parte pelo todo é multiplicado por 100. A multiplicação, na prática, está colocando o resultado em uma **base** diferente.

Isso significa que, em vez de pensarmos em um número arbitrário, podemos usar uma quantidade que é mais fácil de compreender, mas representa a mesma proporção de casos.

A novidade é que essa base **não precisa ser 100** , necessariamente. Um caso frequente é a taxa de homicídios, que geralmente é calculada na base de **100 mil**.

Além de tornar mais fácil entender o que um número representa de fato, o cálculo da taxa serve, principalmente, para comparar fenômenos que acontecem em populações de tamanho diferente.

Veremos como isso funciona na prática, ainda com os dados de assassinatos de 2016. Em Trinidad e Tobago, 420 pessoas foram vítimas de homicídio naquele ano. No Brasil, no mesmo ano, foram aproximadamente 61 mil. **Qual país é mais violento?**

A resposta simples é que mais gente é assassinada no Brasil do que no país caribenho. Entretanto, a população do Brasil é cerca de 200 vezes maior. É natural que a quantidade total de mortes seja maior aqui.

Como podemos responder a essa pergunta de forma justa? **Usando uma taxa que coloque esses números na mesma base.** Assim, conseguimos saber oquão comum são as ocorrências de assassinato dentro de uma população. Veja abaixo o passo a passo e repare como o processo se assemelha ao da porcentagem:

![](RackMultipart20200807-4-10x14ou_html_9766d28aed587bd.png) ![](RackMultipart20200807-4-10x14ou_html_7b72df773481bf49.png) ![](RackMultipart20200807-4-10x14ou_html_126d65ed4fa67410.png)

Os assassinatos, ainda que por pouco, são **menos comuns** no Brasil que em Trinidad e Tobago, mesmo que a contagem de mortes seja maior.

É uma boa prática calcular taxas sempre que formos comparar a realidade de universos de tamanhos diferentes. Entretanto, é bom nunca perder os números absolutos de vista, também.

De acordo com as circunstâncias, controlar os valores por população pode induzir leituras erradas. Precisamos prestar atenção especial na hora de comparar universos de escalas muito diferentes. Quando a população total é muito pequena, poucas ocorrências podem inflar uma taxa artificialmente.

Para entender melhor, vale olhar para os números de mortes por Covid-19 para cada milhão de habitantes em dois países. Na Islândia, essa taxa era de 27 ao final de maio de 2020. Na China, era de 3. A situação do país asiático parece muito melhor sob essa métrica, mas sabemos que a realidade é diferente.

Uma cidade chinesa foi o epicentro do primeiro surto da doença, com milhares de mortes que levaram a medidas compulsórias de isolamento social. No país nórdico, morreram apenas 10 pessoas.

As taxas de ambas as nações são puxadas para extremos opostos porque eles estão em extremos opostos: a China tem bilhões de habitantes, enquanto a Islândia tem menos de 500 mil.

Um único caso da doença teria grande impacto na taxa islandesa, enquanto mesmo uma quantidade de mortes capaz de colocar um sistema de saúde em colapso pouco alteraria a taxa chinesa.

**Inflação**

A análise de dados que envolve valores monetários deve, necessariamente, considerar a inflação do período. Antes de utilizar números de uma série histórica, por exemplo, é preciso verificar se os valores foram corrigidos. Depois de verificar esse detalhe na documentação do banco de dados que pretende utilizar, é hora de fazer a conversão. Para tanto, existem ferramentas gratuitas que automatizam esse processo, como a calculadora do [Banco Central](https://www3.bcb.gov.br/CALCIDADAO/publico/exibirFormCorrecaoValores.do?method=exibirFormCorrecaoValores) e do [IBGE](https://www.ibge.gov.br/explica/inflacao.php).

Tomemos como ponto de partida o poder de compra de um cidadão que, em janeiro de 2005, recebeu R$ 1 mil pelo seu trabalho. Em valores corrigidos pelo Índice Nacional de Preços ao Consumidor Amplo (IPCA), esses R$ 1 mil tornaram-se R$ 2,13 mil em janeiro de 2019. Em outras palavras, este cidadão não teria o mesmo poder de compra caso continuasse recebendo R$ 1 mil em 2019. Por isso, a inflação do período precisa ser observada. Como observa a jornalista Mariana Segala [neste trecho do livro Siga os Números](https://sigaosnumeros.com/sumario/descomplicando-os-dados/como-encontrar-pautas-nos-dados/as-tres-operacoes-fundamentais-da-matematica-para-jornalistas/), atualizar valores de acordo com a inflação ou com os juros do período é uma das habilidades demandadas especialmente dos jornalistas que cobrem economia e finanças. A ausência de correção de valores provocaria uma análise equivocada.

**Série históricas**

A análise temporal de um fenômeno exige dados de série histórica, isto é, informações correspondentes a um grande período de tempo. Podemos pensar, por exemplo, sobre dados de emprego e desemprego, distribuição de renda entre a população, produção agrícola e números de importação e exportação em determinado país.

Se você obtiver acesso apenas às informações referentes a um curto espaço de tempo (poucos meses ou poucos anos), é preciso redobrar os cuidados quanto aos resultados e afirmações contundentes e que remetem ao &quot;melhor&quot; ou &quot;pior&quot; desempenho de um setor. Também é importante observar se a coleta de dados foi feita pela mesma instituição ao longo dos anos e/ou se a metodologia de coleta e apresentação de dados passou por mudanças.

Outro ponto que exige atenção é a sazonalidade, muito importante na comparação entre períodos. Em períodos regulares do ano, por exemplo, o trânsito das cidades costuma ser bastante movimentado. Assim, não é possível comparar a circulação de veículos em períodos &quot;normais&quot; com os meses de janeiro e fevereiro. É natural que a circulação de veículos na cidade caia nos meses de férias escolares.

Produção agrícola e até mesmo criminalidade são outras áreas que bem exemplificam a necessidade de escolher períodos comparáveis entre eles, visto que há oscilação dos dados de acordo com os meses. Por isso, é fundamental que qualquer análise seja feita a partir do mesmo período correspondente no ano ou nos anos anteriores. Na dúvida, consulte um especialista.

Daqui a alguns anos, pense bem antes de comparar qualquer tempo com períodos de 2020: a Covid-19 marcou o ano e precisa ser vista como um fenômeno à parte, que deve ser levado em conta nas análises futuras sobre este ano.

## Estatística para leigos

Depois de entrar em alguns conceitos de matemática básica, precisamos discutir asprincipais noções de estatística. Na linguagem do dia a dia, costumamos chamar de estatística tudo aquilo que é número. Quando um repórter fala de &quot;trazer estatísticas&quot; para uma matéria, geralmente está falando de rechear o texto com exemplos, contagens, porcentagens e afins.

Estatística é, na verdade, uma ciência que se dedica a analisar e interpretar bancos de dados. Geralmente, o jornalista ou comunicador trabalha com um campo específico da área: **a estatística descritiva** , que se preocupa em resumir de forma significativa as características de um conjunto de informações.

O conceito pode parecer estranho quando descrito dessa forma, mas é algo que está muito presente em nossa cotidiano. Os valores de média, moda, e mediana, por exemplo, fazem parte desse campo, assim como os conceitos de desvio padrão, outliers e padrões de distribuição. Vamos entender para o que serve cada um deles.

**Moda, média e mediana**

Você provavelmente já calculou a **média** de alguma coisa, nem que seja a média das notas do seu boletim escolar. O procedimento é simples: somar todos os números de uma série e dividir pela quantidade total de elementos. Você já parou para pensar qual é o objetivo desse cálculo?

Na prática, o cálculo da média tenta encontrar um número que seja capaz de representar todas as entradas de uma série de dados de forma simplificada. Quando calculamos a média das notas de todas as provas que um aluno fez em um ano, esperamos que o resultado seja um número que resuma todas as avaliações em uma só.

Não é algo tão simples e justo quanto parece, como qualquer estudante que tenha ficado insatisfeito com sua nota final já percebeu. No entanto, existem casos em que usar a média é ainda mais complicado.

Veja, na tabela abaixo, a distribuição dos salários de uma empresa:

Quadro X - Salários em uma empresa

| **Empregado** | **Salários (em mil R$)** |
| --- | --- |
| Jéssica | 1.5 |
| Miguel | 2.5 |
| Bernardo | 2.5 |
| Juliana | 2.5 |
| Adriana | 2.5 |
| Carlos | 3.5 |
| Antônia | 3.5 |
| Gabriel | 3.5 |
| Letícia | 4.0 |
| Sandra | 4.5 |
| José | 5.0 |
| Bianca | 5.5 |
| João | 6.5 |
| Camila | 28.0 |
| Amanda | 150.0 |

Ao calcular a média salarial dos funcionários, chegamos a um número de 15 mil reais por mês. Entretanto, **não há uma única pessoa que receba esse valor**. Nesse caso, a média não oferece um bom resumo da realidade.

Isso acontece porque os salários de Camila e Amanda são muito maiores que os demais. Como o cálculo da média simples dá um mesmo peso para todos os elementos, o resultado acaba sendo muito sensível a extremos como esses.

Por sorte, existem outras medidas que podemos usar em situações com essa.

A **mediana** , por exemplo, usa uma tática diferente para encontrar um número representativo do banco de dados: ela divide a série em duas metades e pega o valor que está **exatamente no meio**.

No caso de uma série hipotética [1, 2, **3** , 4, 8], o valor seria o 3, já que há uma mesma quantidade de valores maiores e menores do que ele.

No caso dos salários que mostramos acima, a mediana é um dos salários de R$ 3,5 mil:[1.5, 2.5, 2.5, 2.5, 2.5, 3.5, 3.5, **3.5** , 4.0, 4.5, 5.0, 5.5, 6.5, 28.0, 150.0]. Note como há exatamente sete itens acima e sete itens abaixo do valor selecionado. O valor não é sensível a valores exagerados e oferece um dado mais real.

A **moda** , outra métrica de centralidade, usa uma estratégia mais simples: selecionar, simplesmente, o número que mais se repete. No exemplo acima, é o salário de R$ 2,5 mil, que ocorre com quatro dos 15 funcionários.

Para escolher qual é a melhor métrica para o banco de dados que você tem em mãos, é preciso entender um pouco mais sobre outro conceito de estatística: **a distribuição**.

**Distribuição: dispersão, desvio padrão e outliers**

Ainda seguindo com o exemplo dos salários, vamos prestar mais atenção na característica dos dados que tornou o cálculo da média pouco representativo: havia elementos extremos na série, ou seja, salários muito distantes dos demais e que distorciam o cálculo.

Esse tipo de característica pode ser medida usando estatísticas descritivas de **dispersão**. Para entender melhor quais são as informações de um banco de dados - se ele tem muitos extremos ou é mais uniforme, por exemplo - é muito útil usar um tipo de gráfico chamado histograma. Em resumo, esse gráfico permite observar a distribuição dos dados e identificar pontos fora da curva.

[histograma]

Agora, vamos falar de medidas que, assim como as estatísticas de centralidade que vimos anteriormente, tentam resumir as características de um banco de dados em um número único.

Já vimos como esse tipo de abordagem pode ser perigoso mas, ainda assim, servem para ter uma ideia rápida do tipo de dados com os quais estamos lidando.

O **desvio padrão** , por exemplo, é útil para saber se estamos diante de um banco de dados com muitos valores extremos. Esse número é, na prática, **uma média da distância de cada ponto da média de todos os bancos de dados.**

Confuso? Nem tanto. Vamos voltar aos dados de salários com que trabalhamos, cuja média é R$ 15 mil.

Para calcular o desvio padrão, precisamos calcular a diferença do salário de cada funcionário da média salarial: Jéssica, por exemplo, ganha R$ 1,5 mil, ou seja, está R$ 14,5 mil reais distante da média. Amanda ganha R$ 150 mil, então está R$ 135 mil reais distante da média.

Ao somar todas essas diferenças e dividir pelo total de funcionários, temos o desvio padrão, que tenta resumir o quão uniforme é um banco de dados. Um desvio padrão maior indica dados mais díspares, com a presença de um ou mais extremos.

Nesse caso, o valor é de R$ 37,9 mil. Para saber se ele é significativo, vale comparar com as outras estatísticas que vimos: trata-se de mais do que o dobro da média e é mais de dez vezes maior do que a moda e a mediana.

Também é possível usar o desvio padrão para descobrir o quão extremo é um ponto de dados. Para isso, é preciso dividir o valor pelo desvio padrão.

Por exemplo, vamos analisar novamente o salário de Amanda: R$ 150 mil, divididos pelo desvio padrão de R$ 37,9 mil, resultam em aproximadamente 4 desvios padrão acima da média.

Usualmente, dados que estejam a três desvios padrão ou mais da média, em um banco de dados que segue uma distribuição normal podem ser considerados extremos - ou seja, sãooutliers.

Ainda que um outlierpossa ser de interesse jornalístico, esse tipo de dado pode prejudicar a análise dos demais. Sempre verifique se esse não é o caso antes de interpretar estatísticas descritivas simples.

**Correlação**

Outra técnica estatística útil para o jornalismo é o cálculo da taxa de correlação. Essa medida, que é bastante complexa e quase sempre é calculada com o uso de programas de planilha ou tecnologias equivalentes, estima como o comportamento de duas variáveis está interligado.

Vamos, de novo, deixar o jargão de lado e tentar entender o conceito com um exemplo mais próximo da realidade: temos um banco de dados que mostra a nota que cada estudante tirou no ENEM e a renda média de sua família.

Com um cálculo de correlação, podemos verificar que, quanto maior é a renda da família, melhor a nota tende a ser. Trata-se de uma correlação positiva: quando um dos valores cresce, o outro provavelmente vai crescer também.

Existem as correlações negativas, em que ocorre algo oposto: quando uma das variáveis aumenta, a outra diminui. Um exemplo possível é a relação entre renda média e taxa de analfabetismo. Quanto maior for a renda média entre os moradores de uma cidade, por exemplo, menor tende a ser a prevalência de analfabetismo entre a população.

E o quão forte são essas ligações, afinal? Para mensurar exatamente o quanto duas variáveis estão conectadas, é possível calcular um valor chamado **coeficiente de correlação.**

Existem vários tipos, mas o de uso mais frequente no jornalismo é coeficiente de correlação de Pearson. Ela mede justamente o tipo de relação aqui apresentado e classifica a intensidade do fenômeno de -1 até 1.

Uma correlação de 1 é perfeitamente positiva, em que cada unidade a mais em uma variável gera uma unidade a mais na outra. Uma correlação de -1 é perfeitamente negativa, e uma unidade a mais em uma variável gera uma unidade a menos na outra. Quando o valor é 0, não há correlação alguma e as variáveis não se influenciam.

Entretanto, na prática, é raríssimo encontrar correlações perfeitas ou a total ausência de correlação. O coeficiente se apresenta, na vida real, em frações: 0,8 indica uma correlação forte, por exemplo, enquanto 0,2 indica uma correlação fraca.

Esse tipo de cálculo é útil para fortalecer estatisticamente matérias que mostram como dois fatores estão relacionados. É possível calcular a correlação entre pobreza e acesso à educação ou pobreza e violência, por exemplo.

Contudo, mesmo diante de um coeficiente de correlação alto, é preciso tomar alguns cuidados.

Vamos voltar para o exemplo de notas no Enem. Agora, em vez de comparar a nota de cada estudante com a renda de sua família, você resolveu medir o efeito da arborização na performance escolar. E existe uma correlação clara entre conseguir notas melhores e viver em um bairro cheio de árvores.

Hora de escrever uma matéria espetacular sobre isso, certo? Errado. É hora de pensar um pouquinho mais a fundo.

É muito provável que a variável de renda influencie tanto a quantidade de árvores no bairro de cada estudante como a sua nota na prova. Gente com mais dinheiro mora em locais com melhor estrutura urbana e também tende a ter resultados melhores no Enem.

Não é o excesso de árvores que influencia o desempenho na prova. É a renda que influencia tanto a arborização quanto a nota no exame. Quando não nos atentamos para essa relação escondida, na verdade, estamos medindo uma terceira variável sem nos darmos conta.

Além disso, é possível encontrar dados que se correlacionam de forma perfeita, mas que não tem nenhuma conexão entre si. Existe [até um livro](https://www.amazon.com/gp/product/0316339431/ref=as_li_tl?ie=UTF8&amp;camp=211189&amp;creative=373489&amp;creativeASIN=0316339431&amp;link_code=as3&amp;tag=tylervicom-20&amp;linkId=UO6I3ENRRQUF255J) apenas sobre isso. Entre os exemplos, está até uma correlação de 0.95 (portanto, super forte) entre o consumo de queijo muçarela e a quantidade de pessoas formadas em um curso superior de Engenharia Civil.

É por motivos como esses que existe um mantra entre quem trabalha com análise de dados: **correlação não é causalidade.** Só porque dois fenômenos ocorrem de forma paralela, não podemos afirmar que um **causa** o outro, mesmo que o coeficiente de correlação seja absurdamente alto.

Para afirmar que um fenômeno casou outro, é preciso fazer testes estatísticos mais específicos e poderosos, que não conseguiremos cobrir nesse livro.

Na dúvida, é melhor não avançar o sinal: você não quer ser o cara que disse que viver perto de árvores faz alunos irem melhor na prova, não é mesmo?

**Margem de erro**

Imagine que você queira compreender os hábitos de consumo dos brasileiros ou mesmo quais são suas preferências de voto em uma eleição iminente. É improvável que alguém tenha tempo ou recursos suficientes para ouvir cada um dos 210 milhões de brasileiros. Por isso, trabalha-se com a ideia de amostra, ou seja, um conjunto de pessoas cujas características sociais e demográficas sejam capazes de representar a população como um todo. Dessa forma, as respostas obtidas em uma amostra uma pesquisa podem ser atribuídos a um universo (neste caso, a população inteira).

Ao trabalhar com dados amostrais, portanto, fique atento à margem de erro, que corresponde a quantos percentuais (para mais ou para menos) as informações podem variar. Se 90% dos respondentes de uma pesquisa concordaram com uma afirmação, por exemplo, e a margem de erro for de cinco pontos percentuais, estima-se, então, que entre 85% e 95% pessoas responderam afirmativamente a esta questão.

Pesquisas com margens de erro muito altas (a partir de 10 pontos percentuais) dificilmente trazem dados que representam de forma qualificada uma determinada realidade, e por vezes indicam problemas na metodologia. A margem de erro em pontos percentuais é uma característica importante a ser levada em conta, e deve, inclusive, ser comunicada claramente na reportagem. Em geral, as pesquisas amostrais também divulgam o intervalo de confiança, normalmente de 95%. Isso significa que, se a pesquisa for repetida com amostras aleatórias 100 vezes, em 95 delas o resultado será mesmo.

## Operações de análise de dados

Existem algumas operações básicas que podem ajudar a encontrar padrões e tendências nos dados. De acordo com o software que você usa para trabalhar, os procedimentos podem ter algumas diferenças, mas o raciocínio segue o mesmo.

De início, tente **ordenar os dados** do maior para o menor ou do menor para o maior. Se você está mexendo com dados de gastos governamentais, faz sentido ver qual foi a maior compra de todos, por exemplo.

**Filtrar** a planilha é interessante para ver se o padrão de comportamento dos dados é o mesmo quando olhamos apenas para um segmento deles. Ainda usando a mesma metáfora, pode ser que o gasto médio de um ministério específico seja muito diferente do gasto médio do governo como um todo.

Da mesma forma, **agregar** os dadospode revelar padrões que não seriam vistos de outra forma: em vez de olhar apenas para cada uma das compras governamentais, individualmente, é possível reuni-las em categorias. Quantas foram feitas por cada departamento? Quanto gastou cada ministério? Você conseguirá fazer esta operação usando operadores de linguagens de programação, como o GROUP BY, ou através das tabelas dinâmicas nos editores de planilha.

Com as tabelas dinâmicas, você conseguirá de fato utilizar os editores de planilha para entrevistar seus dados. Imagine que você tenha uma tabela onde cada linha representa repasses de financiamento de campanha e você gostaria de responder a seguinte pergunta: quais doadores financiaram a maior soma de recursos?

Existem várias operações de análise dos dados que são necessárias para respondê-la: primeiro, você precisa agrupar os doadores de acordo com uma coluna. Ao realizar agrupamentos, sempre dê preferência a usar campos identificadores como CPF ou CNPJ ao invés de campos de texto, como o nome, que são mais suscetíveis a erros de digitação.

Ao agrupá-los, será necessário então fazer uma soma na coluna com os valores financiados para, então, ordenar os resultados de forma decrescente e, assim, descobrir os 10 principais financiadores.

Na tabela dinâmica, você conseguirá realizar todas estas operações. Basicamente, a ideia por trás deste recurso é que você deve criar uma nova tabela, que irá &quot;moldar&quot; os dados da planilha original para que eles assumam a forma que você deseja.

Em geral, as linhas dessa nova tabela representam uma entidade, como um doador, nesse exemplo. Nas colunas, geralmente, aparecemos valores agregados por categoria. No exemplo, revelariam a soma total de doações feitas por cada pessoa **.**

Assim, independente do software utilizado, o importante ao entrevistar dados com tabelas dinâmicas é saber identificar qual é a forma que essa nova tabela precisa assumir.

Imagens 24 e 25

![](RackMultipart20200807-4-10x14ou_html_6c770454c7bb490.png)

![](RackMultipart20200807-4-10x14ou_html_ee6b7cd6215d4ab7.png)

_As duas imagens acima mostram como funciona uma tabela dinâmica: o valor pago por cado doador, em diferentes datas, foi agregado em uma única soma. Fonte: elaboração própria_

Por fim, **cruzar** dados também pode ser interessante: o termo significa trazer uma segunda base de dados que possa enriquecer o trabalho de análise. Um exemplo clássico é reunir dados de resultados eleitorais por município com os indicadores de desenvolvimento de cada cidade, por exemplo.

Existem diferentes formas de cruzar tabelas diferentes. Nos editores de planilha, há funções como a procura vertical (PROCV ou, em inglês, VLOOKUP, vertical lookup), que podem resolver cruzamentos mais simples. Porém, à medida que você avançar no trabalho com dados, vai perceber que realizar cruzamentos com editores de planilha não é o ideal. Nestes casos, o recomendável é utilizar linguagens de programação ou SQL, que conta com a poderosa função JOIN, responsável por unir tabelas diferentes.

Seja qual for a ferramenta que você adote, o princípio permanece: para fazer um cruzamento, você precisa de um campo que sirva como identificador, ou seja, uma coluna ou variável que esteja presente nas tabelas que serão cruzadas. A existência de campo identificador serve como uma &quot;ponte&quot; para conectar bases diferentes e é fundamental para realizar cruzamento.

Além disso, também vale atentar para padrões temporais (os gastos do governo crescem em algum momento do ano?), para outliers suspeitos (por que essa compra específica é muito mais cara que as demais?) e para tendências de crescimento (por que os gastos desse ministério subiram tanto a partir do ano passado?).

No final das contas, a chave para uma boa matéria é a curiosidade e a capacidade de fazer boas perguntas para a planilha. Como vimos, é possível fazer muitas coisas com editores de planilha, mas se você quer realmente progredir na análise de dados é altamente recomendável que aprender uma linguagem de programação. Assim, você conseguirá documentar e checar melhor suas análises, além de não ficar limitado às funcionalidades dos editores de planilha.

Como visto no primeiro capítulo, a linguagem SQL pode ser um bom começo. Ao contrário das planilhas, trabalhar com bases de dados em SQL te permitirá lidar com volumes grandes de informações. Com ele, você conseguirá fazer operações de análise, mas tenha em mente que esta é antes de tudo uma linguagem de consulta, como o seu nome indica (Structured Query Language).

Se você quer entrar a fundo na análise de dados, vá para o Python ou R. Na linguagem R, a dica para quem quer trabalhar com análise é a biblioteca Tidyverse, uma biblioteca que reúne diversos recursos que facilitam e muito a lida com os dados. Ele é relativamente simples de ser compreendido e guarda muitas semelhanças com o SQL, de modo que pode ser uma opção interessante para quem quer começar com aquela linguagem para depois alçar vôos maiores. O Tidyverse também já conta com o ggplot2, uma poderosa ferramenta visualização de dados.

Já em Python, um componente fundamental para manuseio de dados é o **pandas**. Trata-se de um pacote bastante robusto, considerado a principal referência para análise de dados nesta linguagem. Em vez de lidar com loops e condicionais, como é comum no mundo da programação, o pandas implementa uma estrutura de dados chamada _dataframe_, de mod semelhante ao Tidyverse, citado acima. Assim, na prática, a análise de dados se assemelha bastante ao trabalho com planilhas, com uma estrutura de colunas e linhas.

Ele pode ainda ser combinado com outras bibliotecas, como o _matplotlib_, parar criar gráficos simples de maneira rápida. Além disso, ele se destaca pela performance ao lidar com grandes volumes de dados ou realizar operações complexas.
=======
Atenção para nomes de pessoas: **nunca faça correções em nomes de pessoas caso não tenha certeza absoluta de que se trata de um erro.** Nomes podem ter variações de grafias que podem não acompanhar sua imaginação. Por isso, não altere se não estiver absolutamente seguro quanto à presença de erro.
>>>>>>> 58e30bf76c36e7715cc0dff0f637c1dbaf075845
