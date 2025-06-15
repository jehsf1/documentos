ISO 27001:2013 - Certificação de SGSI com foco em riscos e controle.
Objetivo: Requisitos para proteger informações e garantir confidencialidade, integridade e disponibilidade para um Sistema de Gestão de Segurança da Informação (SGSI).
Principais Elementos:
•	Planejamento de segurança: Definir objetivos, riscos e oportunidades.
•	Avaliação de riscos: Identificar, avaliar e tratar riscos relacionados à segurança da informação.
•	Políticas de segurança: Definir diretrizes e regras.
•	Monitoramento e auditoria: Avaliar a eficácia do SGSI.

ISO 27002:2022 - Prática e detalhamento dos controles da ISO 27001.
Objetivo: Diretrizes para implementação dos controles de segurança descritos na ISO 27001.
Controles:
•	Segurança física e ambiental.
•	Controle de acesso: Definir e implementar políticas para proteger ativos.
•	Gestão de incidentes: Estabelecer procedimentos para tratar incidentes de segurança.

Controle de Acesso
AAA	Define quem é o usuário (autenticação), o que ele pode fazer (autorização) e o que ele fez (auditoria).
RBAC	Modelo de controle de acesso baseado em papéis atribuídos aos usuários.
MFA	Requer múltiplos fatores de autenticação, elevando o nível de segurança.

ISO 27005:2022 - Riscos em SI = Identificação, Avaliação, Tratamento.
Objetivo: Fornecer orientações sobre a gestão de riscos de segurança da informação.
Passos Principais:
1.	Contextualização: Entender o ambiente e os ativos a serem protegidos.
2.	Identificação de riscos: Identificar as ameaças e vulnerabilidades.
3.	Avaliação de riscos: Analisar o impacto e a probabilidade de cada risco.
4.	Tratamento de riscos: Definir estratégias para mitigação ou aceitação dos riscos.

Políticas de Segurança da Informação - Regras claras para proteção da informação.
Objetivo: Estabelecer as diretrizes e regras para garantir a proteção da informação na organização.
Componentes principais:
•	Política de acesso: Definir quem pode acessar o quê.
•	Política de uso de sistemas: Regras de uso de sistemas e redes.
•	Política de privacidade e confidencialidade: Garantir a proteção de dados pessoais e sensíveis.
•	Revisão periódica: A política deve ser revisada e atualizada conforme necessário.
Políticas definem responsabilidades, procedimentos e padrões.

Gerenciamento de Incidentes - Detectar, Responder, Recuperar e Aprender.
Objetivo: Detectar, responder e recuperar rapidamente de incidentes de segurança para minimizar danos.
Fases:
1.	Identificação: Detectar o incidente.
2.	Classificação e prioridade: Avaliar o impacto e a urgência.
3.	Resposta: Implementar ações para conter e corrigir o incidente.
4.	Análise post-mortem: Avaliar o que aconteceu e implementar melhorias.
Etapas: Detecção → Análise → Resposta → Recuperação → Aprendizado

Gestão de Continuidade de Negócio - Preparar, Testar, Recuperar!
Garantir que a organização continue operando ou se recupere rapidamente em caso de eventos críticos. Componentes:
•	Plano de Continuidade de Negócio (BCP): Estratégias e procedimentos para manter operações.
•	Plano de Recuperação de Desastres (DRP): Estratégias para recuperar infraestruturas críticas.
•	Análise de Impacto no Negócio (BIA): Avaliar os impactos de diferentes cenários de risco e priorizar ações de recuperação.
•	Testes e Exercícios: Realizar testes regulares para garantir a eficácia dos planos.

Classificação de Informações: Processar e atribuir níveis de segurança com base na criticidade e impacto
•	Confidencialidade: Informação seja acessível apenas às pessoas autorizadas. 
•	Integridade: Informação não seja alterada sem autorização e mantenha sua fidedignidade.
•	Disponibilidade: Informação esteja disponível quando necessário. 
•	Não Repúdio: Pessoa ou sistema não possa negar a autoria de uma ação ou transação. 
•	Privacidade: Informações pessoais sejam protegidas e usadas de forma ética e conforme as leis. 
•	Autenticidade: Informação, transação ou comunicação seja genuína e venha de fonte confiável. 
•	Segurança Física e Lógica: Proteção dos ativos de informação tanto no ambiente físico (controle de acesso a locais) quanto no lógico (proteção contra ataques cibernéticos).

 Criptografia: Proteger através da codificação. Garantir confidencialidade, integridade, autenticidade e não repúdio.
•	E-mails seguros: Usar criptografia para proteger o conteúdo.
•	Comunicações seguras: Proteger transmissões de dados, como em HTTPS (protocolo seguro da web).
✅ Simétrica – Usa a mesma chave para criptografar e descriptografar (ex.: AES, DES).
✅ Assimétrica – Usa um par de chaves (pública e privada) para criptografia e autenticação (ex.: RSA, ECC).

Protocolos Criptográficos - Segurança das Comunicações!
•	SSL/TLS: Prot. segurança para comunicação segura pela web. Garante criptografia e segurança da comunicação
Como funciona:
•	Handshake (negociação inicial) – O cliente e o servidor trocam inf. e estabelecem chaves criptográficas.
•	Autenticação – Um certificado digital (como um SSL/TLS) garante que o servidor é legítimo.
•	Criptografia de dados – Todos os dados transmitidos são protegidos contra interceptação e alterações.

🔹 Versões Importantes: SSL 3.0 – Obsoleto e inseguro. TLS 1.0 e 1.1 – Também obsoletos. TLS 1.2 – Padrão usado atualmente. TLS 1.3 – Mais rápido e seguro, eliminando algoritmos fracos.
🔹 Aplicações: Navegação segura (HTTPS), E-mails seguros (SMTP, IMAP, POP com TLS), VPNs baseadas em TLS.

IPsec: Criptografia para segurança de redes IP.

Assinatura Digital = Autenticidade e Integridade, usando chaves privadas.
Certificado Digital: Atesta a autenticidade de uma chave pública e é emitido por uma Autoridade Certificadora (CA).

Hash = Função matemática que gera um valor fixo a partir de dados de entrada 
Garantir integridade e segurança dos dados.
Algoritmos de Hash: Exemplo: SHA-256, que gera um valor único (hash) para o conteúdo.
Características das Funções de Hash:
•	Unidirecional – Não pode ser revertido para obter o valor original.
•	Determinístico – A mesma entrada sempre gera o mesmo hash.
•	Rápido de calcular – Mas difícil de ser revertido.
•	Sensível a mudanças – Pequena alteração na entrada gera um hash completamente diferente.
•	Colisões devem ser raras – Idealmente, entradas diferentes não devem gerar o mesmo hash.

MD5 (Message Digest Algorithm 5): Produz um hash de 128 bits (32 caracteres hexadecimais).

SHA (Secure Hash Algorithm): família de algoritmos mais seguros que o MD5. 
Algoritmo	Tamanho do Hash	Segurança
SHA-1	160 bits (40 caracteres)	Inseguro (colisões encontradas)
SHA-256	256 bits (64 caracteres)	Seguro e amplamente usado
SHA-512	512 bits (128 caracteres)	Muito seguro, mas mais lento

Criptografia de Curvas Elípticas (Assimétrica)
•	Usa curvas matemáticas para criar chaves públicas e privadas, e permite a troca segura de informações, com chaves menores do que outros métodos (como o RSA), mas com a mesma segurança e mais rápida.
•	Exemplo: ECC (Elliptic Curve Cryptography).

Esteganografia = Esconder; Criptoanálise = Quebrar códigos.

PKI = Infraestrutura para gerir chaves e certificados!
•	Definição: Estrutura (hardware, software, políticas e procedimentos necessários) para criar, gerenciar, distribuir e revogar certificados digitais e chaves públicas.
•	Componentes:
•	Autoridade Certificadora (CA): Emite certificados digitais.
•	Repositórios de Certificados: Onde os certificados digitais são armazenados.
•	Chaves Públicas e Privadas: Usadas para garantir a confidencialidade, autenticidade e integridade.

ICP-Brasil = Regula a emissão de certificados digitais e promove a segurança nas transações digitais no Brasil.
Certificado Digital	Arquivo eletrônico que associa uma pessoa (física ou jurídica) a uma chave pública.
Chave Privada	Fica com o titular; usada para assinar digitalmente.
Chave Pública	Está no certificado; usada por terceiros para verificar a assinatura.
•	Funcionalidades:
•	Autenticidade – garante que o emissor é quem diz ser.
•	Integridade – garante que o conteúdo não foi alterado.
•	Não repúdio – o emissor não pode negar que assinou.
•	Validade jurídica – documentos assinados digitalmente têm força legal.
Hierarquia da ICP-Brasil
PCA (Prestadora de Certificação Autorizada)		Autoridade máxima que regulamenta as Autoridades Certificadoras (ACs). Instituto Nacional de Tecnologia da Informação (ITI) é o responsável pela PCA.
AC-Raiz (Autoridade Certificadora Raiz)		Autoridade certificadora de maior confiança. Emite os certificados digitais para as ACs intermediárias.
AC (Autoridade Certificadora Intermediária)		Emite certificados para usuários finais ou para outras ACs (subordinadas).
AR (Autoridade de Registro)		Faz a interface com o usuário. Identifica, autentica e valida os dados antes da emissão.
Titular do Certificado		Pessoa física ou jurídica que usa o certificado para assinar documentos.
•	Emissão de Certificados:
- As ACs subordinadas emitem certificados digitais para pessoas físicas, jurídicas ou servidores.
- Para obter um certificado, é necessário passar por um processo de identificação presencial ou remota, dependendo do tipo de certificado.

•	Assinatura Digital:
- Ao assinar um documento digitalmente, o usuário utiliza sua chave privada para gerar uma assinatura.
- A assinatura é validada pela AC Raiz ou AC intermediária para garantir que ela seja autêntica e não tenha sido modificada.

•	Funcionalidades da Certificação Digital e ICP-Brasil
•	Autenticação: Verifica a identidade de pessoas ou empresas na internet.
•	Assinatura Digital: Garante que um documento digital não foi alterado após a assinatura.
•	Confidencialidade: Garante que apenas o destinatário autorizado leia a mensagem criptografada.
•	Integridade: Certifica que os dados não foram alterados ou corrompidos durante a transmissão.

Gestão de Identidades e Autenticação
•	Autenticação: Processo de verificação da identidade do usuário (Ex: Senha, biometria).
•	Autorização: Determinação dos direitos do usuário após a autenticação (Ex: Acesso a arquivos, permissões).
•	Auditoria: Registro das ações do usuário para monitorar atividades e garantir conformidade (Ex: logs).

Controle de Acesso Baseado em Papéis - Quem você é, o que pode fazer
RBAC: Controle de acesso que dá permissões baseadas no papel ou função.

Autenticação Baseada em Múltiplos Fatores - 3 em 1
MFA: Combina algo que você sabe (senha), algo que você tem (token, celular) e algo que você é (biometria).

RADIUS (Remote Authentication Dial-In User Service) - Controle remoto de acesso
Protocolo para autenticação centralizada e controle de acesso a redes para acesso remoto. 
SSO	Autenticação única: login único para múltiplos sistemas.
OAuth 2.0	Protocolo de autorização delegada, sem compartilhamento de senha.
SAML	Padrão XML para SSO corporativo, via troca de mensagens (assertions).
Keycloak	Solução open source para IAM: autenticação, SSO, OAuth2, SAML, MFA.

SAML – Security Assertion Markup Language 
Fluxo: O usuário tenta acessar um serviço (SP) -> É redirecionado ao IdP para autenticação -> O IdP envia um "SAML assertion" (mensagem com os dados do usuário) -> SP autoriza o acesso.
•	Protocolo XML para troca de informações de autenticação e autorização entre fornecedores de identidade e provedores de serviços.

SSO (Single Sign-On) - Faz o login uma vez e tem acesso a vários sistemas sem precisar se autenticar novamente.
•	Autenticação centralizada: Usuários fornecem credenciais a um servidor de autenticação, que armazena em repositório central. Os que usam SSO podem validar as credenciais do usuário no repositório central.
•	Autenticação federada: Usuários fornecem credenciais a um servidor de identidade externo, que autentica e emite token de acesso. Sistemas usam SSO podem validar o token de acesso do usuário contra o servidor de identidade externo.
Sign-On - Ato de entrar em um sistema com as credenciais. Pode ser único (SSO) ou exigir múltiplos logins.

Keycloak: Plataforma de ger. de identidade open-source para autenticação e autorização, suporta SSO, MFA, etc.

OAuth2 (RFC 6749): Protocolo de autorização que permite que uma aplicação acesse recursos em nome de um usuário, sem precisar da senha do usuário. Muito usado em aplicações web e móveis.

OpenID Connect - OAuth2 + autenticação: Protocolo de autenticação baseado no OAuth2, mas com a adicional verificação da identidade do usuário.
•	Usado para permitir login único em sites e aplicativos sem compartilhar credenciais.

 Monitoramento de Tráfego: Observação e análise do tráfego de rede para detectar comportamentos anômalos, problemas de desempenho e segurança.
Objetivo: Garantir a performance da rede e identificar incidentes de segurança.
Wireshark	Ferramenta gratuita de captura e análise de pacotes de rede.
Packet sniffer	Software que intercepta e exibe pacotes trafegando na rede.
Filtros	Usados para filtrar protocolos, IPs, portas e padrões específicos.
Análise de pacotes	Técnica para identificar problemas, falhas ou comportamentos maliciosos.
Formatos suportados	Trabalha com .pcap (análise offline), .cap, entre outros.

Filtro Wireshark	O que faz
ip.addr == x.x.x.x	Mostra pacotes de/para o IP especificado.
tcp.port == 80	Filtra pacotes usando a porta 80 (HTTP).
http	Mostra apenas pacotes HTTP.
dns	Mostra apenas pacotes DNS.
tcp.flags.syn == 1	Filtra pacotes de início de conexão TCP.

Funcionalidade Wireshark	Descrição
Captura de pacotes	Intercepta tráfego em interfaces de rede (com fio ou Wi-Fi).
Filtros de captura e exibição	Usados para refinar a análise e isolar pacotes relevantes.
Decodificação de protocolos	Suporta centenas de protocolos (TCP, UDP, HTTP, DNS, ARP, etc).
Análise em tempo real ou offline	Permite visualizar tráfego ao vivo ou carregar arquivos .pcap/.cap.
Reassembly de fluxos	Junta pacotes fragmentados (útil para ver mensagens completas).

Tipos de Ataques
•	SQL Injection: Injeção de código SQL em campos de entrada para que um atacante execute comandos no BD
•	Broken Authentication: Falhas no método de autenticação, para que atacantes tenham acesso 
•	Cross-Site Scripting (XSS): Inserção de código JavaScript malicioso em sites, que é executado no navegador do usuário. Exemplo: Roubando cookies de sessão.
•	Insecure Deserialization: Permite exec de código arbitrário ao desserializar dados sem verificar integridade
•	Directory Traversal: Permite acessar arquivos fora do diretório autorizado pela da manipulação de URLs ou caminhos de arquivos.
•	Watering Hole Attack: O atacante compromete sites confiáveis que os alvos frequentemente visitam
•	Cross-Site Request Forgery (CSRF): Fazendo o navegador do usuário realizar ações não autorizadas em um site no qual o usuário está autenticado.
•	Cookie/Session Poisoning: Manipulação ou roubo de cookies de sessão para se passar por outro usuário e obter acesso a dados sensíveis.
•	Buffer Overflow: Exploração de vazio de memória para sobrescrever dados críticos e exec código malicioso.
•	CAPTCHA Attacks: Tentativas de burlar ou automatizar a solução de CAPTCHA 

Ataques de Negação de Serviço - Sobrecarga de sistema para tirar do ar.
•	DoS (Denial of Service): sobrecarrega serviço, para que não consiga responder às requisições legítimas.
•	DDoS (Distributed Denial of Service): DoS realizado por múltiplos sistemas comprometidos
•	PDoS (Permanent Denial of Service): danifica permanentemente o sistema ou serviço, deixando irreparável
•	DRDoS (Distributed Reflection DoS): Ataques distribuídos que usam outros servidores como refletores para amplificar a intensidade do ataque.

Ataques de Reconhecimento - Coleta de informações para invasões futuras
•	Ping Sweeping: Técnica para identificar dispositivos ativos em uma rede através do comando ping.
•	Port Scanning: Técnica para identificar portas abertas em um sistema, visando possíveis vulnerabilidades.
•	Social Engineering: o humano é o alvo, manipulando-o para que forneça informações confidenciais.
•	DNS Footprinting: Técnica p mapear a infra DNS da rede, descobrindo detalhes de servidores e redes.

Ataques Sniffing = Espiar tráfego; Spoofing = Falsificar identidade.
•	Sniffing: Captura do tráfego de rede para analisar pacotes e roubar dados sensíveis . Captura de tráfego de rede.
o	Sniffing Passivo: só observa o tráfego sem interferir ou modificar os pacotes. Capturar e analisar os dados.
o	Sniffing Ativo: captura os pacotes, e pode injetar pacotes falsos ou modificar para alterar o comportamento.
o	Packet Sniffing: captura pacotes individuais de dados que estão sendo transmitidos por uma rede. 
o	Network Sniffing: monitora a rede, analisa dados em trânsito entre dispositivos. Locais(LAN) e Públicas (WAN).
Ferramentas Comuns para Sniffing:
•	Wireshark
•	tcpdump
•	Cain & Abel
•	Ettercap

•	Spoofing: Falsificação de identidade na rede. A vítima pensa que é servidor legítimo, mas é um atacante. 
1.	IP Spoofing: altera o endereço IP de origem do pacote parecendo outra máquina. 
2.	DNS Spoofing (ou Cache Poisoning): manipula/"envenena" o cache DNS de um servidor/pc, fazendo que acredite ser site legítimo. Redireciona o tráfego para o site falso.
3.	ARP Spoofing (ou ARP Poisoning): Protocolo para mapear endereços IP para endereços MAC na rede local. O atacante envia pacotes ARP falsificados para associar seu endereço MAC a um endereço IP legítimo. Permitir ao atacante interceptar ou redirecionar o tráfego da rede.
4.	Email Spoofing: falsifica "De" no e-mail para pareser de fonte confiável. Enganar para realizar uma ação.
5.	Website Spoofing: Site falso, que imita legítimo. Enganar e a vítima insira informações confidenciais.
6.	SMS Spoofing: Nº de telefone de SMS falso para parecer que está sendo enviada de uma fonte confiável. 
7.	Bluetooth Spoofing: Se passa por legítimo na rede Bluetooth, enganando para aceitar a conexão.
Ferramentas Comuns para Spoofing:
•	Ettercap (para ARP Spoofing)
•	Cain & Abel (para Sniffing e Spoofing)
•	FakeAP (para Spoofing de rede Wi-Fi)
•	Mausberry (para Spoofing de Bluetooth)

Ataques Redes Wireless 
•	WEP/WPA Cracking: quebrar protocolos de segurança WEP e WPA para acessar redes Wi-Fi 
•	Evil Twin Attack: O atacante cria uma rede Wi-Fi falsa com o mesmo nome da legítima para enganar.
•	Deauthentication Attack: Envia pacotes para desconectar dispositivos de uma rede wireless, permitindo o acesso não autorizado.

Ataques E-mail - Phishing = Enganar; Spamming = Enviar em massa; Mail Bombing/Storms = Sobrecarregar.
•	Phishing: o atacante se passa por uma entidade confiável para roubar informações
•	Spear Phishing: direcionado a uma pessoa ou organização específica.
•	Whaling: focado em executivos ou figuras de alto nível.
•	Pharming: Redirecionamento malicioso de um site legítimo para um site falso.
•	Spimming: Spam via e-mail, de forma agressiva e direcionada, como mensagens não solicitadas.
o	Spamming: Envio de mensagens não solicitadas para muitos destinatários, comerciais ou maliciosos
o	Mail Bombing: Envio massivo de e-mails para sobrecarregar ou derrubar servidores de e-mail.
o	Mail Storms: Cadeias de e-mails em loop que causam overload em servidores de email, um desastre.
Proteção de Segurança de E-mail: 
•	SPF (Sender Policy Framework): Protocolo que verifica se um servidor de e-mail está autorizado a enviar e-mails em nome de um domínio, prevenindo spoofing.
•	DKIM (DomainKeys Identified Mail): Protocolo que adiciona uma assinatura digital a um e-mail para garantir sua autenticidade e integridade, garantindo que o e-mail não foi alterado.

 Tipos de Malware 
•	Vírus: Software malicioso que se replica e infecta outros programas ou arquivos em um sistema.
•	Worms: Malware que se replica automaticamente e espalha pelas redes, sem programa hospedeiro.
•	Trojans: Malware disfarçado de software legítimo, mas com código malicioso para comprometer ou roubar 
•	Ransomware: Malware que criptografa arquivos e exige resgates para liberá-los.
•	Rootkits: Projetado para ocultar outros malwares e ações do invasor no sistema.
•	Adware: Software que exibe propagandas indesejadas no sistema, coletando dados sobre os usuários.
•	Spyware: Malware espiona as atividades do usuário, roubando dados como senhas e informações pessoais.
•	Botnet: Rede de dispositivos controlados por atacante para realizar ataques em massa, como DDoS.
•	Backdoor: Vulnerabilidade criada por malware para que um atacante tenha acesso remoto e sem restrições
 
Advanced Persistent Threats (APT) - Ataque sofisticado e persistente para roubo de dados.
•	Manter presença em sistemas críticos por longos períodos, furtivamente coletando dados e recursos.

Frameworks de Segurança da Informação e Cibernética 
•	MITRE ATT&CK: Framework que mapeia as táticas e técnicas utilizadas por atacantes cibernéticos, oferecendo uma visão sobre como os ataques são realizados em diferentes estágios.
•	Objetivo: Ajudar na detecção, resposta e mitigação de ameaças cibernéticas.
Incidente de Segurança: Qualquer evento que comprometa a segurança das informações 

CIS Controls (Center for Internet Security): Ações e melhores práticas para defender de ameaças comuns 
Objetivo: Priorizar medidas que ajudem na proteção de redes, sistemas e dados contra incidentes de segurança.
CONTROLES ESSENCIAIS	PRIORIDADE MÁXIMA, PROTEGE CONTRA ATAQUES MAIS COMUNS	1 A 6
CONTROLES FUNDAMENTAIS	Proteção adicional, aumenta a resiliência	7 a 12
CONTROLES ORGANIZACIONAIS	Estratégias avançadas para segurança contínua	13 a 18

Os 18 Controles do CIS v8
🔹 Controles Essenciais (1 a 6) – Proteção básica
1️Inventário e Controle de Ativos – Identifique dispositivos conectados à rede.
2️Inventário e Controle de Software – Monitore os softwares autorizados e bloqueie os não aut.
3️ Proteção de Dados – Proteja dados sensíveis em trânsito e em repouso.
4️ Gestão de Vulnerabilidades – Identifique e corrija vulnerabilidades periodicamente.
5️ Configuração Segura – Utilize configurações seguras em sistemas e dispositivos
6 Gerenciamento de Acessos – Controle e limite acessos administrativos e privilégios.
🔹 Controles Fundamentais (7 a 12) – Segurança avançada
7️ Proteção Contra Malware – Implemente soluções para detectar e bloquear ameaças.
8️ Gestão de Auditoria e Logs – Registre eventos críticos para análise e resposta a incidentes.
9️ Controle de Portas e Protocolos – Restrinja portas e serviços não essenciais.
10 Defesa Contra Engenharia Social – Treine usuários contra phishing e fraudes.
1️1 Monitoramento e Análise de Segurança – Detecte atividades suspeitas na rede.
1️2 Defesa Contra Ataques Wireless – Proteja redes sem fio contra acessos indevidos.
🔹 Controles Organizacionais (13 a 18) – Gestão e Resiliência
1️3 Gestão de Segurança de Aplicações – Desenvolva softwares seguros desde a concepção.
1️4 Resiliência a Incidentes – Estabeleça um plano de resposta a incidentes.
1️5 Gestão de Fornecedores – Avalie a segurança de terceiros e parceiros.
1️6 Segurança na Nuvem – Proteja dados e infraestrutura na nuvem.
1️7 Segurança em Mobilidade – Aplique políticas para proteger dispositivos móveis.
1️8 Gestão de Segurança – Desenvolva uma cultura organizacional de segurança cibernética.

NIST CyberSecurity Framework (NIST CSF): Framework que fornece diretrizes sobre como as organizações podem gerenciar e reduzir os riscos de segurança cibernética. Melhorar a gestão de riscos e fortalecer as defesas.
Ciclo de Resposta a Incidentes:
•	Preparação – Definir políticas, equipe de resposta (CSIRT) e ferramentas.
•	Detecção e Análise – Identificação do incidente por logs, SIEM, alertas.
•	Contenção, Erradicação e Recuperação – Conter impacto, remover ameaças e restaurar sistemas.
•	Pós-incidente – Analisar causa, documentar lições aprendidas e melhorar defesa.
Macete: 🧠 "NIST planeja, MITRE ataca, CIS controla."

MACETES
ISO/IEC 27001: certificação de sgsi com foco em riscos e controle
ISO/IEC 27002: prática e detalhamento dos controles da iso 27001
ISO/IEC 27005: riscos em si = identificação, avaliação, tratamento
Políticas de SI: regras claras para proteção da informação
Gerenciamento de Incidentes: detectar, responder, recuperar e aprender
Gestão de Continuidade de Negócio: preparar, testar, recuperar!
Princípios de Segurança: "C.I.D.N.P.A.S." = confidencialidade, integridade, disponibilidade, não repúdio, privacidade, autenticidade, segurança
Criptografia: criptografia = proteção da informação!
Criptografia: simétrica = mesma chave; assimétrica = chave pública e privada
Assinatura e Certificação Digital: assinatura digital = autenticidade e integridade!
Hash: "Hash = resumo único de dados!
Esteganografia e Criptoanálise: esteganografia = esconder; criptoanálise = quebrar códigos
PKI: infraestrutura para gerir chaves e certificados!"
ICP-Brasil: certificados digitais no brasil
AAA: autenticação, autorização, auditoria
RBAC: quem você é, o que pode fazer
MFA: 3 em 1 (senha + token + biometria).
RADIUS: controle remoto de acesso
SSO: só um login para tudo
Sign-On: a entrada para os sistemas
Keycloak, SAML, OAuth2: identidade e acesso simplificados
OpenID Connect: oauth2 + autenticação
Monitoramento de Tráfego: wireshark = espião da rede!
Ameaças em Web: sql injection, xss, csrf... Ataques contra aplicações web = fique de olho nas falhas
Ataques em Redes: dos = derruba, ddos = múltiplos sistemas, pdos = dano permanente!
Reconhecimento: reconhecimento = descobrir e mapear redes e sistemas
Sniffing e Spoofing: sniffing = espiar tráfego; spoofing = falsificar identidade
Redes Wireless: "Wi-Fi = cracking, falsificação e desconexão forçada
Ataques de E-mail: phishing = enganar; spamming = enviar em massa; mail bombing/storms = sobrecarregar.
Protocolos de Segurança de E-mail: spf = verificar envio autorizado; dkim = assinatura digital para garantir autenticidade
Ataques de Malware: vírus = replica; worms = se espalha sozinho; trojans = se disfarça; ransomware = pede resgate; rootkits = oculta; adware = propaganda; spyware = espiona; botnet = exército de máquinas; backdoor = acesso secreto.
APT: ataque sofisticado e persistente para roubo de dados
Frameworks de Segurança: mitre att&ck = táticas e técnicas; cis controls = ações práticas para defesa; nist csf = gestão de riscos e redução de ameaças.

SSO (Single Sign-On): Método de autenticação em que o usuário se loga uma vez para acessar vários sistemas.

Keycloak: Ferramenta de gerenciamento de identidade (autorização) e autenticação, fácil de integrar com SSO. 

OAuth2: Protocolo p/ permitir que uma aplicação acesse recursos de outra aplicação sem compartilhar senhas. OAuth2 (RFC 6749): padrão de autorização.
SSO = Uma senha p/ todos sistemas. Keycloak = Ferramenta de aut. OAuth2 = Aut acesso sem compartilhar senha.

Message Broker: Sistema que gerencia a troca de mensagens entre diferentes sistemas ou componentes.
🐇 RabbitMQ: fila de mensagens. Implementa o protocolo AMQP (Advanced Message Queuing Protocol).
•	Modelo pub/sub, onde produtores enviam mensagens para filas, e consumidores retiram as mensagens dessas filas. Comunicação desacoplada.
•	Implementa o protocolo AMQP, aberto para mensageria que garante entrega confiável de mensagens. Persistir mensagens nas filas.
•	Criação de clusters para aumentar a escalabilidade e redundância. Filas distribuídas. 
•	Filas: Buffers que armazenam as mensagens enviadas pelos produtores, aguardando consumo.
•	Exchanges: Rotear as mensagens para as filas corretas com base nas bindings e nas regras de roteamento definidas.
🔹 Componentes Principais do RabbitMQ
•	Producer (Produtor): Aplicação ou serviço que envia as mensagens para o RabbitMQ.
•	Queue (Fila): Armazena mensagens enviadas pelos produtores até que o consumidor processe
•	Consumer (Consumidor): Aplicação/serviço recebe e processa as mensagens das filas
•	Exchange: Rotea mensagens para filas certas, seguindo regras de roteamento e bindings config.
•	Binding: Define a relação entre 1 fila e 1 exchange. Determina como as mensagens são roteadas.

Webhooks: APIs reversas (reagem a eventos). Notificação automática enviada de um sistema para outro.
Evento negocial: acontecimento relevante no negócio.
🧠 Rabbit envia, Webhook responde, Evento dispara

Git: Sistema de controle de versão que permite rastrear alterações no código e colaborar com outros.
•	Repositório (Repository): onde todos os arquivos e o histórico de versões do projeto são armazenados.
•	Commit: "foto" do estado atual dos arquivos no repositório, cada tem id único (hash), rastrear alterações.
•	Branch (Ramificação). Branch principal geral é chamado de master ou main. Histórico independente
•	Merge é o processo de combinar as mudanças de um branch de volta ao branch principal.
Comando Git	Descrição
git init	Cria um novo repositório Git.
git clone <url>	Cria uma cópia local de um repositório remoto.
git status	Mostra o status dos arquivos no repositório (modificados, pendentes).
git add <arquivo>	Adiciona arquivos à área de preparação para commit.
git commit -m "mensagem"	Confirma as mudanças com uma mensagem explicativa.
git branch	Lista os branches ou cria um novo branch.
git checkout <branch>	Muda para o branch especificado.
git merge <branch>	Mescla o branch especificado ao branch atual.
git pull	Atualiza o repositório local com as últimas alterações remotas.
git push	Envia as alterações locais para o repositório remoto.
git log	Mostra o histórico de commits.
git diff	Mostra as diferenças entre os arquivos no repositório e no commit.
git reset	Desfaz as mudanças feitas em commits.
git rm <arquivo>	Remove um arquivo do repositório e do sistema de arquivos.
Git = Rastreia alterações no código. GitHub/GitLab = Plataformas online para repositórios.
Kubernetes: Sist Gerencia e orquestra contêineres em ambientes de clusters, garant disponibilidade e escalabilidade
🔹 Kubernetes: orquestrador de contêineres.
🔹 Cluster: conjunto de máquinas trabalhando juntas.
Kubernetes gerencia contêineres em clusters para garantir escalabilidade. Rancher gerencia clusters Kubernetes.
Rancher: Ferramenta de gerenciamento de Kubernetes, facilita administração de clusters e orquestra contêineres.
•	Interface de gerenciamento do Kubernetes.
•	Fácil de usar em ambientes multi-cluster.

CI/CD – Conjunto de práticas para automatizar o desenvolvimento, testes e deploy de aplicações.
🔹 Continuous Integration (CI): Integra o código constantemente. Realiza testes automáticos na alteração.
	Commit de Código: desenvolvedores fazem commit do código frequentemente em um repositório compartilhado (por exemplo, Git).
	Build Automático: Após o commit, um sistema de CI (como Jenkins, Travis CI, CircleCI) inicia automaticamente o processo de build do projeto.
	Execução de Testes: O sistema de CI executa testes automatizados para garantir que o código não quebrou nenhuma funcionalidade existente.
	Relatório de Erros: Se algum erro for detectado, a equipe de desenvolvimento é notificada rapidamente para que a falha seja corrigida.
🔹 Continuous Delivery (CD): Faz q o código seja entregue automaticamente em ambientes de teste
o	Commit e CI: A equipe de desenvolvimento faz commits frequentemente no repositório e os sistemas de CI executam a integração contínua.
o	Pipeline Automatizado: O código é enviado para um pipeline automatizado que inclui a construção, testes, e a validação.
o	Ambiente de Staging: O código é implantado em um ambiente de staging (pré-produção) para garantir que ele funcione corretamente em um ambiente semelhante ao de produção.
o	Pronto para Produção: O código passa por uma revisão final e é aprovado para ser implantado em produção.
🔹 Continuous Deployment: eliminar a intervenção humana no processo de entrega.
	Commit e CI: O desenvolvedor faz o commit do código no repositório.
	CI + Testes: O código é automaticamente compilado e os testes são executados para garantir que a mudança não introduza falhas.
	Deploy para Produção: Se todos os testes passarem, o código é automaticamente implantado em produção. Essa automação ocorre em todos os estágios do pipeline.
	Feedback Instantâneo: Como o código está em produção de forma constante, a equipe recebe feedback imediato sobre a aceitação do código pelos usuários.
Pipeline CI/CD: 
•	Construção (Build): Compilação do código e dependências.
•	Testes: Execução de testes automatizados, como testes unitários e de integração.
•	Deploy: Implantação em ambientes de staging ou produção.
•	Monitoramento: Verificação de logs e métricas após o deploy para garantir a saúde do sistema.
Ferramenta CI/CD	Descrição
Jenkins	Ferramenta de CI/CD amplamente utilizada, com grande flexibilidade e suporte a plugins.
GitLab CI	Integração contínua nativa dentro do GitLab, fácil de usar e configurar.
Travis CI	Ferramenta de CI/CD baseada em nuvem, integrada com GitHub.
CircleCI	Ferramenta de CI/CD focada em eficiência e velocidade de pipelines.
GitHub Actions	Ferramenta de CI/CD integrada ao GitHub, permite automação de fluxos de trabalho.
Azure DevOps	Plataforma da Microsoft para DevOps, incluindo CI/CD e ferramentas gerenciamento de projeto.
Spinnaker	Ferramenta de CD focada em multi-cloud e entrega contínua de software.

Qualidade de Software: capacidade do sistema atender aos requisitos e expectativas do usuário.
•	Fatores de Qualidade (ISO 25010): Funcionalidade: Faz o que deve, Confiabilidade: sem falhas, Usabilidade: É fácil,  Eficiência: desempenho, Manutenibilidade: atualiza sem grandes impactos, Segurança: protege dados.
•	Garantia de Qualidade: Testes de Software: Unitários, integração, regressão e aceitação. Revisões e Inspeções de Código. Automação de Testes.
