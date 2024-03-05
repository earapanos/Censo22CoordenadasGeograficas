
<h1 align="center"> 🗺 Coordenadas Geográficas do Censo IBGE 2022 - Dashboard</h1>

Nessa dashboard você vai poder visualizar os dados das coordenadas geográficas de domicílios. Estes dados foram divulgados pelo Instituto Brasileiro de Geografia e Estatística - IBGE e fazem parte do levantamento realizado pelo Censo demográfico e socioecomômico realizado em 2022.

O objetivo dessa dashboard foi utilizar os dados de coordenadas geográficas disponibilizadas para domicílios e estabelecimentos do IBGE para se analisar espacialmente e geograficamente a sua distribuição nos municípios do Acre, Brasil.

Para que a dashboard pudesse ser construída, foi elaborado um processo de ETL para a normalização dos dados e para que se pudessem ser correlacionadas estas informações com outras tabelas no Banco de Dados Relacional. Com isso foi possível de se obter uma tabela com os nomes dos municípios do estado do Acre e as coordenadas dos domicílios, o que permitiu a representação destas junto ao Looker Studio.

Nas tabelas originais você vai encontrar as seguintes variáveis:

**COD_UF (NUMERIC)** = Variável numérica com o código da unidade federativa;

**COD_MUN (NUMERIC)** = Variável numérica com o código do município;

**COD_ESPECIE (VARCHAR)** = Variável alfanumérica com a categoria e descrição da espécie do endereço e que podem ser:

    1=Domicílio particular
  
    2=Domicílio coletivo
  
    3=Estabelecimento agropecuário
  
    4=Estabelecimento de ensino
  
    5=Estabelecimento de saúde
  
    6=Estabelecimento de outras finalidades
  
    7=Edificação em construção
  
    8=Estabelecimento religioso
  
**LATITUDE** =  Variávem com a Latitude da Coordenada de Localização da Espécie do Endereço;

**LONGITUDE** = Variávem com a Longitude da Coordenada de Localização da Espécie do Endereço;

**NV_GEO_COORD** = Variável com o nível de geocodificação do domicílio ou estabelecimento que podem ser:

    1=Endereço - coordenada original do Censo 2022
  
    2=Endereço - coordenada modificada (apartamentos em um mesmo número no logradouro*)
  
    3=Endereço - coordenada estimada (endereços originalmente sem coordenadas ou coordenadas inválidas**)
  
    4=Face de quadra
  
    5=Localidade
  
    6=Setor censitário

<h3>Data source</h3>

<a href="https://www.ibge.gov.br/estatisticas/sociais/populacao/38734-cadastro-nacional-de-enderecos-para-fins-estatisticos.html?edicao=38891&t=resultados">Todos os dados de domicílios disponibilizados pelo IBGE podem ser acessados aqui!</a>
<a href="https://lookerstudio.google.com/reporting/29cb3a4c-5ab0-4275-b254-ff0b83562033" target="_blank" rel="noreferrer"> <img src="https://github.com/earapanos/Censo22CoordenadasGeograficas/assets/52800638/5919327f-9538-4a53-9a41-304388f35175" alt="dashboard"> </a> 




