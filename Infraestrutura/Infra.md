📌 Serviços de Nuvem (IaaS, PaaS, SaaS): 
🔹 Nuvem Pública: A infraestrutura é compartilhada com outros clientes.
🔹 Nuvem Privada: Utilizada exclusivamente por uma organização, maior controle sobre segurança e performance. Pode ser instalada em um data center próprio ou em um provedor dedicado.
🔹 Nuvem Comunitária: Compartilhada por várias organizações com interesses comuns, com infra colaborativa.
🔹 Nuvem Híbrida: Combina nuvem pública e privada, dados e aplicativos movidos conforme necessário para maior flexibilidade e otimização.
Modelos de serviço: 
🔹 IaaS (Infrastructure as a Service) - Infraestrutura na nuvem, você escolhe e gerencia.
•	servidores, armazenamento, rede e máquinas virtuais, na nuvem.  
🔹 PaaS (Platform as a Service) - Plataforma pronta para desenvolver e hospedar aplicações
🔹 SaaS (Software as a Service) - Software pronto, só usar pela internet.
Google Workspace - Ferramentas de produtividade do Google, como Docs. colaboração e produtividade em tempo real.
Microsoft Office 365 - Pacote Office na nuvem com Teams, OneDrive.
Armazenamento de Dados em Rede
🔹 Network Attached Storage (NAS) - Armazenamento de rede para compartilhamento de arquivos
•	acesso centralizado e compartilhamento de arquivos em uma rede local.
🔹 Direct Attached Storage (DAS) - Armazenamento direto, sem rede, ligado ao computador
•	HDs internos e unidades externas.
🔹 Software Defined Storage (SDS) - Armazenamento controlado por software, independente do hardware
•	Ele permite flexibilidade, escalabilidade e automação na gestão de dados.
🔹 Cloud Storage - Armazenamento na nuvem, acessível de qualquer lugar
•	dados gerenciados e armazenados por provedores de serviços na internet, como Dropbox
Tipo	Função
NAS	Armazenamento em rede (ex: HD compartilhado)
DAS	Armazenamento direto no computador
SDS	Armazenamento gerenciado por software
Cloud Storage	Armazenamento na nuvem
FCP	Protocolo de rede de armazenamento em fibra (Fibre Channel)
CIFS / NFS	Protocolos para compartilhar arquivos (Windows/Linux)
Storage - Sistema para guardar e acessar dados de forma eficiente 

Ambiente Linux (Red Hat e Oracle Linux)
🔹 Instalação, Configuração e Administração
•	Instalação: Durante a instalação, escolhe o tipo de instalação (ex: servidor, workstation) e define as partições do disco rígido. Marcar o tipo de instalação (ex: Servidor) para que as ferramentas de administração sejam instaladas.
•	Configuração Inicial: Após a instalação, configure o hostname, rede (endereço IP, gateway), firewall e segurança (usuários e permissões).
🔹 Configuração de Rede:
•	Arquivo: /etc/sysconfig/network-scripts/ifcfg-eth0 (para configurar interfaces de rede).
•	Comando para reiniciar a rede: systemctl restart network.
🔹 Comandos Comuns:
ps: Ver processos em execução.
top: Monitoramento de processos em tempo real.
df: Ver uso de disco.
du: Ver o tamanho de diretórios.
1.	Gerenciamento de Arquivos e Diretórios
ls = List = Listar arquivos e diretórios
cd = Change Directory = Mudar de diretório
pwd = Print Working Directory = Mostrar diretório atual
cp = Copy = Copiar arquivos
mv = Move = Mover ou renomear arquivos
rm = Remove = Remover arquivos
touch = Tocar = Criar arquivo vazio
mkdir = Make Directory = Criar diretório
rmdir = Remove Directory = Remover diretório vazio
2.	Permissões e Controle de Acesso
chmod = Change Mode = Alterar permissões de arquivos
chown = Change Owner = Alterar proprietário de arquivos
chgrp = Change Group = Alterar grupo de arquivos
3.	Busca e Processamento de Texto
cat = Concatenate = Exibir conteúdo de um arquivo
grep = Global Regular Expression Print = Buscar texto em arquivos
find = Find = Procurar arquivos
man = Manual = Exibir manual de um comando
sort = Sort = Ordenar a saída
wc = Word Count = Contar palavras de um arquivo
head = Head = Exibir primeiras linhas de um arquivo
tail = Tail = Exibir últimas linhas de um arquivo
4.	Processos e Sistema
ps = Process Status = Exibir processos em execução
top = Top = Exibir processos mais ativos
kill = Kill = Matar um processo
bg = Background = Colocar o processo em segundo plano
fg = Foreground = Trazer um processo para o primeiro plano
sleep = Sleep = Atrasar a execução de um comando
5.	Rede e Conectividade
ping = Packet Internet Groper = Testar conectividade de rede
ifconfig = Interface Configuration = Configurar interfaces de rede
netstat = Network Statistics = Exibir estatísticas de rede e conexões
scp = Secure Copy = Copiar arquivos entre máquinas via SSH
df = Disk Free = Ver uso de disco
du = Disk Usage = Ver o tamanho de diretórios
Macete: Para lembrar de comandos de permissões:
chmod = Change Mode
chown = Change Owner
Utilitários	Comandos como ls, cp, mv, grep, etc.
Shell Script	Automatizar tarefas com comandos em sequência
 Microsoft Windows (11 / Server 2022)
Active Directory	Gerencia usuários em redes corporativas
PowerShell	Ferramenta poderosa de automação no Windows
Shell Script: Série de comandos executados no Shell para automatizar tarefas. Usa Bash como o shell mais comum.
🔹 Criação de script: Criar arquivo com extensão .sh e usar o comando chmod +x script.sh para dar permissão exe
🔹 Estrutura básica de um shell script:
#!/bin/bash
echo "Olá, Mundo!"
•	#!/bin/bash: Define o shell a ser usado.
•	echo: Exibe uma mensagem no terminal.
🔹 Comando útil: bash nome_do_script.sh para executar o script.
1. Comandos Básicos de Entrada e Saída
•	echo = Echo = Exibir texto ou variáveis no terminal
•	read = Read = Ler dados do usuário (entrada do teclado)
•	$? = Exit Status = Retorna o código de saída do último comando executado
•	$# = Number of Arguments = Número de parâmetros passados para o script
•	$@ = All Arguments = Todos os parâmetros passados para o script
•	$0 = Script Name = Nome do script ou programa em execução
•	$1, $2, ... = Positional Parameters = Parâmetros passados para o script (como $1, $2, etc.)
•	$(command) = Command Substitution = Executa um comando e substitui seu resultado no script
•	tee = Tee = Lê a entrada e escreve no terminal e em arquivos simultaneamente
2. Controle de Fluxo
Condicionais
•	if = If = Condicional para execução de comandos dependendo de uma condição
•	else = Else = Executar comandos quando a condição do if for falsa
•	elif = Else If = Verificar uma condição alternativa dentro de um if
•	case = Case = Realiza múltiplas verificações em uma variável ou expressão
•	[] = Test = Testa condições dentro de uma expressão
•	[[ ]] = Double Brackets = Testa condições com suporte a expressões regulares e operadores lógicos
Looping (Repetição)
•	for = For = Estrutura de repetição (loop) para iterar sobre uma lista ou intervalo
•	while = While = Estrutura de repetição (loop) que executa enquanto uma condição for verdadeira
•	until = Until = Estrutura de repetição (loop) que executa até uma condição ser verdadeira
•	break = Break = Interrompe a execução de um loop
•	continue = Continue = Pula para a próxima iteração de um loop
Encerramento e Retorno
•	exit = Exit = Encerra a execução do script ou programa
•	return = Return = Retorna de uma função no script
3. Manipulação de Arquivos e Diretórios
•	chmod = Change Mode = Alterar permissões de arquivos dentro do script
•	chown = Change Owner = Alterar proprietário de arquivos dentro do script
•	tar = Tape Archive = Compactar ou descompactar arquivos e diretórios
•	gzip = Gzip = Compactar arquivos com algoritmo gzip
•	gunzip = Gunzip = Descompactar arquivos .gz
•	cut = Cut = Extrair partes específicas de linhas de texto
•	sort = Sort = Ordena linhas de texto
•	uniq = Uniq = Remove linhas duplicadas em uma entrada
•	wc = Word Count = Conta palavras, linhas e caracteres em um arquivo ou entrada
•	df = Disk Free = Ver uso de disco
•	du = Disk Usage = Ver o tamanho de diretórios
4. Processos e Execução
•	ps = Process Status = Exibir processos em execução
•	top = Top = Exibir os processos em tempo real, com informações detalhadas sobre o uso de recursos
•	kill = Kill = Envia um sinal para um processo, normalmente para terminar um processo
•	sleep = Sleep = Pausa a execução do script por um determinado tempo
•	bg = Background = Colocar o processo em segundo plano
•	fg = Foreground = Trazer um processo para o primeiro plano
5. Manipulação de Texto e Strings
•	cat = Concatenate = Exibir conteúdo de um arquivo
•	grep = Global Regular Expression Print = Buscar texto em arquivos
•	awk = Awk = Processamento de texto, ideal para trabalhar com campos e colunas em arquivos
•	sed = Sed = Stream editor, usado para modificar texto em fluxo de dados (substituição, inserção)
•	cut = Cut = Extrair partes específicas de linhas de texto
6. Redirecionamento e Pipes
•	> = Output Redirection = Redireciona a saída de um comando para um arquivo (sobrescreve)
•	>> = Append Output = Redireciona a saída de um comando para um arquivo (acrescenta)
•	< = Input Redirection = Redireciona a entrada de um comando de um arquivo
•	| = Pipe = Redireciona a saída de um comando como entrada de outro comando
7. Comandos Utilitários e Sistema
•	date = Date = Exibe ou define a data e hora atual
•	man = Manual = Exibir manual de um comando
•	kill = Kill = Enviar sinal para um processo, geralmente para finalizá-lo
•	ps = Process Status = Exibir os processos em execução
•	top = Top = Exibir a lista de processos em tempo real, com informações detalhadas sobre o uso de recursos
•	ping = Packet Internet Groper = Testar conectividade de rede
•	ifconfig = Interface Configuration = Configurar interfaces de rede
•	netstat = Network Statistics = Exibir estatísticas de rede e conexões
•	scp = Secure Copy = Copiar arquivos entre máquinas via SSH
Microsoft Windows (Windows 11 - desktop e Windows Server 2022 - servidores)
🔹 Instalação e Configuração:
•	Windows 11: o sistema pede a chave de produto (product key) e a configuração da conta Microsoft.
•	Requisitos: Ter as configurações mínimas (ex: TPM 2.0, Secure Boot).
•	Configuração Inicial: Após a instalação, definir preferências de usuário, rede (Wi-Fi ou Ethernet), atualizações automáticas e privacidade.
•	Windows Server 2022: A instalação é feita de forma similar, mas configura aspectos voltados para servidores, como: Servidor de Domínio, Active Directory, Pasta Compartilhada, entre outros.
Macete: No Windows Server 2022, seleciona "Server with Desktop Experience" para uma interface gráfica.

Active Directory: tecnologia da Microsoft para gerenciar redes e controlar o acesso a recursos de rede.
🔹 Comandos principais:
•	dnsmgmt.msc: Para gerenciar o DNS.
•	dcpromo: Para promover um servidor como Controlador de Domínio (antigo, no novo Windows Server 2022 é configurado pelo Server Manager).
•	Active Directory Users and Computers: Interface gráfica para gerenciar usuários e grupos.
1. Comandos para Gerenciamento de Usuários
•	New-ADUser = Criar Usuário = Cria um novo usuário no Active Directory
•	Set-ADUser = Configurar Usuário = Modifica as propriedades de um usuário existente no AD
•	Get-ADUser = Obter Usuário = Obtém informações sobre um ou mais usuários do AD
•	Remove-ADUser = Remover Usuário = Exclui um usuário do Active Directory
•	Unlock-ADAccount = Desbloquear Conta = Desbloqueia uma conta de usuário que foi bloqueada
•	Enable-ADAccount = Habilitar Conta = Ativa uma conta de usuário desativada
•	Disable-ADAccount = Desabilitar Conta = Desativa uma conta de usuário
•	Set-ADUserPassword = Alterar Senha = Modifica a senha de um usuário no AD
2. Comandos para Gerenciamento de Grupos
•	New-ADGroup = Criar Grupo = Cria um novo grupo de usuários no AD
•	Set-ADGroup = Configurar Grupo = Modifica as propriedades de um grupo existente no AD
•	Get-ADGroup = Obter Grupo = Obtém informações sobre um grupo do AD
•	Add-ADGroupMember = Adicionar Membro ao Grupo = Adiciona usuários a um grupo no AD
•	Remove-ADGroupMember = Remover Membro do Grupo = Remove usuários de um grupo no AD
•	Remove-ADGroup = Remover Grupo = Exclui um grupo do Active Directory
3. Comandos para Gerenciamento de Unidades Organizacionais (OUs)
•	New-ADOrganizationalUnit = Criar OU = Cria uma nova unidade organizacional no AD
•	Set-ADOrganizationalUnit = Configurar OU = Modifica as propriedades de uma unidade organizacional existente
•	Get-ADOrganizationalUnit = Obter OU = Obtém informações sobre uma unidade organizacional no AD
•	Remove-ADOrganizationalUnit = Remover OU = Exclui uma unidade organizacional do Active Directory
4. Comandos para Gerenciamento de Computadores
•	New-ADComputer = Criar Computador = Adiciona um novo computador ao Active Directory
•	Set-ADComputer = Configurar Computador = Modifica as propriedades de um computador existente no AD
•	Get-ADComputer = Obter Computador = Obtém informações sobre um computador do AD
•	Remove-ADComputer = Remover Computador = Exclui um computador do Active Directory
5. Comandos para Gerenciamento de Domínios e Florestas
•	New-ADDomain = Criar Domínio = Cria um novo domínio no Active Directory
•	Get-ADDomain = Obter Domínio = Obtém informações sobre um domínio no AD
•	Set-ADDomain = Configurar Domínio = Modifica as propriedades de um domínio existente no AD
•	Get-ADForest = Obter Floresta = Obtém informações sobre a floresta do Active Directory
•	Set-ADForest = Configurar Floresta = Modifica as propriedades da floresta no AD
6. Comandos de Consulta e Pesquisa
•	Get-ADUser = Obter Usuário = Consulta um usuário ou grupo no AD
•	Get-ADGroupMember = Obter Membros do Grupo = Obtém os membros de um grupo no AD
•	Search-ADAccount = Pesquisar Conta = Pesquisa contas de usuários, computadores ou grupos no AD
•	Get-ADObject = Obter Objeto = Obtém qualquer objeto do Active Directory (usuários, grupos, computadores, etc.)
7. Comandos para Gerenciamento de Senhas
•	Set-ADUserPassword = Alterar Senha = Modifica a senha de um usuário no AD
•	Reset-ADUserPassword = Redefinir Senha = Redefine a senha de um usuário no Active Directory
•	Get-ADUserPasswordPolicy = Obter Política de Senha = Exibe a política de senhas configurada no AD
8. Comandos de Gerenciamento de Replicação
•	Get-ADReplicationPartner = Obter Parceiro de Replicação = informações sobre parceiros de replicação no AD
•	Get-ADReplicationFailure = Obter Falha de Replicação = Exibe falhas de replicação no Active Directory
•	Sync-ADReplication = Sincronizar Replicação = Força a sincronização entre controladores de domínio no AD
9. Comandos para Gerenciamento de Trusts (Confianças)
•	New-ADTrust = Criar Trust = Cria um novo relacionamento de confiança entre domínios
•	Get-ADTrust = Obter Trust = Obtém informações sobre as confianças existentes no Active Directory
•	Remove-ADTrust = Remover Trust = Exclui um relacionamento de confiança no AD
10. Comandos de Relatórios e Auditoria
•	Get-ADUser -Filter * = Listar Usuários = Exibe todos os usuários do Active Directory
•	Get-ADGroup -Filter * = Listar Grupos = Exibe todos os grupos do Active Directory
•	Get-ADAuditPolicy = Obter Política de Auditoria = Exibe as configurações de auditoria no AD
•	Get-ADLogonStatistics = Obter Estatísticas de Logon = Exibe informações de logon de usuários no AD
11. Comandos para Gerenciamento de Política de Grupo (GPO)
•	New-GPO = Criar GPO = Cria um novo Objeto de Política de Grupo (GPO) no AD
•	Get-GPO = Obter GPO = Obtém informações sobre um GPO no Active Directory
•	Set-GPO = Configurar GPO = Modifica um GPO existente no AD
•	Remove-GPO = Remover GPO = Exclui um GPO do Active Directory
12. Comandos de Sincronização com o Azure AD (Se For Usando Azure AD Connect)
•	Start-ADSyncSyncCycle = Iniciar Sincronização = Inicia um ciclo de sincronização do Azure AD Connect com o AD local
•	Get-ADSyncScheduler = Obter Agendador de Sincronização = Exibe o status e a configuração do agendador de sincronização do AD Connect
•	Test-ADSync = Testar Sincronização = Testa a configuração e o status da sincronização com o Azure AD
Powershell: Ferramenta de linha de comando e automação de tarefas no Windows.
🔹 Comandos comuns:
•	Get-Help: Para obter ajuda sobre comandos.
•	Get-Process: Ver todos os processos em execução.
•	Get-Service: Ver todos os serviços no sistema.
•	Set-Service: Modificar propriedades de um serviço (ex: iniciar, parar).
•	Get-EventLog: Ver logs de eventos.
•	Executar scripts: Comando powershell -ExecutionPolicy RemoteSigned p/ permitir execução scripts
•	No PowerShell, os cmdlets seguem formato verbo-substantivo: Get-Process, Set-Service, New-Item.
VMWare: ferramenta para virtualização de servidores
🔹 Máquina Virtual (VM): Máquina que roda em cima de um servidor físico, usando virtualização para funcionar.
•	Hypervisor: Software (mestre) que controla as VMs. Existem dois tipos principais:
•	Tipo 1 (bare-metal): Roda diretamente no hardware, como o VMware ESXi.
•	Tipo 2 (hosted): Roda dentro de um sistema operacional, como VMware Workstation.
🔹 Configuração 
1.	Instalação do VMware ESXi (Vira fábrica de VMs):
•	Instalar o ESXi diretamente no hardware do servidor (é uma instalação bare-metal).
•	Configuração de rede e armazenamento: Definir endereços IP e conectar a storage (armazenamento).
•	Após a instalação, pode acessar a interface do vSphere Client para gerenciamento.
2.	Configuração das VMs:
•	Após instalar o ESXi, cria máquinas virtuais que rodarão sobre esse sistema.
•	Define os recursos da VM (memória, CPU, armazenamento).
🔹 Administração do VMware
1.	vSphere Client - a janela para gerenciar suas máquinas virtuais: Ferramenta principal para gerenciar VMs no VMware. Acessa via navegador/app, configurando VMs, redes, armazenamento e mais.
2.	Gerenciamento de VMs:
•	Ligar/Desligar VMs com facilidade.
•	Snapshots: Tire instantâneos das VMs (como uma foto do estado da VM).
•	Migração de VMs: Com vMotion, é possível mover VM de um host p/ outro sem parar a VM.
1.	VMware High Availability (HA) Se o host cair, a VM se levanta em outro host: as VMs sejam movidas automaticamente para outro servidor, sem tempo de inatividade.
2.	Cluster: Para usar HA, precisa configurar um cluster de servidores. O vCenter Server gerencia esse cluster e possibilita a migração automática das VMs.
3.	Fault Tolerance (FT) a replica está sempre pronta (Tolerância a Falhas) garante que uma VM tenha réplica ativa em outro host. Caso o host primário falhe, a réplica toma o controle sem perder dados.
Remote (Acesso Remoto): Permite que o usuário acesse um desktop ou servidor de outro local.Protocolos comuns:
•	RDP (Remote Desktop Protocol): Usado no Windows.
•	SSH (Tela preta): Usado para Linux.
•	VNC (Virtual Network Computing): Usado em sistemas variados como Linux e Windows.
Desktop Services (Serviços de Desktop)
•	VDI (Virtual Desktop Infrastructure): permite desktop seja virtualizado no servidor e acessado de qualquer dispositivo. Exemplo: VMware Horizon, Citrix XenDesktop.
•	RDS (Remote Desktop Services): em servidores Windows para fornecer acessos simultâneos a múltiplos usuários.
•	Máquinas Virtuais (VMs): São ambientes isolados que emulam um computador físico completo. Cada VM tem seu próprio sistema operacional.
•	Contêineres: + leves que VMs. Compartilham o SO do host, mantêm aplicação e dependências isoladas.
•	Orquestração de Contêineres: Ferramentas para gerenciar e automatizar a execução de contêineres.
•	Docker: Plataforma para criar, distribuir e executar contêineres.
•	Docker Images: São os modelos dos contêineres.
•	Docker Containers: São instâncias de imagens. 
Comando básico: docker run <nome_da_imagem> para executar uma imagem.
•	Kubernetes: Plataforma p/ orquestrar (gerenciar/automatizar) contêineres em clusters de máquinas
•	Pods: Unidades de execução no Kubernetes, geralmente contendo um ou mais contêineres.
•	kubectl: Comando utilizado para interagir com o Kubernetes.
•	Rancher: Plataforma facilita o  gerenciamento de clusters Kubernetes.
Ferramentas de Orquestração de Automação de Infraestrutura:
🔹 Ansible: Ferramenta de automação de TI baseada em playbooks (receitas p/ conf inst ou criar infra).
🔹 Puppet: Outra ferramenta de automação, focada em modelagem e gestão de configurações.
Docker é para criar contêineres, Kubernetes é para gerenciar contêineres, e Rancher é para gerenciar clusters de Kubernetes. Com Ansible e Puppet, automatiza a configuração de infraestrutura.

Alta Disponibilidade (HA): Capacidade do sistema operar de forma contínua, com mínimo de inatividade possível.
Tolerância a Falhas (FT): Capacidade do sistema continuar funcionando mesmo em falha em um dos componentes.
Indicadores de Disponibilidade
🔹 MTBF (Mean Time Between Failures): Confiabilidade (quanto mais tempo entre falhas, melhor).
•	Mede o tempo médio entre falhas de um sistema ou componente.
🔹 MTTR (Mean Time to Repair): Recuperação (quanto menos tempo para recuperar, melhor).
•	Mede o tempo médio necessário para reparar um sistema após uma falha.
🔹 MTTF (Mean Time to Failure): Vida útil do componente (sem reparo possível, só substituição).
•	Mede o tempo médio até a falha de um componente não reparável.
MTBF = tempo entre falhas; MTTR = tempo para reparar; MTTF = tempo até falha.
Clusterização: Técnica de agrupar múltiplos servidores ou componentes p/ que funcionem como um único sistema.
•	Garantir alta disponibilidade e balanceamento de carga. Se um servidor falhar, outro assume.
🔹 Cluster ativo-ativo: Todos os servidores estão ativos e compartilhando a carga de trabalho. 
🔹 Cluster ativo-passivo: Um servidor está ativo, enquanto o outro fica como reserva, pronto para assumir em caso de falha. Um servidor espera enquanto o outro trabalha.
Balanceamento de Carga: distribuir requisições/tarefas entre múltiplos servidores, garantindo não sobrecarga.
🔹 Algoritmos de balanceamento:
•	Round Robin: Distribui as requisições de forma circular entre os servidores. Revezamento.
•	Least Connections: Envia a requisição p/ servidor com - conexões ativas. Servidor + livre recebe.
•	IP Hash: Usa o endereço IP do cliente para determinar o servidor que vai atender a requisição.
Failover: Processo de transição automática p/ sistema reserva quando o principal falha. Evitar a queda do serviço.
🔹 Failover transparente: O usuário não percebe que houve uma falha, pois o serviço continua.
🔹 Failback: Depois que o problema é resolvido, o sistema volta a operar normalmente no servidor principal.
Servidores de Aplicação: Plataformas executam e gerenciam aplicações em um ambiente. Objetivo suporte a aplicações 
🔹 Análise de Desempenho da Rede
•	Envolve monitorar o fluxo de dados e os tempos de resposta entre o servidor e o cliente.
•	Ferramentas comuns:
•	Apache Bench (ab): Ferramenta para testar o desempenho do servidor web Apache.
•	JMeter: Ferramenta popular para simulação de carga e testes de desempenho.
•	Wireshark: Analisador de pacotes de rede para examinar o tráfego.
Para analisar o desempenho da rede, use ferramentas de teste de carga como JMeter ou Apache Bench.

📌 Gerenciamento de Usuários
🔹 JBoss: Utiliza roles (regras) e grupos para gerenciar permissões de usuários.
•	Exemplo: Configuração de roles no application-users.properties e application-roles.properties.
🔹 Apache HTTP Server: Pode usar o mod_auth_basic para autenticação, geralmente combinada com arquivos .htpasswd para gerenciar os usuários e suas permissões.
•	Comando para criar usuário: htpasswd -c /path/to/.htpasswd username.
🔹 IIS (Internet Information Services): O gerenciamento de usuários é feito diretamente através do Active Directory ou controle local de usuários do Windows.
No JBoss, configura roles no application-users.properties. No Apache, usa htpasswd. No IIS, o gerenciamento é feito pelo Active Directory.
🔹 Administração e configuração: Instalar, configurar e otimizar o desempenho do servidor.
🔹 Análise de desempenho: Ver uso de CPU, memória, conexões etc.
🔹 Gerenciamento de usuários: Criar, modificar e controlar permissões.
🔹 Logs de serviços: Verificar arquivos de log para entender falhas ou atividades.
Configuração, Administração e Logs de Serviços
🔹 JBoss produto Had Hat (WildFly - open): Full JEE (Java) – Enterprise Empresa/Comercial
•	Arquivo de configuração: standalone.xml ou domain.xml, onde configura recursos do servidor.
1.	Standalone = Coisa única que roda em um único lugar. 
•	Logs: O JBoss grava logs em standalone/log/server.log. Usa tail -f p/ monitorar o log em tempo real.
•	Reiniciar: ./bin/standalone.sh -c standalone.xml.
🔹 Apache HTTP Server:
•	Arquivo de configuração: httpd.conf, onde define diretivas como DocumentRoot, ServerName, etc.
•	Logs: Logs de acesso e erro ficam em /var/log/apache2/access.log e error.log.
•	Reiniciar: sudo service apache2 restart (Ubuntu) ou sudo systemctl restart httpd (CentOS).
🔹 IIS (Internet Information Services):
•	Arquivo de configuração: Configurações de sites e serviços são feitas através do IIS Manager ou arquivos de configuração XML como applicationHost.config.
•	Logs: O IIS armazena logs em C:\inetpub\logs\LogFiles.
•	Para reiniciar o IIS: Use iisreset.
•	Logs: Em LogFiles, você tem registros detalhados de erros e acessos.
JBoss usa standalone.xml e logs estão em server.log. Apache usa httpd.conf e logs estão em access.log e error.log. IIS usa o IIS Manager e logs ficam em LogFiles.

Tabela de Macetes para Sistemas Operacionais
Instalação Linux	Durante a instalação, escolha o tipo de instalação (ex: Servidor).	Não se esqueça de configurar o hostname e a rede.
Comandos Linux	ls = listar arquivos, cd = mudar diretório.	chmod = mudar permissão, chown = mudar proprietário.
Shell Script	Crie arquivos .sh e use chmod +x para torná-los executáveis.	echo para exibir mensagens.
Instalação Windows 11	Durante a instalação, insira a chave de produto.	Atente-se ao TPM 2.0 e Secure Boot para compatibilidade.
Active Directory	Use Active Directory Users and Computers para gerenciar usuários.	dcpromo para promover um servidor a controlador de domínio (versões antigas).
Powershell	Get-Help para consultar comandos.	Cmdlets: Get-, Set-, New-.

Máquina Virtual (VM)	VMs são como computadores independentes dentro de um servidor físico.	"Máquinas virtuais são falsas, mas funcionam de verdade."
Hypervisor	O hypervisor é o mestre das VMs.	hypervisor é mestre controla as VMs.
Instal VMware ESXi	ESXi instalado diretamente no hardware servidor	ESXi, o servidor uma fábrica de VMs
vSphere Client	É a ferramenta principal para gerenciar VMs.	vSphere Client: a janela para suas VMs.
Snapshots	São como fotos do estado das VMs.	como uma foto das suas VMs.
vMotion	Mover uma VM de host para outro sem parar a VM.	vMotion as VMs movem sem notar
Alta Dispon (HA)	Se um host falhar, a VM é movida automaticamente.	Se o host cair, a VM levanta em outro
Fault Tolera (FT)	Replica uma VM em outro host, sem perda de dados.	a replica está sempre pronta.

Acesso Remoto (Remote)	Use RDP para Windows e VNC para sistemas variados.	RDP para acessar Windows, VNC para sistemas variados.
Serviços de Desktop (VDI/RDS)	VDI virtualiza o desktop completo, RDS compartilha.	o desktop está na nuvem. Com RDS, múltiplos usuários em um servidor.
Máquinas Virtuais e Contêineres	VMs são completos, contêineres são mais leves.	VMs = computadores completos, contêineres = caixas isoladas.
Docker e Kubernetes	Docker para criar contêineres, Kubernetes para gerenciar.	Docker para criar, Kubernetes para gerenciar. Rancher para clusters.
CI/CD	CI integra/testa, CD entrega automaticamente.	Com CI, você integra o código. Com CD, você entrega o código.
Git	git init para inicializar, git push para enviar alterações.	Com Git, controle suas alterações e push para o GitHub.

MTBF (Mean Time Between Failures)	MTBF = tempo entre falhas.
MTTR (Mean Time to Repair)	MTTR = tempo para reparar.
MTTF (Mean Time to Failure)	MTTF = tempo até falha de comp ñ repara

Análise de Desempenho da Rede	Ferramentas como JMeter, Apache Bench, e Wireshark.
Gerenciamento de Usuários (JBoss)	No JBoss, use roles em application-users.properties.
Gerenciamento de Usuários (Apache)	Use htpasswd para gerenciamento de usuários no Apache.
Gerenciamento de Usuários (IIS)	O IIS usa Active Directory ou controle local de usuários.
Configuração do JBoss	Arquivo de configuração: standalone.xml ou domain.xml.
Configuração do Apache	Arquivo de configuração: httpd.conf.
Configuração do IIS	Configurações feitas pelo IIS Manager.
Logs do JBoss	Logs estão em server.log dentro de standalone/log.
Logs do Apache	Logs ficam em access.log e error.log.
Logs do IIS	Logs ficam em C:\inetpub\logs\LogFiles.

