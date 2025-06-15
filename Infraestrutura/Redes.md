Cabeamento Estruturado: Infraestrutura de cabos usada para transmissão de dados. Segue padrões que garantem desempenho e confiabilidade nas redes de comunicação.
🔹 Categorias de Cabeamento (segundo a ABNT NBR 14565:2019):
1.	Cat 5 = Mais lento, até 100 Mbps
•	Velocidade: Até 100 Mbps (Fast Ethernet).
•	Uso: Redes 10/100 Mbps. Não recomendado para redes modernas de alta velocidade.
2.	Cat 5e: Mais rápido, até 1 Gbps
•	Velocidade: Até 1 Gbps (Gigabit Ethernet).
•	Uso: Redes de até 1 Gbps. Maior performance e menor interferência que o Cat 5.
3.	Cat 6: Rápido, até 10 Gbps, em distâncias curtas.
•	Velocidade: Até 10 Gbps em distâncias curtas (até 55 metros).
•	Uso: Ideal para redes de alta velocidade e servidores. Melhor desempenho que o Cat 5e.
4.	Cat 6ª: Rápido e longo, 10 Gbps até 100 metros
•	Velocidade: Até 10 Gbps em distâncias de 100 metros.
•	Uso: Redes de alta performance e ambientes que exigem grande largura de banda.

Fibra Óptica: Usa luz para transmitir dados, oferecendo alta velocidade e grande capacidade de banda. Menos suscetível a interferências e atenuações do que os cabos de cobre.
🔹 Fibra Óptica Monomodo: Longa distância, feixe único de luz
•	Características: Transmite luz em um único feixe. Ideal para longas distâncias.
•	Uso: Conexões de longa distância, como entre cidades ou campi.
•	Diâmetro: Menor (cerca de 8 a 10 micrômetros).
•	Velocidade: Suporta altas taxas de transmissão.
1.	Tipos de Fibra Multimodo (OM)
1.	OM1 (Laranja)
2.	OM2 (Laranja)
3.	OM3 (Aqua/Azul esverdeado)
4.	OM4 (Aqua/Roxo claro)
5.	OM5 (Verde-limão)
6.	OM3 e OM4 para Data Center locais
7.	OM4/OM5 para cabeamento horizontal com switches de alto desempenho.
🔹 Fibra Óptica Multimodo: Distância curta, múltiplos feixes de luz
•	Características: Transmite luz em múltiplos feixes (modos). Ideal para distâncias curtas.
•	Uso: Redes locais ou conexões de curta distância.
•	Diâmetro: Maior (50 a 100 micrômetros).
•	Velocidade: Suporta taxas menores de transmissão em comparação com o monomodo.
🔹 Comutação por circuito:
•	Meio dedicado de transmissão de dados entre dois pontos. 
•	Qualidade de Serviço (QoS) alta e garantida, Latência baixa e constante. Tempo real
🔹 Comutação por pacotes:
•	Dados divididos e enviados independentemente. Cada pacote pode seguir um caminho diferente, cada um com dados e informações de roteamento e no final junta tudo.
•	Tamanho un. Variável, eficiência canal alta, QoS baixa, latência varia, flex de roteamento alta.
🔹 Comutação por células:
•	Usa “blocos” fixos (células) de dados.
•	Utilizadas principalmente em redes ATM (Asynchronous Transfer Mode), onde a transmissão de dados é feita por células fixas de 53 bytes.

PAN (Personal Area Network): Até 10m, Bluetooth, USB, IrDA (dispositivos pessoais)
LAN (Local Area Network): Até 100m, Ethernet (redes domésticas, escritórios)
MAN (Metropolitan Area Network): Até 50km, Fibra ótica, Ethernet Metropolitano (conectar prédios na cidade)
WAN (Wide Area Network) - ): > 50km, Fibra ótica, satélite (conexão entre cidades, países)
WPAN (Wireless Personal Area Network) - Rede pessoal sem fio (como Bluetooth) (IEEE 802.15)
WLAN (Wireless Local Area Network) - Rede local sem fio, como Wi-Fi (IEEE 802.11)
WMAN (Wireless Metropolitan Area Network) - Rede metropolitana sem fio, como WiMax (IEEE 802.16)
WWAN (Wireless Wide Area Network) - Rede ampla sem fio, como redes celulares

 Modelo OSI (Open Systems Interconnection): Como as redes devem ser projetadas e comunicadas.
 🔹 Camadas OSI: 7 camadas. 
1.	Física: Transmissão de dados brutos, como cabos e sinais elétricos. (Fibra, UTP, Bluetooth, USB)
2.	Enlace de dados: Controle de erros e fluxo entre dispositivos mesma rede local(Ethernet, Wi-Fi, PPP, MAC, VLAN)
a.	end físico, controle de acesso à mídia, comutação de dados em redes locais ou exclusão de erros
3.	Rede: Endereçamento e roteamento de pacotes de dados (IP, ICMP, ARP, RIP, OSPF, BGP).
a.	roteamento, endereçamento IP, sub-redes, ou protocólos de roteamento (como o IP)
4.	Transporte: Controle de fluxo e segmentação de dados (TCP, UDP).
a.	confiabilidade, controle de fluxo, divisão de dados em pacotes ou prot de comunicação conf (TCP)
5.	Sessão: Gerencia diálogos e conexões entre aplicações. (NetBIOS, RPC, PPTP)
a.	ger de sessão de comunicação ou estabelecimento e controle de conexões entre disp ou sistemas
6.	Apresentação: Formatação e codificação de dados (SSL/TLS, JPEG, MP3, GIF, ASCII).
a.	codificação, criptografia, compressão de dados ou formato de arquivos
7.	Aplicação: Interação com o usuário e as aplicações (HTTP, HTTPS, FTP, SMTP, POP3, IMAP, DNS).
Camada 1 - Física: Cabo, Wi-Fi, Placa de rede (hardware de comunicação)
Camada 2 - Enlace de Dados: Ethernet, Switches, MAC Address (transmissão de dados local)
Camada 3 - Rede: Roteadores, IP, ICMP (endereçamento e roteamento entre redes)
Camada 4 - Transporte: TCP, UDP, Portas (controle e entrega dos dados entre sistemas)
Camada 5 - Sessão: RPC, NetBIOS (gerenciamento de sessões de comunicação)
Camada 6 - Apresentação: SSL/TLS, JPEG, ASCII (formatação, criptografia, compressão)
Camada 7 - Aplicação: HTTP, FTP, DNS, e-mail (uso final de rede, interação com o usuário)

 Modelo TCP/IP (Transmission Control Protocol/Internet Protocol)
 🔹 Camadas TCP/IP: 4 camadas. 
1 - Acesso à Rede: Física+enlace. Define como dados são transmitidos (Ethernet, Wi-Fi, PPP, MAC, VLAN).
2 - Internet: Endereçamento e roteamento dos pacotes (IP, ICMP, ARP, OSPF, BGP).
3 - Transporte: Garantia de entrega e controle de fluxo (TCP, UDP).
4 - Aplicação: Protocolos para interação com o usuário final (HTTP, HTTPS, FTP, DNS, SMTP, POP3, SNMP).
Acesso à rede (camadas 1 e 2 do OSI) / Internet (camada 3 do OSI) / Transporte (camada 4) / Aplicação (camadas 5, 6,7 )

Protocolos de Comunicação TCP/IP (TCP = Confiabilidade, IP = Roteamento)
Protocolos de roteamento - São usados pelos roteadores para escolher o melhor caminho para enviar os dados.
RIP	Interior (IGP)	Usa número de “saltos” (hops). Simples e antigo.
OSPF	Interior (IGP)	Mais inteligente: calcula o caminho mais rápido com base em custo.
BGP	Exterior (EGP)	Controla o tráfego entre grandes redes, como operadoras (roteia a internet).
VRRP	Redundância	Deixa um roteador de reserva automática.
HSRP	Redundância (Cisco)	Mesma ideia do VRRP, mas exclusivo da Cisco.
Protocolos de comunicação 
•	TCP/IP: Conjunto de regras pra comunicação na internet.
•	TCP: Garante entrega, verifica se chegou certinho (como sedex com aviso de entrega).
•	IP: Define o endereço do remetente e destinatário (como o CEP).
RDMA over Converged Ethernet (RoCE) - RoCE = RDMA sobre Ethernet, alto desempenho, baixa latência
•	Permite a transferência de dados de alta velocidade entre computadores, usando Ethernet. Usa RDMA (Remote Direct Memory Access), que permite o acesso direto à memória entre máquinas, sem a necessidade de intervenção do processador.
•	Obj: Melhorar a latência e o desempenho das redes em ambientes de computação de alto desempenho.
MTU (Maximum Transmission Unit) - Máximo de dados em um pacote, sem fragmentação
•	Garantir que os pacotes não sejam fragmentados na transmissão. O MTU padrão em Ethernet é 1500 bytes.
Jumbo Frames= Pacotes grandes para redes rápidas.  O tamanho até 9000 bytes. Eles são usados para melhorar a eficiência em redes de alta performance.

Hub: Camada 1 (Física), repete sinais para todas as portas, gera colisões, obsoleto
Repetidor: Camada 1 (Física), regenera/amplifica sinais para estender alcance, não filtra dados
Bridge (Ponte): Camada 2 (Enlace), interconecta segmentos, filtra tráfego por MAC, reduz colisões
Switch: Camada 2 (Enlace), comutação de quadros, aprende endereços MAC, encaminha para porta correta, reduz colisões
Roteador: Camada 3 (Rede), encaminhamento de pacotes entre redes, usa endereços IP, determina melhor caminho
Gateway: Camadas superiores (4 a 7), interconecta redes com protocolos diferentes, faz tradução de protocolos

IPv4: (ex: 192.168.0.1)
•	Endereço de 32 bits, representado em 4 octetos 
•	Fórmula: A4.B4.C4.D4 (quatro números de 0 a 255).
•	Unicast/Broadcast/Multicast, fragmentação por roteadores/hosts, cabeçalho 20-60 bytes, Configuração Manual/DHCP
IPv6: (ex: 2001:0db8:85a3::8a2e:0370:7334)
•	Endereço de 128 bits, representado em 8 blocos de 4 caracteres hexadecimais 
•	Unicast/Anycast/Multicast, fragmentação apenas por hosts, cabeçalho fixo 40 bytes, Autoconfiguração automática (SLAAC), Não existe Broadcast (substituído por multicast)
Campo	IPv4	IPv6
Comprimento do end	32 bits (4 bytes)	128 bits (16 bytes)
Formato	Quatro octetos (ex: 192.168.1.1)	Oito blocos de quatro dígitos hexadecimais (ex: 2001:0db8:85a3:0000:0000:8a2e:0370:7334)
Endereço de rede	Prefix e sufixo pela másc de rede	Prefixo de rede (geralmente com notação CIDR)
Classe de Endereço	Classes A, B, C, D, E (especificação de end)	Não possui (endereçamento é hierárquico)
Cabeçalho	20 a 60 bytes, campos como versão, comprimento, etc.	Cabeçalho fixo de 40 bytes, campos como versão, prioridade, etc.
End de Broadcast	Suporta (enviar para todos)	Não há broadcast. Utiliza multicast e unicast
Sub-redes	máscara (ex: 255.255.255.0)	Utiliza prefixo CIDR (ex: 2001:0db8::/32)
Checksum	Possui um campo no cabeçalho	Não possui (integridade garantida por outros meios)
Suporte a NAT 	Suporta para permitir a tradução entre endereços 	Não precisa, possui uma quantidade enorme de endereços
Segurança	opcional e via IPsec 	O IPsec é obrigatório e parte integrante do protocolo
Fragmentação	Suporta de pacotes (pelos roteadores e hosts)	Fragmentação ocorre apenas no host de origem, não nos roteadores
Configuração Automática	configurado automaticamente (DHCP) ou manualmente	Suporte à configuração automática via SLAAC (Stateless Address Auto Configuration)
Cabeçalho IPv4 - Visão Geral
Versão	4 bits	0100 (IPv4).
IHL	4 bits	Comprimento do cabeçalho em palavras de 4 bytes.
Tipo de Serviço	8 bits	Contém o DSCP e ECN.
Comprimento Total	16 bits	Tamanho total do pacote, cabeçalho + dados.
Identificação	16 bits	Identifica fragmentos de pacotes.
Flags	3 bits	Informações sobre fragmentação (DF, MF).
Offset de Fragmentação	13 bits	Posição do fragmento dentro do pacote original.
TTL	8 bits	Tempo de vida do pacote.
Protocolo	8 bits	Identifica o protocolo de camada superior (TCP, UDP, etc.).
Checksum	16 bits	Verificação de integridade do cabeçalho.
Endereço de Origem	32 bits	Endereço IP de origem do pacote.
Endereço de Destino	32 bits	Endereço IP de destino do pacote.
Opções	0-40 bytes	Campo opcional para configurações especiais.
Preenchimento	Variável	Preenchimento para garantir que o cabeçalho tenha um comprimento múltiplo de 32 bits.
Classe A = 1 a 127 / B = 128 a 191 / C = 192 a 223/ D = 224 a 239 / A = 00000000 (0 em decimal) / B = 10000000 (128 em decimal)/ C = 11000000 (192 em decimal)/ D = 11100000 (224 em decimal) / E = 111100000 (240 em decimal)
* Lembrar de contar com o número 0

Segmentação: Dividir dados em pacotes menores para facilitar a transmissão em redes. Cada pacote tem cabeçalho com informação endereço de origem e destino, nº de sequência e informações de controle.pacote (TCP) ou datagrama (UDP).
Endereçamento: Utiliza endereços IP-CPF (IPv4 ou IPv6) para identificar dispositivos e facilitar o roteamento na rede.
CIDR (Classless Inter-Domain Routing) = Flexibilidade no endereçamento de rede
CIDR	Nº de IPs disponíveis	Máscara
/24	256 (254 utilizáveis)	255.255.255.0
/16	65.536	255.255.0.0
/30	4 (2 utilizáveis)	255.255.255.252
 Protocolos 
•	IPSec (Internet Prot Security): Prot de seg para criptografar e autenticar pacotes de dados IP, usado VPNs.
 Macete: IPSec = Segurança para comunicação IP. Camada de rede (IP). Usado VPNs.
- 2 formas de funcionamento:
•	Modo Transporte – Protege apenas a carga útil (dados) do pacote IP.
•	Modo Túnel – Protege o pacote inteiro, criando um túnel seguro entre dois dispositivos.
- Componentes principais:
•	AH (Authentication Header) – Garante autenticidade e integridade dos dados.
•	ESP (Encapsulating Security Payload) – Gar aut, integridade e criptografia dos pacotes.
•	IKE (Internet Key Exchange) – Gerencia chaves criptográficas.
•	HTTPS (HTTP Secure): Versão segura do HTTP, usando SSL/TLS para criptografia.
•	O navegador solicita conexão HTTPS.
•	O servidor envia um certificado digital (SSL/TLS).
•	O navegador valida o certificado.
•	Uma conexão criptografada é estabelecida.
Evita ataques de interceptação (Man-in-the-Middle).
Protocolo	Segurança Camada	Aplicação Principal	Proteções Oferecidas
TLS/SSL	Camada de transporte	Navegadores, e-mails, VPNs	Criptografia e autenticação
IPsec	Camada de rede	VPNs e comunicação entre redes	Criptografia, autenticação e integridade
HTTPS	Camada de aplicação	Navegação na web	Segurança na comunicação web

Protocolo	Função Simples	Exemplo
TCP	Garante entrega dos dados	Acesso a sites, e-mails
UDP	Rápido, mas sem garantia	Vídeos ao vivo, jogos online
ICMP	Testa conexão	Comando ping
IPSec	Segurança para IP (criptografia)	VPNs seguras
ARP	Descobre MAC a partir do IP	Comunicação dentro da LAN
SSH	Acesso remoto seguro	Administrar servidores Linux
SMTP	Envio de e-mails	Envia e-mails do Outlook
HTTP	Acesso a sites	Sites comuns (sem segurança)
HTTPS	Acesso a sites com segurança	Sites com cadeado no navegador
SSL/TLS	Criptografia na rede	Protege HTTPS, e-mails etc.
FTP	Transferência de arquivos	Enviar arquivos pra servidores
NFS	Acesso remoto a arquivos em Linux	Compartilhar pastas entre servidores
SMB	Acesso remoto a arquivos no Windows	Compartilhar pasta pelo Explorador
LDAP	Acesso a diretórios de usuários	Login no Active Directory
DNS	Traduz nomes pra IPs	google.com → 142.250.190.14
DHCP	Distribui IP automaticamente	Quando você conecta no Wi-Fi
IMAP	Ler e-mail no servidor	Ver e-mail no Gmail de qualquer lugar
•	MPLS (Multiprotocol Label Switching): Cria rotas mais rápidas e privadas dentro de redes grandes.
•	Muito usado por empresas. Usa etiquetas (labels) em vez de só IP.
•	SD-WAN (Software-Defined WAN): WAN gerenciada por software. Centralizada e Flexível.
•	Mais inteligente e barata que MPLS.
•	Usa várias conexões (internet comum + links dedicados) de forma eficiente.
NAT (Network Address Translation): Usado para modificar os endereços IP de pacotes de dados, permitindo que múltiplos dispositivos em 1 rede local compartilhem 1 único endereço IP público para comunicar com internet.
🔹 Tipo: Static NAT: Mapeia um único endereço IP privado para um único endereço IP público.
•	Dynamic NAT: Mapeia múltiplos endereços IP privados para um grupo de endereços IP públicos.
•	Port Address Translation (PAT): Também conhecido como overloading, permite que vários dispositivos compartilhem um único IP público ao mapear diferentes portas de origem.
Tipo	IP usado	Exemplo
NAT	IP por IP	1 IP interno → 1 IP externo
PAT	IP + portas	Vários IPs internos → 1 IP externo com portas diferentes
Spanning Tree Protocol (STP IEEE 802.1D): camada 2 (enlace de dados) usado em redes Ethernet p/ evitar looping de rede. 
•	Cria a árvore de expansão (spanning tree) onde só uma rota ativa é escolhida para o tráfego entre switches. As rotas redundantes ficam em estado bloqueado e só ativam se a rota principal falhar.
1.	Root Bridge: O switch com o menor ID (identificador) se torna a raiz da árvore (root bridge). Ele vai ser o ponto central para a definição da melhor rota.
2.	Portas Designadas: As portas de cada switch são categorizadas com base na melhor rota para a root bridge. Se a porta estiver conectada diretamente à root bridge, ela é chamada de porta raiz (root port).
3.	Seleção de Caminho: O STP seleciona o caminho mais curto baseado no custo (menor número de saltos ou menor largura de banda).
4.	Bloqueio de Portas: Se tiver caminhos redundantes, algumas portas vão ser bloqueadas p/ evitar loops.
Protocolos de Roteamento
1.	OSPF (Open Shortest Path First): Roteamento interno rápido, baseado no estado do link
•	Protocolo de Roteamento Link-State.
•	Usado para roteamento interno em redes grandes.
•	Funciona trocando informações de estado de link entre os roteadores p/ definir as melhores rotas.
•	Calcula a menor rota com o algoritmo Dijkstra.
•	Rápido na convergência (detecção de falhas).
2.	BGP (Border Gateway Protocol): Roteamento entre redes (Internet), baseado em políticas
•	Protocolo de Roteamento de Vetor de Caminho.
•	Usado para roteamento entre sistemas autônomos (Internet).
•	Mantém a política de roteamento com base em atributos (como AS path, local preference).
•	Lento na convergência, mas muito escálável e flsexível.
3.	RIP (Routing Information Protocol): Roteamento simples, baseado em contagem de saltos
•	Protocolo de Roteamento de Vetor de Distância.
•	Usado em redes pequenas e médias.
•	Baseado em contagem de saltos como métrica (máximo de 15 saltos).
•	Lento na convergência, pode ter problemas com loops de roteamento.
4.	VRRP (Virtual Router Redundancy Protocol): Redundância de roteador virtual, alta disponibilidade
•	Usado para garantir a alta disponibilidade de roteadores virtuais.
•	Cria um roteador virtual que é compartilhado entre vários roteadores físicos.
•	O roteador mestre é eleito e se ele falhar, outro roteador assume a função.
5.	HSRP (Hot Standby Router Protocol): Backup de roteador, alta disponibilidade
•	Protocolo de redundância usado para fornecer alta disponibilidade.
•	Um roteador ativo (primeiro) e um em espera (backup).
•	O roteador ativo vai encaminhar pacotes, enquanto o backup entra em ação se o ativo falhar.
VLAN (IEEE 802.1Q): dividir uma rede física em várias redes lógicas, com o objetivo de segregar o tráfego de diferentes tipos de dados, melhorar o desempenho e aumentar a segurança.
•	Podem ser configuradas de forma dinâmica ou estática. 
🔹 IEEE 802.1Q:
•	Padrão para a implementação de VLANs em redes Ethernet.
•	Encapsula pacotes com um tag VLAN para identificar a qual VLAN o pacote pertence.
•	Frame Ethernet é marcado com uma tag VLAN de 4 bytes, permitindo que switches saibam a qual VLAN o pacote pertence.
•	VLAN = Rede virtual dentro de uma rede física.
•	Protocolo IEEE 802.1Q marca os pacotes para indicar a qual VLAN pertencem.
VOIP (Voice over IP) Voz pela internet, mais barato e flexível. Voz sobre o IP. Usa prot para converter voz em dados.
🔹 Protocolo H.323= Mais antigo, robusto, e usado em videoconferências
•	Define padrões para chamadas de voz e vídeo através de redes IP. 
•	Complexo e pesado: Tem estrutura mais difícil de configurar e manter, mas é robusto.
•	Suporta voz, vídeo e dados.
🔹 SIP (Session Initiation Protocol) = Protocolo mais leve e flexível, popular em VOIP e aplicativos
•	Mais moderno e leve. Também é para estabelecer e gerenciar chamadas de voz e vídeo
•	Mais fácil de configurar. Usado em uma grande variedade de aplicativos de comunicação.
•	SIP é mais escálável e eficiente do que o H.323.
Qualidade de Serviço (QoS) - Garante qualidade de voz, controlando latência, sem jitter e perda mínima de pacotes: Conj de técnicas para garantir qualidade e a prioridade do tráfego de dados em redes que suportam VOIP.
🔹 Parâmetros de QoS:
1.	Largura de banda: Garante que tráfego de voz tenha a largura nec. para boa qualidade de chamada.
2.	Latência: Tempo de atraso na transmissão dos pacotes de dados. VOIP: ideal ser abaixo de 150 ms.
3.	Jitter: Variação no tempo de chegada dos pacotes. Muito alto pode dar interrupções ou quebra de áudio nas chamadas VOIP.
4.	Perda de pacotes: A perda de pacotes durante uma chamada de VOIP resulta em quebra de voz. 
🔹 Tecnologias para implementar QoS:
•	Política de priorização: Atribui maior prioridade ao tráfego de voz (VOIP) sobre outros tipos de tráfego (como downloads e e-mails).
•	Mecanismos de agendamento: Utilizam métodos como FIFO, WFQ (Weighted Fair Queuing) ou CBWFQ (Class-Based Weighted Fair Queuing) para garantir a entrega eficiente de pacotes de voz.
 Padrão IEEE 802.3 - Ethernet, rede local e transmissão de dados
•	Características Ethernet, tecnologia de rede de transmissão de dados local, principalmente para (LANs).
•	Define como os computadores se comunicam via cabo. Ethernet tradicional é 10 Mbps.
Fast Ethernet - 100 Mbps, upgrade da Ethernet padrão
•	Versão mais rápida da Ethernet padrão, especificada no padrão IEEE 802.3u.
•	Taxa de transmissão: 100 Mbps.
•	Mídia de transmissão: Pode usar cabo de cobre (Cat 5 ou superior) ou fibra ótica.
•	Distância máxima: Até 100 metros com cabos de cobre (Cat 5).
•	Compatibilidade: com a Ethernet original (10 Mbps), permitindo autonegociação de velocidades.
Gigabit Ethernet - 1 Gbps, 10x mais rápido que Fast Ethernet
•	Oferece taxa de transmissão maior, especificada no padrão IEEE 802.3z (fibra ótica) e IEEE 802.3ab (cobre).
•	Taxa de transmissão: 1 Gbps (1.000 Mbps).
•	Mídia de transmissão: Fibra ótica ou cabo de cobre (Cat 5e ou superior).
•	Distância máxima:
Para fibra ótica: Pode alcançar distâncias muito maiores (até 5 km ou mais).
Para cobre (Cat 5e): Distância máxima de 100 metros.
•	Compatibilidade: Suporta autonegociação com velocidades menores (como 10/100 Mbps).
 Redes sem fio (Wireless): Transmissão de dados sem cabos. Utilizam ondas de rádio ou micro-ondas.
🔹 Versões do 802.11:
•	802.11a: Até 54 Mbps na faixa de 5 GHz.
•	802.11b: Até 11 Mbps na faixa de 2.4 GHz.
•	802.11g: Até 54 Mbps na faixa de 2.4 GHz.
•	802.11n: Até 600 Mbps usando duas faixas de frequência (2.4 GHz e 5 GHz).
•	802.11ac: Até 1.3 Gbps (1300 Mbps) usando 5 GHz.
•	802.11ax (Wi-Fi 6): Até 9.6 Gbps com melhorias em capacidade e eficiência de rede.
🔹 IEEE 802.1x é um padrão de controle de acesso para redes sem fio, usado para que só autorizados acessem.
•	Funciona com EAP (Extensible Authentication Protocol), permitindo a autenticação de usuários e dispositivos antes de permitir o acesso à rede.
🔹 WPA (Wi-Fi Protected Access): protocolo de segurança para redes sem fio, melhoria do WEP
•	Usa chave de criptografia dinâmica p/ proteger os dados, melhora a segurança em relação ao WEP.
🔹 WPA2 (Wi-Fi Protected Access 2)
•	mais segura do WPA, usa criptografia AES (Advanced Encryption Standard) em vez da TKIP usada no WPA.
