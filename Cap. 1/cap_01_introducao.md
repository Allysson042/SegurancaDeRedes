<a name="br1"></a> 

Universidade Federal do

Agreste de Pernambuco

Av. Bom Pastor s/n - Boa Vista

55292-270 Garanhuns/PE

T +55 (87) 3764-5500

m http://www.ufape.edu.br

Bacharelado em Ciência da Computação

CCMP3079 Segurança de Redes de Computadores

Prof. Sérgio Mendonça

Atividade Cap. 01 - Introdução

10 de outubro de 2023.

Nome Completo: Allysson Guimarães dos Santos Silva

Questões retiradas do livro-texto da disciplina.

Conforme conversamos em sala de aula, as atividades devem ser realizadas para

apresentação e discussão em sala, sempre nas aulas das quintas-feiras, atribuindo ao

estudante uma nota de 0 ou 1 por cada atividade realizada e apresentada.

**1. O que é a arquitetura de segurança OSI?**

A arquitetura de segurança OSI baseia-se na necessidade das organizações possuírem políticas

de segurança e serviços que permitam avaliar tudo o que esteja relacionado com a segurança

de suas informações. Essa camada é responsável por fornecer mecanismos de segurança para

proteger a integridade, a autenticidade e a confidencialidade dos dados durante a comunicação

em uma rede. Esta camada lida com questões como criptografia, autenticação, controle de

acesso e auditoria.

**2. Qual é a diferença entre ameaças à segurança passivas e ativas?**

Ameaças passivas envolvem observação e obtenção de informações sem interagir diretamente

com o sistema, como espionagem e engenharia social. Ameaças ativas são mais diretas,

visando comprometer sistemas, como malware, ataques DDoS e phishing. A diferença está na

interação direta (ativas) ou não (passivas) com os sistemas-alvo e nas ações de

comprometimento versus observação. Ambos requerem medidas de segurança para proteger

sistemas e dados.

**3. Liste e defina resumidamente as categorias de ataques passivos e**

**ativos à segurança.**

**Ameaças Passivas:**

**Monitoramento de tráfego de rede:** Um atacante observa o tráfego de rede para

capturar informações confidenciais, como senhas, sem interferir ativamente na

comunicação.



<a name="br2"></a> 

**Espionagem:** O roubo de informações confidenciais ou segredos comerciais por

meio da observação ou obtenção de documentos ou dados sensíveis.

**Engenharia social:** Manipulação psicológica de indivíduos para obter informações

confidenciais, como convencer alguém a divulgar senhas.

**Ameaças Ativas:**

**Malware**: Software malicioso, como vírus, worms, trojans e ransomware, que é

projetado para infectar sistemas e realizar ações prejudiciais, como roubo de dados,

destruição de arquivos ou controle remoto do sistema.

**Ataques de negação de serviço (DDoS):** Sobrecarregar um sistema ou rede com

tráfego malicioso para torná-los inacessíveis aos usuários legítimos.

**Ataques de força bruta:** Tentativas repetidas de adivinhar senhas ou chaves de

criptografia para ganhar acesso não autorizado.

**4. Liste e defina resumidamente as categorias dos serviços de**

**segurança.**

**Serviços de Autenticação:** São serviços que verificam a identidade de usuários ou

sistemas antes de conceder acesso a recursos. Isso inclui autenticação de senha,

autenticação biométrica (como impressão digital ou reconhecimento facial) e

autenticação de dois fatores (2FA).

**Serviços de Autorização:** Envolve determinar as permissões de acesso

concedidas aos usuários autenticados. Define o que um usuário pode ou não fazer

após a autenticação. Isso inclui controle de acesso baseado em funções (RBAC) e

políticas de acesso.

**Serviços de Criptografia:** São serviços que protegem a confidencialidade dos

dados por meio da conversão de informações em um formato ilegível (cifrado). Isso

inclui criptografia de dados em repouso e em trânsito, bem como o gerenciamento

de chaves.



<a name="br3"></a> 

**Serviços de Auditoria e Monitoramento:** Envolve o acompanhamento das

atividades do sistema para detectar e responder a incidentes de segurança. Isso

inclui registro de eventos, análise de logs, detecção de intrusões e monitoramento

contínuo da segurança.

**5. liste e defina resumidamente as categorias dos mecanismos de segurança.**

**Controle de Acesso:** Regula o acesso a recursos, garantindo que apenas usuários autorizados

possam utilizá-los;

**Criptografia:** Codifica os dados para proteger sua confidencialidade e integridade;

Assinatura Digital: Fornece autenticidade e integridade em transações eletrônicas;

**Firewalls:** Monitoram e controlam o tráfego de rede, protegendo contra acessos indesejados;

**Detecção e Prevenção de Intrusões:** Identificam atividades maliciosas e tomam medidas para

detê-las;

**Segurança em Camadas:** Implementam várias camadas de defesa para proteger sistemas e

redes;

**Autenticação Multifator**: Exige múltiplos fatores para verificar a identidade dos usuários.

**Respaldo e Recuperação:** Realizam cópias de segurança e permitem a recuperação em caso

de falhas.

**6. Considere um caixa eletrônico, ATM no qual os usuários fornecem um cartão**

**e um número de identificação pessoal (senha). Dê exemplos de requisitos de**

**confidencialidade, integridade e disponibilidade associados com esse**

**sistema e, em cada caso, indique o grau de importância desses requisitos.**

**Confidencialidade:** Proteger dados de conta do usuário e PIN. A importância é muito alta

para evitar roubo de identidade e acesso não autorizado.

**Integridade:** Garantir a integridade de transações financeiras e software do ATM. A

importância é alta para evitar perdas financeiras e ataques.

**Disponibilidade:** Garantir acesso ao ATM e manutenção regular. A importância é alta para

evitar inconveniência e garantir operação confiável.



<a name="br4"></a> 

**7. Para responder as letras abaixo, por favor, consulte o livro-texto da disciplina:**

**(a) Desenhe uma matriz similar ao Quadro 1.4 que mostre o relacionamento**

**entre serviços de segurança e ataques.**

Vazamento de

conteúdo de

mensagens

Análise

de

Disfarce

Repasse

Modificação

de

Negação

do

tráfego

mensagens

serviço

Autenticação

x

x

Controle de

Acesso

x

Confiabilidade

dos dados

x

x

Integridade de

dados

x

x

Irretratabilidade

x



<a name="br5"></a> 

**(b) Desenhe uma matriz similar ao Quadro 1.4 que mostre o relacionamento**

**entre mecanismos de segurança e ataques.**

Vazamento de

conteúdo de

mensagens

Análise

de

Disfarce

Repasse

Modificação

de

Negação

do

tráfego

mensagens

serviço

Codificação

x

x

assinatura

digital

x

Controle de

acesso

x

x

x

integridade de

dados

x

Troca de

autenticaç

ão

x

preenchimento

de tráfego

x

x

Controle de

roteament

o

Notarização

x

x

