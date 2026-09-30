# CONFORMIDADE_ETICA.md

## Identificação do Projeto de Extensão

* **Título do Projeto:** Solução Digital para Organização e Gestão de Estoque de Pequenos Empreendedores
* **Unidade Curricular:** Extensão: Humanismo Solidário, Redes e Comunidades
* **Docente Responsável:** Prof. Marco Machado
* **Curso / Unidade Acadêmica:** Engenharia de Software / Tecnologia da Informação – UCB
* **Público-Alvo / Beneficiários:** Pequenos empreendedores e trabalhadores autônomos

---

## ETAPA 1: Diagnóstico e LGPD

### 1. Mapeamento de Dados da Aplicação de Estoque

A conformidade com a Lei 13.709/2018 (LGPD) exige classificar previamente todos os fluxos de entrada da solução web:

* **Dados Pessoais Comuns:**
1. Nome do Empreendedor: Identificação cadastral do titular da conta e personalização do ambiente de trabalho.


2. E-mail: Credencial primária de autenticação no sistema, recuperação de acesso e notificações transacionais.


3. Telefone / WhatsApp de Contato: Canal operacional direto para suporte, comunicação rápida e alinhamento das etapas de testes da extensão.




* **Dados Pessoais Sensíveis:**
1. Dado Biométrico (Reconhecimento Facial ou Impressão Digital): Avaliado inicialmente para logins sem senha, mas categorizado como sensível de alto risco para o escopo do projeto.


2. Origem Racial/Étnica ou Filiação Sindical: Dados por vezes solicitados em censos de microcrédito ou fomento socioeconômico de pequenos negócios.





### 2. Ficha de Minimização de Dados

 "O dado mais seguro no seu banco de dados é aquele que você não precisou coletar."   
 
 * CPF do Empreendedor [Dado Comum] → ELIMINADO   
   * Motivação: A solução foca estritamente no controle operacional de produtos e quantitativos físicos. A autenticação por ID/e-mail mitiga riscos de exposição de documentos civis e vazamentos.   
 
 * Localização GPS em Tempo Real [Dado Comum] → ELIMINADO   
   * Motivação: Pequenos comerciantes e trabalhadores autónomos operam em pontos fixos ou itinerantes sem necessidade de rastreio contínuo via browser, evitando práticas invasivas de vigilância.   
 
 * Biometria Facial / Digital [Dado Sensível] → ELIMINADO   
   * Motivação: Desproporcional ao propósito da aplicação. A autenticação padrão por credenciais cifradas com hash robusto atende plenamente aos requisitos de segurança sem expor biometria.   
 
 * Faturamento Pessoal / Renda Familiar [Dado Financeiro] → ELIMINADO   
   * Motivação: O sistema é uma ferramenta simplificada de stock e não um software fiscal ou contábil, prescindindo de dados de rendimento.  
 
 

### 3. Matriz RBAC (Role-Based Access Control)

* Empreendedor Titular (Dono do Negócio)
  * Permissões: Acesso integral (CRUD) a produtos, categorias, quantidades em stock, alertas e configuração da própria conta.   
  * Segurança: Isolamento restrito por partição lógica (multi-tenant); o titular nunca tem acesso a dados de outros empreendedores da plataforma.

* Colaborador / Operador de Estoque
  * Permissões: Consulta rápida de catálogo e registo operacional de entradas e saídas de quantidades.   
  * Segurança: Princípio do menor privilégio (Least Privilege). Bloqueio total a relatórios estratégicos, remoção de histórico de transações e alteração de credenciais do negócio.   

* Equipe Técnica / Administrador Extension

---

## ETAPA 2: TCLE & Imagem

### 1. Termo de Consentimento Livre e Esclarecido (TCLE)

```text
TERMO DE ESCLARECIMENTO E PARTICIPAÇÃO COMUNITÁRIA (TCLE)

Você está sendo convidado(a) a participar do projeto de extensão universitária 
"Solução Digital para Organização e Gestão de Estoque de Pequenos Empreendedores", 
desenvolvido por estudantes do curso de Engenharia de Software da Universidade 
Católica de Brasília (UCB), sob coordenação do Prof. Marco Machado.

Por favor, leia atentamente as informações a seguir:

1. Qual é o objetivo do projeto?
   Criar e testar uma ferramenta simples pela internet para ajudar você a 
   organizar, cadastrar e acompanhar a quantidade de mercadorias no seu estoque, 
   facilitando a rotina do seu negócio.

2. A minha participação é obrigatória?
   Não. Sua participação é totalmente voluntária. Você tem a liberdade de 
   recusar ou desistir a qualquer momento, sem que isso traga qualquer custo, 
   prejuízo ou complicação para você ou para o seu comércio.

3. O que será feito com as minhas informações?
   As informações sobre produtos e quantidades cadastradas servirão exclusivamente 
   para testar o funcionamento do sistema e propor melhorias técnicas. Nenhum dado 
   pessoal ou comercial será vendido, compartilhado publicamente ou utilizado para 
   cobranças financeiras, respeitando rigorosamente a Lei Geral de Proteção de Dados (LGPD).

4. Como funciona o uso de fotografias ou imagens?
   As fotos tiradas durante as visitas e oficinas servirão unicamente para comprovação 
   pedagógica perante a universidade. Nenhuma imagem frontal revelará seu rosto ou 
   marcas do seu estabelecimento; todas as imagens serão registradas de costas ou com 
   os rostos integralmente desfocados, focando sempre a tela do celular ou computador.

Local: Brasília - DF, _____ de _________________ de 2026.

___________________________________________________________
Nome legível do(a) Participante

___________________________________________________________
Assinatura do(a) Participante

___________________________________________________________
Assinatura do Acadêmico Extensionista Responsável (UCB)

```

---

### 2. Protocolo de Captação e Preservação de Imagem em Campo

Para resguardar a integridade, privacidade e reputação comercial dos empreendedores locais:

* **Enquadramento Dorsal e Plano Detalhe:** Toda fotografia deve ser capturada pelas costas do usuário ou focada em plano fechado nas mãos operando as interfaces do sistema (telas de cadastro, listas de estoque no celular ou computador).


* **Filtros de Anonimização Obrigatórios:** Aplicação irrestrita de desfoque gaussiano (*gaussian blur*) ou mosaico digital sobre 100% de rostos capturados incidentalmente nos relatórios de evidências.


* **Higienização Visual de Ambientes:** Ocultação e desfoque imediato de documentos fiscais, faturas físicas, fachadas comerciais, endereços residenciais de trabalhadores autônomos ou nomes em uniformes e aventais.


* **Foco no Artefato de Software:** As fotografias para os relatórios das Fases 3, 5 e 6 da extensão focarão no software (telas do protótipo e fluxos de navegação) e nos estudantes da UCB conduzindo os testes, evitando exposições desnecessárias.



---

### 3. Diretrizes de Infraestrutura e Higiene Cibernética

* **Eliminação de Repositórios Públicos Não Protegidos:** Fica estritamente vedado o uso de planilhas abertas ou diretórios públicos em nuvem (ex.: links sem senha no Google Drive) para guardar credenciais ou informações dos comerciantes atendidos.


* **Proteção de Senhas e Conexões:** As senhas dos empreendedores e colaboradores serão armazenadas em banco relacional com funções criptográficas irreversíveis (`bcrypt` com adição de *salt*) e transporte via HTTPS/TLS criptografado.


* **Trabalho Ético e Horizontalidade:** Superação de posturas salvacionistas ("saviocracia"), substituindo termos técnicos herméticos (`deploy`, `API`, `backend`) por instruções claras no Manual de Uso Simplificado e escuta atenta das necessidades dos usuários.


* **Formalização Documental Prévia:** Toda aproximação e execução prática de campo nas etapas de diagnóstico e validação será respaldada pela Carta de Apresentação emitida pela UCB e pela Carta de Aceite assinada pelo parceiro/empreendedor participante.
