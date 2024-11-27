

**Big Data**

Alan Victor Matos Cerqueira \- 01536516  
Amanda Gabriela Bernardo da Costa \- 01566793  
Breno Antônio Alexandrino da Silva \- 01280628  
Cibele Benício Lourenço \- 01535470  
Clóvis Vitor dos Santos Tavares \- 01564866  
Maria Christina Santos Barbosa \- 01565538

**Recife, Novembro de 2024**

## **Resumo Explicativo sobre Arquiteturas de Datawarehouse, Datalake e Datamesh**

## Introdução

Na era da informação, as organizações enfrentam o desafio de lidar com volumes cada vez maiores de dados, que provêm de diversas fontes e formatos. A crescente complexidade desses dados exige soluções eficazes para o seu armazenamento, processamento e análise, de modo a extrair valor estratégico e gerar insights. Para atender a essa demanda, surgiram arquiteturas como **Datawarehouse**, **Datalake** e **Datamesh**, cada uma oferecendo abordagens distintas para gerenciar e otimizar o uso de dados. Essas arquiteturas desempenham um papel fundamental em facilitar análises aprofundadas, permitindo que as empresas tomem decisões mais assertivas. Cada uma delas possui características, vantagens e especificidades únicas, e se adapta a diferentes necessidades organizacionais, atendendo desde cenários que exigem precisão e consistência até aqueles que necessitam de flexibilidade e escalabilidade. A escolha da arquitetura ideal depende do contexto e dos objetivos estratégicos de cada organização, permitindo que ela se ajuste de forma eficiente às suas particularidades.

## Data Warehouse 

O **Datawarehouse** é uma arquitetura estabelecida e amplamente confiável, desenvolvida especificamente para o armazenamento e gerenciamento de dados estruturados. Ele é amplamente adotado por organizações que necessitam de análises históricas detalhadas e relatórios precisos para embasar decisões estratégicas.

#### **Funcionamento e Estrutura:**

* Os dados são extraídos de diversas fontes, transformados para um formato padrão e carregados no repositório (processo **ETL**).  
* Utiliza esquemas rígidos e pré-definidos, como o modelo estrela ou floco de neve, para organizar informações em tabelas relacionadas.  
* Oferece suporte para ferramentas de **Business Intelligence (BI)**, permitindo análises consistentes e relatórios otimizados.

#### **Principais Características:**

* Armazena exclusivamente dados **estruturados** (como tabelas relacionais).  
* Designado para consultas rápidas e análises consolidadas.  
* Alta governança e segurança para dados sensíveis.

#### **Vantagens:**

* **Confiabilidade**: garante consistência, precisão e integridade nos dados armazenados.  
* **Consultas rápidas**: altamente eficiente para relatórios predefinidos e análises rotineiras.  
* **Adequação regulatória**: conformidade com normas como LGPD e GDPR.

#### **Limitações**:

* **Custo elevado**: devido à complexidade de implementação e infraestrutura necessária.  
* **Rigidez**: pouca flexibilidade para incorporar dados não estruturados ou novos formatos.  
* **Escalabilidade limitada**: menos eficiente para lidar com grandes volumes de dados dinâmicos.

#### **Aplicações Práticas**:

* Setores como **finanças**, **seguros** e **saúde** utilizam o Datawarehouse para análises baseadas em métricas precisas e dados consolidados.

## Data Lake

O **Datalake** é uma arquitetura versátil, criada para acomodar grandes volumes de dados em diversos formatos. Sua principal característica é a capacidade de armazenar os dados em seu estado original, possibilitando o processamento e análises avançadas conforme necessário.

#### **Funcionamento e Estrutura:**

* Armazena dados de diversas fontes diretamente no repositório, sem transformações prévias, utilizando o processo **ELT** (Extract, Load, Transform).  
* Aceita dados estruturados, semiestruturados e não estruturados (como arquivos CSV, imagens, vídeos, logs e JSON).  
* Geralmente é hospedado em plataformas de armazenamento escaláveis, como **Amazon S3**, **Azure Data Lake** ou **Google Cloud Storage**.

#### **Principais Características**:

* **Flexibilidade**: suporte para diferentes formatos de dados em um único local.  
* **Armazenamento bruto**: mantém dados sem organização inicial, permitindo múltiplas análises.  
* **Escalabilidade**: ideal para grandes volumes de dados.

#### **Vantagens**:

* **Economia**: custos menores em comparação ao Datawarehouse, especialmente em soluções baseadas em nuvem.  
* **Suporte avançado**: ideal para análises preditivas, machine learning e big data.  
* **Adaptação contínua**: pode incorporar novos tipos de dados sem reestruturação.

#### **Limitações:**

* **Governança complexa**: sem gestão adequada, pode se transformar em um *Data Swamp* (pântano de dados), dificultando a recuperação e análise.  
* **Consultas menos eficientes**: inadequado para relatórios tradicionais e análises rápidas.

#### **Aplicações Práticas:**

* Utilizado em setores como **tecnologia**, **streaming** e **e-commerce**, onde a diversidade e o volume de dados são altos.

## Data Mesh

O **Datamesh** é uma abordagem inovadora que transforma o gerenciamento de dados ao priorizar a descentralização e a autonomia das equipes. Essa solução é ideal para grandes organizações que demandam escalabilidade e uma colaboração eficiente entre diferentes domínios.

#### **Funcionamento e Estrutura:**

* Adota uma arquitetura **descentralizada**, onde cada domínio ou equipe é responsável por seus próprios dados, tratados como produtos.  
* Combina padrões de governança centralizada com execução local, garantindo consistência sem perder flexibilidade.  
* Baseia-se em quatro princípios: propriedade descentralizada, dados como produto, interoperabilidade por meio de padrões e uma plataforma de dados autoatendente.

#### **Principais Características:**

* **Arquitetura descentralizada**: distribuição da responsabilidade por dados entre equipes específicas.  
* **Foco na governança**: garante consistência e conformidade em ambientes descentralizados.  
* **Escalabilidade**: adequada para empresas multinacionais ou com múltiplos domínios de dados.

#### **Vantagens:**

* **Autonomia**: permite que as equipes gerenciem os dados conforme suas necessidades específicas.  
* **Escalabilidade elevada**: funciona bem em organizações complexas com grandes volumes de dados.  
* **Colaboração**: promove integração entre diferentes departamentos e funções.

#### **Limitações:**

* **Mudanças culturais**: exige adaptação organizacional para implementar a governança descentralizada.  
* **Padronização**: a falta de normas claras pode levar a inconsistências e duplicação de dados.

#### **Aplicações Práticas:**

* Empresas de grande porte, como **multinacionais de tecnologia**, **telecomunicações** e **bancos**, onde o compartilhamento de dados entre domínios é essencial.

## Comparando as Arquiteturas

## Conclusão

| Aspecto | Data Warehouse | Data Lake | Data Mesh |
| :---: | :---: | :---: | :---: |
| **Arquitetura** | Centralizada | Centralizada | Descentralizada |
| **Formato de Dados** | Estruturado | Qualquer formato | Focado no domínio |
| **Custos** | Altos | Baixos | Variável |
| **Escalabilidade** | Moderada | Alta | Muito alta |
| **Governança** | Alta | Baixa (se mal gerido) | Alta (quando bem implementado) |
| **Complexidade** | Baixa (bem definida) | Alta (exige gestão) | Alta (requer maturidade) |

Cada arquitetura apresenta vantagens e limitações que as tornam mais adequadas a diferentes cenários. O **Datawarehouse** é ideal para análises estruturadas e geração de relatórios consolidados; o **Datalake** destaca-se pela flexibilidade e capacidade de lidar com grandes volumes de dados em análises avançadas; já o **Datamesh** é ideal para organizações complexas, oferecendo escalabilidade e descentralização. Frequentemente, essas arquiteturas coexistem em ecossistemas híbridos, combinando suas características para atender a diversas demandas organizacionais. A escolha da solução ideal depende dos objetivos, desafios e contexto específico de cada empresa.