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

