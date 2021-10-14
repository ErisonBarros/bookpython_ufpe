# Python

*Prof. Erison Barros*

## Objetivos

Este material foi escrito com o objetivo de introduzir Engenheiros Cartógrafos e Agrimensores  e  e estudantes de Estatística aos conceitos fundamentais da linguagem Python, bem como apresentá-los às ferramentas que mais lhe podem ser úteis, incluindo bibliotecas de computação matemática, visualização de dados, manipulação de bases e bancos de dados, ferramentas de aprendizagem de máquina, computação paralela, computação em GPU, inferência Bayesiana e criação e consumo de API’s Web.

Python é uma linguagem de programação interpretada, de alto nível e de propósito geral. Seu criador, Guido van Rossum, enfatizou legibilidade de código e sua abordagem de orientação a objetos permite que projetos de diversos tamanhos sejam desenvolvidos usando código simples, lógico e fácil de entender, devido a sua sintaxe clara. Além da orientação a objetos, Python também oferece suporte a outros paradigmas de programação, como programação estruturada e programação funcional.

Python é visualmente mais “limpa” do que outras linguagens, além de ser mais intuitiva, pois frequentemente usa palavras da língua inglesa onde outras linguagens usariam pontuações. O nome da linguagem é um tributo ao grupo de comédia britânico Monty Python, o que inspirou os desenvolvedores a fazer com que a linguagem seja divertida de usar. Essa abordagem de desenvolvimento inspirou a criação do neologismo “pythonico”, que quer dizer que o código é natural e está de acordo com a filosofia minimalita e de ênfase na legibilidade. Por outro lado, códigos difíceis de entender or ler são chamados de não-pythonicos. Usuários e admiradores de Python, sobretudo aqueles considerados mais experientes costumam ser chamados de Pythonistas.

[========]

## Por que estudar Python?
Em 2017, o Stack Overflow, website de perguntas e respostas destinado a desenvolvedores, publicou um estudo sobre o rápido crescimento no interesse pela linguagem Python [2]. O estudo considerou apenas o interesse de usuários de países de alta renda e naturalmente avaliou apenas resultados até a sua publicação. A Fig. 1, obtida por meio da ferramenta Stack Overflow Trends, apresenta as curvas para as mesmas linguagens, considerando usuários de todo o mundo (o que muda as curvas em relação ao estudo citado) e resultados até o meio de 2019. Até o meio de 2012, Python era a sexta linguagem menos buscada das 7 analisadas, tornando-se a linguagem de maior interesse apenas 6 anos depois, no meio de 2018.



Esse crescimento do interesse por Python extremamente acentuado a partir de 2012 está conectado ao avanço da área de ciência de dados e conhecimentos relacionados, como aprendizagem de máquina, big data, business analytics, entre outras. Python e R costumam ser as linguagens mais citadas por cientistas de dados em seus perfis em redes sociais como LinkedIn. Segundo análise da Initiative for Analytics and Data Science Standards (IADSS) [3], 100% dos cientistas de dados mencionam conhecimento de Python em seus perfis, enquanto 84% mencionam R. Além disso, como mostra a Fig. 2, o mercado de trabalho abraçou essas duas linguagens, com mais de 70% dos anúncios de vagas para cientistas de dados, retirados de sites como LinkedIn, Indeed, SimplyHired e Monster em outubro de 2018, mencionando Python e mais de 60% mencionando R.

    import pandas as pd
    url = 'https://tmfilho.github.io/pyestbook/data/google-trends-timeline.csv'
    trends = pd.read_csv(url, index_col=0, parse_dates=True)
    trends.corr(method='spearman')



O código abaixo gera um gráfico com as quatro séries temporais de interesse. Os valores são relativos ao maior valor de interesse no período, que nesse caso equivale ao interesse por Python em setembro de 2019.

    import matplotlib.pyplot as plt
    plot = trends.plot()
    plt.xlabel('Semana', fontsize=16)
    plt.show()

Fonte: [https://tmfilho.github.io/pyestbook/guide/01_first.html](https://tmfilho.github.io/pyestbook/guide/01_first.html "https://tmfilho.github.io/pyestbook/guide/01_first.html")