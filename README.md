# 🌞 Correção de Dados de Irradiância Solar com Regressão Linear

## 📄 Sobre o Projeto

Este repositório foi criado com o objetivo de automatizar o processo de correção de dados faltantes ou inconsistentes de **POA (Plane of Array - Irradiância Solar no Plano do Módulo Fotovoltaico)**, utilizando **Machine Learning com foco em Regressão Linear**.

Em usinas solares, o dado de POA é essencial para avaliar a eficiência da geração de energia em relação ao previsto por simuladores como o **PVSyst**. Quando esses dados são perdidos (por falhas em sensores, comunicação, entre outros), a análise de desempenho e os KPIs ficam comprometidos. Este projeto resolve esse problema de forma automática e inteligente.

---

## ✨ Principais Benefícios

- Correção automatizada de falhas nos dados de irradiância
- Economia de tempo para analistas
- Redução de retrabalho e erros manuais
- Aproveitamento de dados de usinas vizinhas (em clusters regionais)
- Melhoria na precisão dos KPIs de eficiência

---

## ⚖️ Tecnologias Utilizadas

- Python 
- Pandas
- NumPy
- Scikit-learn
- yellowbrick
- datetime
- Matplotlib / Plotly (para visualizações)
- Scipy (detecção de outliers e limpeza de dados utilizando Mahalanobis)
- Jupyter Notebook (para testes e desenvolvimento)

---

## ⚡ Como Funciona

1. **Leitura do Dataset**: O modelo consome um DataFrame com informações de produção e irradiância (quando existente).
2. **Pré-processamento**: Limpeza dos dados, normalização, preenchimento de nulos.
3. **Treinamento do Modelo**: Um modelo de regressão linear é treinado com os dados disponíveis.
4. **Predição**: O modelo é usado para prever valores de POA ausentes com base em dados históricos e de usinas semelhantes.
5. **Validação**: Métricas como R² Score e MSE são utilizadas para avaliar a qualidade do modelo.

## 🔧 Customização

- ✏️ Você pode alterar o modelo de regressão ou testar outras técnicas (como regressão polinomial, XGBoost, etc.)
- 🔮 Ajuste o limiar para considerar valores como "faltantes" ou inconsistentes
- ⛅️ Adicione novos datasets de usinas vizinhas para melhorar a previsão

---

## 🚀 Roadmap

- [ ] Generalização dos dados que serão analisados
- [ ] Adicionar suporte para modelos mais robustos (XGBoost, LightGBM)
- [ ] Criar painel em Streamlit para visualização interativa dos resultados
- [ ] Acesso aos modelos pkl utilizando API

---

## 👨‍💼 Autor

**Alexsander Maia Simas**\
Pleno Cientista de Dados | Especialista em Energia Solar\
[LinkedIn](https://www.linkedin.com/in/seu-usuario) | [alexsander@email.com](mailto\:alexsander@email.com)

---

## 📚 Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo [LICENSE](./LICENSE) para mais detalhes.

---

Se você trabalha com dados de energia solar e precisa de uma solução prática para preencher falhas em medições de irradiância, este projeto é pra você! ✨

