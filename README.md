# LAB_DIO_Inteligenciadedocumentos
Laboratório feito no Azure para aprender sobre Inteligência de Documentos e Mineração de Conhecimentos.

Para configurar uma pesquisa, assim como seus insights, é necessário:

-Criar um recurso de IA (Azure AI Services para automação), criar recurso de busca (AI Search) e uma Storage Account (armazenamentos dos dados em que vamos fazer a busca).

-Após criar todos os recursos, devemos mudar as regras de segurança da Storage Account para permitir o acesso anônimo de blob. Após isso, devemos criar um container que vai armazenar os documentos da nossa pesquisa.

-Após criar o container permitindo  o "anonymous read access for containers and blobs", fazemos o upload dos dados que vamos utilizar.

-Depois de armazenar os documentos, podemos usar o Azure AI Search para extrair insights dos documentos usando o assistente de importação de dados (Criar um indexador).

- Com este assistente, você pode criar automaticamente um índice e um indexador para fontes de dados suportadas.

-No Azure AI Search, na página Visão geral , importamos os dados.

-Depois, preenchemos o que é pedido, como: Fonte de dados, Nome da fonte de dados, Dados a extrair, Modo de análise, Cadeia de conexão (aqui nos conectamos ao nosso container, onde armazenamos nossos dados anteriormente), etc.

-Após isso, vamos adicionar as habilidades cognitivas.

- Primeiro, selecionamos o recurso que criamos para a IA.

- Depois, adicionamos os enriquecimentos. Neles adicionamos os campos que nos interessam (Por exemplo: palavras chave, localizações e sentimentos).

- Após isso, criamos o indexador.

- Tendo o indexador criado e configurado, podemos testar o mecanismo de pesquisa no "Search".

Exemplo de Json:

{
 "search": "sentiment:'negative'",
 "count": true
}

É importante ressaltar que esse tipo de ferramenta pode ajudar em muitos tipos de negócios. Por exemplo, você como dono de um negócio pode ver onde pode melhorar de acordo com os reviews negativos dos clientes. Outro exemplo são as investigações, afinal você não precisaria mais ler um documento inteiro, tendo em vista que você pode pesquisar só os insights do documento.










  

  

  
