# 🛡️ Primeiros Cientistas da Cibersegurança



> Projeto desenvolvido como parte do desafio \*\*"Caderno Temático com NotebookLM"\*\* — Curso de Cibersegurança da DIO em parceria com o Santander Open Academy.



\---

## 

## 🎯 Contexto e Objetivos



**Assunto escolhido:** A história e as contribuições dos primeiros cientistas e pesquisadores que moldaram os fundamentos da Cibersegurança:  



\#Alan Turing 

\#Willis Ware 

\#Dorothy Denning 

\#Whitfield Diffie 

\#Martin Hellman 

\#Fred Cohen 

\#Donn Parker 

\#Bob Thomas

\#Ray Tomlinson

\#Leonard Adleman 

\#Basit e Amjad Farooq Alvi 

\#Robert Tappan Morris

**#Entre outros...**

**---**



**Por que esse tema?**



> Acho importante saber como começou os primeiros ataques Cibernéticos e como foi o pensamento de criação de combate contra eles através de criptografia.

> A decodificação de criptografia e um vírus por brincadeira deram inicio a ataques em massa reais, assim como a criação de firewalls contra malwares.



**---**



**Objetivos de estudo:**



* \[x] Conhecer as principais figuras históricas que fundaram os conceitos de segurança da informação;
* \[x] Entender o contexto histórico (guerras, avanços tecnológicos) que motivou essas descobertas;
* \[x] Relacionar essas origens com práticas de cibersegurança usadas atualmente;
* \[x] Praticar curadoria de fontes e engenharia de prompts com IA como ferramenta de estudo.



## \---

## 📚 Curadoria de Fontes



|#Sites de origem das pesquisas |Título da Fonte|Tipo|Link|
|-|-|-|-|
|1           Wikipedia|*Creeper*|Texto/Web|https://pt.wikipedia.org/wiki/Creeper\_(v%C3%ADrus\_de\_computador)|
|2           Wikipedia|Primeiro Vírus de Computador|Texto/Web|https://waveneo.com/primeiro-virus-de-computador-creeper-1971/|
|3           Wikipedia|Morris Worm|Texto/Web|https://pt.wikipedia.org/wiki/Morris\_worm|
|4           Wikipedia|LaPadula|Texto/Web|https://en.wikipedia.org/wiki/Bell%E2%80%93LaPadula\_model|
|5            Web.cs||PDF|https://web.cs.dal.ca/\~gates/papers/nspw06.pdf|



\---

🧠 Engenharia de Prompts e "Cicatrizes"

Aqui documento as perguntas estratégicas que testei no NotebookLM, os resultados obtidos e as dificuldades encontradas pelo caminho.

### 

### Prompt 1

**Pergunta:** Como iniciou os primeiros ataques de vírus cibernéticos da história?



**Resposta obtida (resumo):**



> Os primeiros ataques e programas autorreplicantes de vírus de computador surgiram ao longo de um processo de evolução entre experimentos acadêmicos e infecções no mundo real:



\### 1. O Primeiro Experimento em Rede (1971)

\* \*\*Creeper (1971):\*\* Criado pelo pesquisador Bob Thomas na BBN Technologies para testar se um código conseguiria se mover sozinho entre computadores conectados à rede \*\*ARPANET\*\*. O programa não causava danos, não apagava arquivos e não roubava senhas; apenas exibia a mensagem provocadora: \*"EU SOU O CREEPER: PEGUE-ME SE FOR CAPAZ!"\*.

\* \*\*Reaper (1972):\*\* Criado por Ray Tomlinson para rastrear e apagar o Creeper da rede, sendo considerado o \*\*primeiro antivírus da história\*\*.



\### 2. Intenção Maliciosa e Disfarce (Anos 1970)

\* \*\*Rabbit (1974):\*\* Foi um dos primeiros programas projetados com impacto prejudicial, duplicando-se tão rapidamente dentro do computador que esgotava os recursos do sistema e travava a máquina.

\* \*\*ANIMAL (1975):\*\* Disfarçava-se de jogo de adivinhação de animais enquanto copiava silenciosamente o seu código para todos os diretórios do sistema, sendo considerado um dos primeiros registros de cavalo de Tróia.



\### 3. A Formalização Científica do Termo (1983–1984)

\* \*\*O Experimento na USC (1983):\*\* O estudante de doutorado \*\*Fred Cohen\*\*, orientado pelo professor \*\*Leonard Adleman\*\* na University of Southern California (USC), desenvolveu um experimento em um sistema VAX-11/750 executando Unix. O programa propagou-se em questão de minutos, assumindo controle total do sistema.

\* \*\*Criação do Termo:\*\* Leonard Adleman sugeriu a expressão \*\*"vírus de computador"\*\* para descrever esse comportamento autorreplicante.

\* \*\*Limites Matemáticos (1984):\*\* Em sua tese, Fred Cohen provou matematicamente que é impossível construir um algoritmo de detecção perfeita capaz de identificar todas as variações de vírus sem gerar falsos positivos ou falsos negativos.



\### 4. A Primeira Epidemia no Mundo Real (1986)

\* \*\*Brain (1986):\*\* Desenvolvido pelos irmãos Basit e Amjad Farooq Alvi no Paquistão, o programa tinha como objetivo inicial rastrear a pirataria de um software médico vendido por eles.

\* \*\*Disseminação Global:\*\* O Brain infectava o setor de inicialização (\*boot sector\*) de disquetes de 5,25 polegadas em computadores MS-DOS. Foi o \*\*primeiro vírus a sair de ambientes de laboratório e gerar uma infecção em massa\*\* entre usuários comuns ao redor do mundo.



\### 5. O Ponto de Virada e o Primeiro Grande Ataque em Rede (1988)

\* \*\*Morris Worm (1988):\*\* Criado por Robert Tappan Morris na Universidade Cornell para tentar medir o tamanho da rede. Por conta de uma exceção na lógica do código que forçava a reinfecção de máquinas que já continham o programa, ele se multiplicou descontroladamente.

\* \*\*Impacto na Internet:\*\* O \*worm\* infectou e travou cerca de \*\*6.000 dos 60.000 servidores\*\* conectados à ARPANET/Internet na época (aproximadamente 10% de toda a rede). O caso levou à primeira condenação criminal sob a lei americana de fraudes e abusos computacionais.



💡 \*\*Gostaria de analisar em detalhes a prova matemática de Fred Cohen sobre a impossibilidade do antivírus perfeito, ou entender como o Morris Worm explorou as falhas dos sistemas Unix?



\*\***Fontes citadas pela IA:** Fontes de pesquisa do Wikipedia, cybersecbrazil.com.br e waveneo.com. 



**\*\*Dificuldade encontrada:**

> Ela analisou as pesquisas que fiz nos sites e obtive um resumo completo. Não ouve dificuldade 



\---

## 

## 📖 Miniguia de Estudo (Entrega Final)

### Resumo Estruturado

#### 

#### 1\. ####Alan Turing (1912–1954)

> Durante a segunda guerra mundial utilizando uma máquina que desvendou o "Enigma" criado pelos alemães, conseguiu decodificar os códigos de comunicação entre generais e cientistas alemães.  

#### 

#### 2\. ####Dorothy Denning (1976)

> Estruturou matematicamente usando redes foi pioneira na área de detecção de logs de auditoria para capturar intrusos.  

#### 

#### 3\. ####Fred Cohen e Leonard Adleman (1983–1984)

> Conduziram na época os estudos de código autorreplicáveis, provando matematicamente que é impossível um algoritmo com 100% de eficiência capaz de identificar um invasor de sistemas. Assim foi inaugurado o inicio dos estudos de malware.  

### 

### *---*

### 

### 📔 Glossário

|Termo|Definição|
|-|-|
|Cibersegurança|São códigos inseridos para tentar impedir ou atrasar um ataque de Malware...|
|Criptoanálise|Ciência de decifrar códigos sem ter a chave original.|
|Máquina Enigma|Dispositivo de criptografia usado pelos alemães na 2ª Guerra Mundial, quebrado por Turing e sua equipe.|
|*Dr. Martin Hellman/Herói da Engenharia de Stanford*|Inventor da Criptografia de Chave pública ao lado de Whitfield Diffie e Ralph Merkle na Universidade Stanford nos anos 1970. Hellman revolucionou o campo da Cibersegurança ao inventar a criptografia de chave pública e a troca de chaves Diffie-Hellman. |



\---

### 

### 🔁 Prompts Reutilizáveis para Revisão

Conjunto de prompts prontos para usar em revisões futuras deste tema:



1. `"Faça um resumo de 5 linhas sobre Kali\_Linux para revisão rápida."`
2. `"Crie 5 perguntas de múltipla escolha sobre os pioneiros da Cibersegurança para eu testar meus conhecimentos."`
3. `"Explique sobre Kali\_linux como se eu tivesse 12 anos."`
4. `"Compare as contribuições de Alan Turing e os cientistas de Cibersegurança da atualidade."`



\---

## 

## 🔗 Link do Caderno no NotebookLM



📎 https://notebook.google.com/notebook/08451726-26cb-43ca-8775-e5675fa854b0



\---

## 

## 🚀 Sobre o Projeto

Este repositório foi criado como parte do desafio de projeto **"Cibersegurança"** da [DIO](https://www.dio.me/) em parceria com o **Santander Open Academy**.

