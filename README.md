# BusinessCase
Projeto para a disciplina ECM514-Ciência de Dados

## Análise de Dados de Acidentes em Cidades Americanas

## Integrantes
##### Caio Rabinovich Panes Brunholi	RA: 20.01285-3
##### Felippe Onishi Yaegashi		RA: 20.00255-6
##### Carolina Perez 				RA: 20.00968-2
##### Guilherme Lins Banzato		RA: 20.01561-5

</br>

# Dados Escolhidos
## Nova Iorque

- Detalhes do Evento de Colisão: A tabela de colisões de veículos motorizados contém detalhes sobre o evento de colisão. Cada linha representa um evento de colisão.

- Fonte de Dados: As tabelas de dados de colisões de veículos motorizados incluem informações de todas as colisões de veículos motorizados relatadas pela polícia em Nova York.

- Requisitos para o Relatório de Colisão: O relatório policial (MV104-AN) é obrigatório para colisões onde há feridos ou mortos, ou danos de pelo menos $1000.

- Natureza Preliminar dos Dados: Os dados são preliminares e podem ser alterados quando os formulários MV-104AN são modificados com base em detalhes revisados do acidente.

- Fontes de Estatísticas Atualizadas: Para estatísticas de tráfego mais precisas e atualizadas, deve-se consultar a página de Colisões de Veículos Motorizados do NYPD (atualizada semanalmente) ou Vision Zero View (atualizado mensalmente).


>The Motor Vehicle Collisions crash table contains details on the crash event. Each row represents a crash event. The Motor Vehicle Collisions data tables contain information from all police reported motor vehicle collisions in NYC. The police report (MV104-AN) is required to be filled out for collisions where someone is injured or killed, or where there is at least $1000 worth of damage (https://www.nhtsa.gov/sites/nhtsa.dot.gov/files/documents/ny_overlay_mv-104an_rev05_2004.pdf). It should be noted that the data is preliminary and subject to change when the MV-104AN forms are amended based on revised crash details.For the most accurate, up to date statistics on traffic fatalities, please refer to the NYPD Motor Vehicle Collisions page (updated weekly) or Vision Zero View (updated monthly).

> Due to success of the CompStat program, NYPD began to ask how to apply the CompStat principles to other problems. Other than homicides, the fatal incidents with which police have the most contact with the public are fatal traffic collisions. Therefore in April 1998, the Department implemented TrafficStat, which uses the CompStat model to work towards improving traffic safety. Police officers complete form MV-104AN for all vehicle collisions. The MV-104AN is a New York State form that has all of the details of a traffic collision. Before implementing Trafficstat, there was no uniform traffic safety data collection procedure for all of the NYPD precincts. Therefore, the Police Department implemented the Traffic Accident Management System (TAMS) in July 1999 in order to collect traffic data in a uniform method across the City. TAMS required the precincts manually enter a few selected MV-104AN fields to collect very basic intersection traffic crash statistics which included the number of accidents, injuries and fatalities. As the years progressed, there grew a need for additional traffic data so that more detailed analyses could be conducted. The Citywide traffic safety initiative, Vision Zero started in the year 2014. Vision Zero further emphasized the need for the collection of more traffic data in order to work towards the Vision Zero goal, which is to eliminate traffic fatalities. Therefore, the Department in March 2016 replaced the TAMS with the new Finest Online Records Management System (FORMS). FORMS enables the police officers to electronically, using a Department cellphone or computer, enter all of the MV-104AN data fields and stores all of the MV-104AN data fields in the Department’s crime data warehouse. Since all of the MV-104AN data fields are now stored for each traffic collision, detailed traffic safety analyses can be conducted as applicable.

</br>

## Chicago
- Jurisdição e Fonte de Dados: Os dados de acidentes abrangem apenas as ruas dentro dos limites da cidade de Chicago e sob a jurisdição do Departamento de Polícia de Chicago (CPD). São provenientes do sistema eletrônico de relatórios de acidentes (E-Crash).

- Exclusão de Informações: Os dados excluem qualquer informação pessoal identificável.

- Atualização dos Dados: Os registros são adicionados ao portal de dados quando um relatório de acidente é finalizado ou alterado no E-Crash.

- Disponibilidade dos Dados: Os dados do E-Crash estão disponíveis para alguns distritos policiais desde 2015, mas os dados de toda a cidade só estão disponíveis a partir de setembro de 2017.

- Método de Relato: Cerca de metade dos relatórios de acidentes são auto-relatados pelos motoristas envolvidos nas delegacias locais, e a outra metade é registrada no local do acidente por policiais.

- Registro de Informações: Os parâmetros dos acidentes, como condições da rua, condições meteorológicas e limites de velocidade, são registrados pelos policiais com base nas melhores informações disponíveis naquele momento.

- Possibilidade de Correção: Se informações novas ou atualizadas sobre um acidente forem recebidas, o relatório pode ser alterado posteriormente pelo policial.

- Exclusões no Conjunto de Dados: Acidentes em rodovias interestaduais, rampas de freeways e estradas locais na fronteira da cidade, onde o CPD não é a agência que responde, são excluídos do conjunto de dados.

- Formato de Registro dos Acidentes: Os acidentes são registrados conforme o formato especificado no Relatório de Acidente de Trânsito, SR1050, do Departamento de Transportes de Illinois.

- Critérios de Relatório de Acidentes em Illinois: Acidentes com dano à propriedade de US$ 1.500 ou mais, ou envolvendo lesão corporal, e que acontecem em uma via pública envolvendo pelo menos um veículo em movimento, são considerados acidentes passíveis de relatório, exceto incidentes de "bike dooring".

- Registro Completo de Acidentes pelo CPD: O CPD registra todos os acidentes de trânsito relatados, independentemente do prazo de prescrição, o que significa que o conjunto de dados oficial de acidentes de Chicago pode não incluir todos os acidentes listados.

>Crash data shows information about each traffic crash on city streets within the City of Chicago limits and under the jurisdiction of Chicago Police Department (CPD). Data are shown as is from the electronic crash reporting system (E-Crash) at CPD, excluding any personally identifiable information. Records are added to the data portal when a crash report is finalized or when amendments are made to an existing report in E-Crash. Data from E-Crash are available for some police districts in 2015, but citywide data are not available until September 2017. About half of all crash reports, mostly minor crashes, are self-reported at the police district by the driver(s) involved and the other half are recorded at the scene by the police officer responding to the crash. Many of the crash parameters, including street condition data, weather condition, and posted speed limits, are recorded by the reporting officer based on best available information at the time, but many of these may disagree with posted information or other assessments on road conditions. If any new or updated information on a crash is received, the reporting officer may amend the crash report at a later time. A traffic crash within the city limits for which CPD is not the responding police agency, typically crashes on interstate highways, freeway ramps, and on local roads along the City boundary, are excluded from this dataset.

>All crashes are recorded as per the format specified in the Traffic Crash Report, SR1050, of the Illinois Department of Transportation. The crash data published on the Chicago data portal mostly follows the data elements in SR1050 form. The current version of the SR1050 instructions manual with detailed information on each data elements is available here.

>As per Illinois statute, only crashes with a property damage value of $1,500 or more or involving bodily injury to any person(s) and that happen on a public roadway and that involve at least one moving vehicle, except bike dooring, are considered reportable crashes. However, CPD records every reported traffic crash event, regardless of the statute of limitations, and hence any formal Chicago crash dataset released by Illinois Department of Transportation may not include all the crashes listed here.


</br>

# Business Understanding

## Determinação de Objetivos
### Background
- Em Chicago temos 1 acidente a cada 5 à 6 minutos
- Em Nova Iorque temos 1 acidente a cada 2 à 3 minutos
- Taxa de mortalidade nos Estados Unidos é de 16 para cada 100 mil motoristas

### Objetivos
- Analisar as regiões com maior número de acidentes
- Relação entre o tipo de veículo e número de acidentes
- Relação entre período do ano ou hora com maior tendência à acidentes
- Correlação entre variáveis para entender causas comuns de acidentes

### Critério de sucesso
- Clareza dos resultados
- Identificação clara de padrões
- Correlações estatísticas significativas

</br>
## Avaliação de Situação
### Recursos
- Engenheiros de Computação para realizar a análise
- Datasets com dados coletados por agências governamentais
- Ambiente de trabalho Google
- Python e suas bibliotecas

### Necessidades
- Dados inteligíveis, completos e manipuláveis
- Ambiente de trabalho compatível com a grandeza dos dados
- Colaboradores capacitados

### Limitações
- Tempo disponível para análise
- Dados limitados aos publicados pelas agências governamentais

### Riscos
- Dados insuficientes para gerar conclusões e análises válidas
- Dados incorretos ou enviesados

### Contingências
- Tratamento de dados
- Uso de mais de um dataset

### Custos
- Horas dos colaboradores
- Possíveis custos com plataforma em nuvem
- Custos energéticos

### Benefícios
- Conclusões sobre os principais causadores de acidentes
- Propor soluções para combater acidentes

</br>

## Objetivos do Data Mining
### Objetivos
- Filtrar dados úteis para a análise
- Estabelecer relações entre variáveis
- Determinar correlações entre categorias de dados

### Critério de Sucesso
- Criar um dataset reduzido a partir dos dados originais
- Criar relações mensuráveis
- Gerar insights

</br>

## Planejamento do Projeto
### Plano de Ação
- Seguir a metodología CRISP-DM

### Avaliação inicial
- Diversos dados faltantes
- Inconsistência na descrição dos acidentes
- Dados entre os anos de 2012 e 2024
- Somente dados reportados à polícia

### Ferramentas
- Google Colaboratory
- Bibliotecas Python: Pandas, Matplotlib, NumPy, Seaborn, TensorFlow,
- PyTorch
- GitHub


