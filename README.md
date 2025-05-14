# Recomenda-o-de-filmes-para-Usuarios-

🎬 Sistema de Recomendação de Filmes com KNN
Este projeto constrói um sistema de recomendação baseado em KNN (K-Nearest Neighbors) utilizando o famoso dataset MovieLens. É uma solução focada em aprendizado e aplicabilidade prática, ideal para demonstrar habilidades em Data Science com Python.

📌 Objetivo
Recomendar filmes personalizados para usuários com base em seus gostos e preferências, comparando suas avaliações com as de usuários semelhantes. Você aprenderá como:
* Estruturar dados com pandas.
* Explorar dados com seaborn e matplotlib.
* Implementar um modelo KNN de recomendação do zero.
* Entender a lógica de recomendação baseada em usuários.

🧠 Tecnologias e Bibliotecas
* Python (3.8+)
* pandas, numpy
* matplotlib, seaborn – para visualização
* scikit-learn – para modelo KNN (NearestNeighbors)
* collections.Counter – contagem de gêneros

📊 Análise Exploratória (EDA)
Realizamos uma análise visual e descritiva:
* Quantidade de usuários, filmes e avaliações.
* Distribuição das notas.
* Gêneros mais populares.
* Filmes mais avaliados.
* Correlações e tendências com seaborn.

🧩 Modelo de Recomendação
Utilizamos o algoritmo User-Based KNN:
1. Criei uma matriz de usuários × filmes.
2. Preenchemos os valores ausentes com 0 (ausência de nota).
3. Treinamos o KNN para encontrar usuários semelhantes.
4. Recomendamos filmes que os vizinhos avaliaram bem, mas que o usuário ainda não viu.
O modelo é não supervisionado, pois não há rótulos a prever — apenas agrupamento e comparação de similaridades.

🧪 Exemplo de Uso
python
CopiarEditar
# Recomendar filmes para o usuário de ID 1
recomendados = recomendar_filmes(user_id=1)
for titulo, nota in recomendados:
    print(f"{titulo} (nota média: {nota})")

📂 Arquivos do Projeto
* movies.csv – catálogo de filmes
* ratings.csv – avaliações dos usuários
* recomendador_knn.py – código principal com EDA e sistema de recomendação
* README.md – explicações e instruções

🚀 Como Rodar
1. Clone o repositório
bash
CopiarEditar
git clone https://github.com/seu-usuario/nome-do-repo.git
cd nome-do-repo
2. Instale as dependências
bash
CopiarEditar
pip install -r requirements.txt
3. Execute o notebook ou script .py

🧑‍💻 Autor
Guilherme, Cientista de Dados Jr. Formado em Engenharia da Computação | Pós em Engenharia de Machine Learning Apaixonado por IA, Recomendação e Análise de Dados 📊
