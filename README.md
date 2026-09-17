# 🛡️ Primeiros Cientistas da Cibersegurança

> Projeto desenvolvido como parte do desafio **"Caderno Temático com NotebookLM"** — Curso de Cibersegurança da DIO em parceria com o Santander Open Academy.

---

## 🎯 Contexto e Objetivos

**Assunto escolhido:** A história e as contribuições dos primeiros cientistas e pesquisadores que moldaram os fundamentos da Cibersegurança:

- Alan Turing
- Willis Ware
- Dorothy Denning
- Whitfield Diffie
- Martin Hellman
- Fred Cohen
- Donn Parker
- Bob Thomas
- Ray Tomlinson
- Leonard Adleman
- Basit e Amjad Farooq Alvi
- Robert Tappan Morris
- Entre outros

---

**Por que esse tema?**

> Acho importante saber como começou os primeiros ataques Cibernéticos e como foi o pensamento de criação de combate contra eles através de criptografia.
> A decodificação de criptografia e um vírus por brincadeira deram inicio a ataques em massa reais, assim como a criação de firewalls contra malwares.

---

**Objetivos de estudo:**

- [x] Conhecer as principais figuras históricas que fundaram os conceitos de segurança da informação;
- [x] Entender o contexto histórico (guerras, avanços tecnológicos) que motivou essas descobertas;
- [x] Relacionar essas origens com práticas de cibersegurança usadas atualmente;
- [x] Praticar curadoria de fontes e engenharia de prompts com IA como ferramenta de estudo.

---

## 📚 Curadoria de Fontes

| # | Título da Fonte | Tipo | Link |
|---|---|---|---|
| 1 | Creeper | Texto/Web | https://pt.wikipedia.org/wiki/Creeper_(vírus_de_computador) |
| 2 | Primeiro Vírus de Computador | Texto/Web | https://waveneo.com/primeiro-virus-de-computador-creeper-1971/ |
| 3 | Morris Worm | Texto/Web | https://pt.wikipedia.org/wiki/Morris_worm |
| 4 | Bell–LaPadula Model | Texto/Web | https://en.wikipedia.org/wiki/Bell–LaPadula_model |
| 5 | Paper acadêmico (web.cs.dal.ca) | PDF | https://web.cs.dal.ca/~gates/papers/nspw06.pdf |

---

## 🧠 Engenharia de Prompts e "Cicatrizes"

Aqui documento as perguntas estratégicas que testei no NotebookLM, os resultados obtidos e as dificuldades encontradas pelo caminho.

### Prompt 1

**Pergunta:** Como iniciou os primeiros ataques de vírus cibernéticos da história?

**Resposta obtida (resumo):**

> Os primeiros ataques e programas autorreplicantes de vírus de computador surgiram ao longo de um processo de evolução entre experimentos acadêmicos e infecções no mundo real:

#### 1. O Primeiro Experimento em Rede (1971)
- **Creeper (1971):** Criado pelo pesquisador Bob Thomas na BBN Technologies para testar se um código conseguiria se mover sozinho entre computadores conectados à rede **ARPANET**. O programa não causava danos, não apagava arquivos e não roubava senhas; apenas exibia a mensagem provocadora: *"EU SOU O CREEPER: PEGUE-ME SE FOR CAPAZ!"*.
- **Reaper (1972):** Criado por Ray Tomlinson para rastrear e apagar o Creeper da rede, sendo considerado o **primeiro antivírus da história**.

#### 2. Intenção Maliciosa e Disfarce (Anos 1970)
- **Rabbit (1974):** Foi um dos primeiros programas projetados com impacto prejudicial, duplicando-se tão rapidamente dentro do computador que esgotava os recursos do sistema e travava a máquina.
- **ANIMAL (1975):** Disfarçava-se de jogo de adivinhação de animais enquanto copiava silenciosamente o seu código para todos os diretórios do sistema, sendo considerado um dos primeiros registros de cavalo de Tróia.

#### 3. A Formalização Científica do Termo (1983–1984)
- **O Experimento na USC (1983):** O estudante de doutorado **Fred Cohen**, orientado pelo professor **Leonard Adleman** na University of Southern California (USC), desenvolveu um experimento em um sistema VAX-11/750 executando Unix. O programa propagou-se em questão de minutos, assumindo controle total do sistema.
- **Criação do Termo:** Leonard Adleman sugeriu a expressão **"vírus de computador"** para descrever esse comportamento autorreplicante.
- **Limites Matemáticos (1984):** Em sua tese, Fred Cohen provou matematicamente que é impossível construir um algoritmo de detecção perfeita capaz de identificar todas as variações de vírus sem gerar falsos positivos ou falsos negativos.

#### 4. A Primeira Epidemia no Mundo Real (1986)
- **Brain (1986):** Desenvolvido pelos irmãos Basit e Amjad Farooq Alvi no Paquistão, o programa tinha como objetivo inicial rastrear a pirataria de um software médico vendido por eles.
- **Disseminação Global:** O Brain infectava o setor de inicialização (*boot sector*) de disquetes de 5,25 polegadas em computadores MS-DOS. Foi o **primeiro vírus a sair de ambientes de laboratório e gerar uma infecção em massa** entre usuários comuns ao redor do mundo.

#### 5. O Ponto de Virada e o Primeiro Grande Ataque em Rede (1988)
- **Morris Worm (1988):** Criado por Robert Tappan Morris na Universidade Cornell para tentar medir o tamanho da rede. Por conta de uma exceção na lógica do código que forçava a reinfecção de máquinas que já continham o programa, ele se multiplicou descontroladamente.
- **Impacto na Internet:** O *worm* infectou e travou cerca de **6.000 dos 60.000 servidores** conectados à ARPANET/Internet na época (aproximadamente 10% de toda a rede). O caso levou à primeira condenação criminal sob a lei americana de fraudes e abusos computacionais.

**Fontes citadas pela IA:** Fontes de pesquisa do Wikipedia, cybersecbrazil.com.br e waveneo.com.

**Dificuldade encontrada:**
> Ela analisou as pesquisas que fiz nos sites e obtive um resumo completo. Não houve dificuldade.

### Prompt 2

**Pergunta:** Me mostre o cenário histórico referente às automações de defesa cibernética.

**Resposta obtida (resumo):**

O cenário histórico do desenvolvimento das **automações de defesa cibernética** reflete a transição de controles manuais e isolados para sistemas autônomos de monitoramento, detecção e resposta em tempo real. Essa evolução desdobrou-se em cinco grandes marcos históricos registrados nas fontes:

#### 1. A Abstração do Monitor de Referência e do Núcleo de Segurança (1972–1973)
- **Validação Automática de Acesso:** No relatório *Anderson Report* (1972) para a Força Aérea dos EUA, James P. Anderson introduziu o conceito de **Monitor de Referência** (*Reference Monitor*). A ideia era criar um mecanismo automatizado e à prova de adulterações (*tamper-proof*) que medisse e validasse obrigatoriamente cada tentativa de acesso entre sujeitos e objetos no sistema, sem depender de intervenção humana.
- **Security Kernels e MAC:** Esse modelo evoluiu para a implementação prática de **Núcleos de Segurança (*Security Kernels*)** e sistemas operacionais de alta confiança (como o GEMSOS, liderado por Roger Schell). Eles aplicam automaticamente o Controle de Acesso Obrigatório (MAC) por meio de instruções em hardware e firmware, garantindo a separação de domínios sem necessidade de intervenção do usuário.

#### 2. A Gênese do Monitoramento e Auditoria de Ameaças (1980)
- **Transformação de Logs de Auditoria:** Em 1980, James P. Anderson publicou o estudo seminal *Computer Security Threat Monitoring and Surveillance*. Até então, logs de sistema (como os registros SMF da IBM) eram usados apenas para faturamento e contabilidade.
- Anderson propôs processar esses registros automaticamente para rastrear **usuários clandestinos**, **usurpadores (*masqueraders*)** e **abuso de privilégios (*misfeasance*)**, estabelecendo a base para o surgimento dos Sistemas de Detecção de Intrusão (IDS) e para o processamento automatizado de eventos de segurança.

#### 3. IDES: O Primeiro Sistema Especialista em Tempo Real (1986–1987)
- **Detecção Estatística Automatizada:** Dorothy Denning desenvolveu o modelo **IDES** (*Intrusion Detection Expert System*). O IDES foi projetado como um sistema de correspondência de padrões baseado em regras e em tempo real.
- O sistema analisa automaticamente os registros de auditoria à medida que são gerados, comparando-os com **perfis estatísticos de comportamento** (medidos por contadores de eventos, temporizadores de intervalo e consumo de recursos) para identificar anomalias e gerar alertas automaticamente para o administrador.

#### 4. Autodefesa de Software e Limites Matemáticos da Automação (1983–1988)
- **Checksums Criptográficos Automatizados:** Em palestras sobre a dinâmica viral nos anos 1980, Fred Cohen propôs técnicas automatizadas de autodefesa para softwares. Isso incluía a inserção de verificadores criptográficos baseados em algoritmos como o RSA no próprio código dos programas para checar periodicamente a integridade de seus executáveis e dados.
- **Indecidibilidade Teórica:** Por outro lado, Cohen provou matematicamente (com base no problema da parada de Turing) que a detecção 100% perfeita de vírus de forma totalmente automatizada é **indecidível**, demonstrando que qualquer scanner de antivírus automático incorrerá inevitavelmente em falsos positivos ou falsos negativos.

#### 5. A Era Moderna: SIEM, IPS, Threat Feeds e Sandboxing
Com o avanço das redes abertas e da Internet, a automação defensiva expandiu-se para responder ao volume e à velocidade das ameaças modernas:
- **SIEM (*Security Information and Event Management*):** Evolução direta das trilhas de auditoria de Anderson, centralizando e correlacionando automaticamente logs e alarmes de múltiplos dispositivos de rede.
- **IPS (*Intrusion Prevention System*):** Ao contrário do IDS (que apenas alerta), o IPS automatiza a reação ativa por meio do bloqueio em tempo real (*shunning*) do tráfego ou do IP de origem assim que um ataque ou anomalia é detectado.
- **Feeds Automatizados de Inteligência (*Threat Feeds* & STIX/TAXII):** Firewalls e *gateways* modernos recebem fluxos automatizados de dados sobre ameaças (URLs, hashes e assinaturas de ataques) em tempo real via protocolos padronizados (como STIX e TAXII), ajustando suas regras de bloqueio sem dependência de ação manual.
- **Detonação Automática em Sandboxes:** Uso de ambientes virtualizados para isolar e executar automaticamente arquivos e anexos suspeitos, analisando seu comportamento de forma segura antes que cheguem aos sistemas finais.

**Fontes citadas pela IA:** Fontes de pesquisa do Wikipedia, cybersecbrazil.com.br e waveneo.com.

**Dificuldade encontrada:**
> Muitos sites e documentos em inglês que são difíceis de traduzir; algumas pesquisas não eram sobre o assunto escolhido, então perdi algum tempo escolhendo os resultados que eram realmente relevantes.

---

## 📖 Miniguia de Estudo (Entrega Final)

### Resumo Estruturado

#### 1. Alan Turing (1912–1954)
> Durante a segunda guerra mundial, utilizando uma máquina que desvendou o "Enigma" criado pelos alemães, conseguiu decodificar os códigos de comunicação entre generais e cientistas alemães.

#### 2. Dorothy Denning (1976)
> Estruturou matematicamente, usando redes, uma abordagem pioneira na área de detecção por meio de logs de auditoria para capturar intrusos.

#### 3. Fred Cohen e Leonard Adleman (1983–1984)
> Conduziram os estudos de código autorreplicável, provando matematicamente que é impossível um algoritmo com 100% de eficiência capaz de identificar um invasor de sistemas. Assim foi inaugurado o início dos estudos de malware.

---

### 📔 Glossário

| Termo | Definição |
|---|---|
| Cibersegurança | São códigos inseridos para tentar impedir ou atrasar um ataque de Malware... |
| Criptoanálise | Ciência de decifrar códigos sem ter a chave original. |
| Máquina Enigma | Dispositivo de criptografia usado pelos alemães na 2ª Guerra Mundial, quebrado por Turing e sua equipe. |
| *Dr. Martin Hellman* | Inventor da Criptografia de Chave Pública ao lado de Whitfield Diffie e Ralph Merkle na Universidade Stanford nos anos 1970. Hellman revolucionou o campo da Cibersegurança ao inventar a criptografia de chave pública e a troca de chaves Diffie-Hellman. |

---

### 🔁 Prompts Reutilizáveis para Revisão

Conjunto de prompts prontos para usar em revisões futuras deste tema:

1. `"Faça um resumo de 5 linhas sobre Kali_Linux para revisão rápida."`
2. `"Crie 5 perguntas de múltipla escolha sobre os pioneiros da Cibersegurança para eu testar meus conhecimentos."`
3. `"Explique sobre Kali_Linux como se eu tivesse 12 anos."`
4. `"Compare as contribuições de Alan Turing e os cientistas de Cibersegurança da atualidade."`

---

## 🔗 Link do Caderno no NotebookLM

📎 https://notebook.google.com/notebook/08451726-26cb-43ca-8775-e5675fa854b0

---

## 🚀 Sobre o Projeto

Este repositório foi criado como parte do desafio de projeto **"Cibersegurança"** da [DIO](https://www.dio.me/) em parceria com o **Santander Open Academy**.
