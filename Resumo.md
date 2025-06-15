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

