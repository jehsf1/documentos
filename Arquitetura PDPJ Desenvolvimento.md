Define a estrutura e o funcionamento dos sistemas de TI, abrangendo hardware, software, redes e bancos de dados.
📌 Camadas: Cliente, Servidor e Banco de Dados. Interoperabilidade.
📌 Arquitetura Monolítica (Centralizada)
•	Todos os componentes (dados, processamento e interface) estão em um único servidor.
•	Simples de gerenciar, mas com baixa escalabilidade.
📌 Arquitetura Cliente-Servidor
•	Separação entre cliente (aplicação que solicita dados) e servidor (SGBD que gerencia os dados).
•	Permite múltiplos clientes acessando um banco de dados centralizado.
📌 Arquitetura Distribuída
•	O banco de dados é distribuído entre vários servidores.
•	Melhor escalabilidade e tolerância a falhas.
📌 Arquitetura em Nuvem
•	O banco é hospedado em serviços como AWS RDS, Google Cloud SQL, Azure SQL Database.
•	Alta disponibilidade, escalabilidade e segurança.
🔹 Estratégias de Arquitetura para Alta Performance
Replicação de Dados:  Copia dados a múltiplos servidores para tolerância a falhas e melhor desempenho.:
•	Master-Slave Um servidor principal e réplicas secund. Master-Master Vários servidores ativos juntos
•	Sharding (Particionamento): Divide o banco em múltiplos servidores para melhorar escalabilidade.
•	Cache de Dados: Reduz consultas repetitivas ao banco usando memória rápida (RAM).
•	Indexação: Melhora a velocidade das consultas criando estruturas otimizadas para busca.
🔹 Componentes da Arquitetura de Banco de Dados
1.	Camada Física (Storage Layer): Onde os dados são armazenados em disco ou SSD. Inclui arquivos de dados, índices e logs de transação. Gerenciado pelo SGBD (Sistema de Gerenciamento de Banco de Dados).
2.	Camada Lógica (Logical Layer): Define estrutura e regras do BD (modelos dados, chaves, relações). Implementa tabelas, visões, procedim. armazenados e triggers. Controla transações (ACID) e seg. dos dados.
3.	Camada de Aplicação (Application Layer): Interface onde usuários e sistemas interagem com o BD. Pode sistema ERP, app web ou API conectada ao banco. Utiliza SQL (para relacionais) ou APIs NoSQL p/ operações
🔹 Arquitetura Orientada a Serviços (SOA): reutilizáveis, módulos independentes acessados por diferentes aplicações.
•	Características: Baixo acoplamento: Módulos independentes. Reutilização: Serviços podem ser usados por vários sistemas. Interoperabilidade: Comunicação via padrões como XML, JSON e SOAP. Web Services: RESTful ou SOAP para integração.
•	Princípios Básicos SOA: Padronização contrato de serviço/ Abstração serviço / Baixo acoplamento /Autonomia serviço / Visibilidade serviço / Sem estado / Reusabilidade / Composição serviços / Heterogeneidade
🔹 Arquitetura Distribuída: processam informações em múltiplos servidores ou disp, em vez de centralizar td em 1 local. 
✔ Cliente-Servidor: Comunicação entre um cliente (front-end) e um servidor (back-end).
✔ Peer-to-Peer (P2P): Todos os nós têm função semelhante (exemplo: BitTorrent).
✔ Cloud Computing: Processamento na nuvem (AWS, Azure, Google Cloud).
✔ Edge Computing: Processamento próximo ao usuário (IoT).
🔹 Sistemas Colaborativos
✔ Groupware: Softwares para colaboração em equipe (Google Docs, Microsoft Teams).
✔ Workflows: Automação de processos de negócios.
✔ Sistemas de Gerenciamento de Conhecimento: Wiki, bases de conhecimento.
🔹 Gestão de Conteúdo (ECM) processos, ferramentas e estratégias para armazenar, organizar e acessar informações corporativas. Principais Componentes:
✔ CMS (Content Management System): Sistemas para gerenciar conteúdo digital (WordPress, Joomla).
✔ Indexação e Busca: Organização de documentos e dados.
✔ Controle de Versões: Histórico de alterações em arquivos.
✔ Segurança e Governança: Definição de acessos e proteção de dados.

Gestão do Conhecimento: Processo de criação, compartilhamento e retenção do conhecimento organizacional.
•	Ciclo do Conhecimento (Nonaka & Takeuchi): Socialização, Externalização, Combinação e Internalização.
Gestão da Informação: Organização e controle do fluxo de informações para tomada de decisão.
Gestão de Documentos: Estratégias para classificação, arquivamento e recuperação de documentos.
EIS (Enterprise Information System): Sistemas que integram informações organizacionais para apoiar a gestão.
ECM (Enterprise Content Management): Ferramentas para gerenciamento do conteúdo corporativo.
Trouble Ticket Systems: Sistemas de gestão de chamados para suporte técnico e TI.

🔹 Especificação de Web Services: permitem a comunicação entre sistemas via internet.
✔ SOAP (Simple Object Access Protocol): Baseado em XML, mais estruturado e seguro. (empresas)
✔ REST (Representational State Transfer): Baseado em HTTP (simplicidade, flexibilidade e performance)
✔ JSON e XML: Formatos para troca de dados.
✔ WSDL (Web Services Description Language): Linguagem para descrever serviços SOAP.

🔹 Aplicação em Dispositivos Móveis: considerar desempenho, conectividade e interface adaptável.
✔ Apps Nativos: Desenvolvidos para uma plataforma específica (Android: Kotlin/Java, iOS: Swift).
✔ Apps Híbridos: Criados com frameworks multiplataforma (Flutter, React Native).
✔ PWA (Progressive Web Apps): Aplicações web que funcionam como apps móveis.
Característica	SOAP	REST
Protocolo	Protocolo de comunicação definido	Estilo arquitetural baseado em HTTP
Formato de Dados	XML	JSON, XML, HTML, texto
Método	Pesado e complexo	Leve e simples
Segurança	WS-Security (padrão robusto)	SSL/TLS, OAuth, tokens
Estado	Pode ser sem estado ou com estado	Sem estado (stateless)
Operações	Opera com operações definidas em WSDL	Utiliza métodos HTTP (GET, POST, etc.)
Utilização	Aplicações formais, corporativas	Web, apps móveis, APIs públicas

Java - Linguagem de programação que funciona em qualquer lugar com JVM. Orientada a objetos.
🔹 Compilada e interpretada: código é compilado para bytecode, e é executado pela Java Virtual Machine 
🔹 Estrutura de um Programa Java:
•	Classe: public class NomeDaClasse define a estrutura do código.
•	Método main: public static void main(String[] args) é o ponto de entrada do programa.
•	Comando System.out.println: Exibe uma mensagem na tela.
🔹 Tipos de Dados:
•  Primitivos:
•	int: Inteiro (ex: 10)
•	double: Decimal (ex: 3.14)
•	char: Caractere (ex: 'A')
•	boolean: Verdadeiro ou Falso (ex: true)
•	byte, short, long, float: Outros tipos de números.
•  Não Primitivos (Objetos):
•	String: Cadeia de caracteres (ex: "Olá Mundo").
•	Variáveis: Usar final para declarar uma variável que não pode ser alterada.
•	Retorno de Valores: Métodos podem retornar valores com return.
•	Classe é um molde para criar objetos.
•	Objeto é uma instância da classe.
•	Encapsulamento: Proteger dados e permitir acesso controlado com getter e setter.
•	Herança: Uma classe pode herdar propriedades e métodos de outra classe.
•	Pacotes: Organizam as classes em diretórios.
•	Usar import para incluir bibliotecas externas.

Conceito	Descrição	Exemplo
Classe	Estrutura que define atributos e métodos	class Pessoa
Objeto	Instância da classe	joao = Pessoa()
Abstração	Focar no essencial e esconder complexidade	Interface de um carro
Encapsulamento	Ocultar dados internos e expor só o necessário	Atributos privados com get/set
Herança	Reutilizar código de uma classe existente	Aluno herda de Pessoa
Polimorfismo	Um mesmo método com comportamentos diferentes	falar() em Cachorro e Gato
🔹 Exceções: Eventos anormais ou erros que ocorrem durante a execução de um programa.
•	Exceções podem ser capturadas e tratadas com blocos de código específicos.
•	Exceções verificadas: Erros que o compilador obriga a tratar, como IOException e SQLException.
•	Exceções não verificadas: Erros de tempo de execução que não precisam ser explicitamente tratadas, como NullPointerException ou ArrayIndexOutOfBoundsException.
•	Exceções (em Java) Usa os blocos try, catch, finally para tratar exceções:
•	try: Bloco onde o código pode gerar exceções.
•	catch: Bloco onde a exceção é tratada.
•	finally: Bloco opcional executado sempre, independentemente de ocorrer uma exceção.
🔹 Coleções: Estruturas de dados usadas para armazenar múltiplos elementos de forma eficiente.
•	List: Uma lista ordenada de elementos (permitindo duplicatas). Ex: ArrayList, LinkedList.
•	Set: Uma coleção que não permite duplicatas. Exemplo: HashSet, TreeSet.
•	Map: Uma coleção de pares chave-valor. Exemplo: HashMap, TreeMap.
•	Queue: Uma coleção que representa uma fila. Exemplo: LinkedList, PriorityQueue.
🔹 Streams: operar sobre coleções de maneira declarativa.
•	Não modificam as coleções originais e podem ser encadeadas para criar pipelines de processamento.
•	Stream sequencial: Processa os elementos de maneira sequencial.
•	Stream paralelo: Processa os elementos em paralelo, aproveitando múltiplos núcleos do processador.
•	Operações Comuns em Streams
•	map: Transforma os elementos.
•	filter: Filtra os elementos de acordo com uma condição.
•	reduce: Agrega os elementos em um único valor (ex: soma, contagem).
•	collect: Coleta o resultado em uma nova coleção.
 Microsserviços pequenos serviços que fazem uma coisa bem, em vez de uma grande aplicação monolítica.

API RESTful: criar aplicações que se comunicam via HTTP usando métodos como GET, POST, PUT, DELETE.
•	API (Application Programming Interface): definições e protocolos p/ permitir a comunicação entre sistemas.
•	REST (Representational State Transfer): estilo arquitetura p/ criação serviço web que usa princípios HTTP
•	RESTful significa que a API segue os princípios e restrições do REST.
🔹 Princípios REST
•	Stateless: Comunicação cliente/servidor sem estado. Cada requisição deve ter todas informações.
•	Cacheable: Respostas podem ser armazenadas em cache para melhorar o desempenho.
•	Uniform Interface: Interface uniforme e simples que facilita a interação entre cliente e servidor.
•	Client-Server: Separação entre cliente e servidor, e cada parte tem uma função bem definida.
•	Layered System: Arq ser com múltiplas camadas intermediárias (balanceadores de carga, cache).
🔹 HTTP protocolo de comunicação utilizado em APIs RESTful.
o	Define como as mensagens são enviadas entre o cliente (ex: navegador) e o servidor.
GET	Recuperar dados	GET /usuarios/123
POST	Criar novo recurso	POST /usuarios
PUT	Atualizar recurso existente	PUT /usuarios/123
PATCH	Atualizar parcialmente o recurso	PATCH /usuarios/123
DELETE	Deletar recurso	DELETE /usuarios/123
OPTIONS	Verificar métodos permitidos	OPTIONS /usuarios
Spring: Framework que facilita a criação de aplicações Java.
•	Spring Boot: Configuração rápida de aplicações Java. Inicia o projeto.
•	Spring Cloud: Ferramenta para construir microsserviços.
•	Spring Eureka, Zuul (gateway): Soluções para descoberta de serviços e roteamento de APIs.
o	Swagger: Ferramenta para documentação automática de APIs.
o	MapStruct (mapeamento de DTOs).
→ Spring Boot inicia tudo → Spring Cloud conecta → Eureka registra → Zuul roteia → Swagger documenta.

JSON(JavaScript Object Notation): Formato de dados simples e legível para trocar informações entre sistemas.
Comum em APIs RESTful. Formato leve, fácil de ler e escrever, baseado em pares de chave-valor.
🔹 JPA: Padrão para acessar e manipular dados no BD em Java. Interface de persistência. Mapeamento objeto-relacional (ORM).
o	Simplificar o processo de armazenamento, recuperação, atualização e remoção de dados no banco.
🔹 Hibernate: Ferramenta que implementa JPA para mapear objetos Java para o BD e vice-versa.
🔹 Flyway: Ferramenta que ajuda a migrar versões do BD, garantindo integridade nas atualizações. Versiona
🔹 Envers: auditoria.
JPA- Padrão p/ acesso dados. Hibernate- Ferramenta q implementa o padrão. Flyway- Gerencia mudanças no banco

EntityManager	Interface para manipulação de entidades no contexto de persistência.
@Entity	Anotação que marca uma classe como entidade a ser mapeada para o banco.
@Id	Define a chave primária de uma entidade.
@OneToMany, @ManyToOne	Anotações para definir relações entre entidades.
JPQL	Linguagem de consulta semelhante ao SQL, mas operando sobre as entidades.
🧠 JPA descreve, Hibernate escreve, Envers observa e Flyway migra

Engenharia de Requisitos: levantamento, especificação, validação e gerenciamento dos requisitos ao longo do ciclo.
🔹 Requisitos: Condições ou funcionalidades necessárias p/ um sistema atender às necessidades do usuário.
🔹 Tipos: 
•	Funcionais – O que o sistema deve fazer (ex.: login, processamento de pedidos).
•	Não-Funcionais – Qualidades do sistema (ex.: segurança, desempenho, usabilidade).
🔹 Técnicas: Entrevistas – Workshops – Questionários – Brainstorming – Prototipação.
🔹 Especificação de Requisitos: Documento formal com detalhes funcionais e não-funcionais.
•	Padrões: IEEE 830, User Stories (Scrum), Casos de Uso (UML).
•	Documento de Requisitos de Software (SRS - Software Requirements Specification): Descrições detalhadas das funcionalidades do sistema, Inclui requisitos funcionais e não funcionais.
•	Modelagem de Requisitos: Diagramas UML (Casos de Uso, Diagrama de Classes, etc.). Histórias de Usuário – Pequenas descrições do que o usuário deseja fazer.
🔹 Técnicas de Validação de Requisitos
•	Revisões – Análise crítica do documento solicitante. Conferência de requisitos com stakeholders.
•	Prototipação – Criar modelos iniciais do sistema para validar conceitos antes da implementação final.
•	Protótipos descartáveis – Criados apenas para obter feedback e depois eliminados.
•	Protótipos evolutivos – Refinados continuamente até se tornarem o produto final.
•	MVP (Minimum Viable Product)
•	Produto mínimo viável com só as funcionalidades essenciais para validar hipóteses de mercado.
•	Iteração contínua com base no retorno dos usuários.
🔹 Critérios de Qualidade para Requisitos: 
•	Completos – Não deixam lacunas. Consistentes – Não entram em conflito entre si. Claros – De fácil entendimento. Viáveis – Podem ser implementados com tecnologia disponível.
🔹 Gerenciamento de Requisitos: Após a coleta, os requisitos precisam ser controlados e mantidos 
Rastreabilidade – Relacionamento entre requisitos e funcionalidades implementadas.
Priorização – Identificação dos requisitos mais críticos.
Gerenciamento de mudanças – Controle de modificações ao longo do projeto.
Versionamento – Controle de diferentes versões dos requisitos.
•	Técnicas de Priorização
MoSCoW – Classificação em: Must Have (essencial), Should Have (importante, mas não crítico), Could Have (desejável, mas não essencial) e Won’t Have (não será implementado agora).
100-dollar test – Stakeholders distribuem 100 pontos entre os requisitos mais importantes.
