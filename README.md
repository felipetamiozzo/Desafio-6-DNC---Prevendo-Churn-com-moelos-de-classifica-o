# Desafio-6-DNC---Prevendo-Churn-com-moelos-de-classifica-o
Utilizando modelos de classificação para prever possíveis usuários de streaming a deixarem a plataforma (churn).

# Desafio: Preveja os Usuários com Alta Chance de Deixar seu Streaming

Introdução
Este repositório contém um desafio de classificação para prever quais usuários têm maior chance de cancelar sua assinatura de uma plataforma de streaming. Compreender o perfil dos usuários que estão aumentando o churn é essencial para tomar ações que reduzam essas perdas.

# Contexto
Você trabalha em uma plataforma de streaming e a diretoria está preocupada com o alto índice de usuários cancelando suas assinaturas. Acredita-se que é possível prever se um usuário tem mais chance de deixar a plataforma antes que isso aconteça e, com base nessa informação, tomar ações para reduzir o churn. O objetivo é criar um modelo de classificação que seja capaz de prever se um usuário tem mais chance de cancelar sua assinatura na plataforma ou não.

# Base de Dados
Os dados fornecidos possuem informações sobre as contas dos clientes na plataforma de streaming, divididos entre contas Basic, Standard e Premium, onde cada uma oferece uma gama maior de serviços que a anterior. As colunas são:

client_id: Código de identificação do cliente

age: Idade do cliente

gender: Gênero do cliente

region: Região de origem do cliente

subscription_days: Dias de assinatura ativa do cliente

subscription_type: Tipo de conta

num_contents: Quantidade de conteúdos assistidos

avg_rating: Avaliação média dos conteúdos da plataforma

num_active_profiles: Número de perfis ativos na plataforma

num_streaming_services: Quantidade de serviços de streaming que o cliente possui

devices_connected: Quantidade de dispositivos conectados à conta

churned: Se o cliente cancelou a conta ou não

Etapas do Desafio
1. **Análise Exploratória dos Dados (Data Understanding)**
Carregando base de dados.

Realizando uma descrição estatística dos dados.

Verificandoos tipos de dados.

Verificando a quantidade de valores faltantes.

2. **Tratamento dos Dados (Data Preparation)**
Substitando os valores "NaN" por 0 em colunas específicas (Time_on_platform, Num_streaming_services, Churned, Avg_rating, Devices_connected).

Removendo as linhas nulas nas colunas Gender, Subscription_type e Age.

Transformando valores churned de 0 e 1 para No e Yes.

Convertendo valores float para int.

3. **Modelagem dos Dados - Regressão Logística**
Definindo variáveis X e y para o modelo.

Realizando o .fit do modelo.

Separando em train e test.

Realizando a modelagem.

Plotando a matriz de confusão.

Printando as métricas.

4. **Modelagem dos Dados - Tunning**
Realizando o tunning do modelo para melhorar a acurácia.

Utilizando técnicas de grid search ou similar para encontrar os melhores parâmetros.

5. **Modelagem dos Dados - Random Forest**
Realizando a montagem do grid search.

Realizando o .fit do modelo.

Realizando o tunning.

Realizando a modelagem.

Plotando a matriz de confusão.

Printando as métricas.





