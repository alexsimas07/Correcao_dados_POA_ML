🌞 Correção de Dados de Irradiância Solar com Regressão Linear

📄 Sobre o Projeto

Este repositório foi criado com o objetivo de automatizar o processo de correção de dados faltantes ou inconsistentes de POA (Plane of Array - Irradiância Solar no Plano do Módulo Fotovoltaico), utilizando Machine Learning com foco em Regressão Linear.

Em usinas solares, o dado de POA é essencial para avaliar a eficiência da geração de energia em relação ao previsto por simuladores como o PVSyst. Quando esses dados são perdidos (por falhas em sensores, comunicação, entre outros), a análise de desempenho e os KPIs ficam comprometidos. Este projeto resolve esse problema de forma automática e inteligente.

✨ Principais Benefícios

Correção automatizada de falhas nos dados de irradiância

Economia de tempo para analistas

Redução de retrabalho e erros manuais

Aproveitamento de dados de usinas vizinhas (em clusters regionais)

Melhoria na precisão dos KPIs de eficiência

⚖️ Tecnologias Utilizadas

Python 

Pandas

NumPy

Scikit-learn

Matplotlib / Plotly (para visualizações)

Jupyter Notebook (para testes e desenvolvimento)

⚡ Como Funciona

Leitura do Dataset: O modelo consome um DataFrame com informações de produção e irradiância (quando existente).

Pré-processamento: Limpeza dos dados, normalização, preenchimento de nulos.

Treinamento do Modelo: Um modelo de regressão linear é treinado com os dados disponíveis.

Predição: O modelo é usado para prever valores de POA ausentes com base em dados históricos e de usinas semelhantes.

Validação: Métricas como R² Score e MSE são utilizadas para avaliar a qualidade do modelo.

👨‍💼 Autor

Alexsander Maia SimasPleno Cientista de Dados | Especialista em Energia SolarLinkedIn | alexsander@email.com

📚 Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

Se você trabalha com dados de energia solar e precisa de uma solução prática para preencher falhas em medições de irradiância, este projeto é pra você! ✨
