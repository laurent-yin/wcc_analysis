# wcc_analysis

Lichess page documentation: https://lichess.org/page/world-championships

Each WCC has a study, studies are fetched using: https://lichess.org/api#operation/studyAllChaptersPgn

Source PGNs are found in /analysed_pgns

Analysiscsv.py for extracting analysis and exporting as CSV - sample export is found in analysis.csv

Visualize.py takes in CSV and makes some charts, examples are shown below.

# Output 1: Table of games by combined ACPL

|Year|Game No.|         White Player          |      Black Player    |Combined ACPL|
|:--:|:------:|------------------------------:|---------------------:|:-----------:|
|2021|    3   |          Nepomniachtchi, Ian  |     Carlsen, Magnus  |     6.62    |
|1978|   15   |           Kortschnoj, Viktor  |     Karpov, Anatoly  |     6.67    |
|1987|   18   |               Kasparov, Gary  |     Karpov, Anatoly  |     6.69    |
|1972|   16   |        Fischer, Robert James  |    Spassky, Boris V  |     6.86    |
|2014|    9   |              Carlsen, Magnus  |  Anand, Viswanathan  |     6.95    |
|....|  ....  |              ....             |          ...         |        ...  |
|1886|   11   |  Zukertort, Johannes Hermann  |   Steinitz, William  |   153.59    |
|1957|    9   |           Botvinnik, Mikhail  |    Smyslov, Vassily  |   154.90    |
|1892|   19   |            Chigorin, Mikhail  |   Steinitz, William  |   167.13    |
|1889|   15   |            Chigorin, Mikhail  |   Steinitz, William  |   211.98    |
|1892|   15   |            Chigorin, Mikhail  |   Steinitz, William  |   212.33    |



# Output 2: Some graphs of average combined acpl vs. time
![Barplot](https://github.com/michael1241/wcc_analysis/blob/master/barplot.png)
![Boxenplot](https://github.com/michael1241/wcc_analysis/blob/master/boxenplot.png)
![Boxplot](https://github.com/michael1241/wcc_analysis/blob/master/boxplot.png)
![Boxplot2](https://github.com/michael1241/wcc_analysis/blob/master/boxplot_color_champ.png)
![Boxplot_acpl](https://github.com/michael1241/wcc_analysis/blob/master/boxplot_colored_acpl.png)
![Stripplot](https://github.com/michael1241/wcc_analysis/blob/master/stripplot.png)
![Violinplot](https://github.com/michael1241/wcc_analysis/blob/master/violinplot.png)
![Scatterplot](https://github.com/michael1241/wcc_analysis/blob/master/scatterplot.png)
![Regplot](https://github.com/michael1241/wcc_analysis/blob/master/regplot.png)
![Lmplot](https://github.com/michael1241/wcc_analysis/blob/master/lmplot.png)


# Output 3: All games by ACPL vs. num moves
Note some games are off the table in both x and y axes.
![Gamelengthplot](https://github.com/michael1241/wcc_analysis/blob/master/gamelengthscatterplot.png)
