# ISO 27001:2013 - Certificação de SGSI com foco em riscos e controle.
Objetivo: Requisitos para proteger informações e garantir confidencialidade, integridade e disponibilidade para um Sistema de Gestão de Segurança da Informação (SGSI).
### Principais Elementos:
•	Planejamento de segurança: Definir objetivos, riscos e oportunidades.\
•	Avaliação de riscos: Identificar, avaliar e tratar riscos relacionados à segurança da informação.\
•	Políticas de segurança: Definir diretrizes e regras.\
•	Monitoramento e auditoria: Avaliar a eficácia do SGSI.

# ISO 27002:2022 - Prática e detalhamento dos controles da ISO 27001.
Objetivo: Diretrizes para implementação dos controles de segurança descritos na ISO 27001.
### Controles:
•	Segurança física e ambiental.
•	Controle de acesso: Definir e implementar políticas para proteger ativos.
•	Gestão de incidentes: Estabelecer procedimentos para tratar incidentes de segurança.

# Controle de Acesso
**AAA**	Define quem é o usuário (autenticação), o que ele pode fazer (autorização) e o que ele fez (auditoria).\
**RBAC**	Modelo de controle de acesso baseado em papéis atribuídos aos usuários.\
**MFA**	Requer múltiplos fatores de autenticação, elevando o nível de segurança.

# ISO 27005:2022 - Riscos em SI = Identificação, Avaliação, Tratamento.
Objetivo: Fornecer orientações sobre a gestão de riscos de segurança da informação.
Passos Principais:
1.	Contextualização: Entender o ambiente e os ativos a serem protegidos.
2.	Identificação de riscos: Identificar as ameaças e vulnerabilidades.
3.	Avaliação de riscos: Analisar o impacto e a probabilidade de cada risco.
4.	Tratamento de riscos: Definir estratégias para mitigação ou aceitação dos riscos.

# Políticas de Segurança da Informação - Regras claras para proteção da informação.
Objetivo: Estabelecer as diretrizes e regras para garantir a proteção da informação na organização.
Componentes principais:
•	Política de acesso: Definir quem pode acessar o quê.
•	Política de uso de sistemas: Regras de uso de sistemas e redes.
•	Política de privacidade e confidencialidade: Garantir a proteção de dados pessoais e sensíveis.
•	Revisão periódica: A política deve ser revisada e atualizada conforme necessário.
Políticas definem responsabilidades, procedimentos e padrões.

# Gerenciamento de Incidentes - Detectar, Responder, Recuperar e Aprender.
Objetivo: Detectar, responder e recuperar rapidamente de incidentes de segurança para minimizar danos.
Fases:
1.	Identificação: Detectar o incidente.
2.	Classificação e prioridade: Avaliar o impacto e a urgência.
3.	Resposta: Implementar ações para conter e corrigir o incidente.
4.	Análise post-mortem: Avaliar o que aconteceu e implementar melhorias.
Etapas: Detecção → Análise → Resposta → Recuperação → Aprendizado

# Gestão de Continuidade de Negócio - Preparar, Testar, Recuperar!
Garantir que a organização continue operando ou se recupere rapidamente em caso de eventos críticos. Componentes:
•	Plano de Continuidade de Negócio (BCP): Estratégias e procedimentos para manter operações.
•	Plano de Recuperação de Desastres (DRP): Estratégias para recuperar infraestruturas críticas.
•	Análise de Impacto no Negócio (BIA): Avaliar os impactos de diferentes cenários de risco e priorizar ações de recuperação.
•	Testes e Exercícios: Realizar testes regulares para garantir a eficácia dos planos.

# Classificação de Informações: Processar e atribuir níveis de segurança com base na criticidade e impacto
•	Confidencialidade: Informação seja acessível apenas às pessoas autorizadas. 
•	Integridade: Informação não seja alterada sem autorização e mantenha sua fidedignidade.
•	Disponibilidade: Informação esteja disponível quando necessário. 
•	Não Repúdio: Pessoa ou sistema não possa negar a autoria de uma ação ou transação. 
•	Privacidade: Informações pessoais sejam protegidas e usadas de forma ética e conforme as leis. 
•	Autenticidade: Informação, transação ou comunicação seja genuína e venha de fonte confiável. 
•	Segurança Física e Lógica: Proteção dos ativos de informação tanto no ambiente físico (controle de acesso a locais) quanto no lógico (proteção contra ataques cibernéticos).

# Criptografia: Proteger através da codificação. Garantir confidencialidade, integridade, autenticidade e não repúdio.
•	E-mails seguros: Usar criptografia para proteger o conteúdo.
•	Comunicações seguras: Proteger transmissões de dados, como em HTTPS (protocolo seguro da web).
✅ Simétrica – Usa a mesma chave para criptografar e descriptografar (ex.: AES, DES).
✅ Assimétrica – Usa um par de chaves (pública e privada) para criptografia e autenticação (ex.: RSA, ECC).

# Protocolos Criptográficos - Segurança das Comunicações!
•	SSL/TLS: Prot. segurança para comunicação segura pela web. Garante criptografia e segurança da comunicação
Como funciona:
•	Handshake (negociação inicial) – O cliente e o servidor trocam inf. e estabelecem chaves criptográficas.
•	Autenticação – Um certificado digital (como um SSL/TLS) garante que o servidor é legítimo.
•	Criptografia de dados – Todos os dados transmitidos são protegidos contra interceptação e alterações.

🔹 Versões Importantes: SSL 3.0 – Obsoleto e inseguro. TLS 1.0 e 1.1 – Também obsoletos. TLS 1.2 – Padrão usado atualmente. TLS 1.3 – Mais rápido e seguro, eliminando algoritmos fracos.
🔹 Aplicações: Navegação segura (HTTPS), E-mails seguros (SMTP, IMAP, POP com TLS), VPNs baseadas em TLS.

# IPsec: Criptografia para segurança de redes IP.

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

GOVERNANÇA E TECNOLOGIA
Planejamento Estratégico de TIC - Alinhar TI aos objetivos da empresa para gerar valor.
Garantir que a TIC contribua efetivamente para a missão, visão e valores organizacionais. Maximizar o valor da tecnologia, inovando e apoiando decisões empresariais.

PDTIC - Plano estratégico para TI: Define ações, prioridades e investimentos de TIC no curto, médio e longo prazo. Fases: Diagnóstico, Definição de objetivos, Plano de ação, Monitoramento/revisão.

KPIs de TIC - Medir desempenho da TI para os objetivos organizacionais: Indicadores como tempo de resposta, disponibilidade e QoS medem o desempenho das soluções de TIC e impacto nos objetivos organizacionais.

COBIT - Framework de governança e gerenciamento de TIC. Define objetivos de controle e boas práticas para otimizar TI
•	Governança e gestão de TI para alinhar a tecnologia com os objetivos do negócio e gestão de riscos.
•	Domínios do COBIT 2019:
•	Governança: Avaliar, Dirigir e Monitorar (EDM).
•	Gestão: Alinhar, Planejar e Organizar (APO); Construir, Adquirir e Implementar (BAI); Entregar, Serviço e Suporte (DSS); Monitorar, Avaliar e Medir (MEA).
•	Objetivo: Controlar, auditar e garantir conformidade e eficiência na TI.
•	Uso: Estratégia, conformidade regulatória e gestão de riscos.
•	Principais Características do COBIT
- Foco na Governança e Gestão de TI – Garante que a TI esteja alinhada com os objetivos da empresa
- Baseado em Princípios – Como valor para as partes, abordagem holística e governança end-to-end
- Framework Flexível – Pode ser adaptado a diferentes tipos de organizações e setores
- Integração com Outros Frameworks – Como ITIL, ISO 27001, TOGAF e PMI
•	5 Princípios do COBIT
1.	Atender às necessidades das partes interessadas – A TI deve gerar valor para os negócios
2.	Abranger a organização de ponta a ponta – A governança de TI deve abranger toda a empresa
3.	Aplicar um único framework integrado – COBIT pode ser usado com outros frameworks
4.	Habilitar uma abordagem holística – Considera processos, estruturas organizacionais, cultura, habilidades.
5.	Diferenciar governança e gestão – Governança define objetivos e direção; gestão executa atividades
•	7 Componentes de Governança
1.	Processos – Definem atividades necessárias para atingir os objetivos de governança e gestão
2.	Estruturas Organizacionais – Definem papéis e responsabilidades
3.	Cultura e Comportamento – Influenciam a tomada de decisão
4.	Informação – Dados e relatórios essenciais para a governança
5.	Serviços, Infraestrutura e Aplicações – Recursos tecnológicos utilizados
6.	Políticas e Procedimentos – Regras e diretrizes para a TI
7.	Pessoas, Habilidades e Competências – Capacitação da equipe
✅ Criado por: ISACA (Information Systems Audit and Control Association)
✅ Foco: Governança e gestão da TI alinhadas ao negócio
•	40 objetivos de governança e gestão, organizados no modelo/domínios EDM - APO - BAI - DSS - MEA:
🔹EDM (Evaluate, Direct, Monitor) – Avaliação e monitoramento estratégico da TI
🔹 APO (Align, Plan, Organize) – Planejamento e alinhamento da TI com o negócio
🔹 BAI (Build, Acquire, Implement) – Desenvolvimento e implementação de soluções
🔹 DSS (Deliver, Service, Support) – Entrega e suporte de serviços de TI
🔹 MEA (Monitor, Evaluate, Assess) – Monitoramento e auditoria de desempenho
•	Modelos de Processos: Definem como os processos de TI devem ser conduzidos.
Modelo de Maturidade: avaliar o nível de desenvolvimento dos processos. A escala de maturidade varia de 1 a 5, sendo que o nível 1 é o mais básico e o 5 é o mais otimizado.

Governança → Responsabilidade da alta direção (direção e supervisão)
•	Define objetivos estratégicos e garante conformidade. Avalia, direciona e monitora a TI
Gestão → Responsabilidade dos gestores de TI (execução e controle)
•	Implementa e executa os processos definidos pela governança. Monitora operação e otimiza o uso de TI
RACI
R: Responsible (Responsável): A pessoa que executa a tarefa.
A: Accountable (Aprovador ou Autoridade): A pessoa que tem a última palavra
C: Consulted (Consultado): Quem oferece informações
I: Informed (Informado): Quem precisa ser mantido atualizado
 ITIL v4 - Melhores práticas para entregar serviços de TI com qualidade e valor: Framework. Foca em processos, serviços, continuidade, e melhoria contínua. Governança - Direcionamento e controle das ativ da organização.
🔹 Estrutura do ITIL 4: baseado em dois principais conceitos:
🔹 Sistema de Valor do Serviço (SVS): representa como todos os componentes da organização trabalham juntos para criar valor. Ele é composto por 5 elementos:
1️ Princípios orientadores – Regras que ajudam a tomada de decisões
2️ Governança – Garante que as decisões estejam alinhadas com a estratégia da empresa
3️ Cadeia de valor do serviço – Define as atividades necessárias para entregar serviços
4️ Práticas do ITIL – Substituem os processos do ITIL v3 e são mais flexíveis
5️ Melhoria contínua – Direciona a busca por aperfeiçoamento dos serviços
🔹 Ciclo de Vida dos Serviços: 
1.	Organização e Pessoas: Como os times de TI e os stakeholders trabalham juntos.
2.	Informações e Tecnologia: A infraestrutura de TI, ferramentas e sistemas necessários.
3.	Parceiros e Fornecedores: Gestão das relações externas com fornecedores e parceiros.
4.	Fluxos de Valor e Processos: Como os fluxos de trabalho e processos entregam o valor.
🔹 Sistema de Valor do Serviço (SVS):
•	Dimensões: Orga e pessoas, informação e tec, parceiros e fornecedores, processos e fluxo de valor.
•	Princípios: Foco no valor, comece onde você está, progrida iterativamente com feedback, colabore e promova visibilidade, pense e trabalhe holisticamente, mantenha as coisas simples e práticas, otimize e automatize.
•	ITIL: certificação para indivíduos (profissionais de TI).
•	ISO/IEC 20000: certificação para organizações (que prestam serviços de TI).
•	O elemento central do sistema de valor de serviços (SVS) do ITIL é a cadeia de valor de serviço.
🔹 7 Princípios Orientadores do ITIL 4
1️ Focar no valor – Tudo deve ter um impacto positivo para clientes e stakeholders
2️ Começar de onde está – Aproveitar o que já funciona antes de mudar tudo
3️ Progredir iterativamente com feedback – Melhorias devem ser feitas em ciclos curtos
4️ Colaborar e promover visibilidade – Incentivar a comunicação entre equipes
5️ Pensar e trabalhar holisticamente – Considerar o impacto global das ações
6️ Manter as coisas simples e práticas – Evitar burocracia e complexidade desnecessária
7️ Otimizar e automatizar – Usar tecnologia para melhorar processos
 🔹 Cadeia de Valor do Serviço (CVC): coração do ITIL. 6 atividades que ajudam a entregar valor:
1️ Engajar – Entender as necessidades dos clientes
2️ Planejar – Criar estratégias e políticas para os serviços
3️ Projetar e Transicionar – Desenvolver e implementar novos serviços
4️ Obter e Construir – Adquirir e configurar recursos de TI
5️ Entregar e Suportar – Garantir a operação contínua dos serviços
6️ Melhorar – Buscar constantemente otimizações
1. Práticas de Gerenciamento Geral (General Management Practices) - boas práticas de negócios e governança
1️ Gerenciamento da Arquitetura
2️ Gerenciamento da Melhoria Contínua
3️ Gerenciamento da Segurança da Informação
4️ Gerenciamento do Conhecimento
5️ Gerenciamento da Medição e Relatórios
6️ Gerenciamento de Mudança Organizacional
7️ Gerenciamento de Portfólio
8️ Gerenciamento de Projetos
9️ Gerenciamento de Riscos
10 Gerenciamento Financeiro
1️1 Gerenciamento de Estratégia
1️2 Gerenciamento de Fornecedores
1️3 Gerenciamento da Força de Trabalho e Talento
1️4 Gerenciamento de Relacionamento
2. Práticas de Gerenciamento de Serviços (Service Management Practices) entrega e suporte de serviços de TI
1️ Gerenciamento de Nível de Serviço
2️ Gerenciamento de Disponibilidade
3️ Gerenciamento de Capacidade e Desempenho
4️ Gerenciamento de Continuidade de Serviço
5️ Gerenciamento de Incidentes
6️ Gerenciamento de Problemas
7️ Gerenciamento de Configuração e Ativos de Serviço
8️ Gerenciamento de Mudanças
9️ Gerenciamento de Liberação
10 Gerenciamento de Implantação
1️1 Gerenciamento de Catálogo de Serviço
1️2 Gerenciamento de Requisição de Serviço
1️3 Gerenciamento de Suporte a Serviços
1️4 Gerenciamento de Monitoramento e Eventos
1️5 Gerenciamento de Provedores de Serviço
1️6 Gerenciamento de Continuidade de Negócio
1️7 Gerenciamento de Disponibilidade e Capacidade
3. Práticas de Gerenciamento Técnico (Technical Management Practices) tecnologia e infraestrutura
1️ Gerenciamento de Infraestrutura e Plataforma
2️ Gerenciamento de Desenvolvimento de Software e Soluções
3️ Gerenciamento de Implantação

OKR: objetivos e resultados-chave (meta com resultado mensurável). Ciclo Curto.
 🔹 Estrutura - Componentes
•	O (Objective – Objetivo) - O "o que" se deseja alcançar.
•	KR (Key Results – Resultados-Chave) - O "como" saberemos que o objetivo foi alcançado.
KPI: indicadores de performance.
Característica	Descrição
Mensurável	Deve ser baseado em dados objetivos e quantificáveis.
Relevante	Deve estar alinhado com os objetivos estratégicos da organização.
Alcançável	Realista e viável dentro do contexto operacional.
Temporal	Deve ter um período de medição claro (diário, mensal, trimestral).
Específico	Clareza sobre o que exatamente está sendo medido.

BSC: Balanced Scorecard (indicadores em 4 perspectivas: financeira, clientes, processos, aprendizado).
🧠 OKR sonha, KPI mede, BSC equilibra.

PMBOK (Project Management Body of Knowledge)Processos e áreas p gerenciar projetos com sucesso: Guia public pelo PMI (Project Management Institute) descreve práticas e proc essenciais p o gerenciamento de projetos.
 Estrutura - 3 Partes Fundamentais
🔹 Princípios de Gerenciamento de Projetos
🔹 Domínios de Desempenho
🔹 Modelo de Entrega de Valor e Sistema
12 Princípios do Gerenciamento
Princípio	Descrição 
Foco em valor	Entregar valor ao cliente continuamente.
Liderança como serviço	Liderança baseada em colaboração, empatia e apoio.
Engajamento das partes interessadas	Comunicação e envolvimento eficaz com stakeholders.
Equipes adaptáveis e motivadas	Incentivar colaboração e empoderamento.
Foco em sistemas e pensamento holístico	Compreender o projeto como parte de um sistema maior.
Qualidade como responsabilidade	Todos devem zelar pela qualidade do produto ou serviço.
Complexidade como realidade	Lidar com ambientes incertos e complexos.
Adaptação e Resiliência	Aprender e ajustar-se continuamente.
Entrega de valor frequente e incremental	Criar valor em ciclos curtos.
Transparência e comunicação	Compartilhar informações de forma clara e honesta.
Melhoria contínua	Buscar constantemente aprender e evoluir.
Gestão adaptativa e baseada em mudanças	Flexibilidade para lidar com mudanças.

Domínio	Foco Principal
Partes Interessadas	Engajamento e gerenciamento de stakeholders.
Equipe	Desenvolvimento e desempenho da equipe do projeto.
Abordagem e Ciclo de Vida	Escolha de métodos e estrutura do projeto (ágil, híbrido).
Planejamento	Estratégia e direção para alcançar os objetivos.
Trabalho do Projeto	Execução e entrega dos produtos.
Entrega	Criação e entrega de valor contínuo.
Medição	Monitoramento de desempenho e valor entregue.
Incerteza	Identificação e gestão de riscos e oportunidades.
PMO (Project Management Office): Estrutura organizacional que centraliza a gestão de projetos, metodologias e ferramentas para melhorar a eficácia da gestão de projetos. Escritório de Projetos (padroniza e dá suporte). Tipos: Suporte (consultoria), Controle (monitora conformidade), Diretivo (gerencia projetos). 

Gestão de Portfólio: Processo de selecionar e gerenciar um conjunto de projetos que alinhem com os objetivos estratégicos da organização. Prioriza os projetos conforme objetivos estratégicos.
🧠 PMO Organiza. Portfólio Prioriza.

Desenvolvimento Ágil de Software: Indivíduos e interações acima de proc e ferramentas. Soft funcionando acima de doc abrangente. Colaboração com cliente acima de negociação de contratos. Responder mudanças acima de plano rígido

SCRUM: framework ágil para gestão e des de projetos baseado em iterações chamadas Sprints (1 a 4 semanas).
✅ Origem: Criado por Jeff Sutherland e Ken Schwaber nos anos 1990.
✅ Objetivo: Melhorar a produtividade, transparência e entrega contínua de valor.
✅ Baseado em: Inspeção, adaptação e transparência.
🔹 Papéis: Scrum Master 🏆
•	Facilita o processo SCRUM, removendo impedimentos.
•	Garante que a equipe siga as práticas ágeis.
•	Atua como um coach para o time.
Product Owner (PO) 🎯
•	Representa os interesses do cliente.
•	Prioriza o Product Backlog (lista de funcionalidades).
•	Define os critérios de aceitação dos itens.
Time de Desenvolvimento 👨‍💻👩‍💻
•	Equipe multidisciplinar que desenvolve o produto.
•	Autogerenciável e colaborativo.
•	Responsável por entregar incrementos a cada Sprint.
🔹 Artefatos do SCRUM
Product Backlog (PB) 
•	Lista priorizada de funcionalidades a serem desenvolvidas.
•	Mantida e organizada pelo Product Owner.
Sprint Backlog 
•	Lista de tarefas a serem entregues na Sprint.
•	Criada pelo Time de Desenvolvimento no início de cada Sprint.
Incremento 
•	Resultado da Sprint: um produto ou funcionalidade testado e funcional.
Eventos do SCRUM
1. Sprint (1 a 4 semanas)
•	Período fixo para desenvolvimento de conjunto de funcionalidades. Entrega incremental do produto.
  Sprint Planning: Planejamento da Sprint com base no Product Backlog. Defin escopo e objetivos da Sprint.
 Daily Scrum (Reunião Diária, 15 min) 
•	Equipe compartilha o progresso e possíveis impedimentos.
•	Três perguntas-chave:  O que fiz ontem? O que farei hoje? Há algum impedimento?
Sprint Review 
•	Apresentação do incremento ao Product Owner e stakeholders. Feedback para ajustes futuros.
 Sprint Retrospective 
•	Avaliação do processo SCRUM e melhorias para a próxima Sprint.

KANBAN: Foca no fluxo contínuo de trabalho e na limitação do WIP (Work in Progress).
-  Princípios do Kanban: Visualizar o fluxo de trabalho. Limitar a quantidade de tarefas em andamento. Gerenciar o fluxo de forma eficiente. Melhorar continuamente o processo.
- Quadro Kanban: To Do: Tarefas pendentes. In Progress: Tarefas em andamento. Done: Tarefas concluídas.
Extreme Programming (XP): Desenvolvimento iterativo com foco na qualidade do código. 
Lean Software Development: Minimiza desperdícios. Prioriza entregas rápidas e aprendizado contínuo.
Feature Driven Development (FDD): Desenvolvimento baseado na modelagem de funcionalidades.
Crystal: Conjunto de metodologias adaptáveis de acordo com o tamanho da equipe e criticidade do projeto.

Métricas e Estimativas de Software: usadas para avaliar qualidade, produtividade e desempenho do software.
✔ Métricas de Processo: Avaliam eficiência dos métodos usados no projeto.
✔ Métricas de Produto: Avaliam características do software (ex.: linhas de código, complexidade).
✔ Métricas de Projeto: Medem prazo, custo e esforço.

Estimativas de Software são usadas para prever esforço, tempo e custo do desenvolvimento.Técnicas de Estimativa: 
🔹 Linha de Código (LOC) – Baseada no número de linhas de código escritas.
🔹 Pontos de Função (APF - Análise de Pontos de Função) – Avaliação funcional do sistema.
🔹 COCOMO (COnstructive COst MOdel) – Modelo matemático baseado em dados históricos.

Análise por Pontos de Função (APF): mede o tamanho funcional do software, independente da tecnologia usada. Cada um tem um peso atribuído conforme sua complexidade (Baixa, Média ou Alta). Componentes Avaliados:
🔹 Entradas Externas (EE) – Exemplo: formulário de cadastro.
🔹 Saídas Externas (SE) – Exemplo: geração de relatórios.
🔹 Consultas Externas (CE) – Exemplo: busca de informações.
🔹 Arquivos Lógicos Internos (ALI) – Exemplo: banco de dados interno.
🔹 Arquivos de Interface Externa (AIE) – Exemplo: acesso a base de dados externa.
Etapas do Cálculo de PF: 1️Identificar e Classificar os Componentes Func /  2Atribuir Pesos Funcionais / 3️ Calcular a Contagem N Ajustada 4️ Determinar o Fator de Ajuste / 5️ Calcular os P d Função Ajustados
Atribuição de Pesos Funcionais
Componente	Baixa	Média	Alta
Entradas Externas (EE)	3	4	6
Saídas Externas (SE)	4	5	7
Consultas Externas (CE)	3	4	6
Arquivos Lógicos Internos (ALI)	7	10	15
Arquivos de Interface Externa (AIE)	5	7	10A
- Se o sistema é simples, a soma dos pesos será baixa e o fator de ajuste ficará próximo de 0,65.
-  Se o sistema é complexo, a soma será alta e o fator de ajuste pode chegar até 1,35.

Resolução CNJ nº 370/2021: diretrizes para a governança de TIC no Jud, promovendo segurança, eficiência e transparência nas contratações e serviços de TI.
•	Criação de comitês, PDTIC, acompanhamento e transparência.
•	Objetivo: Promover modernização, integração e segurança dos sistemas/processos judiciais93.
•	Abrangência: Todos os órgãos do PJ brasileiro.
•	Principais Diretrizes: Governança de TIC, Segurança da Informação, Interoperabilidade, Inovação Tecnológica, Sustentabilidade.
•	Coordenação: CNJ coordena e monitora. Envolvimento de todos os tribunais.

Resolução CNJ nº 468/2022: Define as normas de contratação de serviços de TIC no Judiciário, foco em transparência, eficiência e controle. Guia de Contratações STIC
•	Orientações para contratações de TIC: ciclo de vida, requisitos, riscos, fiscalização.
🔹 Tipos:
•	Aquisição de Software: Licenciamento de programas.
•	Serviços de TI: Consultoria, suporte, manutenção.
•	Infraestrutura de TI: Equipamentos, servidores, redes.
Processos de Licitação
🔹 Modalidades:
•	Pregão: Licitação para aquisição de bens e serviços comuns.
•	Concorrência: Para contratações de maior valor.
•	Tomada de Preços: Para serviços com valor intermediário.
🔹 Fases:
•	Planejamento: Definir necessidades e requisitos.
•	Edital: Documento formal com condições da contratação.
•	Seleção: Processo de escolha do fornecedor.
•	Execução e Acompanhamento: Gestão da execução do contrato.

Lei de Licitações e Contratos (14.133/2021): assegurando transparência, eficiência e segurança jurídica.
🔹 Princípios Gerais da Licitação:
•	Legalidade: A licitação deve ser regida por lei.
•	Impessoalidade: A concorrência deve ser feita sem favorecimentos.
•	Moralidade: O processo licitatório deve ser conduzido com honestidade e ética.
•	Publicidade: Todos os atos administrativos devem ser publicamente acessíveis.
•	Eficiência: A administração pública deve buscar a melhor solução em termos de custos e qualidade.
🔹 Modalidades de Licitação
•	Pregão: modalidade mais usada, agora permitida para qualquer valor de contratação.
•	Concorrência: Para contratos de grande vulto (acima de R$ 1,5 milhão).
•	Tomada de Preços: Para contratações intermediárias, com limite de R$ 1,5 milhão.
•	Convite: Para valores menores, mas só para aqueles previamente cadastrados.
•	Leilão: Para a venda de bens públicos móveis e lotes de bens inservíveis.
•	Concurso: Para selecionar projetos artísticos, culturais ou científicos.
•	Diálogo competitivo: Para contratações complexas e inovação, com diálogo prévio com o mercado.
🔹 Procedimentos Licitatórios: caminho mais ágil para contratar.
•	Fase Preparatória: Planejamento e estudos de viabilidade da contratação.
•	Fase Externa: Divulgação dos editais e recebimento das propostas.
•	Fase de Julgamento: Análise e classificação das propostas.
•	Fase de Homologação: Finalização do processo e adjudicação.
🔹 Tipos Contratos Administrativos: 
•	Contratos de Obra: Para construção, reforma ou ampliação de imóveis.
•	Contratos de Fornecimento: Para aquisição de bens.
•	Contratos de Serviço: Para prestação de serviços, como serviços técnicos, de limpeza, etc.
•	Contratos de Concessão e Parceria Público-Privada (PPP): Para serviços e obras de longo prazo.
🔹 Cláusulas Contratuais:
•	Cláusula Penal: Multas e penalidades por descumprimento.
•	Reajuste e Revisão: Possibilidade de ajustes nos contratos variações de custos ou imprevistos.
•	Garantias: Exigência de garantia por parte do contratado, como caução, fiança ou seguro.
🔹 Modalidade de Contratação Direta: Simplifica e amplia os casos de contratação direta (sem licitação) 
•	Dispensa de Licitação: Valor inferior ao limite da modalidade (17.600 compra e 33.000 serviço/obras)
•	Inexigibilidade de Licitação: Quando não há possibilidade de competição.
🔹 Contratação integrada e semi-integrada: Para grandes obras, que envolvem tanto o projeto + execução.
•	Sistema de Registro de Preços (SRP): Ampliado para permitir a contratação de vários fornecedores.
•	Certificados Digitais e Plataforma Eletrônica: O uso para garantir transparência e segurança.
•	Sustentabilidade: Priorizando soluções que minimizem impactos ambientais e a continuidade.
•	Etapas obrigatórias: Estudos técnicos preliminares, termos de referência, planejamento detalhado.
•	Critérios: menor preço, maior desconto, melhor técnica, técnica e preço, maior retorno econômico.
•	Gestor e fiscal do contrato: Obrigatoriedade da designação formal.
•	Plano de contratações anual: Administração deve planejar suas aquisições anualmente.
•	Fases da Licitação (nova ordem):  Planejamento → Elaboração Edital → Divulgação Edital → Apresentação Propostas e Lances→ Julgamento → Habilitação → Recursos→ Homologação e Adjudicação.
•	Sanções e Penalidades: Advertência, Multa, Impedimento de licitar e contratar (até 3 anos), Declaração de inidoneidade (até 6 anos).

Planejamento, Fiscalização e Gestão de Contratos de TIC: Gestão de contratos e acompanhamento das execuções de serviços de TIC, garantindo a qualidade, eficiência e cumprimento dos prazos acordados.
•	Planejamento: estudo técnico preliminar, termo de referência.
•	Fiscalização: acompanhamento da entrega e dos prazos.

Gestão de Riscos: Processo de identificação, análise, avaliação e tratamento (mitigação) e monitoramento de riscos relacionados à segurança e continuidade dos serviços de TI.
•	Garantir que a TI suporte as operações sem expor a organização a riscos indesejados. Identificação, análise, avaliação, tratamento e monitoramento dos riscos.

LGPD = Coleta, armazenamento, uso e compartilhamento de dados pessoais por empresas, órgãos e entidade que processe informações de pessoas físicas. Operação de tratamento feita no Brasil ou ofertar a pessoas no Brasil. 
🔹 Princípios:
•	Finalidade: Os dados devem ser coletados para fins específicos e legítimos.
•	Adequação: O tratamento deve ser adequado à finalidade para a qual os dados foram coletados.
•	Necessidade: Somente os dados estritamente necessários devem ser coletados.
•	Livre acesso – O titular tem direito de acessar seus dados e saber como são tratados
•	Qualidade dos dados – As informações devem ser exatas, claras e atualizadas.
•	Transparência: Titulares dos dados devem ser informados claramente sobre o tratamento dos dados
•	Segurança: Os dados pessoais devem ser protegidos contra acessos não autorizados e vazamentos.
•	Prevenção – Adoção de medidas para evitar danos aos titulares.
•	Não discriminação – O tratamento de dados não pode ser usado para práticas discriminatórias.
•	Responsabilização e prestação de contas – Empresas e órgãos demonstrar conformidade LGPD.
🔹 Dados Pessoais e Categorias Especiais
•	Dados Pessoais – Qualquer informação que identifique ou possa identificar uma pessoa (nome, CPF).
•	Dados Sensíveis – Informações que podem causar discriminação (origem racial, religião, biometria)
•	Dados Anonimizados – Dados que não podem identificar um indivíduo diretamente (estatísticas).
•	Dados de Crianças e Adolescentes – Requerem consentimento dos pais ou responsáveis. ECA
🔹 Bases Legais para o Tratamento de Dados
•	Consentimento – O titular autoriza o uso dos dados.
•	Cumprimento de obrigação legal – Quando há necessidade para cumprir leis (registro de funcionários)
•	Execução de contratos – Para prestação de serviços e relações contratuais.
•	Proteção da vida – Para evitar danos à vida ou à saúde do titular.
•	Legítimo interesse – Quando há interesse legítimo da empresa, sem violar direitos do titular.
•	Proteção ao crédito – Para consultas a serviços de crédito, como SPC e Serasa.
•	Processo judicial – Dados podem ser usados para defesa judicial ou administrativa.
🔹 Direitos do Titular dos Dados
•	Confirmar a existência de tratamento de dados.
•	Acessar os dados armazenados.
•	Corrigir informações incompletas ou erradas.
•	Revogar consentimento a qualquer momento.
•	Solicitar a exclusão de dados (direito ao esquecimento).
•	Solicitar portabilidade dos dados para outra empresa.
🔹 Agentes de Tratamento e Responsabilidades
•	Controlador – Responsável por tomar decisões sobre os dados (ex.: empresa que coleta informações).
•	Operador – Processa os dados seguindo ordens do controlador (ex.: empresa terceirizada de TI).
•	Encarregado (DPO - Data Protection Officer) – Responsável por garantir o cumprimento da LGPD.
🔹 Segurança e Penalidades
•	Empresas devem adotar medidas técnicas e organizacionais para proteger os dados.
•	Vazamentos devem ser comunicados à ANPD e aos titulares afetados.
•	Advertência: Primeira infração pode resultar em uma advertência.
•	Multas: Podem chegar a até 2% do faturamento da empresa (limitada a R$ 50 milhões por infração).
•	Suspensão de atividades: Empresa pode ser suspensa de realizar atividades tratamento de dados.
•	Bloqueio de dados: Os dados podem ser bloqueados até que a situação seja regularizada.

Autoridade Nacional de Proteção de Dados (ANPD) responsável pela fiscalização e regulação no Brasil.
•	Elaboração de normas para a aplicação da LGPD.
•	Fiscalização e auditoria de empresas para garantir a conformidade.
•	Orientação sobre o cumprimento da LGPD.

ARQUITETURA PDPJ
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

SEGURANÇA
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

Administração de Sistema da Informação:
🔹Sistemas de Processamento de Transações (SPT): monitora as transações.
🔹Sistemas de Informações Gerenciais (SIG):  Relatórios de desempenho para ter previsão de melhora.
🔹Sistemas de Apoio à Decisão (SAD): é a tomada a decisão em relação a problemas não usuais
🔹Sistemas de Apoio ao Executivo (SAE): são as tomadas de decisão “master”, são a longo prazo 
Estrutura da Governança de TI:
🔹Princ: Alinham estratégico, entrega valor, gerenciamento riscos, otimização recursos e medição desempenho.
🔹Componentes: Estruturas Organizacionais (comitês e papéis de decisão)/Processos (definição de diretrizes e normas)/Mecanismos de Controle (auditorias, indicadores e compliance).
🔹Cadeia de valor integrada (CVI) conjunto macroprocessos e processos em uma visão estratégica.
🔹 Tipos de gerenciamento de processos de Negócio: Centrado ser humano / Centrado documentos / Centrado integração (pouco ou nenhuma interferência humana) - Coordenação de sistemas de softwares diferentes.
🔹 Tipos de Processos de Negócio:
Processos primários: natureza interfuncional e compõem a cadeia que entrega valor diretamente para cliente. Processos de suporte:  suporte e habilitam outros processos. Processos de gerenciamento:  medir, monitorar e controlar atividades de negócio. Asseguram que processos atinjam suas metas.

Planejamento Estratégico de TIC. Como a TIC apoia objetivos da organização. Avaliação ambiente interno e externo
 🔹 Plano Diretor de TIC (PDTIC) - Plano que Direciona Toda a Infra de Computação
•	Documento que planeja ações, metas, sistemas e infraestrutura. Deve ser revisado periodicamente.
•	Baseado em diagnóstico e alinhamento estratégico.
o	Fases: Diagnóstico, Definição de objetivos, Plano de ação, Monitoramento/revisão.
🔹 Indicadores de desempenho - Sem indicador, não tem direção
•	Medem se a TIC está entregando valor.
•	Devem estar alinhados aos objetivos do negócio.

NORMATIVOS PDPJ
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
BANCO DE DADOS
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

📌 Segurança e Gerenciamento de Acesso
🔹 Autenticação e Autorização – Controle de acesso por usuário/grupo.
🔹 Criptografia – Proteção dos dados armazenados e em trânsito.
🔹 Backup e Recovery – Estratégias para recuperação de dados.
🔹 Monitoramento – Logs e métricas para identificar anomalias.

INFRAESTRUTURA
📌 ISO/IEC 20000 - Norma para garantir serviços de TI eficazes e de qualidade
Garantir que a gestão de serviços de TI seja eficaz e que os serviços sejam entregues de forma consistente, atendendo aos acordos de nível de serviço (SLAs) e necessidades do negócio.
🔹 Componentes:
•	Planejamento e implementação de sistemas de gestão de serviços.
•	Melhoria contínua dos serviços de TI.
•	Avaliação e controle dos serviços e processos.
Gerenciamento de incidentes: urgência (o mais rapidamente possível com o mínimo de interrupção).
Gerenciamento de problemas: prevenir a ocorrência de um incidente e uma análise do impacto, causa e soluções.
Modelagem de Processos com BPMN: Notação gráfica para modelar processos de negócio. 
🔹 Elementos:
•	Atividades: Tarefas a serem realizadas.
•	Eventos: Início, fim e outros eventos que afetam o processo.
•	Gateways: Pontos de decisão ou ramificação no fluxo.
•	Fluxos de sequência: Conexões que indicam a ordem das atividades.
•	Pools e Lanes: Representação de participantes ou departamentos.
🔹 Técnicas de Análise de Processos
•	Mapeamento de Processos: Identificação e documentação dos fluxos de trabalho.
•	Análise de Gargalos: Identificação de pontos de atraso ou ineficiência.
•	Análise de Valor Agregado: Avaliar valor agregado pelas atividades.
•	Análise de Fluxo de Trabalho: Verificação de redundâncias e falhas na comunicação.
🔹 Melhoria de Processos
•	PDCA (Plan, Do, Check, Act): Ciclo contínuo de planejamento, execução, verificação e ação.
•	Six Sigma: Redução de defeitos e variação nos processos.
•	Lean: Eliminação de desperdícios e maximização do valor.
•	Kaizen: Melhoria contínua com mudanças incrementais.
🔹 Integração de Processos
•	Integração por TI: Sistemas como ERP para conectar áreas da organização.
•	Automação de Processos: Uso de software para reduzir intervenção humana.
•	Comunicação Interdepartamental: Melhoria na troca de informações entre departamentos.
🔹 Gestão Estratégica de Processos
•	Alinhamento com Estratégia: Garantir que processos atendam aos objetivos organizacionais.
•	Mapeamento Estratégico: Definir processos necessários para alcançar as metas.
•	Avaliação de Performance: Monitoramento contínuo dos processos para garantir sucesso.
•	Desenvolvimento de Capacidades: Melhorar as capacidades organizacionais para execução eficaz.
🔹 Output: resultado direto e tangível (ou intangível) de um serviço.
🔹 Outcome: impacto duradouro ou benefício que o resultado gera ao cliente ou organização no tempo.
🔹 Tempo de recuperação (OTR) descreve o tempo máximo aceitável que pode decorrer após a interrupção do serviço até que a sua falta cause impacto na organização.

Planejamento Estratégico: Processo de análise, formulação e implementação de estratégias para alcançar os objetivos organizacionais de longo prazo.
•	Fases: Análise do ambiente (interna e externa), definição de objetivo, formulação de estratégias, implementação e monitoramento.
Balanced Scorecard (BSC): Equilibrar metas financeiras e não financeiras para alcançar os objetivos estratégicos.
🔹 Perspectivas: Financeira: Resultados financeiros
•	Clientes: Satisfação e fidelidade do cliente.
•	Processos Internos: Eficiência dos processos internos.
•	Aprendizado e Crescimento: Capacitação dos funcionários e inovação.
Planejamento Estratégico Situacional (PES): Planejar ações estratégicas baseadas na análise do contexto e nas necessidades reais da organização.
🔹 Fases: Diagnóstico situacional. Formulação de estratégias. Implementação e avaliação.
Análise de Cenários: Antecipar mudanças e riscos, criando estratégias para lidar com cenários distintos.
🔹 Fases: Identificação de fatores chave. Elaboração de cenários futuros. Desenvolvimento de estratégias para diferentes cenários.
Metodologias para Medição de Desempenho: métodos usados para avaliar a eficácia das ações organizacionais.
•	Indicadores chave de desempenho (KPIs): Medidas específicas para avaliar o progresso.
•	Métricas financeiras: Como lucro, ROI.
•	Métricas não financeiras: Satisfação do cliente, eficiência dos processos.
Indicadores de Desempenho: Medidas quantitativas e qualitativas que avaliam o desempenho organizacional.
•	Formulação: Definir metas claras e mensuráveis.
•	Análise: Acompanhamento contínuo e ajustes nas estratégias com base nos resultados obtidos.
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
🔹 Técnicas de Validação e Ajuste de Modelos
- Validação Cruzada: Técnica usada para avaliar o desempenho do modelo. Tipos: 
•	Holdout: Divide os dados em treino e teste (ex.: 80%-20%).
•	K-Fold: Divide os dados em K partes e treina k vezes.
•	Leave-One-Out (LOO): Cada dado é testado individualmente.
- Overfitting: Modelo memoriza os dados e não generaliza bem. 
•	Solução: Regularização (L1, L2), poda de árvores, dropout em redes neurais.
- Underfitting: Modelo não aprende padrões suficientes. 
•	Solução: Aumentar complexidade do modelo, adicionar mais dados.
🔹 Arquitetura MVC e Princípios de Projeto
•	Modelo-Visão-Controlador (MVC) – Divide a aplicação em três camadas: 
•	Modelo – Gerencia dados e regras de negócio.
•	Visão – Interface do usuário.
•	Controlador – Coordena a interação entre Modelo e Visão.
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
Perímetros de segurança: defesas que protegem a rede e as aplicações contra acessos não autorizados e ataques cibernéticos. Inclui ferramentas e sistemas que monitoram, controlam, protegem dados dentro e fora da rede.
Firewall - Defesa de rede, decide o que pode entrar e sair. software (um servidor) ou hardware (um dispôs. dedicado).
🔹 Firewall Proxy = Intermediário entre usuário e a rede, segurança e cache
•	filtra solicitações e respostas de rede. Pode oferecer cache, aumentando a velocidade de navegação.
•	Protege a rede ao ocultar o endereço IP interno e examinar profundamente o tráfego.
WAF (Web Application Firewall) - Protege as aplicações web contra ataques como SQL Injection e XSS
•	Camada de segurança aplicações web, filtrar, monitorar e bloquear ataques direcionados a app, SQL Injection XSS
SIEM (Security Information and Event Management) - Coleta e analisa logs para detectar e responder a ameaças
Identity and Access Management (IAM) - Garante quem pode, o quê e quando. Controla id e permissões de acesso.

Privileged Access Management (PAM) - Controla e monitora o acesso de usuários privilegiados
•	Sub do IAM, Assegura que o acesso a contas críticas seja monitorado e controlado.
IPTables - Firewall em Linux, controla pacotes e tráfego
IDS/IPS (Intrusion Detection System/Intrusion Prevention System) 
•	IDS (Sistema de Detecção de Intrusões): Detecta e alerta sobre possíveis intrusões ou atividades suspeitas 
•	IPS (Sistema de Prevenção de Intrusões): Vai além, bloqueando ativamente as ameaças detectadas.
VPN (Virtual Private Network) - Rede segura pela internet, garante privacidade
•	Criptografa comunicação entre o dispositivo do usuário e a rede, garantindo confidencialidade e integridade.
Antivírus: Software projetado para detectar, prevenir e remover malware (vírus, worms, trojans).
Antispam: Ferramenta para bloquear ou filtrar e-mails indesejados, pode ser um vetor para phishing ou malware.
AntiDDoS - Protege contra ataques DDoS, mantém a rede no ar
•	Proteção contra ataques de negação de serviço distribuída: é uma tecnologia que detecta e mitiga ataques DDoS, garantindo que a infraestrutura da rede permaneça funcionando durante o ataque.
Ameaças e ataques:
🔹 Negação de serviço (DoS/DDoS) – Sobrecarga de sistema para tirá-lo do ar.
🔹 Ataques de reconhecimento – Coleta de informações para invasões futuras.
🔹 Sniffing – Captura de tráfego de rede.
🔹 Spoofing – Falsificação de identidade para enganar sistemas.
Gerenciamento de Redes envolve a administração, monitoramento e controle de redes de computadores 
 SNMP (Simple Network Management Protocol) - Protocolo para monitorar e gerenciar dispositivos de rede (roteadores, switches, servidores). Dispositivos enviam informações p/ sistema centralizado, que pode coletar e gerenciar 
MIBs (Management Information Bases) - BD que armazena as informações dos dispositivos gerenciados, como uso de CPUne nível de memória. Estruturadas em árvore hierárquica com variáveis e valores a serem consultados via SNMP.
NMS (Network Management System) - Gerenciar e monitorar dispositivos de rede, com interface gráfica. Coleta dados do SNMP e exibe de forma visual e interativa para os administradores de rede. 
Agentes SNMP - Sensores nos dispositivos de rede que coletam dados e enviam para o NMS
Ferramentas de monitoramento: Usadas para coletar, analisar e visualizar dados de desempenho de sistemas, aplicativos e redes. Ajudam na detecção de falhas, análise de tendências e melhoria de performance.
Logging: Coleta de logs (registros) de eventos/transações em sistemas p/ monitoramento contínuo, auditoria e diagnóstico.
🔹 Zabbix 
•	Funcionalidades: Monitora métricas de desempenho, como uso de CPU, memória, disco, além de realizar detecção de falhas e alertas automáticos.
🔹 Grafana - Visualização de dados com painéis e gráficos interativos
•	Funcionalidades: Permite gráficos dinâmicos, dashboards customizáveis, alertas visuais e integração com várias fontes de dados.
🔹 Elasticsearch - Pesquisa e análise de grandes volumes de dados em tempo real
•	Geralmente é parte de um stack mais amplo, como o ELK Stack (Elasticsearch, Logstash e Kibana).
•	Funcionalidades: Indexa e pesquisa grandes volumes de dados, oferece consultas em tempo real e é altamente escalável.
🔹 Kibana - Visualização dos dados do Elasticsearch em gráficos e painéis
•	Funcionalidades: Criação de gráficos, mapas de calor e dashboards para exibir dados históricos e em tempo real.
🔹 Application Performance Monitoring (APM) - monitoram a performance de aplicações em tempo real
•	Funcionalidades: Monitora tempo de resposta, latência, transações, erros de código e uso de recursos de aplicações em tempo real.
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
Backup: Processo de criar cópias de segurança dos dados p/ proteção contra.
🔹 Políticas de Backup: Definem regras, procedimentos e estratégias p/ realização de backups. Devem incluir:
Frequência, Tipo de backup, Armazenamento, Retenção: Por quanto tempo, Recuperação Como, Testes
🔹 Política de Backup = 4 Rs:
•	Regularidade: Frequência dos backups (diário, semanal, etc.).
•	Retenção: Quanto tempo os backups são guardados.
•	Recuperação: Como recuperar os dados em caso de falha.
•	Revisão: Verifique se os backups funcionam e estão completos.
Tipos de Backup:
🔹 Backup Completo (Full Backup): É a cópia completa, sempre. 
🔹 Backup Incremental: Copia o que mudou depois do último backup ("incremento" é um "acréscimo"). 
🔹 Backup Diferencial: Copia o que mudou desde o último full.
🔹 Backup Espelhado (Mirror Backup): Cópia exata dos dados de origem, sem compressão ou deduplicação.
🔹 Backup em Nuvem: Armazenamento em provedores de serviços de nuvem (ex: Google Drive, AWS S3).
Veritas NetBackup - Backup Corporativo Pesado e Recuperação de Dados
•	Suporta backup em nuvem, dispositivos locais e servidores remotos.
•	Oferece recuperação automatizada e escalabilidade.
•	Suporta backup de dados em ambientes multi-plataforma.
Robocopy (Robust File Copy): nativa do Windows para cópia de arquivos e diretórios com funcionalidades avançadas. 
•	Suporta cópias incrementais e recuperação de falhas.
•	Permite configurar logs para monitoramento.
RSync: backup e sincronização de arquivos que utiliza um algoritmo eficiente para copiar e sincronizar dados entre sistemas locais e remotos. "Sincronização Inteligente"
•	Utiliza compressão e deduplicação, otimizando o uso de banda e espaço.
•	Suporta sincronização incremental, ou seja, somente os dados alterados são copiados.
•	Amplamente utilizado em sistemas Unix/Linux.
•	RSync como detetive: só copia o que mudou e faz de forma eficiente, sem sobrecarregar.
Deduplicação: limpar o espaço de armazenamento eliminando arquivos redundantes. "Evitar Repetição"
•	Elimina duplicatas de arquivos ou dados armazenados, reduzindo o uso de espaço.
•	Pode ser feita de forma local (no servidor de backup) ou remota (na nuvem).
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

Lei nº 8.112/1990
🔹 Ingresso no Serviço Público
•	Concursos públicos: Obrigatórios para todos os cargos de provimento efetivo.
•	Nomeação: Após aprovação em concurso, o servidor é nomeado para o cargo.
•	Estágio probatório: Até 3 anos para avaliar sua aptidão para o cargo.
🔹 Direitos dos Servidores Públicos
•	Remuneração: O servidor tem direito à remuneração pelo exercício de suas funções.
•	Licença: O servidor pode ter direito a licenças saúde, maternidade e outras previstas na lei.
•	Estabilidade: Após o estágio probatório, o servidor adquire a estabilidade no cargo.
•	Aposentadoria: O servidor tem direito à aposentadoria conforme as regras estabelecidas pela lei.
🔹 Deveres dos Servidores Públicos
•	Lealdade e probidade: Atuar com lealdade ao Estado e com probidade no exercício do cargo.
•	Eficiência: É obrigação do servidor realizar suas atividades com eficiência e de forma responsável.
•	Sigilo: O servidor deve manter sigilo sobre informações confidenciais.
•	Assiduidade e pontualidade: O servidor deve cumprir seus horários de trabalho e ser assíduo.
🔹 Penalidades
•	Advertência: Aplicada em caso de infração leve.
•	Suspensão: O servidor pode ser suspenso por até 90 dias.
•	Demissão: O servidor pode ser demitido por infrações graves, como abandono de cargo.
•	Cassação de aposentadoria: Em casos graves, a aposentadoria pode ser cassada.
🔹 Licenças 
1. Licença para Tratar de Interesse Particular sem R$
•	Prazo: Até 3 anos, podendo ser renovada por igual período, com limite máximo de 3 anos.
2. Licença para Tratamento de Saúde com R$ integral ou proporcional (necessidade médica)
•	Prazo: prazo é dado pela autoridade médica, podendo ser prorrogado, desde que haja justificativa.
3. Licença à Gestante com R$ integral
•	Prazo: 120 dias (4 meses), podendo ser prorrogado por até mais 60 dias, caso a gestante opte pela prorrogação.
4. Licença à Adotante com R$ integral
•	Prazo: 120 dias (4 meses), a partir da adoção da criança.
5. Licença-Paternidade com R$ integral
•	Prazo: 5 dias corridos, a partir do nascimento do filho.
6. Licença por Motivo de Doença em Pessoa da Família com R$ integral
•	Prazo: Até 30 dias consecutivos, pode prorrogado por + 30 dias, com comprovação da necessidade.
7. Licença para o Servidor Exercente de Mandato Classista com R$ integral
•	Prazo: Durante o período do mandato classista.
8. Licença para Desempenho de Mandato Eletivo sem R$
•	Prazo: Durante o mandato eletivo, pode o servidor reassumir seu cargo quando o mandato acabar.
9. Licença para Tratamento de Saúde Mental com R$ integral depend da avaliação médica
•	Prazo: Até 24 meses, conforme recomendação médica, com possibilidade de prorrogação.
10. Licença para Realização de Cursos de Pós-Graduação sem R$
•	Prazo: Depende da necessidade do curso e da autorização do órgão competente.
11. Licença para Capacitação com R$ integral
•	Prazo: varia o tipo, é de acordo com o planejamento do servidor e da administração pública.
12. Licença para Servidores Acidentados em Serviço com R$ integral
•	Prazo: determinado pela necessidade do tratamento e recuperação, conforme avaliação médica.
13. Licença para o Servidor que Se Encontra em Situação de Risco Imediato com R$ integral
•	Prazo: O prazo será determinado pela autoridade competente, dependendo da situação.
🔹 Regime Disciplinar
•	Abandono de cargo: Não comparecer + de 30 dias consecutivos pode ser demitido.
•	Improbidade administrativa: Pode ser punido com demissão/cassação de aposentadoria.
•	Desídia: Falta de interesse ou negligência no trabalho, podendo levar a advertência ou suspensão.
🔹 Procedimentos Administrativos: em caso de infrações, o servidor deve ser submetido a um PAD
•	Inquérito administrativo: Para apurar a infração cometida, um inquérito é instaurado.
•	Defesa: O servidor tem o direito de se defender antes de qualquer penalidade ser aplicada.
•	Decisão: Após apuração e defesa, a decisão final é tomada pela autoridade competente.
Indiciamento e Citação	10 dias	Para apresentação de defesa escrita após ser indiciado.
Relat Final da Comissão	Até 60 dias (+ 60)	Comissão deve concluir o processo no prazo, 
Decisão da Aut Julga	20 d após o relatór final	A decisão pode absolver, aplicar penalidade ou arquivar.
Recurso Adm	30 d ciência decisão	servidor pode recorrer à autoridade superior da que deu a penalidade.
Revisão de PAD	A qualquer tempo	Se surgirem fatos novos ou provas que justifiquem rever a penalidade.
Situação	Pode Perder Cargo?	Condições
Estável por PAD	✅ Sim	Após apuração com ampla defesa e contraditório
Estável por sentença	✅ Sim	Sentença judicial transitada em julgado
Estágio probatório	✅ Sim	Avaliação insatisfatória durante o período
Recondução	🔄 Sim (retorna ao anterior)	Se inabilitado em estágio probatório ou reintegração do ocupante
Reversão	🔄 Sim 	Aposentado por invalidez ou voluntária nos últimos 5 anos
Demissão (Perda da Função)
Decorrente de infração disciplinar grave. Ex: inassiduidade, improbidade, abandono de cargo, corrupção.
Perda de Cargo (Servidor Estável)
Só pode ocorrer: 
✅ em virtude de sentença judicial transitada em julgado;
✅ processo administrativo disciplinar (PAD) com ampla defesa;
✅ mediante procedimento de avaliação de desempenho, garantida ampla defesa.
Carreiras
1. Analista Judiciário (nível superior)
2. Técnico Judiciário (nível médio)
3. Auxiliar Judiciário (extinta para novos ingressos)
Progressão	Passagem do servidor para o padrão de vencimento seguinte dentro da mesma classe.	✅ 12 meses no padrão atual (interstício)
✅ Resultado satisfatório na avaliação de desempenho
Promoção	Passagem do servidor do último padrão de uma classe para o primeiro padrão da classe seguinte.	✅ 12 meses no padrão atual
✅ Resultado satisfatório em duas avaliações de desempenho consecutivas ou 2 em um período de 5 anos
Analista Judiciário	A, B, C	5 padrões por classe	Ingressa na Classe A, Padrão 1
Técnico Judiciário	A, B, C	5 padrões por classe	Ingressa na Classe A, Padrão 1
GAJ – Gratificação de Atividade Judiciária	Percentual sobre o vencimento básico: 90% do vencimento básico dos cargos efetivos
GAE – Gratificação de Atividade Externa	Exclusiva para cargos com atividades externas (ex: oficiais de justiça) – percentual específico
Adicional de Qualificação (AQ)	Para servidores com cursos de especialização, mestrado ou doutorado reconhecidos
Lei nº 9.784/1999:
1.	Princípio da Legalidade: Adm Pública agir sempre de acordo com a lei.
2.	Princípio da Impessoalidade: sem favoritismo, em busca do interesse público e não de interesses pessoais.
3.	Princípio da Moralidade: princípios éticos e de boa-fé, sempre com respeito aos direitos e deveres do cidadão.
4.	Princípio da Publicidade: garantindo que a sociedade tenha conhecimento e acesso às decisões
5.	Princípio da Eficiência: utilizando os recursos disponíveis com o máximo de eficácia, eficiência e efetividade.
6.	Princípio da Ampla Defesa e do Contraditório
7.	Princípio da Proporcionalidade: não sendo excessivos ou desnecessários.
8.	Princípio da Razoabilidade: sem excessos, respeitando o bom senso e evitando medidas arbitrárias.
Início e Procedimento do Processo Administrativo: de ofício (iniciativa da Adm) ou a pedido do interessado.
Publicidade dos Atos Administrativos: salvo em casos de sigilo justificados (ex: segurança nacional).
Decisão Motivada: fundamentada, com a exposição dos motivos de fato e de direito que a justificam.
Notificação/Intimação: ser notificado sobre a instauração e ser intimado das decisões que afetem seus direitos.
Súmula de Decisões: Adm deve manter registro das decisões tomadas, de forma que haja uma continuidade. 
Revisão de Atos Administrativos: podem revogados por conveniência administrativa ou anulados por ilegalidade. A revogação é um ato discricionário, enquanto a anulação é um ato vinculativo, devido a vícios de legalidade.
Atos Administrativos Nulos: com vício de ilegalidade é nulo, passível de anulação pela própria Adm Púb ou Jud.
Exceções: Sigilo: quando necessário para a segurança do Estado, a ordem pública, ou inf de interesse privado.
Interesse Público: interesse público como prioridade.
Prazo para decisão do processo administrativo:
o	Prazo geral: decidir o processo até 30 dias, a partir do início do processo.
	Prorrogação: por igual período, desde que seja justificado e comunicado ao interessado.
Prazo para manifestação do administrado: manifestar, apresentar documentos e justificar sua posição.
o	Prazo geral: 10 dias após notificado sobre a instauração do processo/proposta de decisão
Prazo para recurso administrativo: administrativo prejudica o adm, ele pode interpor um recurso administrativo.
o	Prazo: O prazo para interposição de recurso é de 10 dias, contados da ciência da decisão
Prazo para reconsideração: reconsiderar um ato ou decisão é de 5 dias.
Prazo para conclusão do processo: de 30 dias, podendo prorrogar 1x vez por igual período 
Prazo de resposta ao pedido de informações: LAI 20 dias, prorrogáveis por mais 10 dias, caso haja justificativa.
2.	Notificação e intimação: toma uma decisão, ela deve notificar o interessado de forma clara e precisa.
o	Prazo: A notificação e a intimação devem ser feitas dentro de um prazo razoável, mas não especifica.
Prazos: Adm Pub não se manifeste dentro do prazo, a parte interessada solicita decisão/arquivamento do processo.
Suspensão do prazo: necessidade de diligências complementares, prazo pode ser suspenso. Se admi não for encontrado ou necessidade de providências que dependem de terceiros (infor externas), pode suspenso tempo determinado

SQL Injection	O atacante insere comandos SQL maliciosos em campos de entrada (como formulários), para acessar e modificar o banco de dados.	Validação e higienização de entradas de usuário, uso de consultas preparadas e práticas de segurança de banco de dados.
Cross-Site Scripting (XSS)	O atacante injeta código JavaScript malicioso em páginas web que, quando carregadas pelo usuário, executam ações maliciosas.	Sanitização de entradas de usuário, uso de Content Security Policy (CSP) e escapar caracteres especiais no HTML.
Cross-Site Request Forgery (CSRF)	O atacante engana o usuário para que ele realize uma ação indesejada em um site onde está autenticado.	Uso de tokens CSRF em formulários, verificação de origem dos pedidos e manter o usuário logado por sessões curtas.
Drive-By Download	O atacante utiliza vulnerabilidades em sites para instalar malware no computador da vítima sem seu conhecimento.	Manter o navegador e plugins atualizados, utilizar bloqueadores de scripts e ter antivírus ativo.
Man-in-the-Middle (MitM)	O atacante intercepta e altera a comunicação entre o cliente e o servidor, roubando ou modificando dados.	Criptografar a comunicação com HTTPS, utilizar certificados digitais e verificar a identidade dos servidores.

Ameaças em Redes e Wireless
DoS (Denial of Service)	Ataque simples de uma única fonte. Visa sobrecarregar sistema-alvo.	Um host envia tráfego até esgotar recursos
DDoS (Distributed DoS)	Ataque distribuído a partir de várias máquinas (botnet).	Usa centenas ou milhares de dispositivos zumbis
UDP Flood	Envio maciço de pacotes UDP aleatórios para sobrecarregar portas.	Não exige conexão prévia, rápido e difícil de mitigar
TCP SYN Flood	Explora a conexão TCP enviando múltiplos SYN sem finalizar o handshake.	Consome memória e recursos do servidor
HTTP Flood	Envio de requisições HTTP (GET ou POST) massivas para sobrecarregar webservers.	Difícil de distinguir de tráfego legítimo
ICMP Flood (Ping Flood)	Uso intensivo de pacotes ICMP (ping) para congestionar banda e processamento.	Requer grande largura de banda
DNS Amplification	Envia requisições DNS forjadas que resultam em grandes respostas ao alvo.	Ataque indireto com alta taxa de amplificação
NTP Amplification	Similar ao DNS, mas usando servidores NTP (Network Time Protocol).	Resposta chega a ser 500 vezes maior que a requisição
Smurf Attack	Envio de ICMP para endereço broadcast com IP do alvo (spoofing).	Obsoleto, mas ainda pode ocorrer se redes não forem filtradas
Slowloris	Abre conexões HTTP e mantém-nas incompletas por longos períodos.	Afeta servidores Apache e similares, usa baixo tráfego
Ping of Death	Envio de pings malformados acima do tamanho permitido (fragmentação anormal).	Hoje mitigado por sistemas modernos
Teardrop Attack	Envio de pacotes IP fragmentados com sobreposição incorreta.	Explora falhas antigas no reassemblamento de pacotes
🔹 Como prevenir:
1.	DoS/DDoS: Implementar firewalls, sistemas anti-DDoS, CDNs e rate limiting.
2.	Spoofing: Autenticação forte, criptografia de tráfego e verificação de pacotes.
3.	Sniffing: Criptografar comunicação, usar VPNs e Wi-Fi seguro.

Evil Twin	O atacante cria um ponto de acesso Wi-Fi falso com o mesmo nome (SSID) de uma rede legítima, fazendo com que os usuários se conectem a ele.	Evitar conectar-se automaticamente a redes Wi-Fi, verificar o nome da rede antes de se conectar e usar VPNs.
War Driving	O atacante dirige por áreas públicas e mapeia redes Wi-Fi vulneráveis, buscando redes abertas ou mal configuradas.	Usar criptografia WPA2 ou WPA3, ocultar o SSID e verificar a segurança da rede regularmente.
WPA/WPA2 Cracking	O atacante tenta quebrar a senha de redes Wi-Fi protegidas com WPA/WPA2, utilizando técnicas como força bruta ou dicionário.	Usar senhas fortes e longas, evitar palavras comuns e habilitar o WPA3, que é mais seguro que o WPA2.
Replay Attack	O atacante captura pacotes de dados transmitidos na rede Wi-Fi e os retransmite para realizar ações fraudulentas, como acessar sistemas com dados antigos.	Usar criptografia forte, implementação de nonce (números aleatórios) e verificação de pacotes.
Jamming	O atacante envia sinais de rádio em frequências de Wi-Fi para bloquear a comunicação, causando desconexão ou falha na rede.	Usar redes com frequências diferentes e monitorar sinais de rádio para detectar interferências.
🧠DoS derruba, spoof engana, sniff espiona.

Ameaças por E-mail
Phishing	O atacante envia um e-mail que imita uma instituição legítima para enganar o usuário e obter dados confidenciais (como senhas e informações bancárias).	Não clicar em links suspeitos, verificar o remetente e usar ferramentas de filtro de spam. Ativar autenticação de dois fatores (2FA).
Spear Phishing	Ataque mais direcionado, onde o atacante personaliza o e-mail para um alvo específico, criando maior credibilidade.	Verificar o remetente e os links antes de clicar, usar ferramentas de verificação de links e manter softwares atualizados.
Business Email Compromise (BEC)	O atacante se passa por um executivo ou funcionário da empresa para fraudar transações financeiras ou obter informações confidenciais.	Treinamento de funcionários, verificar e-mails financeiros com um segundo canal de comunicação e usar ferramentas de detecção de fraude.
Malware Anexado	O atacante envia um e-mail com anexo malicioso (ex: vírus, trojan), que, ao ser aberto, compromete o sistema do usuário.	Não abrir anexos de fontes desconhecidas, ter antivírus atualizado e habilitar análise de segurança em e-mails.
Spoofing de E-mail	O atacante falsifica o endereço de e-mail do remetente para enganar o destinatário e fazer o e-mail parecer legítimo.	Verificar o domínio do e-mail, usar SPF, DKIM e DMARC para autenticação de e-mails e configurar sistemas de filtragem de e-mail.

Malwares
Termo	Descrição
Vírus	Malware que se anexa a arquivos e se propaga ao ser executado.
Cavalo de Troia	Malware disfarçado de software legítimo, permitindo acesso remoto.
Ransomware	Malware que criptoque ou bloqueia dados, exigindo resgate para liberá-los.
Spyware	Malware que espiona atividades e rouba dados do usuário.
Adware	Malware que exibe anúncios indesejados e pode redirecionar o tráfego.
Worm	Malware autossuficiente que se replica e se espalha sem intervenção.
Botnet	Rede de dispositivos infectados, controlados remotamente para ataques.
Rootkit	Malware que se oculta no sistema, permitindo acesso contínuo.
Backdoor	Porta dos fundos que permite acesso remoto sem ser detectado.
APT	Ataque sofisticado e persistente, direcionado a organizações específicas, com o objetivo de roubo de dados e espionagem.
Tabela de Macetes sobre o OWASP Top 10
Vulnerabilidade	Descrição
A1 - Broken Access Control	Falha no controle de acesso, permitindo acessos não autorizados.
A2 - Cryptographic Failures	Falha em criptografar dados sensíveis corretamente.
A3 - Injection	Inserção de comandos maliciosos, como SQL Injection.
A4 - Insecure Design	Falta de segurança no design e arquitetura da aplicação.
A5 - Security Misconfiguration	Configuração incorreta de segurança, expondo vulnerabilidades.
A6 - Vulnerable and Outdated Components	Uso de componentes desatualizados ou vulneráveis.
A7 - Identification and Authentication Failures	Falhas nos processos de autenticação e identificação.
A8 - Software and Data Integrity Failures	Manipulação de software ou dados, comprometendo sua integridade.
A9 - Security Logging and Monitoring Failures	Falta de registro e monitoramento de eventos de segurança.
A10 - SSRF	O servidor faz requisições externas ou internas em nome do atacante.

Ética: normas e valores que orientam comportamentos considerados adequados, justos e responsáveis
Programa de Integridade Corporativa: estabelecer cultura de integridade, compliance e ética dentro da organização.
🔹 Etapas de Elaboração:
•	Diagnóstico: Avaliação dos riscos éticos e de conformidade.
•	Políticas e Procedimentos: Criação de normas que guiem os colaboradores.
•	Treinamentos e Capacitação: Disseminação de conhecimentos sobre ética e compliance.
•	Canal de Denúncias: Ferramenta para comunicação de comportamentos inadequados.
🔹 Implementação:
•	Execução das Políticas: Colocação em prática as estratégias e processos definidos.
•	Designação de Responsáveis: Nomeação de profissionais para liderar a iniciativa.
•	Engajamento de Liderança: Comprometimento dos líderes para fomentar a cultura de integridade.
🔹 Monitoramento:
•	Avaliação Contínua: Medição da eficácia das políticas.
•	Auditorias e Revisões: Identificação de áreas de melhoria e ajustes necessários.
•	Relatórios de Conformidade: Avaliação do cumprimento das diretrizes e regras corporativas.
🔹 Boas Práticas: Cultura de Transparência/ Treinamento Contínuo/ Fomento à Ética/Responsabilidade Compartilhada: Todos na organização são responsáveis pela manutenção da integridade.

Práticas ESG Corporativa: Conjunto de práticas empresariais voltadas para os aspectos ambientais (Environmental), sociais (Social) e de governança (Governance).
🔹 Ambiental (E): Compromisso com a sustentabilidade e práticas que minimizem o impacto ambiental.
🔹 Social (S): Responsabilidade social com funcionários, fornecedores e comunidade, e respeito direitos hum.
🔹 Governança (G): Práticas empresariais transparentes, com boa gestão e responsabilidade fiscal.
•	Planejamento: Definir metas claras para cada área (ambiental, social e governança) e cronograma. 
•	Implementação: Integrar práticas ESG nas políticas/opers da emp. Envolver stakeholders e colaboradores 
•	Monitoramento: Realizar auditorias para garantir que as metas e objetivos ESG sejam cumpridos.
🔹 Boas Práticas ESG Corporativa: Transparência, Comprometimento de Liderança, Inovação e Melhoria 
Código de Conduta Ética: Documento que estabelece normas de comportamento e atitudes esperadas.
Código Disciplinar: Condutas inadequadas e as sanções em caso de infrações.
Planejamento e Gestão Estratégica de TI
🔹 PETI (Plano Estratégico de TI): Define diretrizes estratégicas para TI alinhadas ao negócio.
🔹 Planejamento Estratégico de TI (PETI): É definição d diretrizes e inic de TI alinhadas aos obj estratégicos 
🔹 Objetivos do PETI: Garantir que TI suporte os objetivos da empresa. Priorizar investimentos e projetos estratégicos. Melhorar eficiência e governança da TI. Reduzir riscos e aumentar segurança da informação.
Principais Elementos do PETI:
•	Missão, visão e valores da TI: Define o propósito e direção da TI.
•	Análise SWOT: Identifica forças, fraquezas, oportunidades e ameaças.
•	Mapeamento dos processos de TI: Alinha a TI às necessidades do negócio.
•	Plano de investimentos em TI: Define orçamento e prioridades.
PDTI (Plano Diretor de TI): Documento operacional para implementar a estratégia de TI.
🔹 Indicadores de Desempenho(KPIs): Mede eficácia e eficiência da TI, como SLA, disp. e tempo resposta.
Gestão Estratégica de TI: Adm contínua da TI com foco objetivos estratégicos, tecnologia contribua para o sucesso.
🔹 Objetivos da Gestão Estratégica de TI:
•	Acompanhar e ajustar o PETI conforme mudanças no negócio.
•	Gerenciar projetos e serviços de TI para garantir entrega de valor.
•	Medir e melhorar o desempenho da TI (indicadores e métricas).
•	Gerenciar riscos e conformidade regulatória.
🔹 Indicadores de Gestão Estratégica de TI:
•	SLA (Service Level Agreement): Tempo de resposta, disponibilidade.
•	ROI (Retorno sobre Investimento): Eficiência financeira da TI.
•	Métricas de Segurança: Incidentes, tempo médio de resposta a ameaças.
📌 PETI → Foco no planejamento de longo prazo e alinhamento estratégico.
📌 Gestão Estratégica de TI → Execução e monitoramento contínuo do PETI.
Brainstorming: técnica de geração de ideias em grupo. Criada por Alex Osborn.
🔹 Princípios:
•	Suspensão do julgamento: Nenhuma ideia deve ser criticada no momento da geração.
•	Quantidade sobre qualidade: Quanto mais ideias, maior a chance de encontrar boas soluções.
•	Livre associação: Ideias podem ser desenvolvidas a partir de outras.
•	Diversidade de pensamentos: Incentiva a participação de diferentes perfis e experiências.
🔹 Etapas:
•	Definição do problema: Estabelecer um tema ou desafio claro.
•	Geração de ideias: Participantes sugerem ideias livremente.
•	Registro das ideias: Anotação de todas as contribuições.
•	Discussão e refinamento: Seleção e aprimoramento das melhores ideias.
🔹 Variações:
•	Brainwriting: Ideias são escritas antes da discussão em grupo.
•	Brainstorming reverso: Participantes pensam formas de piorar o problema, e depois inverte a lógica.
•	Brainstorming digital: Uso de plataformas online para colaboração remota.
BPMN (Business Process Model and Notation): padrão gráfico para modelagem de processos de negócio. Criado pela OMG (Object Management Group), facilita a comunicação entre analistas de negócio, desenvolv. e gestores
•	Objetivo: Representar processos de forma clara e padronizada.
•	Uso: Automação de processos, melhoria contínua, análise de fluxo de trabalho.
🔹 Principais de elementos:
1️ Fluxo de Processo (Flow Objects)
•	Evento (círculo) – Início, fim e outros eventos que afetam o processo. 
⭕ Início (Start Event)
🎯 Intermediário (Intermediate Event)
⭕❗ Fim (End Event)
•	Atividade (retângulo com cantos arredondados) – ação ou tarefa a ser realizada. 
🔹 Tarefa (Task) – Uma única atividade executável.
🔹 Subprocesso (Subprocess) – Um conjunto de tarefas dentro do processo.
•	Gateway (losango) – Pontos de decisão ou ramificação no fluxo
🔀 Exclusivo (XOR) – Somente um caminho pode ser seguido.
🔄 Paralelo (AND) – Todos os caminhos são seguidos simultaneamente.
🔁 Inclusivo (OR) – Pode seguir um ou mais caminhos.
2️ Fluxo de Conexão (Connecting Objects) - Conexões que indicam a ordem das atividades
•	Sequência (seta cheia) – Define a ordem das atividades.
•	Mensagem (seta pontilhada) – Representa a troca de mensagens entre participantes.
3️ Swimlanes (Raia de Processo) - Representação de participantes ou departamentos
•	Pool – Representa um ator ou organização.
•	Lane – Subdivisão dentro de um pool para representar departamentos ou funções.
4️ Artefatos (Artifacts)
•	📜 Dados (Data Object) – Informações usadas ou geradas no processo.
•	🔖 Grupo (Group) – Agrupamento visual de atividades relacionadas.
•	📝 Anotações (Annotation) – Comentários para facilitar a compreensão.
🔹 Técnicas de Análise de Processos
•	Mapeamento de Processos: Identificação e documentação dos fluxos de trabalho.
•	Análise de Gargalos: Identificação de pontos de atraso ou ineficiência.
•	Análise de Valor Agregado: Avaliar valor agregado pelas atividades.
•	Análise de Fluxo de Trabalho: Verificação de redundâncias e falhas na comunicação.
🔹 Melhoria de Processos
•	PDCA (Plan, Do, Check, Act): Ciclo contínuo de planejamento, execução, verificação e ação.
•	Six Sigma: Redução de defeitos e variação nos processos.
•	Lean: Eliminação de desperdícios e maximização do valor.
•	Kaizen: Melhoria contínua com mudanças incrementais.
🔹 Integração de Processos
•	Integração por TI: Sistemas como ERP para conectar áreas da organização.
•	Automação de Processos: Uso de software para reduzir intervenção humana.
•	Comunicação Interdepartamental: Melhoria na troca de informações entre departamentos.
🔹 Gestão Estratégica de Processos
•	Alinhamento com Estratégia: Garantir que processos atendam aos objetivos organizacionais.
•	Mapeamento Estratégico: Definir processos necessários para alcançar as metas.
•	Avaliação de Performance: Monitoramento contínuo dos processos para garantir sucesso.
•	Desenvolvimento de Capacidades: Melhorar as capacidades organizacionais para execução eficaz.
Design Thinking: Centrada na pessoa para solução de problemas complexos, na colaboração e experimentação. 
🔹 Princípios 
•	Empatia: Compreender as necessidades do usuário.
•	Colaboração: Trabalho multidisciplinar para ampliar perspectivas.
•	Experimentação: Prototipação rápida e aprendizado contínuo.
•	Iteração: Testes constantes para refinar soluções.
🔹 Etapas (Stanford d.school): Dimersão (Empatia) → Def do Problema → Ideação → Prototipação → Teste 
Lean Startup: Foco na experimentação rápida, aprendizado contínuo e uso eficiente de recursos. Criada por Eric Ries, busca reduzir desperdícios e acelerar a inovação. Princípios 
•	Construir – Medir – Aprender: Processo cíclico de desenvolvimento e validação.
•	Produto Mínimo Viável (MVP): Versão simplificada do produto para testes rápidos.
•	Validação de hipóteses: Uso de feedback real para ajustar a solução.
•	Pivotagem (Pivot): Mudança de estratégia baseada em dados reais.
•	Iteração rápida: Pequenas melhorias constantes ao invés de grandes mudanças de uma vez.
🔹 Ciclo Lean Startup: Construir: Criar um MVP p/ testar hipóteses. Medir: Coletar dados e feedback dos usuários. Aprender: Analisar os resultados e decidir se mantém ou muda a estratégia.
MVP (Produto Mínimo Viável): versão mais simples de um produto que pode ser criada e colocada no mercado 
•	Funcionalidade básica: Só características essenciais para que os usuários interajam com o produto.
•	R$ reduzido: O MVP permite testar com o - de investimento possível, economizando recursos 
•	Feedback rápido: Coloca na rua p/ que usuários possam testar e fornecer feedback sobre a solução.
Pivotagem: permite que o negócio se reoriente com base no feedback real do mercado.
•	Pivotagem de produto: Alteração do próprio produto (funcionalidades ou modelo).
•	Pivotagem de mercado: Mudança no público-alvo para um mercado diferente.
•	Pivotagem de modelo de negócio: Mudança na forma como a empresa gera receitas 
Ciclo Construir-Medir-Aprender: etapas interativas e contínuas e adaptativa no desenvolvimento de produtos
1.	Construir: criar a versão + simples possível que permita testar as hipóteses de mercado
2.	Medir: como ele está sendo usado. dados quantitativos e qualitativos. 
3.	Aprender: a equipe avalia os resultados e aprende com as interações dos usuários. 
Contratação de TI: 
🔹 Tipos:
•	Aquisição de Software: Licenciamento de programas.
•	Serviços de TI: Consultoria, suporte, manutenção.
•	Infraestrutura de TI: Equipamentos, servidores, redes.
🔹 Processos de Licitação
 Modalidades:
•	Pregão: Licitação para aquisição de bens e serviços comuns.
•	Concorrência: Para contratações de maior valor.
•	Tomada de Preços: Para serviços com valor intermediário.
🔹 Fases:
•	Planejamento: Definir necessidades e requisitos.
•	Edital: Documento formal com condições da contratação.
•	Seleção: Processo de escolha do fornecedor.
•	Execução e Acompanhamento: Gestão da execução do contrato.
ISO/IEC 27001: Norma internacional para Sistemas de Gestão de Segurança da Informação (SGSI). Define requisitos para proteger informações e garantir confidencialidade, integridade e disponibilidade.
→ 27001 = Sistema de Gestão (manda)
→ 27002 = Guia de boas práticas (orienta)
•	Principais pontos: Gestão de riscos, política de segurança, controles de acesso, auditorias e melhoria contínua.
ISO/IEC 27005: Norma complementar à 27001, focada em Gestão de Riscos de Segurança da Informação.
•	Principais etapas: Identificação, análise, avaliação e tratamento de riscos.
•	 "I.A.T.R.A.M" Identificação → Análise → Tratamento → Aceitação → Monitoramento
Incidente de Segurança: Qualquer evento que comprometa a segurança das informações
🔹 Ciclo de Resposta a Incidentes (NIST SP 800-61):
1️ Preparação – Definir políticas, equipe de resposta (CSIRT) e ferramentas.
2️ Detecção e Análise – Identificação do incidente por logs, SIEM, alertas.
3️ Contenção, Erradicação e Recuperação – Conter impacto, remover ameaças e restaurar sistemas.
4 Pós-incidente – Analisar causa, documentar lições aprendidas e melhorar defesa.
Segurança da Informação: Proteção contra acessos não autorizados, alterações ou destruição de dados.
Confidencialidade – Restrição de acesso a usuários autorizados.
 Integridade – Garantia de que os dados não foram alterados sem permissão.
 Disponibilidade – Dados e sistemas devem estar acessíveis quando necessários.
Classificação da Informação: Categorização de dados com base na criticidade e impacto (ex. Restrita, Confidencial).
✅ Não repúdio – Garantia de que o autor de uma ação não pode negá-la (ex.: assinatura digital).
✅ Autenticidade – Confirmação da identidade de usuários ou sistemas.
✅ Segurança física – Proteção de servidores, redes e dispositivos físicos.
✅ Segurança lógica – Controles de acesso, criptografia e autenticação.
Lei de Acesso à Informação (Lei nº 12.527/2011)
🔹 Objetivo: Garantir transparência e acesso a informações públicas.
🔹 Abrangência: Todos os órgãos públicos dos três poderes.
🔹 Princípios:  Publicidade regra, sigilo como exc. Transparência ativa e passiva. Clareza e disp das informações.
🔹 Prazos: Resposta em até 20 dias, prorrogáveis por 10 dias. 
🔹 Exceções: Informações sigilosas (segurança nacional, dados pessoais).
Protocolos de Autenticação e Acesso
SSO (Single Sign-On)	Permite que o usuário acesse múltiplos sistemas com uma única autenticação.	Mecanismo de login	Empresas, Google Workspace, Microsoft AD	Maior conveniência; Reduz senhas	Se comprometido, afeta vários sistemas
OAuth 2.0	Protocolo de autorização delegada. Permite acesso limitado a recursos por apps.	Autorização (token)	Login com Google, APIs, apps mobile	Seguro, baseado em tokens; Sem senha compartilhada	Complexidade na implementação
OpenID Connect (OIDC)	Camada de identidade sobre o OAuth 2.0. Permite autenticação real de usuários.	Autenticação + OAuth	Autenticação federada, login social	Complementa OAuth; fornece dados do usuário	Requer compreensão de ambos protocolos
SAML (2.0)	Protocolo XML para SSO e autenticação entre domínios (B2B e SAML-based login).	Autenticação federada	Empresas, universidades, governo	Maduro, bem suportado em SSO empresarial	Baseado em XML; mais pesado e complexo
LDAP	Protocolo para consulta e autenticação em diretórios como o Active Directory.	Diretório / Acesso	Redes corporativas, autenticação interna	Rápido, centralizado, padrão aberto	Pouca segurança nativa (usa TLS ou LDAPS para proteger)
Kerberos	Protocolo de autenticação com base em “tickets”. Muito usado em ambientes Windows.	Autenticação segura	Windows, Active Directory	Seguro, usa criptografia simétrica	Complexo; sensível a sincronização de tempo
RADIUS	Protocolo para autenticação remota e AAA (auth, authorization, accounting).	Acesso remoto	Redes Wi-Fi empresariais, VPN	Centraliza controle de acesso remoto	Menos moderno; dependente da rede
MFA / 2FA	Múltiplos fatores de autenticação: algo que você sabe + tem + é (senha + token + biometria).	Fator de segurança	Bancos, e-mails, apps sensíveis	Alta segurança; dificulta invasões	Pode gerar fricção na experiência do usuário
Identidade Digital	Conjunto de atributos que identificam um usuário em um sistema.	Identificar o sujeito	Login, nome de usuário, e-mail, certificado digital
Autenticação	Processo de verificar se o usuário é quem diz ser.	Confirma identidade	Senha, biometria, token, autenticação via SSO
Autorização	Processo de conceder ou negar acesso a recursos com base na identidade verificada.	Controlar permissões	Acesso a arquivos, sistemas, permissões de administrador
Controle de Acesso	Conjunto de políticas para gerenciar quem pode fazer o quê em um sistema.	Definir e aplicar regras de acesso	ACL, RBAC, políticas de grupo (GPO)
Autenticação Multifator (MFA)	Combinação de dois ou mais métodos de autenticação.	Aumentar segurança	Senha + SMS, senha + biometria, token + autenticação facial
Single Sign-On (SSO)	Login único para acessar múltiplos sistemas.	Reduzir número de autenticações	Acesso ao Gmail + Drive + YouTube com uma conta Google
Provisionamento de Identidade	Criação, alteração e remoção de contas de usuários em sistemas e diretórios.	Gerenciar ciclo de vida da identidade	Ativação automática de contas, desativação após desligamento
Federation (Federação)	Compartilhamento de identidade entre domínios/sistemas diferentes.	Integração de autenticação entre domínios	Login com conta corporativa em sistema de terceiros
RBAC (Role-Based Access Control)	Controle baseado em papéis/funções atribuídos a usuários.	Atribuir acesso por função	"Usuário = Analista", logo tem acesso apenas ao sistema X
ABAC (Attribute-Based Access Control)	Controle baseado em atributos (usuário, recurso, contexto).	Controle mais granular e dinâmico	"Se for gerente + horário comercial + IP interno → acesso"
Least Privilege (Privilégio Mínimo)	Princípio de segurança onde o usuário recebe apenas as permissões estritamente necessárias.	Reduzir riscos	Usuário comum sem acesso de root/admin
IAM (Identity and Access Management)	Conjunto de processos e tecnologias para gerenciar identidades e acessos.	Governança de identidade e acesso	Azure AD, Okta, AWS IAM, Google IAM
Funções de Hash
Algoritmo	Tipo / Geração	Tamanho da Saída	Características Principais	Situação de Uso
MD5	Criptográfico (antigo)	128 bits	Rápido, mas inseguro (colisões conhecidas)	Verificação de integridade de arquivos simples (NÃO para segurança)
SHA-1	Criptográfico (antigo)	160 bits	Mais seguro que MD5, mas obsoleto – vulnerável a colisões	Git, SSL legado (depreciado para segurança)
SHA-256	Criptográfico (moderno)	256 bits	Altamente seguro, parte da família SHA-2, resistente a colisões	Assinaturas digitais, blockchain, tokens JWT
SHA-512	Criptográfico (moderno)	512 bits	Variante mais longa do SHA-256, usada quando se deseja maior segurança	Segurança de arquivos grandes ou críticos
SHA-3	Criptográfico (mais novo)	224 a 512 bits	Projeto independente do SHA-2 (usa Keccak); maior resistência a ataques	Aplicações modernas que exigem robustez extra
Bcrypt	Hash adaptativo	Variável (~192 bits)	Resistente a força bruta; possui "sal" e é lento por design	Armazenamento seguro de senhas
Scrypt	Hash adaptativo	Variável	Derivado de Bcrypt, ainda mais resistente (usa CPU + memória)	Senhas e carteiras de criptomoedas
PBKDF2	Derivação de chave	Variável	Usa HMAC + número alto de iterações; padrão em segurança corporativa	Senhas, autenticação, derivação de chaves
CRC32	Verificação (não criptográfico)	32 bits	Muito rápido, mas não é seguro; usado apenas para verificação de integridade	Compressão, redes, ZIP, arquivos ISO
•	Bcrypt, Scrypt, PBKDF2 → ideais para senhas.
•	CRC32 → não criptográfico, apenas checagem de erros.
Códigos de Autenticação de Mensagem (MACs)
Definição	Função criptográfica que gera um código-resumo (tag) com base em mensagem + chave secreta.
Objetivo	Garantir integridade (mensagem não foi alterada) e autenticidade (veio de quem diz ser).
Reversibilidade	Não aplicável: objetivo é verificar, não decifrar.
Base Criptográfica	MACs são geralmente baseados em algoritmos simétricos (ex: AES, SHA).
Verificação	O receptor recalcula o MAC com a mesma chave e compara com o MAC recebido.
HMAC	Baseado em hash	Usa SHA-1, SHA-256 ou SHA-3 com chave secreta. Robusto e muito usado.	Autenticação de APIs, TLS, autenticação JWT
CMAC	Baseado em AES	MAC construído sobre cifrador simétrico (ex: AES). Mais seguro que CBC-MAC.	Sistemas embarcados, NFC, IoT
CBC-MAC	Baseado em cifrador em modo CBC	Simples, mas inseguro para mensagens de tamanho variável.	Aplicações específicas com mensagens fixas
UMAC / VMAC	Baseados em universal hashing	Altíssimo desempenho, menos comuns.	Aplicações que exigem alta velocidade
KMAC	Baseado em SHA-3	Versão moderna e mais segura do HMAC com SHA-3.	Aplicações de segurança moderna (NIST compliant)
Princípios: Integridade: garante que a mensagem não foi alterada. Autenticidade: confirma que veio do remetente legítimo. Confidencialidade não é o foco do MAC (usa-se junto a criptografia, se necessário).
•	MAC≠Hash: hash ñ usa chave MAC usa com chave simétrica. não cifram, só validam origem + integridade.



