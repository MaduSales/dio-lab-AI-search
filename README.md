# dio-lab-AI-search

Neste penúltimo desafio da DIO sobre Azure IA Fundamentals, exploramos mais acerca de Document Intelligence e Mineração de Conhecimentos utilizando a ferramenta AI Search para indexação e consulta de Dados. Assim, aqui vai um passo a passo de como fazer essa indexação para enriquecimento da Inteligência Artificial:

## Link que usei: 
[Documentação Oficial da IA Search](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html)


## 📑 1º Passo: Criando um Azure AI Search resource
No Portal da Azure, precisamos selecionar o botão de "criar recurso", procurar pela opção <i>Azure AI Search</i> e crie esse recurso seguindo as instruções recomendadas pela documentação. Após a conclusão da instalção, usaremos esse recurso para usará enriquecer os dados no armazenamento de dados com insights (palavras-chave) gerados por IA.
<br>
<br>

## 📩 2º Passo: Criando um Azure AI services resource
Retorne para a homepage, lique em "criar recurso" novamente e selecione a opção <i>Azure AI services</i>. Configure o recurso de acordo com a documentação oficial.
<br>
<br>

## 🗂️ 3º Passo: Criando uma Storage Account
Como uma Storage Account funciona como um armazenamento, volta até a homepage e selecione novamente "criar recurso", pesquise por <i>Storage account</i> e configure seguindo o passo a passo da documentação. Após a criação, vá no menu ao lado e no painel, escolhe "configurações" para ativar a função <i>Allow Blob anonymous access</i>.
<br>
<br>

## 📋 4º Passo: Inserindo documentos no Azure Storage
Ainda na página do Storage Account, no menu ao lado, selecione "Contêineres" e então "Criar", siga as orientações do documento oficial. Agora, para subirmos uma fonte de dados no Storage, precisamos baixar o arquivo zip sobre resenhas de Cafés que o próprio Azure deixa disponível na documentação oficial: [](https://aka.ms/mslearn-coffee-reviews). Após extrair todos os arquivos do zip, faça upload deles no contêiner que havia sido criado anteriormente.
<br>
<br>

## 🖥️ 5º Passo: Indexando os documentos
Depois de ter os arquivos no Storage, podemos utilizar a tecnologia do Azure AI Search para extrair insights (palavras-chave) dos documentos. O portal do Azure oferece um assistente de Importação de dados para que crie automaticamente um índice e um indexador para fontes de dados com suporte. Dessa forma, criamos um índice para importar aqueles documentos que estavam no Storage para o índice do Azure AI Search, e assim é possível fazer buscas com as palavras-chave desejadas para saber qual foi o retorno sobre determinados insights.
