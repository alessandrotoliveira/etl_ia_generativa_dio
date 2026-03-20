# etl_ia_generativa_dio
Este projeto demonstra um pipeline ETL (Extract, Transform, Load) simples e eficaz que utiliza a API do Google Gemini para gerar mensagens de saúde personalizadas com base no Índice de Massa Corporal (IMC) dos usuários.

🚀 Objetivo
O script lê uma base de dados de clientes, calcula a categoria de saúde com base no IMC e utiliza IA generativa para criar recomendações motivacionais curtas e personalizadas para cada indivíduo.

🛠️ Tecnologias Utilizadas
Python 3.x

Pandas: Para manipulação e análise de dados.

Google Generative AI (Gemini API): Para a geração de conteúdo inteligente.

Google Colab: Ambiente de desenvolvimento (opcional).

📋 Estrutura do Projeto
etl_ia_generativa_dio.py: O script principal contendo a lógica de extração, transformação e integração com a IA.

clients.csv: Arquivo de dados de entrada contendo informações de usuários (ID, Nome, IMC).

⚙️ Como Funciona
Extração (Extract): O Pandas carrega os dados do arquivo clients.csv.

Transformação (Transform):

O código classifica o IMC em categorias (Baixo peso, Peso normal, Sobrepeso ou Obesidade).

Um prompt é enviado ao modelo gemini-1.5-flash para gerar uma dica de saúde de até 100 caracteres.

Carga (Load): O script percorre a lista de usuários e exibe/armazena as mensagens geradas pela IA.

🔧 Configuração e Uso
Chave da API: Você precisará de uma chave de API do Google Gemini. No Google Colab, ela deve ser armazenada nos "Secrets" com o nome gemini_api.
