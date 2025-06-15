ITIL v4
•	Definição: Conjunto de boas práticas para gerenciamento de serviços de TI.
•	Descrição: Foca em geração de valor, adaptabilidade e integração com metodologias como Agile, Lean e DevOps.
•	Classificação:
o	Práticas gerais, de gerenciamento de serviços e práticas técnicas.
•	Princípios: Foco no valor, simplificação, colaboração, otimização, iteração com feedback.

Cabeamento Estruturado
•	Definição: Sistema padronizado de infraestrutura de cabos.
•	Descrição: Facilita a organização, manutenção e expansão de redes de forma modular.
•	Classificação: Subsistemas (ex: cabeamento horizontal, backbone) e categorias (Cat5e, Cat6...).
•	Comparações comuns: Cabeamento estruturado x improvisado (mais eficiente, seguro e gerenciável).
•	Princípios: Flexibilidade, padronização, modularidade.

Técnicas de Circuitos, Pacotes e Células
•	Definição: Modos de comutação de dados nas redes.
•	Descrição:
o	Circuito: canal dedicado.
o	Pacotes: dados divididos em blocos independentes.
o	Células: blocos de tamanho fixo (ATM).
•	Classificação: Comutação por circuito, pacotes ou células.
•	Comparações comuns: Circuito (previsível) x Pacote (eficiente); Pacote x Célula (controle de latência).
•	Princípios: Compartilhamento eficiente, controle de tráfego e latência.
Comunicação dedicada (circuito), dividida (pacote) ou fixa (célula). "Circuito = fixo; Pacote = flexível"

Modelos OSI e TCP/IP
•	Definição: Estruturas conceituais de funcionamento das redes.
•	Descrição:
o	OSI: 7 camadas (ex: Física à Aplicação).
o	TCP/IP: 4 camadas (Acesso à rede, Internet, Transporte, Aplicação).
•	Classificação: OSI é referência teórica; TCP/IP é implementação prática.
•	Comparações comuns: OSI detalhado, mas teórico; TCP/IP mais utilizado na prática.
•	Princípios: Encapsulamento, modularidade, independência.

TCP/IP, RoCE, MTU, Jumbo Frames
•	Definição: Conjunto de protocolos para comunicação em rede.
•	Descrição:
o	TCP/IP: base da internet.
o	RoCE: comunicação direta entre memórias via Ethernet.
o	MTU: tamanho máximo de quadro (padrão 1500 bytes).
o	Jumbo Frames: quadros maiores, usados em redes de alto desempenho.
•	Classificação: TCP/IP divide-se em 4 camadas.
•	Comparações comuns: TCP x UDP; MTU padrão x Jumbo.
•	Princípios: Confiabilidade, controle de fluxo e congestionamento.

CIDR (Classless Inter-Domain Routing)
•	Definição: Técnica para alocação eficiente de endereços IP.
•	Descrição: Usa notação com barra (ex: 192.168.0.0/24), sem classe fixa.
•	Classificação: Substitui as antigas classes A, B, C.
•	Comparações comuns: CIDR x Classful Routing → CIDR é mais flexível.
•	Princípios: Economia de IPs, agregação de rotas (route summarization).

Serviços de Nuvem: IaaS, PaaS, SaaS
•	Definição: Modelos de serviço da computação em nuvem.
•	Descrição:
o	IaaS: Infraestrutura como serviço (máquinas virtuais).
o	PaaS: Plataforma como serviço (ambientes de desenvolvimento).
o	SaaS: Software como serviço (Google Docs, Gmail).
•	Classificação: Níveis de abstração.
•	Comparações comuns: IaaS (controle total), PaaS (sem gerenciamento de infraestrutura), SaaS (uso direto).
•	Princípios: Elasticidade, escalabilidade, autosserviço.

Protocolos Criptográficos
•	Definição: Conjunto de regras para comunicação segura.
•	Descrição: Incluem SSL/TLS, IPSec, HTTPS, SSH.
•	Classificação:
o	Em repouso (armazenamento) ou em trânsito (comunicação).
•	Comparações comuns: SSL (obsoleto) x TLS (atual).
•	Princípios: Confidencialidade, integridade, autenticidade.

Hashes e Algoritmos de Hash
•	Definição: Função que transforma dados em valor fixo.
•	Descrição: Garante integridade (ex: SHA-256, MD5).
•	Classificação: Criptográficos e não criptográficos.
•	Comparações comuns: MD5 (rápido, mas inseguro) x SHA-2 (mais seguro).
•	Princípios: Irreversibilidade, avalanche, unicidade.

Criptografia Simétrica e Assimétrica
•	Definição:
o	Simétrica: mesma chave para cifrar/decifrar.
o	Assimétrica: chave pública/privada.
•	Descrição:
o	Simétrica: mais rápida.
o	Assimétrica: mais segura para comunicação.
•	Classificação: AES (simétrica), RSA (assimétrica).
•	Comparações comuns: Simétrica (desempenho) x Assimétrica (segurança).
•	Princípios: Confidencialidade, autenticidade (quando combinadas).

Public Key Infrastructure (PKI)
•	Definição: Sistema que gerencia criptografia com chaves públicas.
•	Descrição: Usa certificados digitais emitidos por autoridades confiáveis (CAs).
•	Classificação: Infraestrutura centralizada de segurança.
•	Comparações comuns: PKI x Web of Trust.
•	Princípios: Autenticidade, integridade, confiança.

Controle de Acesso
•	Definição: Mecanismo que regula quem pode acessar o quê.
•	Descrição: Pode ser baseado em papéis (RBAC), atributos (ABAC) ou listas (ACL).
•	Classificação:
o	Discricionário, obrigatório, baseado em papéis, atributos.
•	Comparações comuns: RBAC x ABAC.
•	Princípios: Privilégio mínimo, separação de funções.

RADIUS
•	Definição: Protocolo de autenticação, autorização e contabilização (AAA).
•	Descrição: Usado para gerenciar acesso remoto (VPN, Wi-Fi corporativo).
•	Classificação: Protocolo cliente-servidor.
•	Comparações comuns: RADIUS x TACACS+ (menos granularidade).
•	Princípios: Centralização, segurança no acesso.

Sniffer de Rede e Wireshark
•	Definição: Ferramentas para capturar e analisar tráfego de rede.
•	Descrição:
o	Sniffer: captura pacotes.
o	Wireshark: interface gráfica para análise profunda.
•	Classificação: Ferramentas passivas.
•	Comparações comuns: Tcpdump (linha de comando) x Wireshark (visual).
•	Princípios: Monitoramento, diagnóstico, análise forense.

Ataques OWASP Top 10 (2021)
•	Definição: Lista dos principais riscos de segurança em aplicações web.
•	Descrição: Ex: SQL Injection, XSS, Insecure Deserialization, CSRF, etc.
•	Classificação: Riscos críticos.
•	Comparações comuns: XSS (inserção de scripts) x CSRF (exploração de sessão).
•	Princípios: Validação de entrada, autenticação segura, controle de acesso.

DoS, DDoS, PDoS, DRDoS
•	Definição: Ataques que visam tornar sistemas indisponíveis.
•	Descrição:
o	DoS: ataque direto.
o	DDoS: múltiplos dispositivos.
o	PDoS: dano físico/permanente.
o	DRDoS: amplificação via terceiros.
•	Classificação: Por origem, impacto e técnica.
•	Comparações comuns: DDoS (mais difícil de mitigar) x DoS (mais simples).
•	Princípios: Exploração de recursos, saturação de sistemas.

Ping Sweeping, Port Scanning, Social Engineering, DNS Footprinting
•	Definição:
o	Ping sweep: verifica hosts ativos.
o	Port scanning: detecta portas abertas.
o	Social engineering: manipulação psicológica.
o	DNS footprinting: coleta de informações DNS.
•	Classificação: Reconhecimento (passivo x ativo).
•	Comparações comuns: Scanning (técnico) x engenharia social (humana).
•	Princípios: Coleta de informações, preparação de ataque.

Sniffing e Spoofing
•	Definição:
o	Sniffing: interceptação de tráfego.
Spoofing: falsificação de identidade.

•	Descrição:
o	Sniffing: passivo.
o	Spoofing: ativo (ex: IP, MAC, ARP).
•	Classificação: Ataques de rede.
•	Comparações comuns: Spoofing engana; sniffing espiona.
•	Princípios: Violação de confidencialidade e integridade.

 Ataques Wireless
•	Definição: Ameaças às redes Wi-Fi.
•	Descrição: Incluem Rogue AP, Evil Twin, jamming, WPA cracking.
•	Classificação: Interferência, engenharia social, força bruta.
•	Comparações comuns: Jamming (nega serviço) x Evil Twin (rouba dados).
•	Princípios: Autenticidade, confidencialidade, controle de acesso.

Phishing, Spamming, Mail Bombing, Mail Storms
•	Definição:
o	Phishing: enganar para roubar dados.
o	Spamming: envio massivo de mensagens.
o	Mail bombing: sobrecarregar caixa.
o	Mail storms: respostas em massa acidentais.
•	Classificação: Engenharia social e negação de serviço.
•	Comparações comuns: Spear phishing (alvo específico), whaling (altos executivos).
•	Princípios: Engano, sobrecarga, disfarce.

SPF e DKIM
•	Definição: Mecanismos de autenticação de e-mails.
•	Descrição:
o	SPF: especifica servidores autorizados.
o	DKIM: usa assinatura digital.
•	Classificação: Proteções contra falsificação de remetente.
•	Comparações comuns: SPF (origem) x DKIM (integridade).
•	Princípios: Autenticidade e integridade de e-mail.

MITRE ATT&CK, CIS Controls, NIST CSF
•	Definição: Frameworks de segurança cibernética.
•	Descrição:
o	MITRE ATT&CK: matriz de táticas e técnicas usadas por atacantes.
o	CIS Controls: 18 controles prioritários de segurança.
o	NIST CSF: estrutura para gestão de riscos de cibersegurança.
•	Classificação: Modelos de referência.
•	Comparações comuns: MITRE (base técnica), CIS (ações práticas), NIST (estratégico).
•	Princípios: Prevenção, detecção, resposta, recuperação e proteção.

