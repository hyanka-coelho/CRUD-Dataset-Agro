O Ministério da Agricultura e Pecuária (Mapa) é responsável pela gestão das políticas públicas de estímulo à agropecuária, 
pelo fomento do agronegócio e pela regulação e normatização de serviços vinculados ao setor.
O dataset escolhido abrange Relação de Produtores Orgânicos de todo o Brasil e de países que exportam para o Brasil.

O dataset abrange:
Tipo de entidade - Organismos de avaliação da conformidade orgânica
Entidade - O nome das entidades
País - país de origem do produto
UF - Permite selecionar a unidade da federação
Cidade - Cidade de origem do produtor
Situação cnpo - informe se o produtor está ativo
CNPF, CNPJ - Identificação do produtor
Escopo - Permite selecionar o escopo do produtor
Atividades - Tipo de Atividade
Contato - Informação de contato

Para construir a modelagem foi realizado a separação dessas informações em 3 tabelas diferentes: entidades, produtor e localidade.
Assim é possível navegar entre as tabelas com o id incremental, criado para relacionar as mesmas.
No código sql é possível observar a criação das tabelas, sua relação e depois a inserção dos dados para preencher as informações,
no final tem a consulta relacionada aos dados onde é capturado os produtores e suas entidades que estão no Brasil e apresentam o cnpj ativo.

site oficial da base de dados: https://dados.agricultura.gov.br/sv/dataset/cadastro-nacional-de-produtores-organicos