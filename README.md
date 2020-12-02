# central-pesquisas-2020
![](https://github.com/Nexo-Dados/central-pesquisas-2020/blob/main/nexo.png) 
Banco de dados de pesquisas utilizado pelo Nexo Jornal na central de pesquisas das eleições municipais de 2020


## Sobre

Neste repositório, o **Nexo** disponibiliza os dados utilizados na central de pesquisas das eleições municipais de 2020, para a prefeitura das capitais brasileiras. Os dados foram coletados diariamente pela equipe de Gráficos do jornal.

As publicações originais podem ser acessadas aqui:

* [Central de pesquisas 1º turno](https://www.nexojornal.com.br/interativo/2020/10/23/Central-de-Pesquisas-2020-a-corrida-pelo-comando-de-capitais)
* [Central de pesquisas 2º turno](https://www.nexojornal.com.br/interativo/2020/11/24/Central-de-Pesquisas-2020-a-disputa-do-2%C2%BA-turno-nas-capitais)

## Estrutura das tabelas

Os arquivos do primeiro e segundo turno estão separados. Ambos são um arquivo .csv, com padrão americano de separação, utilizando vírgulas. Os arquivos possuem as mesmas variáveis.

* UF: sigla do estado da capital.
* CIDADE: nome da capital.
* COD_IBGE: código de 7 dígitos, identificador único das cidades.
* TURNO: identificação de primeiro ou segundo turno.
* CANDIDATURA: nome da candidata ou do candidato. Os nomes divergem do nome de urna. Todos têm no máximo 14 caracteres.
* PARTIDO: sigla do partido.
* DATA: data final em que a pesquisa foi coletada.
* PERCENTUAL: percentual **arredondado** das intenções de voto. Caso o valor original tivesse 5 na primeira casa decimal, o percentual foi arredondado para cima.
* INSTITUTO: instituto de pesquisa que realizou a coleta.
* REGISTRO_TSE: registro oficial da pesquisa. Existe apenas uma pesquisa Datafolha com reigstro duplicado, mas com datas diferentes.
* AMOSTRA: número de pessoas entrevistadas.

Consideração importante: os dados do primeiro turno referem-se aos votos totais, incluíndo brancos, nulos e indecisos. Essa categoria é agregada como "Brancos/nulos/indecisos" e o partido está como missing. Já os dados do segundo turno, são apenas os votos válidos, excluindo essa categoria. Essa decisão foi tomada pois nem todos os institutos estavam divulgando os votos totais.

Os dados do segundo turno foram coletados a partir do dia 15 de novembro. Pesquisas de intenção de voto com cenários hipotéticos de segundo turno foram desconsideradas.

## Dúvidas ou inconsistências

Em caso de dúvidas ou inconsistências nos dados, você pode abrir uma "issue" no GitHub ou entrar em contato pelo e-mail infografia@nexojornal.com.br

## Política de uso dos dados

O uso dos dados é livre, desde que o **Nexo** seja citado como fonte intermediária dos dados. 

Os dados originais são dos institutos de pesquisa e foram coletados a partir de diversas fontes na imprensa e de releases dos próprios institutos. 
























