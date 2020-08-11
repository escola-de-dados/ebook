# Limpe

A limpeza de dados é uma etapa fundamental de qualquer trabalho com dados. Em geral, ela não é muito empolgante, mas pode tomar um tempo considerável do seu trabalho. Aqui, você irá organizar os dados para que seja possível posteriormente realizar análises, operações matemáticas, filtros, ordenações, enfim, tudo que você precisa para responder às perguntas desejadas.

Ao limpar seus dados, você irá alterar as informações originais da planilha. Por isso, é importante tomar nota das alterações, bem com manter uma cópia da versão original. Em caso de problemas com seu trabalho de verificação e limpeza, você sempre poderá recomeçar do zero.

Caso você utilize linguagens de programação, o próprio código já serve como esta documentação. Além disso, há os chamados notebooks, que costumam ser ótimas ferramentas para documentar códigos e processos de limpeza e análise dos dados. Eles também permitem que você acrescente comentários e lembretes para si ou para seus colegas. Entre os notebooks mais conhecidos estão o Jupyter Notebook e o Colab do Google.

Antes de começarmos a listar os problemas mais comuns para limpeza de dados, é importante que você conheça o conceito de "dados organizados" (tidy data). Trata-se de um forma de organizar dados tabulares, proposto por Hadley Wickham, um dos desenvolvedores de maior destaque da comunidade de R.

Apesar do tempo que cientistas de dados passam limpando a matéria-prima do seu trabalho, ele notou que há pouca reflexão sobre este processo, ao contrário do que acontece com etapas como a análise e visualização de dados, onde há um largo acúmulo de reflexões teóricas e práticas. Por isso, ele concebeu a ideia de tidy data.

De acordo com esta noção, cada tabela registra um certo fenômeno (despesas de um órgão do governo, as notas de alunos, resultados de jogos de futebol ou da situação de pacientes de um hospital, por exemplo). Cada ocorrência será registrada em uma linha ou em uma observação. Cada característica deste fenômeno será uma variável ou coluna e, por fim, a descrição destas características serão chamadas de valores e ocuparão as células.

![No modelo do "tidy data" significa que cada variável deve ter sua própria coluna, cada observação deve ter sua própria linha e cada valor deve ter sua própria célula.](images/limpe/tidydata.png)

A seguir, um exemplo de uma tabela fora do formato tidy data.

| **Nome/Registro** | **Turma** | **Biologia** | **Química** | **Física** |
| --- | --- | --- | --- | --- |
| Marcela Nunes - 20351 | A | 7 | 6 | 6 |
| Ricardo Fernandes - 20589 | C | 5 | 4 | 7 |

Na tabela acima, o fenômeno capturado são notas de alunos. Mas repare que a variável "disciplina" ocupa diferentes colunas. No formato tidy data, essa planilha deveria ter uma coluna chamada "disciplina", onde as matérias estivessem declaradas nas células abaixo dessa coluna.

Outro problema que pode ser visto na tabela são as linhas referentes à coluna Nome/RA. Nesse caso, há duas informações (valores) em uma mesma célula: o nome do estudante e o registro do aluno (um código identificador).

Porém, percebemos que os nomes dos alunos estão separados dos registros por um hífen. Deste modo, podemos usar esse padrão para separar estes valores em colunas ou variáveis distintas, utilizando editores de planilha ou linguagens de programação, por exemplo. Como dissemos, o reconhecimento de padrões que permitam a limpeza dos dados será o seu maior aliado nesta etapa.

Para Hadley Wickham, todas estas questões precisam ser corrigidas antes de qualquer trabalho de análise ou visualização de dados. Assim, a tabela deveria ficar assim para atender o formato do *tidy data*.

| **Nome** | **Registro** | **Turma** | **Disciplina** | **Nota** |
| --- | --- | --- | --- | --- |
| Marcela Nunes | 20351 | A | Biologia | 7 |
| Marcela Nunes | 20351 | A | Química | 6 |
| Marcela Nunes | 20351 | A | Física | 6 |
| Ricardo Fernandes | 20589 | C | Biologia | 5 |
| Ricardo Fernandes | 20589 | C | Química | 4 |
| Ricardo Fernandes | 20589 | C | Física | 7 |

Com a organização dos dados, as disciplinas se tornaram uma única coluna, com diferentes valores. Além disso, há uma linha para cada observação (ou seja, notas de aluno em disciplinas) e o nome e número de registro do aluno também foram separados.

## Ferramentas e técnicas de limpeza

Na etapa de limpeza dos dados, mais uma vez, é possível usar tanto linguagens de programação ou softwares com interfaces gráficas. Para trabalhar com planilhas simples e constituídas por poucas linhas, softwares de editores de planilhas (Excel, Google Sheets ou LibreOffice, por exemplo) correspondem à principal solução para quem não domina linguagens de programação.

Mas há também programas úteis para a limpeza de dados, que são gratuitos e possuem interfaces gráficas. Eles irão ampliar em muito suas habilidades na padronização de dados. Nesta seção, falaremos mais sobre estas soluções e, a seguir, conheceremos uma linguagem para descrição de padrões, que podem ser aplicados em diferentes programas e plataformas: as expressões regulares.

**Expressões regulares**

Uma expressão regular, também conhecida como Regex, é uma forma comum e concisa de representar algum tipo de padrão em texto. Isso ocorre em uma variedade de aplicações e linguagens, seja pesquisando em um documento, seja fazendo operações de *Localizar e Substituir* ou limpando um conjunto de dados. Muitas linguagens de programação e editores de texto/planilha permitem o uso de expressões regulares. As sintaxes, por sua vez, podem diferir levemente de acordo com a linguagem ou o programa em uso.

As expressões regulares podem parecer enigmáticas e confusas à primeira vista, mas não se assuste. O importante é entender que as letras e caracteres podem ter significados especiais. Um exemplo bastante simples é:

				[0-9]

Esta é uma expressão regular bem simples, que seleciona todos os números entre 0 e 9 em uma sequência de caracteres. Poderia ser útil se você tem um campo com textos e números e precisa separá-los, por exemplo.

Se você precisa descrever padrões para obter informações específicas de sequência de texto, por exemplo, então, provavelmente é o caso de começar a aprender expressões regulares. Explorar a fundo esta sintaxe exigiria um guia por si só. Mas se você quiser ter uma introdução ao funcionamento de expressões regulares, vale conferir [este tutorial da Escola de Dados](https://escoladedados.org/tutoriais/expressao-regular-pode-melhorar-sua-vida/) e utilizar sites como Regex ou Regex101 para testar as operações na prática. Eles podem ser úteis também para "traduzir" expressões regulares que você encontrar na internet, indicando o significado de cada caractere.

**Programas úteis**

A expressão regular é uma linguagem "universal", que você poderá utilizar tanto em editores de planilha, quanto ao escrever códigos com Python e R. Ela também pode ser utilizada em outros tipos de programas, que possuem funções específicas para a limpeza de dados.

Nesta seção, iremos abordar duas destas ferramentas: o OpenRefine e o Workbench.

O OpenRefine é uma ferramenta voltada à limpeza de dados. Ele consegue carregar arquivos em diferentes formatos (inclusive JSON), transformar para tabelas e então aplicar diversas operações, como a remoção de duplicatas, criação ou remoção de linhas e colunas, normatizações, correção de ortografia entre outras funções.

Além disso, o OpenRefine mantém um "log" com todas as operações que foram feitas nos dados originais. Este registro é extremamente útil, caso você precise refazer uma operação ou reaplicar as transformações realizadas em outros dados que seguem os mesmos padrões.

O OpenRefine também conta funcionalidades muito práticas, que permitem padronizar textos com erros de digitação ou grafias distintas. Ele permite até mesmo a consulta a APIs mais simples, que você pode utilizar para preencher novas colunas a partir de dados existentes. O OpenRefineé uma ferramenta de código-aberto, que conta com versões para Windows, Mac e GNU/Linux. Para utilizá-lo, você irá precisar instalá-lo no seu computador.

Se você preferir utilizar uma solução online, pode utilizar o Workbench. Na realidade, esta plataforma é uma ferramenta útil para todas etapas do trabalho com dados, não só a limpeza.

Nela, você pode carregar dados em tabelas, realizar raspagens de dados ou carregar informações do Twitter, por exemplo, para em seguida realizar transformações de limpeza ou operações de análise e visualização dos dados. Na área de limpeza, atualmente, o Workbench oferece funções para remoção de colunas duplicadas, preenchimento de células nulas, geração automática de colunas com identificadores únicos, união e separação de colunas, extração de valores com expressão regular, entre outras funcionalidades.

## Tópicos de atenção

Nesta seção, veremos alguns tópicos que merecem atenção especial na hora de limpar dados, independente da ferramenta ou software que você irá utilizar.

### Ausência de valor

Um problema comum nos conjuntos de dados são a ausência de valor, ou um valor vazio, que pode ser representado de diferentes formas. O nulo (null), a célula em branco, o NA (*not available*) e o número zero podem significar coisas completamente diferentes, dependendo de quem coletou esses dados. Ainda que na programação cada uma dessas representações tenha significados distintos, é preciso verificar.

Para o aprendizado introdutório, é importante entender que qualquer um desses valores em uma planilha pode significar 0. Em outra ocasião, porém, o 0 ou a ausência do valor representa que aquele dado não foi coletado ou que foi perdido. Busque mais informações contextuais junto à fonte original. Diante disso, será possível avaliar se a ausência de valor será mantida ou excluída da análise.

### Entradas duplicadas

Um dos erros mais comuns em bases de dados é quando uma entrada aparece duas vezes por engano. Verifique se há duplicatas exatas no arquivo: em caso positivo, pode ser que você esteja diante de um erro. Porém, só é possível saber se um registro duplicado é um erro ou não conhecendo bem as "regras de negócio" por trás da base de dados.

Considerando um exemplo sobre a Covid-19, poderíamos pensar que determinado estado ou cidade apresenta duas linhas de informação, quando o correto é apenas uma. Se a linha aparecer duas vezes em um conjunto de dados, é preciso entender o motivo. É um erro ou uma atualização/complementação? Atente também às planilhas que envolvem dados financeiros e transações. Vale contatar a fonte primária dos dados e entender o que houve.

### Cabeçalho com informações inúteis

Alguns órgãos públicos oferecem, de praxe, informações técnicas no cabeçalho e no rodapé das planilhas (exemplo: nome do órgão responsável, data da coleta, explicações sobre a metodologia). Embora esse conteúdo auxilie a dar contexto ao material coletado, atrapalham na hora de fazer a análise. Por isso, antes de começar a editar as informações, faça uma cópia do arquivo original - as informações extras podem servir para tirar dúvidas e complementar o material. No entanto, essas mesmas informações de cabeçalho atrapalham a análise (ao fazer uma simples ordenação de valores, por exemplo) e precisam ser removidas.

### Grafia distinta

Ao comparar dados, certifique-se de que nomes de cidades estão registrados com a mesma grafia. Por exemplo, diferentes linhas podem conter a seguinte variação da cidade mais famosa do mundo: Nova Iorque, Nova York, New York, NY - ou, ainda, erros de digitação, como "Nova Yok" e tantas outras possibilidades. Para que possa fazer a análise, é preciso corrigir as grafias estabelecendo uma única versão (as expressões regulares podem ser particularmente úteis aqui). Do contrário, operações realizadas com esses registros podem ficar comprometidas. Não se esqueça de documentar as mudanças.

Atenção para nomes de pessoas: nunca faça correções em nomes de pessoas caso não tenha certeza absoluta de que se trata de um erro. Nomes podem ter variações de grafias que podem não acompanhar sua imaginação. Por isso, não altere se não estiver absolutamente seguro quanto à presença de erro.
