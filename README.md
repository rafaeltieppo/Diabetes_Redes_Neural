🧠 Preditor de Risco de Diabetes com Redes Neurais (MLP)
Este projeto aplica técnicas de Ciência de Dados e Inteligência Artificial para prever o risco de um paciente desenvolver diabetes tipo 2, utilizando dados clínicos coletados rotineiramente. A proposta surgiu como parte de um trabalho acadêmico apresentado no TechDay da Faculdade e busca demonstrar, de forma prática, como uma Rede Neural Artificial pode apoiar o diagnóstico precoce e a prevenção da doença.

📊 Sobre o Dataset
O conjunto de dados utilizado é uma versão tratada do Pima Indians Diabetes Dataset, amplamente utilizado para estudos de classificação na área da saúde. Contém informações médicas básicas de pacientes, como:

Idade

Sexo

Glicose

Pressão arterial

Espessura da pele

Insulina

Índice de Massa Corporal (IMC)

O atributo alvo (RESULTADO) indica se o paciente possui diabetes (1) ou não (0).

🔎 Etapas do Projeto
Carregamento e limpeza de dados

Remoção de colunas irrelevantes (ID, nome).

Substituição de valores zero inválidos por NaN.

Preenchimento dos NaN com a mediana da variável.

Pré-processamento

Conversão de variáveis categóricas (como SEXO) para valores numéricos.

Normalização dos dados com StandardScaler.

Balanceamento

Utilização do SMOTE (Synthetic Minority Over-sampling Technique) para lidar com o desbalanceamento entre classes (diabéticos vs. não diabéticos).

Treinamento do modelo

Modelo: MLPClassifier do scikit-learn.

Arquitetura: 2 camadas ocultas com 200 neurônios cada.

Otimizador: adam.

Estratégia de regularização: alpha=0.1 e early_stopping=True.

Avaliação

Acurácia de ~79.87% na base de teste.

Predições em tempo real com entrada de dados manual via terminal.

🧪 Modelo Utilizado
MLPClassifier (Rede Neural Multicamadas)

Ativação: ReLU

Camadas ocultas: (200, 200)

Parada antecipada: early_stopping=True

Normalização: StandardScaler

Balanceamento: SMOTE

📈 Resultados
Acurácia obtida: 79.87%

Interface de terminal para realizar testes com novos pacientes.

Diagnóstico acompanhado de probabilidade estimada.
