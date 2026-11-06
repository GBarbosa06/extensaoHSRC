# UNIVERSIDADE CATÓLICA DE BRASÍLIA – UCB
**Pró-Reitoria Acadêmica | Curricularização da Extensão Universitária**  
**Disciplina:** Extensão – Cooperação: Humanismo Solidário, Redes e Comunidades  
**Docente Responsável:** Prof. Marco Antonio de Abreu Machado  
**Aula 09:** Prototipagem Visual, Testes de Usabilidade e Coleta de Evidências  
**Atividade:** Exercício Prático Desafiador – Auditoria de Usabilidade e Crise Ética 
* **Aluno:** Guilherme de Andrade Barbosa - UC24101201
* **Comunidade Parceira:** Cooperativa Recicla Vida (Ceilândia – DF)

---

## 1. RECÁLCULO E META DE CONTINGÊNCIA MÉTRICA (TCR E SUS)

### 1.1 Diagnóstico do Cenário Crítico Inicial
* **TCR Registrado Inicialmente:** $33,33\%$ (Inadmissível para homologação extensionista; meta mínima $\ge 80\%$).
* **Score SUS Inicial:** $42,5$ pontos (Classificado como Grau F / Pior que a média histórica de $68,0$; atrito cognitivo severo).
* **Diagnóstico de Severidade:** Falha de Severidade Nível 4 (Catástrofe de Usabilidade no login e fluxo de pesagem), provocando abandono, desorientação e frustração no operador (Seu Valdemar, 64 anos).

---

### 1.2 Memória de Cálculo e Meta de Contingência do TCR (Task Completion Rate)

A fórmula canônica da Taxa de Conclusão de Tarefas é dada por:

$$TCR = \left[ \frac{\sum c_i}{N \times T} \right] \times 100\%$$

Onde:
* $N = 4$ usuários/operadores da cooperativa avaliados.
* $T = 3$ tarefas essenciais da rotina:
  * **$T_1$:** Autenticação Simplificada no Terminal de Pesagem.
  * **$T_2$:** Lançamento Rápido de Pesagem de Fardo.
  * **$T_3$:** Fechamento e Emissão do Romaneio Diário.
* $c_i = 1$ para sucesso autônomo sem intervenção; $c_i = 0$ para bloqueio ou necessidade de suporte.

#### Quadro Projetado de Validação Pós-Ajustes:

| Operador / Perfil | $T_1$: Autenticação (PIN) | $T_2$: Pesagem Direta | $T_3$: Romaneio | Sucessos Individuais |
| :--- | :---: | :---: | :---: | :---: |
| **Seu Valdemar (64a, Pesagem)** | 1 (Sucesso) | 1 (Sucesso) | 1 (Sucesso) | $3/3$ |
| **Dona Francisca (58a, Triagem)** | 1 (Sucesso) | 1 (Sucesso) | 0 (Hesitou na data) | $2/3$ |
| **Marcos (31a, Logística)** | 1 (Sucesso) | 1 (Sucesso) | 1 (Sucesso) | $3/3$ |
| **Raimundo (60a, Prensa)** | 1 (Sucesso) | 1 (Sucesso) | 1 (Sucesso) | $3/3$ |
| **Total de Sucessos por Tarefa** | **$4/4$** | **$4/4$** | **$3/4$** | **$11/12$** |

#### Demonstração Aritmética:
* **Total de tentativas planejadas:** $N \times T = 4 \times 3 = 12$ tarefas simuladas.
* **Total de tarefas concluídas com plena autonomia:** $4 + 4 + 3 = 11$ tarefas.
* **Razão de Eficácia:** $\frac{11}{12} = 0,91666...$
* **TCR Projetado:** $0,91666... \times 100\% = 91,67\%$

**Parecer Extensionista:** A redução de atrito elevou o TCR de $33,3\%$ para **$91,67\%$**, superando com folga o piso de contingência estipulado em $85,0\%$.

---

### 1.3 Memória de Cálculo e Meta de Contingência da Escala SUS (System Usability Scale)

A fórmula canônica do Score SUS (Brooke, 1986) é dada por:

$$\text{Score SUS} = \left[ \sum_{i \in \text{ímpares}} (R_i - 1) + \sum_{j \in \text{pares}} (5 - R_j) \right] \times 2,5$$

Onde as respostas variam de 1 (Discordo Totalmente) a 5 (Concordo Totalmente).

#### Tabulação Projetada da Resposta Média de Validação Comunitária:

| Item | Afirmação Padronizada da Escala SUS | Tipo | Resposta Média ($R$) | Pontuação Convertida |
| :---: | :--- | :---: | :---: | :---: |
| **1** | Acho que gostaria de utilizar este sistema frequentemente no galpão. | Ímpar (+) | 5 | $5 - 1 = 4$ |
| **2** | Achei o sistema desnecessariamente complexo para a pesagem. | Par (-) | 2 | $5 - 2 = 3$ |
| **3** | Achei o sistema muito fácil de usar na minha rotina de trabalho. | Ímpar (+) | 5 | $5 - 1 = 4$ |
| **4** | Acho que precisaria de suporte de TI da Católica para conseguir operar. | Par (-) | 1 | $5 - 1 = 4$ |
| **5** | Achei que o registro de peso e o romaneio estavam bem integrados. | Ímpar (+) | 4 | $4 - 1 = 3$ |
| **6** | Achei que havia muita inconsistência ou contradição nas telas. | Par (-) | 1 | $5 - 1 = 4$ |
| **7** | Imagino que a maioria dos cooperados aprenderia a usar muito rápido. | Ímpar (+) | 5 | $5 - 1 = 4$ |
| **8** | Achei o sistema muito complicado e pesado de operar com as mãos sujas. | Par (-) | 2 | $5 - 2 = 3$ |
| **9** | Senti-me muito confiante e seguro ao lançar os fardos no sistema. | Ímpar (+) | 4 | $4 - 1 = 3$ |
| **10** | Precisei aprender muitas coisas difíceis antes de conseguir trabalhar. | Par (-) | 2 | $5 - 2 = 3$ |
| **SOMA**| **Soma Total dos Fatores Normalizados** | — | — | **$35$ pontos** |

#### Demonstração Aritmética:
$$\text{Score SUS} = 35 \times 2,5 = 87,5\text{ PONTOS}$$

**Parecer Extensionista:** O índice sobe de inaceitáveis $42,5$ pontos para **$87,5$ pontos**, atingindo o Grau "A" (Excelente) na curva de Bangor/Sauro. Isso assegura autonomia operacional plena aos cooperados sem tutela acadêmica contínua.

---

## 2. PROTOCOLO DE REDESENHO EM 3 INTERVENÇÕES DIRETAS

Para extirpar a intimidação técnica e restaurar a soberania operacional de Seu Valdemar, a interface sofrerá as seguintes refatorações ergonômicas imediatas:

```
+-----------------------------------------------------------------------+
|  TERMINAL DA BALANÇA - COOPERATIVA RECICLA VIDA                      |
|                                                                       |
|  QUEM ESTÁ OPERANDO?                                                  |
|  [ FOTO: SEU VALDEMAR ] -> Digite seu PIN: [ * ] [ * ] [ * ] [ * ]    |
|                                                                       |
|  +--------------------+  +--------------------+  +------------------+ |
|  |     [ 1 ]          |  |     [ 2 ]          |  |     [ 3 ]        | |
|  +--------------------+  +--------------------+  +------------------+ |
|  |     [ 4 ]          |  |     [ 5 ]          |  |     [ 6 ]        | |
|  +--------------------+  +--------------------+  +------------------+ |
|  |     [ 7 ]          |  |     [ 8 ]          |  |     [ 9 ]        | |
|  +--------------------+  +--------------------+  +------------------+ |
|  |   [ LIMPAR ]       |  |     [ 0 ]          |  |   [ ENTRAR ]     | |
|  +--------------------+  +--------------------+  +------------------+ |
|                                                                       |
|  ATALHO RÁPIDO:                                                       |
|  +-----------------------------------------------------------------+  |
|  |      PESAGEM RÁPIDA: [ FARDO DE PAPELÃO (22pt) ]               |  |
|  |                  -> BASTA APERTAR AQUI <-                       |  |
|  +-----------------------------------------------------------------+  |
+-----------------------------------------------------------------------+
```

### Intervenção A: Substituição de Login/Senha Alfanumérica por PIN Numérico Visual de 4 Dígitos
* **Falha Original:** Exigência de digitação de e-mail institucional e senha complexa com caracteres especiais em teclado convencional, incompatível com a rotina de galpão e gerando bloqueio motor e psicológico.
* **Nova Arquitetura:** 
  * Seleção do operador pela foto do perfil e nome grande (24pt).
  * Teclado numérico na tela (formato caixa eletrônico / banco 24h) com teclas largas ($72 \times 72\text{ px}$).
  * Autenticação via código numérico de 4 dígitos (PIN), eliminando qualquer necessidade de alternar caracteres alfanuméricos.

### Intervenção B: Aumento da Tipografia de Botões para 22pt e Contraste Estrito (WCAG)
* **Falha Original:** Rótulos em fontes pequenas (12pt a 14pt) em tons de cinza sobre branco, ilegíveis sob luz natural difusa do galpão e para operadores na faixa da terceira idade.
* **Nova Arquitetura:**
  * Tipografia em escala generosa: rótulos operacionais e comandos com **22pt** em negrito (*Inter* ou *Roboto*).
  * Contraste superior a $7:1$ utilizando botões sólidos em Azul Marinho (`#102C57`) com texto em Branco Puro (`#FFFFFF`), além de botões de alerta positivo em Verde Escuro (`#1B5E20`).
  * Altura mínima de área de toque de $56\text{ px}$, prevenindo cliques falsos causados por dedos calejados ou uso de luvas de proteção mecânica.

### Intervenção C: Criação de Atalho de Pesagem Direta em um Único Clique ("One-Click Weight")
* **Falha Original:** Fluxo labiríntico que exigia navegar por menu lateral, abrir formulário modal, selecionar cooperado, material, tara e data antes de salvar.
* **Nova Arquitetura:**
  * Interface de pesagem em tela única de alta prioridade.
  * Botões de acesso rápido aos materiais mais frequentes (ex.: "FARDO DE PAPELÃO", "PET PRENSADO", "LATINHA").
  * Ao posicionar o fardo na balança, o operador clica no botão do material e o registro é gravado instantaneamente, disparando o aviso de áudio e visual: *"Peso de X kg anotado no caderno da cooperativa com sucesso!"*.

---

## 3. PLANO DE SANEAMENTO ÉTICO E CONFORMIDADE COM A LGPD (LEI 13.709/2018)

Diante do desvio ético constatado (fotografia de cooperados em fila de vulnerabilidade sem consentimento), adota-se o seguinte protocolo de remediação:

### 3.1 Protocolo de Revogação e Expurgo Irreversível de Arquivos
* **Eliminação Imediata de Mídias (Art. 16, LGPD):** Todos os registros fotográficos contendo rostos de cooperados em situação de fila de pesagem/assistência serão permanentemente apagados dos smartphones, cartões de memória, pastas em nuvem (Google Drive/OneDrive) e grupos de mensagens instantâneas (WhatsApp) da equipe.
* **Certidão de Destruição de Dados:** Emissão de uma ata declaratória, assinada por todos os integrantes da bancada acadêmica, atestando que nenhum arquivo visual com potencial estigmatizante ou expositivo foi compartilhado externamente ou permanecerá em arquivos pessoais.

### 3.2 Repactuação do Termo de Consentimento Livre e Esclarecido (TCLE)
* **Assinatura Institucional e Individual (Art. 6º, VI e Art. 8º, LGPD):** Reapresentação formal do TCLE à Presidência da Cooperativa Recicla Vida e aos cooperados participantes das sessões de teste.
* **Linguagem Cidadã e Acessível:** O termo deve ser lido em voz alta pelos estudantes, redigido em português estritamente claro, explicando que as informações coletadas destinam-se exclusivamente à validação acadêmica na plataforma AVA da Universidade Católica de Brasília, sendo vedada qualquer utilização para redes sociais pessoais ou marketing.

### 3.3 Política de Registro Fotográfico Extensionista Ético
* **Foco Estrito nas Mãos e nos Instrumentos de Bancada:** Enquadramentos estritamente focados na interação técnica: dedos apontando para o protótipo de papel, mãos posicionando fardos na balança e telas do terminal.
* **Princípio da Minimização da Imagem (Art. 6º, III, LGPD):** Rostos não serão enquadrados. Caso haja registro de plano aberto em reuniões coletivas deliberativas, aplicar desfoque digital total (*gaussian blur*) sobre as faces antes de qualquer inserção em relatórios acadêmicos.
* **Devolvimento Solidário:** Envio de todos os registros técnicos autorizados à liderança da cooperativa, permitindo que a entidade os utilize em suas próprias prestações de contas institucionais e relatórios socioambientais.

---

## 4. PITCH ESCRITO DE HOMOLOGAÇÃO E DEFESA COMUNITÁRIA

*(Manifestação lida pela equipe perante a Diretoria da Cooperativa Recicla Vida)*

> "Senhores diretores da Cooperativa Recicla Vida e estimado Seu Valdemar: viemos hoje, com humildade, pedir desculpas. A extensão universitária da Universidade Católica de Brasília existe para construir caminhos de autonomia e respeito, mas nossa primeira atitude expressou vaidade acadêmica. Ao impor um sistema labiríntico e registrar fotos sem consentimento, reproduzimos o erro de tratar o conhecimento prático da comunidade como inferior. A indignação do Seu Valdemar não foi uma falha dele, mas sim um diagnóstico incontestável de que nossa interface falhou e desrespeitou a rotina desta cooperativa. Rasgamos nossos layouts de gabinete e voltamos à bancada para ouvir. Descentralizamos a técnica para colocá-la a serviço da autoridade de quem carrega a reciclagem nos braços: trocamos as senhas difíceis por um teclado numérico simples, ampliamos as letras para leitura sem esforço e criamos o botão de pesagem rápida em um clique. Eliminamos todas as imagens constrangedoras e garantimos que nenhuma informação deste galpão seja exposta. Nosso compromisso não é com notas ou diplomas, mas em garantir que este caderno digital sirva com dignidade à soberania e ao sustento do Seu Valdemar e de cada cooperado."

