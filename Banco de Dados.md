Conceitos Fundamentais de Banco de Dados
Um Banco de Dados (BD) é um sistema organizado para coletar, armazenar e gerenciar dados, facilitando sua consulta, manipulação e análise. O Sistema Gerenciador de Banco de Dados (SGBD) é o software que permite essa gestão, controlando o acesso, a segurança e a integridade dos dados.

Características Essenciais e Funções de um SGBD
Independência dos Dados: Crucial para o Cebraspe. Refere-se à capacidade de alterar o esquema (estrutura) físico ou lógico do banco de dados sem que as aplicações que o utilizam precisem ser modificadas.
Independência Física: Mudanças na forma como os dados são armazenados fisicamente (ex: tipo de disco, organização de arquivos) não afetam a visão lógica ou as aplicações.
Independência Lógica: Mudanças na estrutura lógica (ex: adicionar uma coluna a uma tabela) têm impacto mínimo ou nulo nas aplicações existentes.
Controle de Concorrência: Gerencia o acesso simultâneo aos dados por múltiplos usuários, evitando conflitos e garantindo a consistência. Métodos comuns incluem travas (locks) e timestamping (estampa de tempo).
Segurança de Dados: Protege as informações através de controle de autenticação (verificar quem é), autorização (o que pode fazer), permissões e criptografia (dado em repouso e em trânsito).
Backup e Recuperação: Permite a criação de cópias de segurança (backups) e a restauração (recovery) dos dados em caso de falhas (hardware, software, erro humano). Técnicas como journals (logs de transação) são vitais para a recuperação.
Integridade dos Dados: Garante que os dados sejam consistentes, válidos e não sejam corrompidos, aplicando regras e restrições.
Integridade de Entidade: Garante que a chave primária de uma tabela não contenha valores nulos e seja única.
Integridade Referencial: Garante que qualquer valor de chave estrangeira seja nulo ou corresponda a um valor de chave primária válido na tabela referenciada. Evita "registros órfãos".
Integridade de Domínio: Garante que os valores de uma coluna estejam dentro de um conjunto predefinido de valores ou sigam um formato específico (ex: um campo idade não pode ser negativo).
Suporte a Transações (Propriedades ACID): Um dos tópicos mais cobrados! Garante que as operações em um banco de dados sejam confiáveis.
Atomicidade (Atomicity): Uma transação é tratada como uma única unidade indivisível. Ou todas as suas operações são concluídas com sucesso (commit), ou nenhuma delas é (rollback).
Consistência (Consistency): Uma transação leva o banco de dados de um estado válido para outro estado válido. Ela não viola as regras de integridade.
Isolamento (Isolation): Múltiplas transações concorrentes são executadas de forma isolada umas das outras, como se estivessem ocorrendo sequencialmente. Evita problemas como leituras sujas, leituras não repetíveis e leituras fantasmas.
Durabilidade (Durability): Uma vez que uma transação é confirmada (commit), suas alterações são permanentes e persistem mesmo em caso de falhas subsequentes do sistema.
Concorrência e Seus Problemas Comuns
É comum o Cebraspe cobrar problemas de concorrência:

Problema de Atualização Perdida (Lost Update): Duas transações tentam atualizar o mesmo dado, e a atualização de uma delas é sobrescrita pela outra, sem ser aplicada.
Leitura Suja (Dirty Read): Uma transação lê dados que foram modificados por outra transação, mas que ainda não foram confirmados (commit). Se a segunda transação fizer rollback, a primeira leu um dado que nunca existiu de fato.
Leitura Não Repetível (Non-Repeatable Read): Uma transação lê o mesmo dado duas vezes e obtém valores diferentes porque outra transação modificou (e confirmou) o dado entre as duas leituras.
Leitura Fantasma (Phantom Read): Uma transação executa uma consulta que retorna um conjunto de linhas. Posteriormente, a mesma consulta é executada e retorna um número diferente de linhas porque outra transação inseriu ou excluiu linhas que satisfazem a condição da consulta.
Modelagem de Dados
A modelagem de dados é o processo de estruturar os dados para que sejam facilmente armazenados e acessados.

Modelos de Dados
Modelo Conceitual (Entidade-Relacionamento - ER):
Foco em entidades (objetos de interesse, ex: Cliente, Produto), atributos (características das entidades, ex: nome, preço) e relacionamentos (associações entre entidades, ex: Cliente FAZ Pedido).
Representação gráfica usando diagramas ER.
Conceitos-chave: Cardinalidade (1:1, 1:N, N:N) e Opcionalidade (participação mínima).
Modelo Lógico: Transforma o modelo conceitual em estruturas detalhadas para um tipo específico de banco de dados (geralmente relacional), independente do SGBD.
Define tabelas, colunas (atributos), chaves primárias e estrangeiras, e restrições de integridade.
Modelo Físico: Implementação concreta do modelo lógico em um SGBD específico.
Define tipos de dados específicos do SGBD, índices, esquemas de armazenamento, partições, etc.
Abordagem Relacional (mais cobrado)
O modelo relacional organiza os dados em tabelas inter-relacionadas, compostas por linhas (registros ou tuplas) e colunas (atributos).

Chaves:
Chave Primária (PK): Um ou mais atributos que identificam unicamente cada registro em uma tabela. Não pode ter valor nulo e deve ser única.
Chave Estrangeira (FK): Um atributo (ou conjunto de atributos) em uma tabela que referencia a chave primária de outra tabela, estabelecendo um relacionamento. Garante a integridade referencial.
Chave Candidata: Qualquer atributo ou conjunto de atributos que possa ser uma chave primária (única e não nula). A PK é uma das chaves candidatas escolhida.
Chave Composta: Uma chave primária ou candidata formada por dois ou mais atributos.
Relacionamentos (Cardinalidade):
1:1 (Um para Um): Uma ocorrência de uma entidade se relaciona com apenas uma ocorrência de outra entidade. Raro, mas pode ser usado para dividir tabelas muito grandes ou representar subtipos.
1:N (Um para Muitos): Uma ocorrência da primeira entidade se relaciona com múltiplas ocorrências da segunda entidade. A chave estrangeira vai para o lado "N". (Ex: Um Cliente pode ter Vários Pedidos; Pedido tem uma FK para Cliente).
N:N (Muitos para Muitos): Múltiplas ocorrências de uma entidade se relacionam com múltiplas ocorrências de outra. Requer a criação de uma tabela associativa (ou de ligação/junção/intersecção) que contém as chaves primárias das duas tabelas originais como chaves estrangeiras. (Ex: Muitos Alunos podem cursar Muitas Disciplinas; Tabela "Matrícula" associa Aluno e Disciplina).
SQL (Structured Query Language)
É a linguagem padrão para consultar e manipular dados em bancos de dados relacionais.

DDL (Data Definition Language): Usada para definir ou modificar a estrutura do banco de dados.
CREATE TABLE, ALTER TABLE, DROP TABLE, CREATE INDEX, DROP INDEX, CREATE VIEW, DROP VIEW.
DML (Data Manipulation Language): Usada para manipular os dados dentro das tabelas.
SELECT (consultar), INSERT (inserir), UPDATE (modificar), DELETE (remover).
DCL (Data Control Language): Usada para controlar permissões de acesso aos dados.
GRANT (conceder permissões), REVOKE (revogar permissões).
TCL (Transaction Control Language): Usada para gerenciar transações.
COMMIT (confirmar transação), ROLLBACK (desfazer transação), SAVEPOINT (definir ponto de retorno).
Normalização e Desnormalização (muito cobrado!)
Normalização: Processo de organizar os dados em tabelas para eliminar redundâncias e garantir a integridade dos dados, reduzindo anomalias de inserção, atualização e exclusão. As Formas Normais (FN) são regras que guiam esse processo.
Nível	Objetivo	Requisitos (estar na FN anterior)	Problema Eliminado
1FN (Primeira Forma Normal)	Eliminar grupos repetitivos e garantir atomicidade dos atributos.	Todos os atributos devem conter valores atômicos (indivisíveis). Não deve haver colunas multivaloradas ou compostas complexas.	Redundância básica, dados complexos em uma célula.
2FN (Segunda Forma Normal)	Eliminar dependências parciais.	Estar na 1FN. Todos os atributos não-chave devem depender da chave primária inteira (e não apenas de parte dela, se for chave composta).	Dependência parcial da chave primária composta.
3FN (Terceira Forma Normal)	Eliminar dependências transitivas.	Estar na 2FN. Atributos não-chave não devem depender de outros atributos não-chave (ou seja, evitar dependência transitiva).	Redundância por dependência transitiva. Ex: Se Cidade depende de CEP, e CEP não é PK, Cidade está transitivamente dependente.
BCNF (Forma Normal de Boyce-Codd)	Versão mais rigorosa da 3FN, para casos especiais onde há múltiplas chaves candidatas sobrepostas.	Estar na 3FN. Toda dependência funcional não trivial deve ser de uma superchave (qualquer chave que unicamente identifica uma tupla).	Problemas raros de redundância e anomalias que a 3FN não resolve.

Exportar para as Planilhas
Desnormalização: Processo oposto, onde tabelas são combinadas ou dados são duplicados (controladamente) para melhorar o desempenho de consultas, especialmente em sistemas que exigem alta performance de leitura (ex: Data Warehouses). Introduce redundância planejada.
Modelos Não Relacionais (NoSQL) - Cobrado em contexto de Big Data
Abordagens alternativas para armazenamento, para lidar com grandes volumes de dados, alta escalabilidade e esquemas flexíveis. Priorizam disponibilidade e tolerância a partição (segundo o teorema CAP) em detrimento da consistência estrita (muitas vezes, com consistência eventual em vez de ACID completo).

Teorema CAP (Brewer's Theorem): Um sistema distribuído de dados pode garantir no máximo dois dos três requisitos:

Consistência (Consistency): Todos os nós têm os mesmos dados no mesmo momento.
Disponibilidade (Availability): O sistema está sempre operacional e responde a cada solicitação.
Tolerância à Partição (Partition Tolerance): O sistema continua operando mesmo se houver falha na comunicação entre partes do sistema (partições de rede).
Bancos NoSQL geralmente escolhem AP ou CP, enquanto bancos relacionais ACID tendem a ser CA (sem tolerância à partição em sua forma pura distribuída).
Tipos Comuns de NoSQL:

Chave-Valor (Key-Value): Redis, DynamoDB. Simples, rápido para leitura/escrita.
Documentos (Document-Oriented): MongoDB, Couchbase. Armazenam dados em documentos flexíveis (JSON, BSON, XML). Ideal para dados com estrutura variável.
Colunar (Column-Family): Cassandra, HBase. Otimizados para agregações e grandes volumes de dados que podem ser lidos em blocos de colunas.
Grafos (Graph): Neo4j, Amazon Neptune. Representam dados como nós e arestas, ideais para dados com muitas relações complexas.
Modelo Multidimensional (muito cobrado em BI)
Organiza dados em cubos de dados para análise.

Dimensões: Categorias pelas quais os dados podem ser analisados (ex: Tempo, Local, Produto, Cliente). São os eixos do cubo.
Medidas/Fatos: Valores numéricos que são objeto de análise (ex: Vendas, Lucro, Quantidade). São os valores dentro do cubo.
Operações OLAP:
Slice: Selecionar uma única dimensão para análise.
Dice: Selecionar um subconjunto de dados em múltiplas dimensões.
Drill-down: Navegar para um nível mais detalhado (ex: de Ano para Mês).
Roll-up: Navegar para um nível mais agregado (ex: de Mês para Ano).
Pivot/Rotate: Reorientar a visualização do cubo.
Sistemas de Gerenciamento de Banco de Dados (SGBD) - Comparativo
Reforçando os pontos que o Cebraspe valoriza:

Característica	PostgreSQL	MySQL	Oracle Database	H2 Database
Licença	Open Source (Licença PostgreSQL)	Open Source (GPL, com Enterprise Edition proprietária)	Proprietário (Alto custo)	Open Source (Licença MPL 2.0 ou EPL 1.0)
Tipo	Relacional Objeto-Relacional (suporta recursos de OO)	Relacional (Puro)	Relacional Objeto-Relacional	Relacional (Puro)
Uso Ideal	Data Warehousing, GIS (PostGIS), complexidade, integridade de dados rigorosa, pesquisa.	Aplicações Web (LAMP/LEMP stack), alta velocidade de leitura simples, blogs, e-commerce.	Missão crítica, grandes volumes de transações (OLTP), alta disponibilidade, segurança governamental/bancária.	Testes unitários/integração, caches, aplicações embarcadas Java, prototipagem.
Suporte a Tipos Complexos	Extensa (JSONB, XML, arrays, tipos geométricos/GIS com PostGIS). Permite criar tipos customizados.	Básico (JSON limitado, sem XML nativo robusto).	Extensa (JSON, XML, geoespacial, multimídia). Tipos de dados proprietários avançados.	Básico (tipos SQL padrão).
Confiabilidade e Conformidade ACID	Alta, rigoroso em ACID, excelente para transações complexas.	Alta (com InnoDB), mas menos rigoroso em alguns aspectos de Isolamento padrão que PostgreSQL.	Extremamente alta, padrão ouro em ACID, robustez para falhas.	Alta para seu propósito (garante ACID), mas não para produção em larga escala.
Escalabilidade	Horizontal (replicação, sharding), Vertical (hardware). Excelente para escrita e complexidade.	Horizontal (replicação master-slave, sharding com MySQL Cluster). Excelente para leitura.	Horizontal (RAC - Real Application Clusters, Sharding), Vertical. Desempenho otimizado em escala.	Limitada ao ambiente de uso (desenvolvimento/testes).
Comunidade/Suporte	Ativa comunidade Open Source, vários provedores comerciais.	Enorme comunidade Open Source, suporte Oracle.	Suporte técnico Oracle de alto nível.	Boa comunidade para desenvolvimento Java.
Recursos Avançados	MVCC (Controle de Concorrência Multiversão), Triggers, Views, Funções, Stored Procedures, Particionamento, Federação.	Triggers, Views, Funções, Stored Procedures, Federação.	RAC, Data Guard, Active Data Guard, Flashback, Partitioning, Advanced Security.	Modo Servidor, Modo Embutido, Modo In-Memory, persistência em disco.

Exportar para as Planilhas
Modos do H2 Database (Relevante para contexto de desenvolvimento)
Modo In-Memory: O banco de dados reside na memória RAM. Os dados não são persistidos após a execução/reinicialização. Ideal para testes rápidos, caches e cenários onde a persistência não é necessária.
Modo Persistente: O banco de dados é persistido em disco (em um arquivo .mv.db ou H2 no diretório do usuário ou em um local especificado). Garante que os dados não sejam perdidos após o encerramento da aplicação.
Macete para o Cebraspe:

PostgreSQL é banco PRO (Profissional/Robusto/Completo): Pense em PostgreSQL para Projetos complexos, Parcialmente Objeto-Relacional, Padrões SQL avançados, Parceria com GIS (PostGIS).
H2 é banco TESTE (Leve/Desenvolvimento): Lembre-se de H2 para Homologação, Hardware leve, Habilidoso para testes e desenvolvimento.
Business Intelligence (BI) e Análise de Dados
BI é o processo de transformar dados brutos em informações úteis e acionáveis para apoiar a tomada de decisões estratégicas.

Data Lake:
Armazenamento de Dados Brutos: Recebe dados em seu formato original, sem esquema predefinido (schema-on-read).
Flexibilidade: Ideal para Big Data e dados não estruturados (logs, redes sociais, sensores).
Baixo Custo: Geralmente usa armazenamento de baixo custo (HDFS, S3).
Exploração: Ótimo para cientistas de dados e analistas que precisam explorar dados sem restrições.
Data Warehouse (DW):
Dados Estruturados e Históricos: Armazena dados limpos, transformados e estruturados, otimizados para consultas analíticas e relatórios complexos.
Orientado a Assunto: Organizado por temas de negócios (vendas, clientes).
Integrado: Dados de múltiplas fontes são consolidados.
Não Volátil: Uma vez carregados, os dados não são alterados, apenas adicionados.
Esquema Predefinido (Schema-on-write): Os dados são transformados para se encaixar em um esquema predefinido antes de serem armazenados. Modelagem em estrela ou floco de neve.
Data Mart:
Um pequeno Data Warehouse, focado em um setor específico ou departamento. Contém um subconjunto de dados do DW.
Vantagens: Mais rápido para análises focadas, menor custo, mais fácil de construir.
Pode ser dependente (alimentado pelo DW principal) ou independente (alimentado diretamente por fontes de dados).
ETL (Extract, Transform, Load): Processo crucial no BI.
Extract (Extrair): Captura dados de diversas fontes (relacionais, planilhas, sistemas legados, APIs, etc.).
Transform (Transformar): Fase mais crítica e complexa. Limpa, padroniza, valida, agrega, desduplica e aplica regras de negócio aos dados. Garante a qualidade e a consistência.
Load (Carregar): Insere os dados transformados no destino final (DW, Data Mart, Data Lake). Pode ser carga total ou incremental.
ELT (Extract, Load, Transform): Variação onde os dados brutos são primeiro carregados para o destino (geralmente um Data Lake) e a transformação ocorre depois, no próprio ambiente de destino. Comum em Big Data.
OLAP (Online Analytical Processing):
Ferramentas e técnicas para consultas rápidas e interativas em cubos de dados (modelo multidimensional).
Permite análises complexas, agregadas e drill-down/roll-up.
Contrasta com OLTP (Online Transaction Processing), que foca em operações transacionais de pequena escala e alta frequência.
Data Mining:
Descoberta de Conhecimento: Processo de extrair padrões, tendências ocultas, correlações e insights valiosos de grandes conjuntos de dados, usando algoritmos de ML, estatística e IA.
Técnicas Comuns: Classificação, Clusterização (agrupamento), Regressão, Regras de Associação.
Data Mesh:
Arquitetura Descentralizada: Foco na propriedade de dados por domínio e na autonomia das equipes.
Dados tratados como produtos de dados, servidos via APIs, com governança federada.
Contraste com arquiteturas monolíticas de DW/Data Lake centralizados.
Ciência de Dados e Inteligência Artificial (IA)
A Ciência de Dados usa métodos científicos, algoritmos e sistemas para extrair insights e conhecimento a partir dos dados.

Machine Learning (ML)
Campo da IA que permite que sistemas aprendam com os dados, sem programação explícita.

Tipos de Aprendizado (reforçando):
Supervisionado: Classificação (ex: spam/não-spam, diagnóstico de doença) e Regressão (ex: previsão de preço de imóvel, temperatura). Requer dados com rótulos (saídas corretas).
Não Supervisionado: Clusterização/Agrupamento (ex: segmentação de clientes, detecção de anomalias), Redução de Dimensionalidade (ex: PCA). Não requer rótulos, busca padrões intrínsecos.
Semissupervisionado: Combina pequenas quantidades de dados rotulados com grandes quantidades de dados não rotulados.
Por Reforço: Agentes aprendem por tentativa e erro em um ambiente dinâmico, recebendo recompensas ou penalidades. (ex: jogos, robótica).
Por Transferência: Reutiliza um modelo pré-treinado (em uma tarefa similar) para acelerar o aprendizado em uma nova tarefa, reduzindo a necessidade de grandes volumes de dados.
Deep Learning (Aprendizado Profundo) - Ênfase em Redes Neurais
Subcampo do ML que utiliza Redes Neurais Profundas (com muitas camadas ocultas) para aprender representações hierárquicas de dados complexos.

Redes Neurais (NN):
Neurônios Artificiais: Unidades de processamento que recebem entradas, aplicam pesos, somam e passam por uma função de ativação (ex: ReLU, Sigmoid, Tanh) para produzir uma saída.
Camadas:
Entrada: Recebe dados brutos.
Ocultas: Realizam a maior parte do processamento, extraindo características complexas. O "profundo" do Deep Learning vem da quantidade de camadas ocultas.
Saída: Produz o resultado final.
Pesos e Bias: Parâmetros que a rede ajusta durante o treinamento para otimizar suas previsões.
Treinamento:
Feedforward: Os dados fluem da entrada para a saída.
Erro: O erro entre a saída prevista e a real é calculado (função de custo/perda).
Retropropagação (Backpropagation): Algoritmo que calcula o gradiente do erro em relação aos pesos e bias.
Gradiente Descendente (e variações como Adam, SGD): Otimizador que ajusta os pesos e bias na direção que minimiza o erro.
Tipos de Redes Neurais Mais Comuns em Provas:
Perceptron: A rede neural mais simples, para classificação binária linearmente separável.
Redes Neurais Convolucionais (CNNs): Especializadas em processamento de imagens e vídeos. Usam camadas convolucionais (filtros) para detectar padrões espaciais, pooling para reduzir dimensionalidade. (ex: reconhecimento facial, diagnóstico por imagem).
Redes Neurais Recorrentes (RNNs): Especializadas em dados sequenciais (texto, séries temporais, áudio). Possuem "memória" que permite que informações de passos anteriores influenciem os atuais. Sofrem com o problema do gradiente evanescente/explosivo.
LSTMs (Long Short-Term Memory) e GRUs (Gated Recurrent Units): Variações avançadas de RNNs que resolvem os problemas de memória de longo prazo das RNNs tradicionais, sendo muito usadas em NLP.
Transformers: Arquitetura dominante em NLP e IA Generativa. Baseiam-se em mecanismos de atenção (self-attention) que permitem processar sequências em paralelo e capturar dependências de longo alcance de forma mais eficiente que RNNs/LSTMs. São a base dos LLMs.
GANs (Generative Adversarial Networks): Duas redes (Gerador e Discriminador) competem: o Gerador cria dados sintéticos, o Discriminador tenta diferenciar dados reais dos gerados. Usadas para criar imagens, áudios, vídeos realistas.
Modelos de Linguagem e IA Generativa
Processamento de Linguagem Natural (NLP): Área que permite aos computadores entender, interpretar e gerar linguagem humana.
Tarefas Comuns: Classificação de texto, análise de sentimento, tradução automática, sumarização, chatbots.
Grandes Modelos de Linguagem (LLMs): Modelos de IA massivamente treinados em texto.
Capacidades: Compreensão de linguagem natural, geração de texto coerente, tradução, sumarização, resposta a perguntas.
Exemplos: GPT (OpenAI), PaLM (Google), Llama (Meta).
IA Generativa: Cria novos conteúdos (texto, imagens, vídeo, código) a partir de padrões aprendidos.
Técnicas Essenciais:
Fine-tuning (Ajuste Fino): Adaptação de um modelo pré-treinado (em uma tarefa geral) para uma tarefa mais específica usando um conjunto de dados menor e mais direcionado.
RLHF (Reinforcement Learning from Human Feedback): Uso de feedback humano (avaliações) para refinar o comportamento de modelos generativos, alinhando suas saídas com as preferências humanas.
Avaliação de Modelos e Técnicas de Ajuste (muito importante!)
Matriz de Confusão: Ferramenta fundamental para avaliar o desempenho de modelos de classificação.
Verdadeiro Positivo (VP): Real = Positivo, Previsto = Positivo. (Acerto)
Falso Positivo (FP): Real = Negativo, Previsto = Positivo. Erro Tipo I (falso alarme).
Verdadeiro Negativo (VN): Real = Negativo, Previsto = Negativo. (Acerto)
Falso Negativo (FN): Real = Positivo, Previsto = Negativo. Erro Tipo II (perda de detecção).
Métricas de Desempenho (cobrança frequente):
Acurácia: (VP + VN) / (VP + FP + VN + FN). Proporção de previsões corretas. Pode ser enganosa em classes desbalanceadas.
Precisão (Precision): VP / (VP + FP). Dos que o modelo previu como positivos, quantos são realmente positivos. Importante quando o custo de um FP é alto.
Recall (Sensibilidade ou Cobertura): VP / (VP + FN). Dos que são realmente positivos, quantos o modelo identificou corretamente. Importante quando o custo de um FN é alto.
F1-Score: 2 * (Precisão * Recall) / (Precisão + Recall). Média harmônica, útil quando há desbalanceamento de classes e você busca um equilíbrio entre Precisão e Recall.
Especificidade: VN / (VN + FP). Dos que são realmente negativos, quantos o modelo identificou corretamente.
Árvores de Decisão: Modelo interpretável, mas propenso a overfitting.
Critérios de Divisão:
Gini Impurity (para classificação): Mede a probabilidade de um elemento ser classificado incorretamente se escolhido aleatoriamente. Quanto menor, mais pura a partição.
Entropia (para classificação): Mede a desordem ou incerteza. Quanto menor, mais puro.
MSE (Mean Squared Error para regressão): Mede o erro médio quadrático.
Técnicas de Poda (Pruning): Usadas para combater overfitting em árvores de decisão, removendo ramos que não contribuem significativamente para a generalização.
Overfitting (Sobreajuste): O modelo "memoriza" os dados de treinamento (incluindo ruídos), performando bem no treino, mas muito mal em dados novos/não vistos.
Soluções:
Mais Dados de Treino: Aumentar a quantidade e diversidade dos dados.
Regularização (L1 - Lasso, L2 - Ridge): Adiciona uma penalidade à função de custo para manter os pesos pequenos, evitando que o modelo se ajuste demais aos dados.
Dropout (em Redes Neurais): Desliga aleatoriamente alguns neurônios durante o treinamento para evitar coadaptação.
Poda (Pruning) de Árvores: Remover nós redundantes.
Validação Cruzada: Para ter uma estimativa mais confiável do desempenho.
Underfitting (Subajuste): O modelo é muito simples e não consegue capturar os padrões essenciais dos dados, performando mal tanto no treinamento quanto em dados novos.
Soluções:
Aumentar Complexidade do Modelo: Usar um modelo mais sofisticado (ex: mais camadas em uma NN).
Adicionar Mais Features: Incluir variáveis mais relevantes.
Reduzir Regularização.
Validação Cruzada: Técnica para avaliar o desempenho do modelo de forma mais robusta e evitar que o resultado dependa de uma única divisão de dados.
Holdout: A divisão mais simples (ex: 80% treino, 20% teste). A métrica de desempenho é menos confiável pois depende da partição.
K-Fold Cross-Validation: Divide os dados em K "dobras". O modelo é treinado K vezes, usando K-1 dobras para treinamento e 1 dobra para teste em cada iteração. A média dos K resultados dá uma estimativa mais robusta.
Leave-One-Out (LOO): Caso extremo de K-Fold onde K é igual ao número de amostras (cada amostra é um conjunto de teste uma vez). Computacionalmente caro para grandes datasets.
Big Data
Os 3 V's (mais cobrado):
Volume: Grande quantidade de dados (petabytes, exabytes).
Velocidade: Taxa de geração e processamento dos dados (streaming de dados, IoT).
Variedade: Diversidade de tipos e formatos de dados (estruturados, semi-estruturados, não estruturados).
Outros V's (menos cobrados, mas podem aparecer): Veracidade (confiança nos dados), Valor (capacidade de gerar insights).
Tecnologias Comuns: Hadoop, Spark, Kafka.
Qualidade de Dados: Fundamental para que as análises de Big Data sejam úteis.
Características: Precisão, Completude, Consistência, Atualidade, Validade, Unicidade.
Governança de TI e Legislação do CNJ
A governança de TI garante que a tecnologia da informação apoie os objetivos de negócio de uma organização, com foco em gestão de riscos, segurança e eficiência.

Frameworks e Modelos de Governança de TI (Cebraspe adora!)
TOGAF (The Open Group Architecture Framework): Framework de arquitetura corporativa.
Objetivo: Alinhar a TI com os objetivos de negócio, fornecendo uma abordagem sistemática para planejar, projetar, implementar e governar a arquitetura de informação corporativa.
Domínios de Arquitetura:
Arquitetura de Negócios: Estratégias, organização, processos de negócio.
Arquitetura de Dados: Estrutura de dados lógicos e físicos, gerenciamento de dados.
Arquitetura de Aplicações: Sistemas de informação e suas interações.
Arquitetura de Tecnologia: Infraestrutura de TI (hardware, software, redes).
COBIT (Control Objectives for Information and Related Technologies): Framework de governança e gestão de TI.
Foco: Fornecer um modelo de referência para a governança e gestão de TI, definindo objetivos de controle e processos para atingi-los.
Princípios: Atender às necessidades das partes interessadas, Cobrir o empreendimento de ponta a ponta, Aplicar um framework único integrado, Possibilitar uma abordagem holística, Separar a governança da gestão.
ITIL (Information Technology Infrastructure Library): Framework de melhores práticas para gestão de serviços de TI.
Foco: Gerenciamento de serviços de TI ao longo de todo o ciclo de vida (estratégia, desenho, transição, operação e melhoria contínua de serviço).
BPM (Business Process Management - Gerenciamento de Processos de Negócio - CBOK):
Ciclo de Vida: Modelagem (desenhar os processos), Execução (implementar), Monitoramento (acompanhar desempenho), Otimização (melhorar continuamente).
Legislação do CNJ (Essencial para a prova!)
O Cebraspe costuma cobrar não apenas o objetivo geral, mas também detalhes específicos e a numeração das normativas.

Resolução CNJ nº 335/2020 - Plataforma Digital do Poder Judiciário (PDPJ):
Objetivo Principal: Instituir a PDPJ para aprimorar o acesso à Justiça, a tramitação de processos e a transparência. Foco na interoperabilidade e integração dos sistemas eletrônicos do Judiciário.
Princípios: Publicidade, eficiência, transparência, segurança, interoperabilidade.
Conceitos-Chave: Integração de sistemas, tramitação eletrônica, comunicação entre tribunais, acesso de cidadãos e operadores de direito.
Portaria CNJ nº 252/2020 - Governança de TI no Judiciário:
Foco: Fortalecer a governança de TI, padronizar procedimentos, e melhorar a gestão de recursos de TI.
Estrutura de Governança: Estabelece papéis como Comitê de Governança de TI e Unidades Gestoras de TI.
Diretrizes: Segurança da Informação, Integração de Sistemas, Desenvolvimento de Sistemas (boas práticas), Adoção de Soluções Inovadoras (cloud, big data), Planejamento Estratégico de TI, Metodologias Ágeis (incentivo), Avaliação de Resultados, Indicadores de Desempenho, Auditorias.
Portaria CNJ nº 253/2020 - Regras de Segurança e Gestão de Dados Sensíveis:
Foco: Regula a gestão e segurança da informação, com ênfase em dados sensíveis (conforme LGPD).
Importância: Criptografia, controle de acesso rigoroso, auditorias de segurança, planos de contingência, tratamento de incidentes.
Resolução CNJ nº 522/2023 - Diretrizes de TI para Governança e Segurança:
Atualiza e complementa normativas anteriores.
Foco: Governança de TI, Gestão de Riscos (com base em ISO 31000 e NIST SP 800-30), Segurança da Informação (controle de acessos, proteção de dados, segurança cibernética).
Processo de Gestão de Riscos (fases): Comunicação e Consulta → Contextualização → Identificação → Análise → Tratamento → Monitoramento → Retroalimentação. (Cuidado com a ordem!)
Portaria CNJ nº 131/2021 - Digitalização dos Processos:
Estabelece padrões técnicos para a digitalização e a implantação de tecnologias para processos judiciais.
Resolução CNJ nº 396/2021 - Segurança e Controle de TI em Infraestruturas:
Normas para processamento de dados e segurança cibernética nas infraestruturas de TI. Foco em diretrizes de segurança e protocolos de monitoramento.
Portaria CNJ nº 162/2021 - Regras para Gestão de Contratos de TI:
Diretrizes para transparência e controle na contratação de serviços e produtos de TI. Abrange desde a fase de planejamento até a fiscalização da execução contratual.
PDPJ (Plataforma Digital do Poder Judiciário)
Objetivos Centrais: Integração (chave!), Facilitação de Acesso, Otimização de Tramitação, Segurança.
Funcionalidades: Consulta Processual, Envio/Recebimento de Documentos, Acompanhamento de Audiências (telepresenciais), Integração entre Tribunais, Assinatura Digital (validade jurídica).
Benefícios: Agilidade, Redução de Custos, Acesso Facilitado, Segurança Jurídica, Transparência.
Funcionamento: Sistema Centralizado e Interligado (interoperabilidade), Interfaces de Acesso, Integração com Outros Sistemas.

Um Banco de Dados (BD) é um sistema organizado para coletar, armazenar e gerenciar dados, facilitando sua consulta, manipulação e análise. O Sistema Gerenciador de Banco de Dados (SGBD) é o software que permite essa gestão, controlando o acesso, a segurança e a integridade dos dados.

Características de um SGBD
Independência dos Dados: Permite que as aplicações se conectem ao banco de dados sem se preocupar com a sua estrutura interna.
Controle de Concorrência: Gerencia o acesso simultâneo aos dados por múltiplos usuários, evitando conflitos e garantindo a consistência.
Segurança de Dados: Protege as informações através de controle de autenticação, autorização, permissões e criptografia.
Backup e Recuperação: Permite a criação de cópias de segurança e a recuperação dos dados em caso de falhas.
Integridade dos Dados: Garante que os dados sejam consistentes, válidos e não sejam corrompidos, aplicando regras e restrições.
Suporte a Transações (ACID): Garante que as operações sejam Atômicas (tudo ou nada), Consistentes (mantêm a integridade do BD), Isoladas (não interferem em outras transações) e Duráveis (persistentes mesmo após falhas).
Modelagem de Dados
A modelagem de dados é o processo de estruturar os dados para que sejam facilmente armazenados e acessados.

Modelos de Dados
Modelo Conceitual (Entidade-Relacionamento - ER): É um esboço inicial e gráfico que descreve a estrutura do banco de dados, focando em objetos ou conceitos (Entidades), suas propriedades (Atributos) e as associações entre eles (Relacionamentos).
Modelo Lógico: Transforma o modelo conceitual em estruturas mais detalhadas, geralmente normalizadas, independentes do SGBD específico. Para o modelo relacional, define as tabelas, colunas e chaves.
Modelo Físico: É a implementação concreta do modelo lógico em um SGBD específico, considerando aspectos como tipos de dados, índices e estruturas de armazenamento.
Abordagem Relacional
O modelo relacional organiza os dados em tabelas inter-relacionadas, compostas por linhas (registros ou tuplas) e colunas (atributos).

Tabelas: Estruturas que contêm os dados.
Chaves Primárias (PK): Um ou mais atributos que identificam unicamente cada registro em uma tabela. Pode ser simples (um atributo) ou composta (dois ou mais atributos).
Chaves Estrangeiras (FK): Um atributo (ou conjunto de atributos) em uma tabela que referencia a chave primária de outra tabela, estabelecendo um relacionamento.
Relacionamento 1:1 (Um para Um): Uma ocorrência de uma entidade se relaciona com apenas uma ocorrência de outra entidade. Pode levar à fusão de tabelas.
Relacionamento 1:N (Um para Muitos): Uma ocorrência da primeira entidade se relaciona com múltiplas ocorrências da segunda entidade. A chave estrangeira vai para o lado "N".
Relacionamento N:N (Muitos para Muitos): Múltiplas ocorrências de uma entidade se relacionam com múltiplas ocorrências de outra. Requer a criação de uma tabela associativa (ou tabela de ligação) que contém as chaves primárias das duas tabelas originais como chaves estrangeiras.
SQL (Structured Query Language)
É a linguagem padrão para consultar e manipular dados em bancos de dados relacionais.

DDL (Data Definition Language): Usada para criar, alterar e apagar objetos no banco de dados (ex: CREATE TABLE, ALTER TABLE, DROP TABLE).
DML (Data Manipulation Language): Usada para consultar e modificar os dados dentro das tabelas (ex: SELECT, INSERT, UPDATE, DELETE).
Normalização e Desnormalização
Normalização: É o processo de organizar os dados em tabelas para eliminar redundâncias e garantir a integridade dos dados, reduzindo anomalias de inserção, atualização e exclusão. As Formas Normais (FN) são regras que guiam esse processo:
Nível	Objetivo	Requisitos	Problema Eliminado
0FN (Não normalizado)	Organizar dados ainda brutos, sem estrutura.	Dados podem conter grupos repetitivos e informações redundantes.	Nenhum problema resolvido ainda.
1FN	Eliminar grupos repetitivos e garantir atomicidade.	Todos os atributos devem conter valores atômicos (indivisíveis). Eliminar colunas multivaloradas ou compostas.	Redundância básica e repetição de grupos.
2FN	Eliminar dependências parciais.	Estar na 1FN. Todos os atributos não-chave devem depender da chave primária inteira (e não de parte dela).	Dependência parcial da chave.
3FN	Eliminar dependências transitivas.	Estar na 2FN. Atributos não-chave não devem depender de outros atributos não-chave (evitar dependência transitiva).	Redundância por dependência transitiva.
BCNF (Forma Normal de Boyce-Codd)	Versão mais rigorosa da 3FN, para casos específicos de dependências complexas.	Estar na 3FN. Toda dependência funcional é de uma superchave.	Problemas raros não resolvidos pela 3FN.

Exportar para as Planilhas
Desnormalização: É o processo oposto à normalização, onde tabelas são combinadas ou dados são duplicados para melhorar o desempenho de consultas, especialmente em sistemas que exigem alta performance de leitura, como Data Warehouses. Pode introduzir redundância.
Modelos Não Relacionais (NoSQL)
São abordagens alternativas para o armazenamento de dados, projetadas para lidar com grandes volumes de dados (Big Data) e alta escalabilidade, com esquemas mais flexíveis. Priorizam desempenho e escalabilidade em detrimento da consistência rigorosa (muitas vezes, com consistência eventual em vez de ACID completo).

Chave-Valor: Armazena dados como pares de chave e valor (ex: Redis).
Documentos (JSON): Armazena dados em estruturas flexíveis baseadas em documentos, geralmente JSON (ex: MongoDB).
Grafos: Representa dados como nós (entidades) e arestas (relacionamentos) (ex: Neo4j).
Colunar: Armazena dados em colunas em vez de linhas, otimizado para agregações e consultas analíticas (ex: Cassandra).
Modelo Multidimensional
Organiza dados em dimensões e medidas, formando uma estrutura de cubo de dados. É amplamente utilizado em Data Warehouses e análises de Business Intelligence (BI) para análises rápidas e consultas agregadas.

Dimensões: Categorias pelas quais os dados podem ser analisados (ex: tempo, localização, produto).
Medidas: Valores numéricos que são objeto de análise (ex: vendas, lucro, quantidade).
Sistemas de Gerenciamento de Banco de Dados (SGBD) - Comparativo
Característica	PostgreSQL	MySQL	Oracle Database	H2 Database
Licença	Open Source	Open Source	Proprietário	Open Source
Tipo	Relacional (avançado)	Relacional (rápido e fácil)	Relacional (robusto e poderoso)	Relacional (leve)
Uso Ideal	Consultas complexas, desenvolvimento de aplicações	Web, leituras simples, aplicações pequenas/médias	Grandes empresas, alta performance e escalabilidade	Testes, desenvolvimento local, aplicações embarcadas
Suporte a Tipos Complexos	Extensa (JSON, XML, geoespacial, etc.)	Limitado	Extensa (inclusive geoespacial)	Básico
Suporte a Transações	Completo (ACID)	Completo (ACID)	Completo (ACID)	Completo (ACID)
Escalabilidade	Alta (Replicação, Particionamento)	Alta (Replicação)	Alta (Replicação)	Limitada (mais para ambientes controlados)
Performance em Consultas	Muito boa em consultas complexas	Boa em leituras simples	Excelente em transações grandes	Boa para seu propósito (desenvolvimento/testes)
Recursos Avançados	Funções extras, consultas recursivas, índices personalizados	Boa para uso geral, comunidade grande	Segurança, backup/recuperação, clusterização	Modos In-Memory e Persistente
Custo	Gratuito	Gratuito (com opções pagas de suporte)	Alto (licenciamento pago)	Gratuito

Exportar para as Planilhas
Modos do H2 Database
Modo In-Memory: O banco de dados reside na memória RAM. Os dados não são persistidos após a execução, sendo ideal para testes rápidos ou caches.
Modo Persistente: O banco de dados é persistido em disco no diretório do usuário ou em um local especificado, garantindo que os dados não sejam perdidos após o encerramento da aplicação.
Macete para o Cebraspe:

PostgreSQL é banco PRO: Considerado um SGBD relacional mais completo e avançado, com funcionalidades robustas para projetos complexos.
H2 é banco TESTE: Ideal para ambientes de desenvolvimento e teste devido à sua leveza e facilidade de uso, especialmente no modo em memória.
Business Intelligence (BI) e Análise de Dados
BI é o processo de transformar dados brutos em informações úteis e acionáveis para apoiar a tomada de decisões estratégicas.

Data Lake: Um grande repositório que armazena dados brutos, não estruturados ou semi-estruturados, em seu formato original. Flexível para diversas análises futuras.
Data Warehouse (DW): Um armazém de dados centralizado e organizado, otimizado para consultas e relatórios complexos. Armazena dados históricos de múltiplas fontes, após passarem por um processo de transformação.
Data Mart: Um pequeno Data Warehouse, focado em um setor específico ou departamento da organização. Contém um subconjunto de dados do DW, otimizado para análises mais rápidas e específicas. Pode ser dependente (alimentado pelo DW principal) ou independente (alimentado diretamente por fontes de dados).
ETL (Extract, Transform, Load): Processo fundamental na construção de Data Warehouses e Data Marts.
Extract (Extrair): Captura dados de diversas fontes (bancos de dados, planilhas, sistemas legados, etc.).
Transform (Transformar): Trata, limpa, filtra, valida e estrutura os dados conforme as regras de negócio e os requisitos do destino. Envolve padronização, agregação e deduplicação.
Load (Carregar): Insere os dados transformados no repositório final (Data Warehouse ou Data Mart). Pode ser feito em lotes periódicos ou em tempo real (streaming).
OLAP (Online Analytical Processing): Ferramentas e técnicas que permitem consultas rápidas e interativas para análises multidimensionais complexas em Data Warehouses.
Data Mining: Processo de extrair padrões, tendências ocultas e insights valiosos de grandes conjuntos de dados, usando algoritmos de Machine Learning e estatística.
Data Mesh: Abordagem descentralizada para a arquitetura de dados, onde a propriedade e a gestão dos dados são distribuídas entre diferentes equipes, promovendo autonomia e escalabilidade.
Ciência de Dados e Inteligência Artificial (IA)
A Ciência de Dados usa métodos científicos, algoritmos e sistemas para extrair insights e conhecimento a partir dos dados.

Machine Learning (ML)
Campo da IA que permite que sistemas aprendam com os dados, sem programação explícita.

Tipos de Aprendizado:
Supervisionado: Modelos são treinados com dados que contêm rótulos (respostas conhecidas), buscando aprender um mapeamento de entrada para saída (ex: classificação, regressão).
Não Supervisionado: Modelos buscam encontrar padrões ou estruturas em dados sem rótulos (respostas conhecidas), como agrupamento (clustering) ou redução de dimensionalidade.
Semissupervisionado: Mistura dados rotulados e não rotulados para o treinamento, aproveitando o volume de dados não rotulados.
Por Reforço: Agentes aprendem a tomar decisões em um ambiente para maximizar uma recompensa acumulada, por meio de tentativa e erro (similar a um jogo).
Por Transferência: Reutiliza um modelo pré-treinado em uma tarefa para uma nova tarefa relacionada, aproveitando o conhecimento adquirido.
Deep Learning (Aprendizado Profundo)
É um subcampo do Machine Learning que utiliza Redes Neurais Profundas para aprender com dados complexos. Simula a estrutura do cérebro, usando múltiplas camadas de neurônios artificiais para processar informações e reconhecer padrões mais avançados.

Redes Neurais: Consistem em camadas de nós (ou neurônios) que processam informações. Cada nó recebe entradas, calcula e transmite saídas para os próximos.
Componentes:
Neurônios Artificiais: Funções matemáticas que recebem entradas, aplicam pesos, somam e ativam uma saída.
Camadas:
Camada de Entrada (Input Layer): Recebe os dados brutos. Cada neurônio representa uma característica do dado.
Camadas Ocultas (Hidden Layers): Onde ocorre o processamento principal dos dados. Em Deep Learning, existem várias camadas ocultas.
Camada de Saída (Output Layer): Fornece o resultado final da rede (valor contínuo para regressão, classe para classificação, etc.).
Pesos e Bias: Parâmetros ajustáveis durante o treinamento que influenciam a força das conexões entre os neurônios e o limite de ativação.
Treinamento (Aprendizado): Ajusta os pesos e bias da rede para reduzir o erro entre as previsões e os valores reais. O algoritmo de retropropagação (backpropagation) é comumente usado, juntamente com o gradiente descendente, para otimizar esses parâmetros.
Tipos de Redes Neurais:
Perceptron: Rede neural simples para classificação binária.
Redes Neurais Convolucionais (CNN): Especializadas em processamento de imagens, utilizando filtros para detectar padrões.
Redes Neurais Recorrentes (RNN): Possuem feedback entre as camadas, permitindo processar sequências temporais (texto, séries temporais) e "lembrar" informações passadas.
Redes Neurais de Longo Curto Prazo (LSTM): Tipo avançado de RNN que resolve o problema do desvanecimento do gradiente, permitindo que a rede lembre de dependências de longo prazo em sequências.
Redes Generativas Adversariais (GAN): Duas redes (gerador e discriminador) competem entre si para gerar dados realistas e aprender a distingui-los de dados reais.
Modelos de Linguagem e IA Generativa
Processamento de Linguagem Natural (NLP): Campo da IA focado em permitir que computadores entendam, interpretem e gerem linguagem humana.
Grandes Modelos de Linguagem (LLM): Modelos de IA (baseados em redes neurais como Transformers) treinados em enormes volumes de texto, capazes de entender e gerar texto de forma natural para tarefas como tradução, resumo e criação de conteúdo.
IA Generativa: Tipo de IA que cria novos conteúdos (texto, imagens, áudio, código) a partir dos dados aprendidos. Baseiam-se em redes neurais profundas e frequentemente utilizam técnicas como ajuste fino (fine-tuning) com dados específicos e Aprendizado por Reforço com Feedback Humano (RLHF) para melhorar a qualidade das gerações.
Avaliação de Modelos e Técnicas de Ajuste
Matriz de Confusão: Ferramenta para avaliar o desempenho de modelos de classificação. Compara os resultados previstos com os resultados reais.
Termos para classificação binária:
Verdadeiro Positivo (VP): Previu positivo, e o real é positivo.
Falso Positivo (FP): Previu positivo, mas o real é negativo (Erro Tipo I).
Verdadeiro Negativo (VN): Previu negativo, e o real é negativo.
Falso Negativo (FN): Previu negativo, mas o real é positivo (Erro Tipo II).
Métricas de Desempenho (derivadas da matriz de confusão):
Acurácia: Proporção de previsões corretas sobre o total de previsões.
Precisão (Positive Predictive Value): Dos classificados como positivos, quantos são realmente positivos (VP / (VP + FP)).
Recall (Sensibilidade): Dos realmente positivos, quantos foram corretamente identificados (VP / (VP + FN)).
F1-Score: Média harmônica entre Precisão e Recall, útil quando há desbalanceamento de classes.
Árvores de Decisão: Estrutura hierárquica para classificação ou regressão, que divide os dados em subconjuntos com base em atributos.
Critérios de divisão: Gini (classificação), Entropia (classificação), MSE (regressão).
Vantagens: Interpretação simples.
Desvantagens: Sensível a dados desbalanceados e pode sofrer overfitting.
Overfitting (Sobreajuste): O modelo aprende os dados de treinamento tão bem que memoriza ruídos e não generaliza para novos dados.
Soluções: Regularização (L1, L2), poda de árvores, dropout em redes neurais, aumento da quantidade de dados de treinamento.
Underfitting (Subajuste): O modelo é muito simples para capturar os padrões dos dados de treinamento, resultando em baixo desempenho tanto no treinamento quanto em dados novos.
Soluções: Aumentar a complexidade do modelo, adicionar mais dados relevantes, usar features mais robustas.
Validação Cruzada: Técnica para avaliar o desempenho do modelo de forma mais robusta, reduzindo a variância.
Holdout: Divide os dados em conjuntos de treino e teste (ex: 80% treino, 20% teste).
K-Fold: Divide os dados em K "dobras". O modelo é treinado K vezes, usando K-1 dobras para treinamento e 1 dobra para teste em cada iteração.
Leave-One-Out (LOO): É um caso especial de K-Fold onde K é igual ao número de amostras, ou seja, cada dado é testado individualmente enquanto os demais são usados para treino.
Big Data
Refere-se a grandes volumes de dados que são difíceis de processar usando ferramentas tradicionais. Caracterizado pelos "3 Vs":

Volume: Enorme quantidade de dados.
Velocidade: Dados gerados e processados em alta velocidade.
Variedade: Diversidade de tipos e formatos de dados (estruturados, semi-estruturados, não estruturados).
A Qualidade de Dados é crucial para o Big Data e a Ciência de Dados, garantindo que os dados sejam precisos, completos, consistentes e atualizados para análises confiáveis e decisões assertivas.

Governança de TI e Legislação do CNJ
A governança de TI garante que a tecnologia da informação apoie os objetivos de negócio de uma organização, com foco em gestão de riscos, segurança e eficiência.

Resoluções e Portarias do CNJ (Conselho Nacional de Justiça)
A série de resoluções e portarias do CNJ visa modernizar, padronizar e aumentar a eficiência, transparência e segurança da TI no Poder Judiciário.

Resolução CNJ nº 335/2020 - Transformação Digital no Judiciário:

Define critérios e procedimentos para a gestão de processos de transformação digital no Judiciário.
Estabelece parâmetros para a implementação de tecnologias digitais visando mais eficiência e transparência.
Portaria CNJ nº 252/2020 - Procedimentos e Governança de TI no Judiciário:

Fortalecer a Governança de TI: Cria uma estrutura para a gestão eficiente e segura dos sistemas e recursos de TI no Judiciário.
Padronizar Procedimentos: Define processos e metodologias comuns para a implementação de soluções tecnológicas em diversos órgãos.
Melhorar a Gestão de Recursos: Assegura o uso eficiente dos recursos de TI, garantindo segurança, continuidade e eficácia.
Estrutura de Governança de TI: Implica uma organização hierárquica com:
Comitê de Governança de TI: Supervisiona políticas e define diretrizes/prioridades para projetos de tecnologia.
Unidades Gestoras de TI: Em cada órgão, responsáveis pela execução e manutenção das políticas de tecnologia.
Gestão de Projetos e Recursos: Processos claros para alocação de recursos e gerenciamento de projetos.
Diretrizes para a Gestão de TI:
Segurança da Informação: Medidas rigorosas para proteção e integridade das informações e dados sensíveis.
Integração de Sistemas: Incentiva a interoperabilidade entre os diversos sistemas dos órgãos.
Desenvolvimento e Implementação de Sistemas: Deve seguir boas práticas de governança e ser baseado em necessidades reais.
Adoção de Soluções Tecnológicas Inovadoras: Incentivo ao uso de tecnologias como cloud computing e big data.
Planejamento e Execução de Projetos de TI:
Planejamento Estratégico: Projetos alinhados aos objetivos institucionais e orçamento.
Metodologias Ágeis: Incentivo ao uso para otimizar a execução, com entregas rápidas e flexibilidade.
Avaliação de Resultados: Monitoramento e avaliação contínuos para medir a eficiência das soluções.
Acompanhamento e Monitoramento:
Indicadores de Desempenho: Para avaliar qualidade e eficácia das soluções.
Auditorias e Revisões: Para garantir conformidade e transparência.
Portaria CNJ nº 253/2020 - Regras de Segurança e Gestão de Dados Sensíveis no Judiciário:

Regula a gestão de dados e a segurança da informação dentro do Poder Judiciário.
Cria protocolos de segurança cibernética e confidencialidade para o manejo de informações sensíveis.
Resolução CNJ nº 522/2023 - Diretrizes de TI no Judiciário para Governança e Segurança:

Foca em Governança de TI, gestão de riscos, segurança da informação, controle de acessos e proteção de dados.
Visa melhorar a eficiência operacional e garantir a segurança no uso da TI nos tribunais.
Princípios e Modelos de Gestão de Riscos: Identificação, análise e mitigação de riscos organizacionais.
Normas Internacionais: Menciona ISO 31000 (Gestão de Riscos) e NIST SP 800-30 (TI).
Processo de Gestão de Riscos: Comunicação e Consulta → Contextualização → Identificação → Análise → Tratamento → Monitoramento → Retroalimentação.
Portaria CNJ nº 131/2021 - Digitalização dos Processos e Sistemas Judiciais:

Define os padrões técnicos para a implantação de tecnologias e a digitalização dos processos no Judiciário.
Resolução CNJ nº 396/2021 - Segurança e Controle de TI nas Infraestruturas do Judiciário:

Estabelece normas para o processamento de dados e segurança cibernética nas infraestruturas de TI do Judiciário.
Cria diretrizes de segurança e protocolos de monitoramento e controle para as infraestruturas de TI.
Portaria CNJ nº 162/2021 - Regras para Gestão de Contratos de TI no Judiciário:

Define diretrizes para a gestão de contratos de TI, visando maior transparência e controle na contratação de serviços e produtos.
Importante notar: A menção de "PJE" nesta portaria no material original parece ser um erro ou interpretação equivocada do resumo, pois o foco principal da Portaria CNJ nº 162/2021 é a gestão de contratos de TI em geral, e não especificamente a padronização do PJe. A padronização do PJe e a interoperabilidade são temas tratados em outras normativas ou como objetivos mais amplos do CNJ.
Plataforma Digital do Poder Judiciário (PDPJ)
A PDPJ é uma iniciativa estratégica para integrar os sistemas eletrônicos do judiciário, visando maior eficiência, transparência e acessibilidade na tramitação de processos.

Objetivos Principais:
Integração de Sistemas: Conectar sistemas eletrônicos de diferentes órgãos do Judiciário.
Facilitar o Acesso à Justiça: Proporcionar acesso digital a processos, audiências e informações judiciais.
Otimizar a Tramitação de Processos: Reduzir tempo e custos do andamento dos processos.
Segurança: Garantir que informações processuais sejam armazenadas e compartilhadas com segurança e sigilo.
Funcionalidades da PDPJ:
Consulta Processual: Consulta em tempo real com informações atualizadas.
Envio e Recebimento de Documentos: Facilita o manuseio eletrônico.
Acompanhamento de Audiências: Possibilita acompanhamento remoto.
Integração entre Tribunais: Conecta diversas esferas da Justiça para facilitar o fluxo.
Assinatura Digital: Garante autenticidade e validade jurídica dos documentos.
Benefícios da PDPJ:
Agilidade: Redução do tempo de tramitação e decisões.
Redução de Custos: Menos custos operacionais, eliminação de papel e deslocamento.
Acesso Facilitado: Acesso e acompanhamento de processos a qualquer momento e lugar.
Segurança Jurídica: Assinatura digital e protocolos de segurança garantem autenticidade e integridade.
Transparência: Permite a consulta de informações relevantes ao público.
Funcionamento PDPJ:
Sistema Centralizado e Interligado: Diferentes tribunais acessam e compartilham dados.
Interface de Acesso: Interfaces específicas para tarefas (consulta, envio de documentos).
Integração com Outros Sistemas: Interoperabilidade entre as diversas esferas da Justiça.
Governo Eletrônico e Inovação na Gestão Pública
Governo Eletrônico: Utilização da Tecnologia da Informação para modernizar a administração pública.
Eixos: Transparência, Participação Cidadã e Eficiência.
Comunicação na Gestão Pública: Importância da comunicação clara e eficaz entre governo e sociedade.
Compras Governamentais e Gestão de Contratos:
Sustentabilidade nas Contratações: Inclusão de critérios ambientais e sociais.
Compras Centralizadas: Redução de custos e padronização.
Organização Sistêmica da Administração Pública Federal:
Sistemas Estruturantes:
SIASG (Sistema Integrado de Administração de Serviços Gerais): Compras e contratos.
SIAFI (Sistema Integrado de Administração Financeira do Governo Federal): Gestão financeira.
Sigepe (Sistema de Gestão de Pessoas do Governo Federal): Gestão de pessoal.
Inovação Tecnológica e Gestão Pública
Brainstorming: Técnica para geração de ideias para inovação.
Design Thinking: Abordagem centrada no usuário para solução criativa de problemas.
Lean Startup: Metodologia para validação rápida de projetos e produtos.
Arquitetura Corporativa de TI e Inovação em IA
Arquitetura Corporativa de TI (TOGAF - The Open Group Architecture Framework): Estrutura para alinhar a TI com os objetivos de negócio de uma organização.

Componentes: Arquitetura de Negócios, Arquitetura de Dados, Arquitetura de Aplicações e Arquitetura de Tecnologia.
BPM (Business Process Management - Gerenciamento de Processos de Negócio - CBOK): Disciplina que foca na otimização de processos de negócio.

Ciclo: Modelagem, Execução, Monitoramento e Otimização de Processos.
IA como Serviço e Inovação
AI-as-a-Commodity: A Inteligência Artificial oferecida como um serviço, integrada via APIs e produtos SaaS, eliminando a necessidade de desenvolvimento do zero.
Benefícios: Acessibilidade (qualquer porte de empresa), Padronização (modelos prontos), Custo Reduzido, Escalabilidade e Integração Simples.
IA Gateway: Middleware que conecta aplicações a múltiplos modelos de IA, permitindo a escolha dinâmica da melhor solução para uma determinada tarefa.
Desenvolvimento de Soluções GenAI: Combina engenharia de software, MLOps (Machine Learning Operations) e pipelines de dados para criar sistemas com IA generativa, utilizando redes neurais profundas (especialmente Transformers) e técnicas como fine-tuning e RLHF.
PostgreSQL: Sistema gerenciamento de banco de dados relacional de código aberto e altamente extensível.

H2 Database: Banco de dados leve, usado em testes e desenvolvimento local (Embutido quanto em servidor).
•	Modo In-Memory: BD será em memória, e os dados não serão persistidos após a execução.
•	Modo Persistente: BD será persistido em disco no diretório do usuário.

Característica	PostgreSQL	MySQL	Oracle DB
Licença	Open Source	Open Source	Proprietário
Suporte a Tipos Complexos	Extensa (JSON, XML, etc.)	Limitado	Extensa (inclusive geoespacial)
Suporte a Transações	Completo (ACID)	Completo	Completo (ACID)
Escalabilidade	Alta (Replicação, Particionamento)	Alta (Replicação)	Alta
Performance em Consultas	Muito boa em consultas complexas	Boa em leituras simples	Excelente em transações grandes
🧠 Macete: PostgreSQL é banco PRO | H2 é banco TESTE

Resolução CNJ nº 522/2023 - Diretrizes de TI no Judiciário para governança e segurança.
 🔹 Governança de TI, gestão de riscos, segurança da informação, controle de acessos e proteção de dados.
 🔹 Melhorar a eficiência operacional e garantir segurança no uso de TI nos tribunais.
 🔹 Princípios e Modelos de Gestão de Riscos: Identificação, análise e mitigação de riscos organizacionais.
 🔹 Normas internacionais: ISO 31000 (Gestão de Riscos), NIST SP 800-30 (TI).
 🔹 Processo de Gestão de Riscos: Comunicação e Consulta → Contextualização → Identificação → Análise → Tratamento → Monitoramento → Retroalimentação

Arq Corporativa de TI (TOGAF) (The Open Group Architecture Framework) – Estrutura para alinhar TI e negócios.
 🔹 Componentes: Arquitetura de Negócios, Dados, Aplicações e Tecnologia.
BPM (Gerenciamento de Processos de Negócio - CBOK): Ciclo: Modelagem, Execução, Monit e Otim de Processos.
Resolução CNJ nº 335/2020 - Transformação digital no Judiciário para mais eficiência e transparência
•	Define critérios e procedimentos para a gestão de processos de transformação digital no âmbito do Jud.
•	Dá parâmetros para implementação de tec dig para eficiência e transparência na gestão dos processos.
Portaria CNJ nº 252/2020 - Procedimentos e governança de TI no Judiciário
•	Define os procedimentos para a gestão e monitoramento da governança de TI dentro do Judiciário.
•	Estabelece diretrizes de governança p/ utilização de tec em proc jud e na adm de infraestruturas de TI
Portaria CNJ nº 253/2020 - Regras de segurança e gestão de dados sensíveis no Judiciário
•	Regula a gestão de dados e a segurança da informação dentro do Poder Judiciário.
•	Cria protocolos de seg cibernética e confidencialidade para o manejo de informações sensíveis no judicial.
Portaria CNJ nº 131/2021 - Digitalização dos processos e sistemas judiciais
•	Define os padrões técnicos para a implantação de tecnologias e a digitalização dos processos no Judiciário.
Resolução CNJ nº 396/2021 - Segurança e controle de TI nas infraestruturas do Judiciário
•	Normas para o processamento de dados e segurança cibernética nas infraestruturas de TI do Judiciário.
•	Cria diretrizes de segurança e protocolos de monitoramento e controle para as infraestruturas de TI.
Portaria CNJ nº 162/2021 - Regras para gestão de contratos de TI no Judiciário
•	Define diretrizes para a gestão de contratos relacionados a tecnologia da informação, visando maior transparência e controle na contratação de serviços e produtos de TI.

PDPJ: Integrar os sistemas eletrôn. do jud., para tramitação de processos + eficiente, transparente e acessível.
 🔹 Objetivos Principais:
•	Integração de sistemas: Conectar os sistemas eletrônicos de diferentes órgãos do Judiciário
•	Facilitar o acesso à Justiça: Proporcionar acesso digital a processos, audiências e informações judiciais.
•	Otimizar a tramitação de processos: Reduzir o tempo e custos do andamento dos processos judiciais.
•	Segurança: Informações processuais sejam armazenadas e compartilhadas com segurança e sigilo.
 🔹 Funcionalidades da PDPJ: facilitar a interação entre os envolvidos no processo judicial
•	Consulta Processual: Permite a consulta de processos em tempo real, com informações atualizadas.
•	Envio e Recebimento de Documentos: Facilita o manuseio de forma eletrônica
•	Acompanhamento de Audiências: Possibilita o acompanhamento remoto de audiências e sessões 
•	Integração entre Tribunais: Conecta diversas esferas da Justiça, facilitando o fluxo entre os órgãos.
•	Assinatura Digital: Documentos assinados digitalmente garantindo a autenticidade e validade jurídica.
 🔹 Benefícios da PDPJ
•	Agilidade: Redução do tempo de tramitação de processos e decisões judiciais.
•	Redução de Custos: menos custos operacionais, eliminação do papel e menos de deslocamento.
•	Acesso facilitado: Pode acessar e acompanhar processos a qualquer momento e de qualquer lugar.
•	Seg. Jurídica: Ass digital e prot segurança, a autenticidade e a integridade dos documentos são garantidas.
•	Transparência: para que qualquer um possa consultar informações relevantes.
 🔹 Funcionamento PDPJ: 
•	Sistema Centralizado e Interligado: Para que diferentes tribunais acessem e compartilhem dados.
•	Interface de Acesso: Interfaces específicas para realizar tarefas como (ex: consulta e envio de doc.)
•	Integração com Outros Sistemas: integração e interoperabilidade entre as diversas esferas da Justiça.
 Portaria nº 252/2020: regular e padronizar a gestão de TI no Judiciário
 🔹 Fortalecer a Governança de TI: Criar estrutura para gestão + eficiente e segura dos sistemas no jud.
 🔹 Padronizar procedimentos: Definir processos e metodologias comuns p/ implementação de soluções tecnológicas nos diversos órgãos do Judiciário.
 🔹 Melhorar a gestão de recursos: Assegurar que os recursos de TI sejam usados de forma eficiente, garantindo segurança, continuidade e eficácia nas operações.
Estrutura de Governança de TI: organização hierárquica, com órgãos específicos responsáveis pela coordenação, supervisão e implementação de projetos de TI em diferentes níveis.
 🔹 Comitê de Governança de TI: Supervisionar a implementação das políticas de TI, definindo as diretrizes e prioridades para os projetos de tecnologia.
 🔹 Unidades Gestoras de TI: Cada órgão do Judiciário deve ter sua própria unidade gestora de TI, responsável por garantir a execução e manutenção das políticas de tecnologia no seu âmbito.
 🔹 Gestão de Projetos e Recursos: A portaria estabelece a criação de processos claros para a gestão de projetos e a alocação de recursos tecnológicos nos órgãos do Judiciário.
Diretrizes para a Gestão de TI: garantir a eficiência e segurança na gestão de TI no Judiciário.
🔹 Segurança da Informação: Os órgãos do Judiciário devem adotar medidas rigorosas para garantir a proteção e integridade das informações processuais e dados sensíveis.
🔹 Integração de Sistemas: A portaria incentiva a integração entre os diferentes sistemas utilizados pelos órgãos do Judiciário, promovendo uma comunicação mais eficiente e evitando redundâncias.
🔹 Desenvolvimento e Implementação de Sistemas: Deve seguir boas práticas de governança e ser baseado em necessidades reais de usuários do Judiciário.
🔹 Adoção de Soluções Tecnológicas Inovadoras: Necessidade de adotar soluções inovadoras e adequadas às necessidades do Judiciário, utilizando tecnologias como cloud computing e big data.
Planejamento e Execução de Projetos de TI
🔹 Planejamento Estratégico: Os projetos de TI devem ser alinhados aos objetivos institucionais do Judiciário e com o orçamento disponível.
🔹 Metodologias Ágeis: Uso incentivado para otimizar a execução de projetos, garantindo entregas rápidas e flexibilidade nas modificações.
🔹 Avaliação de Resultados: Todos os projetos de TI devem ser monitorados e avaliados para medir os resultados e a eficiência das soluções implantadas.
Acompanhamento e Monitoramento: acompanhamento contínuo das iniciativas de TI no Judiciário
🔹 Indicadores de Desempenho: Permitam avaliar a qualidade e a eficácia das soluções implantadas.
🔹 Auditorias e Revisões: Garantir a conformidade e a transparência nos processos de gestão de TI.
Portaria nº 162/2021: PJE 
🔹 Padronizar o PJe: Definir os procedimentos e as metodologias p/ implementação do PJe.
🔹 Garantir a interoperabilidade: Todos os sistemas de PJe sejam interoperáveis.
🔹 Incentivar a adoção de tecnologias: Para garantir + agilidade e segurança na tramitação de processos.
•	Padronização dos processos: Todos os tribunais devem seguir as normas estabelecidas p/ uniformidade.
•	Capacitação: O CNJ determina treinamentos contínuos para garantir a eficiência no uso do sistema.
•	Facilidade de uso: O sistema deve ser intuitivo e acessível, para que qualquer usuário
•	Prazo de implementação: De forma gradual, com prazos para a adesão total do sistema.
•	Compatibilidade entre sistemas: Compatível com outros sistemas e processos já usados pelos tribunais, 
•	Uniformidade: Os tribunais devem adotar a mesma plataforma e procedimentos definidos.
•	Acompanhamento contínuo: O CNJ será responsável por acompanhar a implantação do PJe nos tribunais.
•	Auditoria e fiscalização: Auditorias periódicas para avaliar a qualidade e a eficiência da implantação e uso.

Governo Eletrônico e Inovação na Gestão Pública
🔹 Governo Eletrônico: Uso da TI para modernizar a administração pública.
•	Eixos: Transparência, Participação Cidadã, Eficiência.
🔹 Comunicação na Gestão Pública: Importância da comunicação clara entre governo e sociedade.
🔹 Compras Governamentais e Gestão de Contratos: Sustentabilidade nas contratações – Critérios ambientais e sociais. Compras centralizadas – Redução de custos e padronização.
🔹 Organização Sistêmica da Administração Pública Federal: Sistemas estruturantes: SIASG (Compras), SIAFI (Financeiro), Sigepe (Pessoal).

Inovação Tecnológica e Gestão Pública
•	Brainstorming – Geração de ideias para inovação.
•	Design Thinking – Solução criativa baseada no usuário.
•	Lean Startup – Validação rápida de projetos

Banco de Dados: Sistema organizado para coletar, armazenar e gerenciar dados. Facilitar consulta, manipulação e análise.

Abordagem Relacional: Modelo de banco de dados onde os dados são organizados em tabelas inter-relacionadas.
•	Tabelas: Estruturas que contêm os dados.
•	Relacionamentos: Conexões entre tabelas usando chaves primárias e estrangeiras.
•	SQL (Structured Query Language): Linguagem para consultar e manipular dados no banco relacional.
Modelo Entidade-Relacionamento (ER): Modelo gráfico que descreve a estrutura de um banco de dados.
•	Entidades: Objetos ou conceitos que têm dados associados.
•	Relacionamentos: Associações entre entidades.
•	Atributos: Propriedades de entidades ou relacionamentos.
MySQL - Rápido e fácil, ideal para web, mas com limitações em performance.
Oracle - Potente, ideal para grandes empresas, mas exige licenciamento.
•	Robusto e poderoso, empresas que precisam de alta performance e escalabilidade.
•	Licenciamento pago, oferece recursos avançados de segurança, backup e recuperação.
PostgreSQL - Avançado, aberto, e ótimo para consultas complexas:
•	BD Rel avançado de código aberto, para consultas complexas e desenvolvimento de aplicações.
•	Oferece funcionalidades extras como suporte a JSON, consultas recursivas, e índices personalizados.
SGBD: Software q gerencia bancos de dados e controla o acesso, a segurança e a integridade dos dados.
🔹 Tarefas como backup, recuperação de dados, otimização de consultas e controle de usuários.
🔹 Características de um SGBD:
•	Independência dos Dados - SGBD permite que as aplicações se conectem ao banco de dados sem precisar se preocupar com a estrutura interna do banco.
•	Controle de Concurrency - Controla o acesso simultâneo aos dados sem conflitos
•	Segurança de Dados - Protege com controle de autenticação, autorização, permiss. e criptografia.
•	Backup e Recuperação - Faz cópias de segurança e recupera dados quando necessário.
•	Integridade dos Dados - Garante que os dados sejam consistentes, válidos e não sejam corrompidos.
•	Suporte a Transações - Garante que as operações sejam atômicas (tudo / nada) = seguro e coerente.
Modelagens de Dados: Processo de estruturar os dados para que sejam facilmente armazenados e acessados.
🔹 Modelo Relacional: Tabelas com chaves que se relacionam. Facilita consulta e integridade referencial.
•	Estrutura: Usa tabelas para armazenar dados. As tabelas têm linhas (tuplas) e colunas (atributos).
•	Relações: As tabelas podem ser relacionadas por meio de chaves primárias e chaves estrangeiras.
•	Usa SQL (Structured Query Language) para consultas e manipulação.
•	Garante ACID (Atomicidade, Consistência, Isolamento, Durabilidade).
DDL (Data Definition Language) – Criação e alteração de tabelas (CREATE, ALTER, DROP).
DML (Data Manipulation Language) – Consulta e modificação de dados (SELECT, INSERT, UPDATE, DELETE).
•	A chave primária pode ser simples ou composta:
Simples--> um atributo 
Composta--> dois ou mais atributos
	1:1 --> fusão de tabelas;
	1:N --> chave estrangeira vai pro lado N;
	N;N --> tabela associativa
🔹 Modelos Não Relacionais (NoSQL) - grandes volumes de dados e alta escalabilidade.
•	Usa diferentes formatos:
•	Chave-Valor (Redis)
•	Documentos JSON (MongoDB)
•	Grafos (Neo4j)
•	Colunar (Cassandra)
•	Não exige esquema fixo de dados.
•	ACID relaxado: priorizar desempenho e escalabilidade, com consistência eventual.
🔹 Modelo Multidimensional: Dimensões+Medidas = Cubo de dados/análises rápidas e consultas agregadas
•	Estrutura: Organiza dados em dimensões e medidas, formando uma estrutura de cubo.
•	Exemplo: Usado em Data Warehouses e análises de Business Intelligence (BI).
•	Estrutura: Dimensões (ex: tempo, local) e medidas (ex: vendas, lucro).
Modelo Conceitual (Entidade-Relacionamento) → Esboço inicial.
Modelo Lógico → Estruturas normalizadas.
Modelo Físico → Implementação no SGBD.
📌 Normalização/Desnormalização - Proc de organizar dados em tabelas para ñ redundâncias e garantir integridade.
•	Eliminar anomalias (como duplicação de dados) e facilitar a manutenção dos dados.
Nível	Objetivo	Requisitos	Problema Eliminado
0FN (Não normalizado)	Organizar dados ainda brutos, sem estrutura.	Dados podem conter grupos repetitivos e informações redundantes.	Nenhum problema resolvido ainda.
1FN	Eliminar grupos repetitivos e garantir atomicidade.	Todos os atributos devem conter valores atômicos (indivisíveis). Eliminar colunas multivaloradas ou compostas.	Redundância básica e repetição de grupos.
2FN	Eliminar dependências parciais.	Estar na 1FN. Todos os atributos não-chave devem depender da chave primária inteira (e não de parte dela).	Dependência parcial da chave.
3FN	Eliminar dependências transitivas.	 Estar na 2FN. Atributos não-chave não devem depender de outros atributos não-chave (ou seja, evitar dependência transitiva).	Redundância por dependência transitiva.
BCNF	Versão rigorosa da 3FN (em casos especiais).	 Estar na 3FN. Toda dependência funcional é de uma superchave.	Problemas raros não resolvidos pela 3FN.
🔹 Desnormalização: Proc. oposto, tabelas são combinadas p/ melhorar o desempenho de consultas.

Árvores de Decisão: Estrutura hierárquica para classificação/regressão. Divide dados em subconjuntos base em atributos.
🔹 Critérios de divisão: 
•	Gini (para classificação) → Mede a impureza dos dados.
•	Entropia (para classificação) → Mede a desordem dos dados.
•	MSE (para regressão) → Minimiza o erro.
Vantagens: Interpretação simples. Desvantagens: Sensível a dados desbalanceados e pode sofrer overfitting.
Business Intelligence – BI: Transforma dados em informações para tomar decisões estratégicas. 
🔹 Data Lake: Grande repositório de dados brutos e não estruturados. 
🔹 Data Warehouse: Armazém org. centralizado para dados históricos. Otimiza consultas e relatórios complexos.
Suporta análise de dados de múltiplas fontes para relatórios e consultas.
🔹 Data Mart: Pequeno Data Warehouse focado em um setor. Dados mais específicos e rápidos para análises. Pode ser dependente (vinculado DW principal) ou independente (alimentado diretamente por fontes de dados).
🔹 Data Mining: Extração de padrões, tendências ocultas e insights dos dados. 
🔹 Data Mesh: Dados distribuídos entre diferentes equipes, promovendo autonomia e escalabilidade.
🔹 ETL: Extrair, Transformar e Carregar dados para análise
•	Processo de preparação dos dados para o Data Warehouse ou Data Mart.
•	Extract (Extrair): Captura dados de diversas fontes (bancos relacionais, planilhas, sistemas legados).
•	Transform (Transformar): Trata, limpa, filtra e estrutura os dados conforme as regras de negócio.
•	Load (Carregar): Insere os dados transformados no repositório final (DW ou Data Mart).
•	Pode ser feito em lotes periódicos ou em tempo real (streaming).
🔹 OLAP (Online Analytical Processing): Consultas rápidas e interativas para análises complexas
ETL prepara os dados, Data Warehouse os armazena e OLAP permite consultas rápidas. Data Lake é onde os dados brutos são guardados, e Data Mesh descentraliza a gestão de dados.

Ciência de Dados: Usa métodos científicos, algoritmos e sistemas para extrair insights a partir de dados. 

Machine Learning - ML: Máquinas que aprendem com os dados, sem programação explícita

Matriz de Confusão: Ferramenta para avaliar o desempenho. Compara os resultados previstos os reais e vê como está.
Tabela de duas dimensões (linhas e colunas), onde cada linha representa uma classe real e cada coluna representa uma classe prevista. Pode ser usada em classificações binárias ou multiclasse.
🔹 Termos para o caso binário:
•	Verdadeiro Positivo (VP): Previu que a classe é positiva e a classe real também é positiva
•	Falso Positivo (FP): Previu que a classe é positiva, mas a classe real é negativa.
•	Verdadeiro Negativo (VN): Previu que a classe é negativa e a classe real também é.
•	Falso Negativo (FN): Previu que a classe é negativa, mas a classe real é positiva.
🔹 Métricas de desempenho:
o	Acurácia:
o	Precisão:
o	Recall:
o	F1-Score:
Deep Learning: Redes neurais profundas que aprendem com dados complexos
•	Simula a estrutura do cérebro, usando camadas de neurônios artificiais para processar informações.
•	Automatizar processo de aprendizado, p/ reconhecimento de padrões mais avançados (ex: imagens, txt).
Processamento de Linguagem Natural (NLP) - Computadores entendendo e gerando linguagem humana
•	Analisar e gerar linguagem humana para que as máquinas entendam ou respondam adequadamente.
Big Data - Grandes volumes de dados difíceis de processar com ferramentas tradicionais
•	Envolve a coleta, armazenamento, processamento e análise de muitos dados.
•	Extrair insights valiosos de grandes conjuntos de dados para apoiar decisões empresariais e previsões.
Big Data = 3 Vs: Volume, Velocidade, Variedade → “Muito, Rápido e Diferente!”
Qualidade de Dados - Dados precisos, completos, consistentes e atualizados
•	Dados de baixa qualidade podem levar a análises incorretas e decisões erradas.
•	Garantir que os dados sejam úteis e confiáveis para análise e tomada de decisão.
Tipos de Aprendizado: 
🔹 Supervisionado: Dados com rótulos (respostas conhecidas)
🔹 Não Supervisionado: Encontrar padrões ou grupos sem respostas conhecidas
🔹 Semissupervisionado: Mistura de dados rotulados e não rotulados
🔹 Reforço: Aprendizado por recompensa e penalidade, tipo um jogo
🔹 Transferência: Aprender de um problema e aplicar em outro relacionado
Grandes Modelos de Linguagem (LLM) - IA treinada para entender e gerar texto de forma natural
•	Gerar, traduzir, resumir ou entender texto com alta precisão. 
IA Generativa - IA que cria novos conteúdos a partir de dados aprendidos
AI-as-a-Commodity: IA como serviço, integrada a APIs e produtos SaaS. IA sem desenvolvimento do zero.
- Acessibilidade – Empresas de qualquer porte podem utilizar IA sem expertise técnica profunda.
- Padronização – Modelos prontos para uso, semelhantes a produtos de prateleira.
- Custo Reduzido – Não é necessário desenvolver uma IA do zero, apenas consumir como serviço.
- Escalabilidade – Pode ser usada sob demanda e escalada conforme necessário.
- Integração Simples – APIs e serviços em nuvem facilitam a adoção.
IA Gateway: Middleware que conecta aplicações a múltiplos modelos de IA p/ escolha dinâmica da melhor solução.
Desenvolvimento de Soluções GenAI: Combina engenharia de software, MLOps e pipelines de dados para criação de sistemas com IA generativa.
•	Baseiam-se em redes neurais profundas, especialmente do tipo transformer.
•	Diferença entre IA tradicional (discriminativa) e IA generativa.
•	Ajuste fino (fine-tuning) com dados específicos.
•	Aprendizado por Reforço com Feedback Humano (RLHF).
Redes Neurais - Consistem em camadas de nós (ou neurônios) que processam informações. Cada nó recebe entradas, calcula e transmite saídas para os próximos. Reconhecimento de padrões, classificação e previsões.
🔹 Componentes: Neurônios artificiais: Funções matemáticas que processam entradas.
•	Camadas: Entrada, oculta e saída.
•	Pesos e bias: Ajustáveis para melhorar a precisão.
🔹 Três camadas principais: Entrada → Oculta (Processamento) → Saída
🟢 Camada de Entrada (Input Layer) - Recebe os dados brutos.
•	Cada neurônio representa uma característica do dado de entrada (ex: pixels, atributos).
🔵 Camadas Ocultas (Hidden Layers) - Onde ocorre o processamento dos dados.
•	Cada neurônio realiza cálculos combinando os pesos dos sinais recebidos, aplica uma função de ativação e passa o resultado adiante.
•	Redes profundas (Deep Learning) possuem várias camadas ocultas.
🔴 Camada de Saída (Output Layer) - Fornece o resultado final da rede. Pode ser:
•	1 valor contínuo (em regressão), 1 classe (em classificação), múltiplos valores (tarefas multiclasse).
🔹 Tipos de Redes Neurais
1.	Perceptron - Rede simples para classificação binária com uma única camada de neurônios. 
2.	Redes Neurais Convolucionais (CNN) - Redes para imagens, com filtros para detectar padrões. 
3.	Redes Neurais Recorrentes (RNN) - Redes neurais com feedback entre suas camadas, lembra de informações passadas. Usadas para sequências temporais, como texto ou séries temporais.
4.	Redes Neurais de Longo Curto Prazo (LSTM) - Tipo avançado de RNN que resolve o problema do desvanecimento do gradiente, permitindo lembranças mais longas de dados importantes.
5.	Redes Generativas Adversariais (GAN) - Redes que competem entre si para gerar coisas realistas. Uma gera novos dados (gerador) e outra que tenta identificar se os gerados são F ou V discriminador
🔹 Aprendizado da Rede (Treinamento) - Ajusta os pesos e bias durante o treinamento para reduzir o erro.
Usa-se o algoritmo de retropropagação (backpropagation) com gradiente descendente para atualizar os pesos com base no erro da saída. Ligação com deep learning.

🔹 Técnicas de Validação e Ajuste de Modelos
- Validação Cruzada: Técnica usada para avaliar o desempenho do modelo. Tipos: 
•	Holdout: Divide os dados em treino e teste (ex.: 80%-20%).
•	K-Fold: Divide os dados em K partes e treina k vezes.
•	Leave-One-Out (LOO): Cada dado é testado individualmente.
- Overfitting: Modelo memoriza os dados e não generaliza bem. 
•	Solução: Regularização (L1, L2), poda de árvores, dropout em redes neurais.
- Underfitting: Modelo não aprende padrões suficientes. 
•	Solução: Aumentar complexidade do modelo, adicionar mais dados.
