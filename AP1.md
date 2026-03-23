1## 1. Termo de Abertura

O presente projeto tem como objetivo o desenvolvimento de uma plataforma de gestão financeira pessoal integrada ao ecossistema Open Finance, visando automatizar o controle de receitas e despesas e fornecer ao usuário uma visão centralizada e inteligente de suas finanças. O sistema busca resolver a dificuldade enfrentada por usuários que utilizam múltiplas instituições financeiras e dependem de controles manuais, oferecendo integração automática de dados, categorização inteligente e visualização por meio de dashboards personalizados.  

Os principais stakeholders do projeto incluem o usuário final, que utilizará a plataforma para gerenciar suas finanças, as instituições financeiras responsáveis pelo fornecimento dos dados via Open Finance, a equipe de desenvolvimento encarregada da construção do sistema e o parceiro tecnológico responsável pela infraestrutura de integração.  

O escopo do projeto contempla a integração com APIs do Open Finance, importação automática de dados financeiros, categorização de transações, disponibilização de dashboards e implementação de um chatbot para consultas financeiras. Não fazem parte do escopo funcionalidades como execução de transações financeiras (ex: pagamentos e transferências) ou integrações com instituições fora do ecossistema Open Finance.

---

## 2. Descrição do Projeto

O projeto consiste no desenvolvimento de uma aplicação de gestão financeira pessoal que se integrará diretamente às instituições financeiras do usuário por meio do ecossistema Open Finance Brasil. A plataforma tem como objetivo centralizar e automatizar o controle financeiro, eliminando a necessidade de inserções manuais de dados e proporcionando uma visão unificada e inteligente das finanças do usuário.

A aplicação permitirá a categorização automática de receitas e despesas, utilizando algoritmos de Inteligência Artificial (IA) e Processamento de Linguagem Natural (PLN) para interpretar o histórico de transações. Além disso, o usuário contará com um ambiente de dashboards personalizáveis (“playground”), no qual poderá organizar e definir quais informações deseja visualizar em seu painel.

Um dos principais diferenciais do projeto será a implementação de um agente de IA que atuará como um consultor financeiro virtual. Esse agente será capaz de realizar análises preditivas de saldo, sugerir otimizações no orçamento e alertar sobre gastos atípicos ou cobranças indevidas. A interação será projetada de forma natural e conversacional, permitindo ao usuário realizar consultas como: “quanto gastei com transporte no último trimestre?”.

A arquitetura do sistema será projetada para ser escalável e segura, garantindo conformidade com a Lei Geral de Proteção de Dados (LGPD) e seguindo boas práticas de segurança da informação, como criptografia de ponta a ponta e utilização de protocolos seguros como OAuth2 e mTLS para comunicação com APIs do Open Finance.

---

## 3. Requisitos

### Requisitos Funcionais (RF)

- **RF01 – O sistema deve permitir a conexão com APIs do Open Finance para importação automática de dados financeiros.**  
  Origem: Negócio  

- **RF02 – O sistema deve permitir a visualização de dados financeiros por meio de dashboards personalizáveis pelo usuário.**  
  Origem: Negócio  

- **RF03 – O sistema deve permitir a categorização e organização de receitas e despesas.**  
  Origem: Negócio  

- **RF04 – O sistema deve disponibilizar um chatbot para que o usuário possa consultar informações sobre suas finanças de forma conversacional.**  
  Origem: Negócio  

- **RF05 – O sistema deve permitir a criação de subgrupos (famílias) de categorias financeiras.**  
  Origem: Negócio  

- **RF06 – O sistema deve permitir que o usuário tenha controle total sobre suas categorias (criar, editar e remover).**  
  Origem: Negócio  

- **RF07 – O sistema deve permitir o treinamento e a customização do modelo de IA com base no comportamento do usuário.**  
  Origem: Sistema  

---

### Requisitos Não Funcionais (RNF)

- **RNF01 – O sistema deve apresentar tempo de resposta inferior a 2 segundos para operações principais.**  
  Origem: Sistema  

- **RNF02 – O sistema deve suportar no mínimo 100 usuários simultâneos.**  
  Origem: Sistema  

- **RNF03 – O sistema deve garantir a segurança dos dados por meio de mecanismos como criptografia e autenticação segura.**  
  Origem: Sistema  

- **RNF04 – O sistema deve estar em conformidade com a Lei Geral de Proteção de Dados (LGPD).**  
  Origem: Negócio
    
- **RNF05 – O sistema deve garantir a criptografia de ponta a ponta dos dados e utilizar protocolos seguros de comunicação (OAuth2 e mTLS), assegurando a proteção das informações durante todo o processo de transmissão e armazenamento.**
  Origem: Sistema
---

### Requisitos de Domínio (RD)

- **RD01 – O acesso aos dados financeiros do usuário deve ocorrer apenas mediante consentimento explícito via Open Finance.**  

- **RD02 – Toda transação financeira deve estar associada a pelo menos uma categoria.**  

- **RD03 – Categorias financeiras podem ser organizadas em grupos e subgrupos definidos pelo usuário.**  

---

## 4. Fontes de Requisitos e Técnicas de Levantamento

O levantamento de requisitos foi realizado a partir de múltiplas fontes e técnicas, visando garantir uma compreensão abrangente das necessidades do sistema.

- **Brainstorm:** Foi realizada uma sessão de brainstorming entre os integrantes do grupo para identificar funcionalidades relevantes, com base nas necessidades percebidas no gerenciamento financeiro pessoal. As ideias foram organizadas considerando tanto a experiência do usuário quanto as necessidades técnicas do sistema.

- **Análise comparativa de aplicativos:** Foi conduzida uma análise de aplicativos financeiros existentes, como Itaú, Bradesco, Inter, Banco do Brasil e Nubank, com base na experiência prática dos integrantes do grupo. Essa análise permitiu identificar boas práticas, funcionalidades essenciais e limitações das soluções atuais, contribuindo diretamente para a definição dos requisitos do sistema.
