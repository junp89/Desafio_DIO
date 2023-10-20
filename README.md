## Explorando IA Generativa em um Pipeline de ETL com Python

### Desafio 

#### Contexto: Você é um cientista de dados no Santander e recebeu a tarefa de envolver seus clientes de maneira mais personalizada. Seu objetivo é usar o poder da IA Generativa para criar mensagens de marketing personalizadas que serão entregues a cada cliente.

- Seu trabalho é consumir o endpoint GET https://sdw-2023-prd.up.railway.app/users/{id} (API da Santander Dev Week 2023) para obter os dados de cada cliente.
- Depois de obter os dados dos clientes, você vai usar a API do ChatGPT (OpenAI) para gerar uma mensagem de marketing personalizada para cada cliente. Essa mensagem deve enfatizar a importância dos investimentos.
- Uma vez que a mensagem para cada cliente esteja pronta, você vai enviar essas informações de volta para a API, atualizando a lista de "news" de cada usuário usando o endpoint PUT https://sdw-2023-prd.up.railway.app/users/{id}.

### Resolução

A solução do desafio foi feita no Google Colab [https://github.com/junp89/Desafio_DIO_Explorando-IA-Generativa-em-um-Pipeline-de-ETL-com-Python/blob/main/Desafio_de_Projeto_Santander_Bootcamp_2023_Ci%C3%AAncia_de_Dados_com_Python.ipynb].

Como alternativa ao Chat GPT-4, explorei a API do Google Bard. No entanto, encontrei desafios relacionados à chave da API e às respostas não diretas do Bard, o que dificultou o envio dessas informações de volta para a seção "news" dos usuários. Experimentei também o Hugging Face, mas as frases geradas não foram assertivas. Finalmente, consegui utilizar com sucesso a versão 3.5 do Chat GPT.





