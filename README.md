# **Previsão de Preços de Imóveis Usando Regressão Ridge**

---

## **📌 Descrição do Projeto**
Este projeto tem como objetivo prever os preços de imóveis utilizando técnicas de **Ciência de Dados** e **Machine Learning**, aplicando **Regressão Regularizada Ridge** para lidar com multicolinearidade entre variáveis.

A análise foi realizada com base em um **dataset de imóveis** que contém características como tamanho, qualidade da construção, localização e outros atributos relevantes. Além disso, foram aplicadas etapas de pré-processamento de dados, tratamento de outliers e validação cruzada.

---

## **🛠️ Tecnologias Utilizadas**
As bibliotecas e ferramentas usadas neste projeto incluem:

- **Python** (versão 3.8 ou superior)
- **Pandas** - Manipulação e limpeza de dados
- **NumPy** - Operações numéricas
- **Matplotlib** e **Seaborn** - Visualização de dados
- **Scikit-learn** - Modelagem e métricas de avaliação

---

## **🔍 Metodologia**
1. **Análise Exploratória**:
   - Visualização da distribuição dos preços e correlação entre variáveis.

2. **Pré-processamento dos Dados**:
   - Remoção de **outliers** usando o método **IQR**.
   - Tratamento de variáveis categóricas com **dummies**.
   - Criação de uma **proxy** para a localização através do preço médio por `zipcode`.

3. **Modelagem**:
   - Aplicação da **Regressão Ridge** para lidar com multicolinearidade.
   - Validação cruzada para avaliar a performance do modelo.

4. **Avaliação**:
   - Métricas utilizadas: **R²**, **MAE** (Erro Absoluto Médio) e **RMSE** (Raiz do Erro Quadrático Médio).
   - Visualização: Comparação entre valores reais e previstos, distribuição dos resíduos e análise dos coeficientes do modelo.

---

## **📊 Resultados Obtidos**
- **R²**: 0.7745  
- **MAE**: $72,101  
- **RMSE**: $97,476  
- **Validação Cruzada**: R² médio de 0.7779  

### **Gráficos e Visualizações**
1. **Valores Reais vs. Previstos**  
   ![Valores Reais vs. Previstos](images/RealVsPrevisto.png)

2. **Distribuição dos Resíduos**  
   ![Distribuição dos Resíduos](images/Residuos.png)

3. **Importância das Variáveis**  
   ![Importância das Variáveis](images/Importancia_Variaveis.png)

---

## **📂 Estrutura do Projeto**
```plaintext
|-- README.md
|-- data/
|   |-- house_data.csv          # Dataset original
|-- notebooks/
|   |-- Pratica_Regressao.ipynb # Jupyter Notebook com o código do projeto
|-- images/
|   |-- RealVsPrevisto.png   # Gráfico: Valores Reais vs. Previstos
|   |-- Residuos.png # Gráfico: Distribuição dos Resíduos
|   |-- Importancia_Variaveis  .png # Gráfico: Importância das Variáveis
|-- requirements.txt            # Lista de bibliotecas necessárias
```



🚀 Como Executar o Projeto
Siga os passos abaixo para executar o projeto em sua máquina:

1. Clone o Repositório:

```bash
git clone https://github.com/seu-usuario/projeto-regressao-ridge.git
cd projeto-regressao-ridge
```

2. Instale as Dependências:
```bash
pip install -r requirements.txt
Execute o Notebook: Abra o Jupyter Notebook e execute o arquivo:
```

3. Execute o Notebook: Abra o Jupyter Notebook e execute o arquivo:
```bash
jupyter notebook
```


🧩 Próximos Passos
- Testar outros modelos de regularização, como Lasso e ElasticNet.
- Criar interações entre variáveis (ex.: grade * sqft_living).
- Aplicar técnicas de feature scaling para melhorar o desempenho.

📚 Referências
- Livro: "Estatística Prática para Ciência de Dados"
- Documentação do Scikit-learn: https://scikit-learn.org/
  
🔗 Contato
Se você tiver dúvidas ou sugestões, entre em contato:
- 📧 Email: teodorobfelipe@gmail.com
- 💼 LinkedIn: www.linkedin.com/in/felipe-teodoro-bandeira
