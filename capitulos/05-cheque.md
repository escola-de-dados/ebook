# Cheque
Até agora, você aprendeu, em linhas gerais, o que são dados e como encontrá-los ou obtê-los. Para começar a fazer análises, é preciso mergulhar na etapa de **verificação e limpeza** dos dados.

Você pode estar com uma planilha (aparentemente) bem estruturada na sua frente e ansioso para analisá-la, mas se você seguir direto para essa etapa e pular este capítulo poderá se frustrar, ter que refazer a análise ou, pior, publicar informações erradas.

É comum que as bases de dados não cheguem prontas para análise e precisem passar por uma série de verificações e limpezas. É bastante frequente detectar inconsistências ou retirar colunas para reduzir o tamanho de uma base de dados e lidar com elas mais facilmente.

A **verificação** consiste na busca de elementos que comprovem que os dados coletados estão corretos, são consistentes e que não há falta de informação que comprometa o seu trabalho posterior. Esse processo envolve desde as checagens mais básicas e aparentemente banais, como verificações de formato (texto ou numérico, por exemplo) a outros pontos mais complexos, que envolvam comparar os dados com outras fontes.

A checagem é uma etapa fundamental do trabalho que dados. Na prática, ela deve ocorrer de forma transversal, desde a obtenção até a visualização. Ou seja, ao realizar uma raspagem de dados, é importante que durante esta coleta você já verifique se as informações estão sendo capturadas corretamente. Na análise e visualização, o mesmo acontece. Faça a checagem dos dados e, se possível, compare-os com os resultados obtidos por outras fontes.

Já falamos sobre a importância de observar a documentação que acompanha as bases de dados. Este é o primeiro passo para começar a verificação: procure pelo dicionário de dados. Em alguns casos, esse documento pode vir com diferentes nomes: leia-me, nota técnica, nota informativa, anexo etc. Esse arquivo, que funciona como uma espécie de bula, incluirá explicações sobre as variáveis adotadas na estruturação das informações.

Nesse documento, idealmente, haverá também informações detalhadas sobre as unidades de medidas utilizadas (gramas, quilos ou toneladas, por exemplo) e os formatos adotados (número absoluto, índice, taxa, percentual etc.).

**Dados, assim como humanos, são imperfeitos**

Até mesmo uma fonte que conhecemos bem e tem as melhores credenciais possíveis pode se enganar: um especialista pode cometer um erro de avaliação, a testemunha de um evento pode se confundir e alguém que tenta relembrar um acontecimento histórico que vivenciou pode ser traído pela própria memória.

O mesmo vale para bancos de dados. Até algumas das melhores bases possíveis, mantidas e atualizadas por instituições relevantes e confiáveis, podem trazer problemas como esses. No caso das planilhas, essas falhas podem se apresentar como erros de digitação, entradas duplicadas e outros problemas do gênero. O papel do repórter é verificar se a informação que recebe é legítima antes de publicar, não importa se ela venha da boca de um especialista renomado ou de um banco de dados do governo.

Tomemos como exemplo um caso ocorrido durante a pandemia de Covid-19 no Brasil. Ao final da tarde, como de costume, o Ministério da Saúde divulgou uma imagem com os números atualizados de casos e mortes pela doença em todas os estados do país. No dia 20 de abril de 2020, foi publicado um dado que indicava crescimento substancial da epidemia em São Paulo: a tabela mostrava que as mortes passaram, em 24 horas, de 1.015 para 1.307 - um surreal crescimento de 30%, muito acima do que havia sido observado nos dias anteriores.

O número recorde chegou a aparecer na manchete de portais de notícias, mas estava errado. Por sorte, o crescimento fora do padrão chamou a atenção dos jornalistas mais atentos, que começaram a cobrar explicações do Ministério.

Resposta: o que aconteceu não foi um crescimento sem precedentes, mas um erro de digitação. O total de mortes não havia pulado de 1.015 para 1.307, mas sim para 1.037. O dado foi retificado.

Esse exemplo é excessivamente dramático, já que trata de uma estatística que estava no centro da agenda de notícias nacional e dificilmente passaria despercebido. Ainda assim, é ilustrativo de como apenas as credenciais oficiais não são suficientes para garantir precisão.

Há casos em que esses erros são mais difíceis de detectar. O [_Basômetro_](https://arte.estadao.com.br/politica/basometro/), ferramenta do Estadão, compreende dados de votos da Câmara dos Deputados para medir quanto apoio o Poder Executivo tem entre parlamentares. Em acesso às bases de dados das votações, desde 2003, foram percebidas algumas inconsistências: havia uma votação em que apareciam mais de 513 registros de deputados. Isso é impossível, já que a Câmara só tem esse número de membros. O que aconteceu, afinal? Alguns deputados, não se sabe o motivo, apareciam duplicados nos dados.

Pela lógica, cada sessão de votação precisava cumprir alguns requisitos para que os dados fossem válidos: não poderia ter registro de mais de 513 votos, não poderia ter mais de um voto registrado para um mesmo deputado e assim por diante. Apenas aplicando esses filtros à base de dados inteira, foi possível detectar e corrigir outras sessões com problemas semelhantes.

## Biografando dados

Uma parte fundamental após a obtenção das informações é realizar uma espécie de **biografia dos dados**. Basicamente, você precisa entender minimamente a origem, a captação, o recorte e as limitações dos dados nas suas mãos. Isso pode parecer fácil, mas é preciso atenção. Um deslize nesta etapa e toda seu trabalho futuro com os dados estará comprometido. Por isso, nesta seção, iremos explicar um pouco deste método de verificação e checagem de dados.

Por que é importante biografar os dados antes de entrevistá-los?

Para seguir com a metáfora, vamos pensar no processo de apuração de uma reportagem tradicional, que não usa muitos dados quantitativos: o repórter, quando se encontra com a fonte, faz uma série de perguntas e usa as respostas para produzir a matéria. Isso é uma entrevista, obviamente.

No trabalho com dados, o equivalente acontece quando o jornalista começa a mexer em filtros e classificações para descobrir qual foi o maior gasto de um departamento do governo no ano, por exemplo.

Entretanto, a entrevista não é o começo de uma apuração jornalística. Antes de falar com qualquer pessoa, o bom repórter precisa fazer a lição de casa. Além de estudar o tema da conversa e preparar perguntas, ele precisa também descobrir o máximo sobre as características da pessoa com quem vai falar.

Quem é o entrevistado? Quais são seus interesses? Quais são suas áreas de especialidade e atuação? Ele tem alguma conexão com pessoas ou grupos que podem gerar conflitos de interesse? Existe alguma controvérsia relevante a seu respeito? Ele costuma ser ouvido por outros jornalistas? Ele tem um histórico confiável como informante? Ele é respeitado pelos seus pares? É preciso saber a resposta para essas perguntas antes de buscar informações com uma fonte. 

O mesmo vale para um banco de dados. Tentar entrevistar uma planilha sem saber detalhes sobre ela é uma receita infalível para erros. Biografar dados é fazer essa pesquisa prévia, etapa necessária antes de qualquer tentativa de análise quantitativa.

E o que devemos procurar saber sobre uma planilha antes de partir para a entrevista? A cientista de dados Heather Krause [dá um exemplo prático](https://www.youtube.com/watch?v=yCuRQc4xuhA) com base em um de seus temas de pesquisa mais recorrentes: violência contra a mulher.

O entrevistado da vez era um relatório público pela ONU em 2015. Uma fonte de confiança, certo?

Bem, vamos ver o que ela descobriu sobre a coleta de dados durante o trabalho de biografia e pensar um pouco sobre como esses detalhes podem impactar os números.

O primeiro passo foi analisar com atenção o **apêndice estatístico** do relatório. Esses documentos complementares são, geralmente, bem chatos de ler, mas reúnem informações metodológicas importantes sobre a coleta de dados de qualquer fonte.

Como dissemos anteriormente, você pode acabar esbarrando nele com outro nome: dicionário de dados, metadados, anexo metodológico. Enfim, o que importa é que lá estão detalhes sobre os campos que aparecem na planilha, o que eles significam e como foram preenchidos. Exige força de vontade, mas é essencial superar a linguagem de bula de remédio desses documentos.

O que Krause descobriu nesse exercício de atenção e paciência? Que os métodos de coleta de informação variam de país para país e de ano para ano, o que dificulta comparações.

Exemplo: no Malawi, um país do sudeste africano, foi registrada uma variação inesperada nas taxas de violência de uma pesquisa para a outra, entre 2004 e 2005. O número subiu desproporcionalmente e, logo em seguida, voltou o cair.

O que aconteceu nesse intervalo? Será que houve um grande evento político, social e cultural que gerou esse pico? Parece uma boa história, não?

A explicação, porém, era bem menos empolgante. No ano do crescimento desproporcional, quem fez a coleta de dados foi uma instituição privada, com uma metodologia descrita apenas como "inovadora", sem mais detalhes.

Nos outros anos, a coleta foi feita por agências financiadas com recursos governamentais, que usavam uma metodologia mais tradicional e transparente.

A variação, portanto, é provavelmente efeito desse percalço na continuidade histórica dos dados e não consequência de uma mudança no mundo real. E os problemas não paravam por aí!

Além do uso de fontes diferentes, a data de coleta dos dados variava radicalmente entre os diferentes países. O relatório inclui informações de 2003 e 2013 sob o rótulo de "números mais recentes disponíveis", por exemplo.

O jornalista desavisado poderia, então, ao tentar contrastar dois países, acabar comparando uma realidade atual com outra que, provavelmente, não é mais relevante.

Essas limitações importantes estavam presentes em um relatório global da ONU, que é tida como uma fontes mais confiáveis para assuntos internacionais. Por sorte, os autores da pesquisa foram transparentes e incluíram essas possíveis falhas metodológicas no documento.

Entretanto, nem todo banco de dados é tão "honesto". Muitos dados públicos não vêm acompanhados de um detalhamento tão minucioso das próprias limitações. Muita vezes sequer vêm acompanhados de uma descrição decente do que significa cada um dos campos da planilha.

Diante de um cenário como esse, o trabalho do repórter inclui entrar em contato com os autores do levantamento para tirar todas as dúvidas possíveis. Como dissemos brevemente antes, a dica é nunca presumir o que um rótulo de coluna significa ou de que forma os dados foram reunidos. Sempre é preciso fazer esse trabalho prévio.

Krause resume o processo de biografia de dados com uma lista de perguntas que precisam de resposta antes da apuração seguir em frente:

**Quem coletou os dados e por que os coletou?**
Fique de olho em possíveis conflitos de interesse e em outras formas que a autoria da pesquisa podem afetar os dados. Algumas são menos óbvias. Por exemplo, pesquisas sobre renda costumam ter resultados diferentes quando são feitas por instituições governamentais. Não é conspiração, mas sim desconfiança: as pessoas tendem a subestimar o quanto ganham, com medo de possíveis cobranças ou impostos.

**Como os dados foram coletados?** 
Os dados vêm de um censo que fala com todas as pessoas do país, batendo de porta em porta? São feitos com base em um recorte amostral da população? São coletados por telefone? São inseridos em um programa de banco de dados por policiais ou médicos? São consolidados automaticamente por um sistema automático? Tudo isso afeta a representatividade, a qualidade e as conclusões que podemos tirar dos números.

**Quando os dados foram coletados ou atualizados?** 
Uma pegadinha comum é que os dados divulgados em um ano mostram, na realidade, o cenário de outro momento. Um exemplo comum são os resultados de pesquisas eleitorais. Como, em época de eleição, a opinião pública costuma mudar rápido, a pesquisa representa o estado das coisas no dia de campo (ou seja, no dia em que os pesquisadores fizeram as entrevistas) e não na data de divulgação, que costuma ser até dois dias depois. 


## Tópicos de atenção

Para analisar os dados de uma planilha, é importante que você entenda o que significa cada linha e cada coluna da sua tabela. Imagine uma base de dados sobre Covid-19 no Brasil. O primeiro passo é entender o que ela registra: cada linha na tabela é um paciente atendido ou o total de casos de uma cidade, por exemplo? Depois de entender o que as linhas significam na sua tabela, é importante compreender cada coluna.

Uma coluna ou variável chamada "localidade", por exemplo, pode representar pelo menos duas coisas: o município de residência de um cidadão ou a localidade onde ele foi atendido. Não raro, pessoas recebem atendimento de saúde fora do município onde vivem. Por isso, é preciso ficar atento à documentação e à descrição do significado das variáveis de uma planilha.

Se sua base for muito grande para você fazer checagens de todos os registros, uma dica é separar uma amostra aleatória dos seus dados e verificar se está tudo certo. É importante que a seleção seja aleatória. Por exemplo, se você checa apenas as primeiras linhas de uma tabela com registros em ordem cronológica, problemas que tenham ocorrido mais próximos ao fim do período podem passar despercebidos.

**Completude e coerência**

A identificação da eventual falta de registros em um banco de dados deve ser imediatamente verificada junto à fonte original. Exemplo: você obteve os dados do Ministério da Saúde sobre os contaminados pela Covid-19 nas 27 unidades federativas do Brasil e, ao checar se todas elas estão presentes na base de dados, constata que um estado ou um município está ausente. Reflita: o que tal ausência significa? Significa que ninguém foi contaminado ou que os municípios ou estados não foram analisados?

Se você receber soma, dados agregados ou operações matemáticas já realizadas, mas também tiver acesso aos dados desagregados, a recomendação é refazer e checar os cálculos. Especialmente se a base de dados foi elaborada manualmente, erros neste sentido não são incomuns.

Para entender melhor a importância desse processo, aí vai uma história real. Em uma redação de jornal, dois profissionais estavam produzindo uma matéria sobre filiações partidárias e as migrações de pessoas entre partidos. Enquanto um jornalista de dados ficou responsável pela a obtenção dos dados na página do Tribunal Superior Eleitoral (TSE), via web scraping, outro tinha a missão de fazer as análises a partir dos dados coletados.

Quando as perguntas foram respondidas e o texto e a visualização estavam prontos, foi notada a ausência de dois partidos da análise. Consequentemente, as duas siglas estavam ausentes na reportagem e na infografia. O fato provocou estranheza: será que nenhuma pessoa dessas duas legendas políticas nunca trocaram de partido? Onde estão seus filiados?

Após uma conversa entre os profissionais, eles resolveram checar cada etapa do processo e concluíram que havia um erro no processo. Em função dos descuidos, a reportagem estava comprometida, uma vez que retratava as migrações de filiados de um partido ao outro utilizando tanto números absolutos quanto percentuais. Portanto, a ausência das duas legendas alterava, também, os cálculos realizados para os demais partido. Por sorte, porém, a matéria estava "pronta" com antecedência, o que permitiu refazê-la antes do envio do conteúdo para a gráfica responsável pela impressão do jornal.

Este caso permite refletir sobre o que poderia ser feito para evitar o erro e a consequente repetição de procedimentos. O desfecho seria diferente se houvesse uma verificação básica que mostrasse a presença de todos os 33 partidos na base de dados obtida via web scraping. O erro ocorreu duas vezes: na ausência de verificação da planilha recebida e, antes disso, na falta de detecção do problema na hora da captura dos dados, quando uma primeira verificação deveria ter sido feita.

A história se torna ainda mais complexa porque o código que havia sido desenvolvido para a raspagem e obtenção dos dados fora usado para uma reportagem anterior, que não apresentou erro em relação ao número de partidos.

O que mudou, então?

Os responsáveis pelo site do TSE alteraram a grafia das siglas desses partidos, fazendo com que o código, que já estava pronto, não conseguisse mais identificar as siglas. Por isso, **muito cuidado se for reutilizar um código**. Às vezes os responsáveis pelas páginas na web fazem pequenas alterações que podem comprometer a obtenção de dados recentes.

Este exemplo também mostra que a checagem das informações pode (e deve!) ser aplicada também na etapa de obtenção de dados, de modo a mitigar possíveis problemas posteriores. Ao fazer raspagens de dados, faça sempre uma checagem dos dados em todas as etapas para garantir que todas informações estão sendo capturadas adequadamente.

E mesmo dados estruturados em planilhas podem vir acompanhados de muitos problemas. O jornalista de dados precisa ser minucioso e desconfiado. O trabalho com as bases de dados não admitem fios soltos e, por isso, o trabalho de verificação e limpeza inclui identificar potenciais problemas para eliminá-los imediatamente.

**Valores anormais**

Uma das primeiras etapas na checagem de dados com números ou valores é a identificação dos chamados **valores extremos ou outliers**. Números que destoam muito dos demais podem ter dois significados: serem de fato casos especiais que merecem investigação ou serem frutos de erros.

Em uma análise sobre a despesa de parlamentares com diárias, por exemplo, é interessante observar se um deles se sobressai em termos de gastos públicos em relação aos seus colegas. Em uma prestação de contas de campanha ou declarações de bens de políticos, o mesmo pode acontecer.

Números extremos, seja para mais ou para menos, podem ser chamativos. Lembre-se, porém, de verificar as informações antes de seguir uma possível história: o que ocorre, às vezes, é o preenchimento incorreto de informações. Na declaração de patrimônio de candidatos a um cargo eletivo, por exemplo, a simples adição do número zero infla o valor dos bens declarados. Por isso, a checagem dos valores extremos ou anormais nas planilhas é uma etapa fundamental não só da análise mas também da checagem da integridade dos dados.

**Unidades de medida**

Fique atento quanto às unidades de medida (milhas, quilômetros, pés) ou moedas (real, dólar, peso, libra e outros) utilizadas em um banco de dados. Nem sempre essas informações são padronizadas. Para descobrir qual é o caso, leia cuidadosamente a documentação. Não presuma, por exemplo, que todas as planilhas criadas no Brasil estão estruturadas em reais.

Se estiver trabalhando com dados de diversas fontes, escolha a unidade de medida ou moeda com a qual pretende trabalhar e realize as conversões necessárias. Se possível, acrescente colunas e sinalize as alterações.

Verifique, sobretudo, em que formato estão os números da base de dados com a qual pretende trabalhar. Em alguns casos, não haverá casas decimais. É o que ocorre com o número de nascimentos, mortes e outros: não é possível que haja 3,2 óbitos ou 10,8 nascimentos, por exemplo. Se uma coluna reúne informações sobre *pageviews* (número de acessos), da mesma forma, não pode conter números decimais.

