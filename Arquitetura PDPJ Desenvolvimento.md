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

🔹 Arquitetura MVC e Princípios de Projeto
•	Modelo-Visão-Controlador (MVC) – Divide a aplicação em três camadas: 
•	Modelo – Gerencia dados e regras de negócio.
•	Visão – Interface do usuário.
•	Controlador – Coordena a interação entre Modelo e Visão.

Git: Ferramenta de versionamento de código fonte, usada para controlar alterações em projetos de software.
•	git init: Inicializa um repositório Git.
•	git clone: Clona um repositório existente.
•	git commit: Registra as alterações feitas.
•	git push: Envia suas alterações para o repositório remoto.
🔹 GitHub: Plataforma que hospeda repositórios Git, facilitando a colaboração em projetos.
🔹 GitLab – Alternativo ao GitHub e rodar as pipelines. 
1. Comandos de Configuração
•	git config = Configuração = Configura as opções do Git (nome de usuário, e-mail, editor, etc.)
Exemplo: git config --global user.name "Seu Nome"
•	git config --global user.name = Exibir Nome do Usuário = Mostra o nome de usuário configurado no Git
•	git config --global user.email = Exibir E-mail = Mostra o e-mail configurado no Git
•	git config --global core.editor = Configurar Editor = Configura o editor padrão do Git (ex: vim, nano, code, etc.)
2. Comandos para Criar e Inicializar Repositórios
•	git init = Inicializar Repositório = Cria um novo repositório Git no diretório atual
•	git clone = Clonar Repositório = Clona um repositório remoto para o diretório local
Exemplo: git clone https://github.com/usuario/repo.git
3. Comandos de Estado e Informações do Repositório
•	git status = Status = Mostra o estado atual do repositório (arquivos modificados, arquivos não rastreados, etc.)
•	git log = Log = Exibe o histórico de commits do repositório
Exemplo: git log --oneline para uma visão simplificada
•	git show = Mostrar Commit = Exibe detalhes de um commit específico
Exemplo: git show <commit_id>
•	git diff = Diferenças = Exibe as diferenças entre os arquivos não comprometidos e o repositório
Exemplo: git diff para ver alterações não comitadas
4. Comandos de Trabalho com Branches
•	git branch = Listar ou Criar Branch = Exibe, cria ou remove branches
Exemplo: git branch para listar os branches
Exemplo: git branch nome-da-branch para criar um novo branch
•	git checkout = Trocar de Branch = Muda para um branch específico
Exemplo: git checkout nome-da-branch
•	git checkout -b = Criar e Mudar para Branch = Cria um novo branch e já muda para ele
Exemplo: git checkout -b nova-branch
•	git merge = Mesclar Branches = Mescla as alterações de um branch para outro
Exemplo: git merge nome-da-branch
•	git rebase = Rebase = Aplica as alterações de um branch em outro branch, reescrevendo o histórico
Exemplo: git rebase nome-da-branch
5. Comandos de Commit
•	git add = Adicionar Arquivos = Adiciona alterações ao índice (staging area)
Exemplo: git add arquivo.txt ou git add . para adicionar todos os arquivos modificados
•	git commit = Commit = Registra as alterações no repositório local
Exemplo: git commit -m "Mensagem do commit"
•	git commit --amend = Alterar Último Commit = Modifica o último commit (ótimo para corrigir erros de mensagem ou adicionar novos arquivos)
•	git reset = Reset = Desfaz alterações feitas no índice (não no repositório)
Exemplo: git reset arquivo.txt para remover um arquivo do staging area
6. Comandos de Sincronização com Repositórios Remotos
•	git remote = Remoto = Gerencia repositórios remotos associados ao repositório local
Exemplo: git remote -v para listar os repositórios remotos
•	git push = Enviar para Repositório Remoto = Envia os commits locais para o repositório remoto
Exemplo: git push origin master para enviar a branch master para o repositório remoto origin
•	git pull = Atualizar de Repositório Remoto = Atualiza o repositório local com as alterações do repositório remoto
Exemplo: git pull origin master
•	git fetch = Buscar Atualizações = Baixa atualizações do repositório remoto, mas não faz merge automaticamente
•	git remote add = Adicionar Repositório Remoto = Adiciona um repositório remoto ao repositório local
Exemplo: git remote add origin https://github.com/usuario/repo.git
•	git push --force = Forçar Push = Força o envio para o repositório remoto (geralmente usado após um rebase)
Cuidado! Pode sobrescrever mudanças no remoto.
7. Comandos de Excluindo e Limpeza
•	git rm = Remover Arquivo = Remove arquivos do diretório e do repositório
Exemplo: git rm arquivo.txt
•	git reset = Reset = Desfaz alterações no histórico (volta para um commit anterior)
Exemplo: git reset --hard <commit_id>
•	git clean = Limpeza = Remove arquivos não rastreados (não versionados) do diretório de trabalho
Exemplo: git clean -f para remover arquivos não rastreados
8. Comandos de Comparação e Revisão
•	git diff = Diferenças = Compara as alterações feitas nos arquivos antes de um commit
Exemplo: git diff para mostrar o que foi alterado
•	git difftool = Ferramenta de Diferença = Abre uma ferramenta externa para comparar alterações, como meld ou vimdiff
•	git log --oneline = Histórico Simplificado = Exibe os commits de forma compacta, uma linha por commit
9. Comandos de Stashing (Guardar Temporariamente Alterações)
•	git stash = Armazenar Alterações = Guarda as modificações atuais (não comitadas) para um estado limpo
Exemplo: git stash
•	git stash pop = Recuperar Alterações = Aplica as modificações guardadas no stash e remove do stash
•	git stash list = Listar Stashes = Exibe os stashes guardados
•	git stash drop = Remover Stash = Exclui um stash específico da lista
10. Comandos de Rebase e Cherry-pick
•	git rebase = Rebase = Aplica commits de uma branch em outra, reescrevendo o histórico de commits
•	git cherry-pick = Pick = Aplica um commit específico de outro branch ao seu branch atual
Exemplo: git cherry-pick <commit_id>
11. Comandos de Tagging (Marcadores de Versão)
•	git tag = Listar Tags = Exibe todas as tags do repositório
•	git tag <tag_name> = Criar Tag = Cria uma tag para marcar um commit
Exemplo: git tag v1.0
•	git push --tags = Enviar Tags = Envia todas as tags para o repositório remoto
•	git tag -d <tag_name> = Excluir Tag = Remove uma tag do repositório local
Exemplo: git tag -d v1.0
12. Comandos de Segurança e Auditoria
•	git blame = Atribuição de Linha = Mostra quem fez a última modificação em cada linha de um arquivo
•	git log --stat = Log com Estatísticas = Exibe o histórico de commits com informações sobre modificações no código

