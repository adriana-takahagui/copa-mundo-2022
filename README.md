# Previsão da Copa do Mundo Qatar 2022

![Screenshot](world-cup-2022-banner-template-design.jpg)

---

Ao tentar prever o resultado de uma partida da Copa ou quem será o campeão, não é sobre adivinhar, mas sim sobre quantificar a probabilidade desse evento ocorrer dadas as variáveis.

Para isso, neste projeto, utilizaram-se:
* o **Ranking FIFA** para calcular a força de cada seleção, e assim calcular a média de gols.
* a **distribuição de probabilidade de Poisson** para calcular a distribuição de probabilidade de gols de uma partida (considerando de 0 a mais de 7 gols), que tem como entrada a média de gols.


Foram realizadas 100.000 simulações de cada evento. 

O código apresentado e utilizado para gerar os dados que podem ser vistos no dashboard foi baseado no algoritmo desenvolvido pelo professor Ricardo Rocha. Logo, toda a lógica do cálculo das probabilidades é mérito do mesmo. 

Além de realizar algumas adaptações e alterações para atender o resultado desejado, uma alteração feita no código foi adicionar simulações para cada dia de Copa, ou seja, conforme os jogos iam acontecendo a cada dia, os resultados desses jogos foram imputados na simulação, gerando novas probabilidades para cada dia. Isto foi feito com o intuito de acompanhar a evolução das probabilidades ao longo do evento, assim como gerar novas probabilidades para as etapas futuras com base nos resultados dos jogos. 

O algoritmo tem como input as duas tabelas em "DadosCopaDoMundoQatar2022.xlsx" (que se encontra em "dados"). <br>
E gera como outputs as seguintes tabelas: 
* outputEstimativasJogosCopa: contém as probabilidades de vitória, empate e derrota. 
* outputPlacaresPartida: contém a distruibuição de probabilidades de gols da partida.  

E para cada dia de simulação, gera os outputs:
* outputSimulaçõesCopaDoMundo: resultado das 100.000 simulações de um dado dia com as probabilidades de cada etapa da Copa para cada seleção. 
* outputProbabilidadesPorEtapa: contém as probabilidades de cair em cada etapa da Copa.
* outputAvançoPorEtapa: contém as probabilidades de avançar em cada etapa da Copa.

Para desenvolver o dashboard, também me inspirei no trabalho apresentado pela professora Juliana Scudilio. <br>
Como fontes de dados para o dashboard, além dos outputs listados acima e das duas tabelas em "DadosCopaDoMundoQatar2022.xlsx", também criei uma tabela com os resultados dos jogos. 

Para visualizar o código comentado, clique [aqui]( https://github.com/adriana-takahagui/copa-mundo-2022/blob/main/Minicurso_FLAI_Data_Science_na_Copa_do_Mundo_Qatar_2022.ipynb ). 

Para visualizar o resultado em um dashboard interativo e dinâmico, clique [aqui]( https://app.powerbi.com/view?r=eyJrIjoiMTAyMTkyYmEtODIwMi00ZTEwLTkzMzktYTk1MTM5OWMyMjAxIiwidCI6IjgxMTFjMzgxLThjM2EtNDNkMS05ODc4LTA5ZjAzZGQ0N2Y1NiJ9 ).

