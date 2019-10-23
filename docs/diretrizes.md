# 1. Definição do problema 
Utilizar a técnica de localização de fingerprint sem nenhuma otimização resulta em uma **baixa precisão** para ambientes urbanos que contém muitas construções e obstáculos. 

# 2. Ferramentas utilizadas
 - Python 3
 - Jupyter notebook
 - Bibliotecas de python para machine learning 
   - scikit 
   - pandas
   - numpy
   - seaborn

# 3. Apresentação da solução 
Nossa prosposta é pré-processar os dados e usar os dados pré-processados como entrada para a técnica de localização figerprint combinada com modelos de machine learning. O objetivo é aumentar a **precisão** da localização dos dispositivos móveis.

# 4. Resultados
## 4.1 Análise dos dados (Média, desvio-padrão, features etc.)
## 4.2 Dois métodos de localização, sendo um deles alguma técnica básica de referência 
 - **Baseline**: Fingerprint
 - Fingerprint combinando com modelos de machine learning
## 4.3 Histograma dos erros em metros (*) 
## 4.4 BoxPlot dos erros em metros (*) 
## 4.5 Mapa de comparação: posições preditas vs. posições reais (*); 
## 4.6 Erro de localização Médio, Mínimo, Máximo e desvio-padrão (*) 
## 4.7 Erro de localização Médio, Mínimo, Máximo e desvio-padrão (Base de Teste) (#); 
## 4.8 Arquivo Resultados.csv com as colunas pontoId, lat, lon , lat_pred, lon_pred e erro_loc. Onde lat_pred e lon_pred são as coordenadas preditas.
- rssi_3_2RSSI Grupo 3 – Setor 2;
- rssi_3_3RSSI Grupo 3 – Setor 3;
- delay_1 Atraso de propagação Grupo 1 (passos de 234m);
- delay_2 Atraso de propagação Grupo 2 (passos de 234m);
- delay_3 Atraso de propagação Grupo 3 (passos de 234m);
- erro_loc é o erro de localização em metros.

##### (*)  Os  itens  em  questão  devem  ser  gerados  a  partir  de  uma  base  de  dados  contendo  10%  de amostras  retiradas  da  base  de  treino.  Recomenda-se  que  essas  amostras  não  sejam  utilizadas para treinar o algoritmo proposto. 
##### (#) O item em questão deve ser gerado a partir da base de teste que só será utilizada no dia da apresentação do projeto (SERÁ AJUSTADO NOS PRÓXIMOS DIAS)
# 5. Conlusões e dificuldades