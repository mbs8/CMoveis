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
Usar random forest e MLP para gerar fingerprints e estimar as posições (latitude e longitude) dos pontos de teste.

## 4. Resultados
### 4.1 Análise dos dados
### 4.2 Métodos de localização propostos
- **Baseline:** Fingerprint usando modelo de propagação Cost231Hata
- **Solução:** Dois modelos de _machine learning_ para servir como modelo de propagação na geração do fingerprint
  - _Random forest_ 
  - _Multi Layer Perceptron_ (MLP)
### 4.3 Histograma dos erros em metros

### 4.4 BoxPlot dos erros em metros
### 4.5 Mapa de comparação posições preditas vs. posições reais
### 4.6 Erro de localização em metros
**Método 1:** Apenas medições
**Método 2:** Apenas fingerprint 20 x 20
**Método 3:** Fingerprint 20 x 20 + medições
**Método 4:** Random forest
**Método 5:** Random forest + fingeprint
**Método 6:** MLP
**Método 7:** MLP + fingerprint

## 5. Conclusão e dificuldades