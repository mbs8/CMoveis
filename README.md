# Projeto ES290 - Comunicações Móveis
## 1. Definição do problema
Identificar a localização (latitude e longitude) de um móvel a partir da potência do sinal enviada pelas antenas (BST's) para o dispositivo móvel.
## 2. Ferramentas utilizadas
 - Python 3
 - Jupyter notebook
 - Bibliotecas de python para machine learning 
   - scikit 
   - pandas
   - numpy
   - seaborn
 - Biblioteca auxiliar de calculo de distâncias geográficas: PyRadioLoc

## 3. Solução proposta
Usar random forest para gerar fingerprints e estimar as posições (latitude e longitude) dos pontos de teste. Também comparar com uso de random forest e MLP para previsão direta da loacalização do usuário (latitude e longitude).

## 4. Resultados

### 4.1 Análise dos dados
Da base de dadas LocTreino_Equipe_4.csv
<img src="images/data_visualization.png" alt="compararion_map_1" width="1400" height="250">  

### 4.2 Métodos de localização propostos
- **Baseline:** Fingerprint usando modelo de propagação Cost231Hata
- **Solução:** Dois modelos de _machine learning_ para servir como modelo de propagação na geração do fingerprint e para previsão direta de latitude longitude
  - _Random forest_ 
  - _Multi Layer Perceptron_ (MLP)
### 4.3 Histograma dos erros em metros
**Apenas Medições**  
<img src="images/histogram_1.png" alt="histogram_1" width="400" height="300">
  
  
**Apenas Fingerprint 20 x 20**  
<img src="images/histogram_2.png" alt="histogram_2" width="400" height="300">  
  
  

**Fingerprint 20 x 20 + medições**  
<img src="images/histogram_3.png" alt="histogram_3" width="400" height="300">  
  
  
**Random Forest**  
<img src="images/histogram_4.png" alt="histogram_4" width="400" height="300">  
  
  
**MLP**  
<img src="images/histogram_5.png" alt="histogram_5" width="400" height="300">  
  
  
**Fingerprint + Random Forest (sem otimização)**  
<img src="images/histogram_6.png" alt="histogram_6" width="400" height="300">  
  
  
**Fingerprint + Random Forest (com otimização)**  
<img src="images/histogram_7.png" alt="histogram_7" width="400" height="300">  
  

### 4.4 BoxPlot dos erros em metros
**Apenas Medições**  
<img src="images/boxplot_1.png" alt="boxplot_1" width="400" height="300">  
  
  
**Apenas Fingerprint 20 x 20**  
<img src="images/boxplot_2.png" alt="boxplot_2" width="400" height="300">  
  
  
**Fingerprint 20 x 20 + medições**  
<img src="images/boxplot_3.png" alt="boxplot_3" width="400" height="300">  
  
  
**Random Forest**  
<img src="images/boxplot_4.png" alt="boxplot_4" width="400" height="300">  
  
  
**MLP**  
<img src="images/boxplot_5.png" alt="boxplot_5" width="400" height="300">  
  
  
**Fingerprint + Random Forest (sem otimização)**  
<img src="images/boxplot_6.png" alt="boxplot_6" width="400" height="300">  
  
  
**Fingerprint + Random Forest (com otimização)**  
<img src="images/boxplot_7.png" alt="boxplot_7" width="400" height="300">  
  
  
### 4.5 Mapa de comparação posições preditas vs. posições reais
**Apenas Medições**  
<img src="images/comparation_map_1.png" alt="compararion_map_1" width="700" height="600">  
  
  
**Apenas Fingerprint 20 x 20**  
<img src="images/comparation_map_2.png" alt="compararion_map_2" width="700" height="600">    
   
  
**Fingerprint 20 x 20 + medições**  
<img src="images/comparation_map_3.png" alt="compararion_map_3" width="700" height="600">    
  
  
**Random Forest**  
<img src="images/comparation_map_4.png" alt="compararion_map_4" width="700" height="600">  
  
  
**MLP**  
<img src="images/comparation_map_5.png" alt="compararion_map_5" width="700" height="600">  
  
  
**Fingerprint + Radom Forest (sem otimização)**
<img src="images/comparation_map_6.png" alt="compararion_map_6" width="700" height="600">  
  
  
**Fingerprint + Radom Forest (com otimização)**
<img src="images/comparation_map_7.png" alt="compararion_map_7" width="700" height="600">  
  
  

### 4.6 Erro de localização em metros
**Método 1:** Apenas medições  
**Método 2:** Apenas fingerprint 20 x 20  
**Método 3:** Fingerprint 20 x 20 + medições  
**Método 4:** Random forest  
**Método 5:** MLP  
**Método 6:** Fingerprint + Random Forest (sem otimização)    
**Método 7:** Fingerprint + Random Forest (com otimização)  

<img src="images/erros.png" alt="erros" width="525" height="250">  

## 5. Conclusão e dificuldades