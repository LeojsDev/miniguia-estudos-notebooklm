# Caderno de Estudos: Conceitos Básicos de Computação em Nuvem com NotebookLM

## 🎯 Contexto e Objetivos
Este repositório foi criado para o Desafio de Projeto da DIO com o objetivo de construir e organizar um caderno temático focado nos **Conceitos Básicos de Computação em Nuvem (Cloud Computing)**. 

### Objetivos de Aprendizado:
- Compreender a evolução histórica da TI (Mainframe -> Cliente/Servidor -> Cloud).
- Diferenciar com clareza os modelos de serviço: IaaS (Infraestrutura), PaaS (Plataforma) e SaaS (Software).
- Compreender os modelos de implantação de nuvem (Pública, Privada, Híbrida e Comunitária).
- Entender conceitos fundamentais como Virtualização, Elasticidade e a mudança financeira de CAPEX (Investimento em Capital) para OPEX (Despesas Operacionais).

---

## 📚 Curadoria de Fontes
Para alimentar o NotebookLM e gerar os resumos e análises, selecionei e fiz o upload das seguintes referências:

1. **Livro:** *Cloud Computing - Nova Arquitetura da TI*  
   - **Autor:** Manoel Veras (Editora Brasport, 2012)  
   - **Foco:** Definições formais do NIST, conceitos de Datacenter, Virtualização e arquitetura de infraestrutura.
2. **Livro:** *Amazon AWS - Descomplicando a computação na nuvem*  
   - **Autor:** Jonathan Lamim Antunes (Editora Casa do Código)  
   - **Foco:** Aplicação prática dos conceitos de IaaS (EC2), armazenamento (S3) e banco de dados (RDS) no ecossistema AWS.
3. **Livro:** *Cloud Computing - Computação em Nuvem: Transformando o mundo da TI*  
   - **Autor:** Cezar Taurion (Editora Brasport, 2009)  
   - **Foco:** Visão estratégica de negócios, transição para o modelo SaaS, elasticidade e a mudança no financiamento da TI (CAPEX vs OPEX).

---

## 🧠 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Nesta etapa, explorei a criação de perguntas estratégicas para extrair o melhor conhecimento dos livros selecionados. 

### Prompts Utilizados:
1. **Contexto Histórico:** *"Com base nos livros do Manoel Veras e Cezar Taurion, explique a evolução pendular da arquitetura de TI (Mainframes para Cliente/Servidor e depois de volta para Cloud Computing). Quais eram os gargalos da arquitetura antiga que a nuvem resolve?"*
2. **Modelo Financeiro:** *"Usando o livro do Cezar Taurion como referência, explique detalhadamente a diferença econômica entre CAPEX e OPEX no contexto de adoção de computação em nuvem. Como a elasticidade ajuda a evitar o superdimensionamento?"*
3. **Modelos de Serviço e Responsabilidade:** *"Crie uma tabela comparativa detalhada explicando IaaS, PaaS e SaaS. Para cada modelo, mostre de quem é a responsabilidade pela segurança/gerenciamento (cliente ou provedor) e dê um exemplo prático baseado no livro da AWS (ex: EC2, S3, RDS)."*

### ⚡ Cicatrizes e Aprendizados (Troubleshooting):
* **Contexto de Época:** Como os livros do Taurion (2009) e Veras (2012) são do início da consolidação da nuvem, a IA inicialmente trouxe alguns dados datados sobre provedores. **Ajuste:** Precisei refinar as perguntas especificando para focar nos *conceitos estruturais* (que continuam 100% válidos hoje) e usar o livro do Jonathan Lamim para complementar com a visão prática moderna da AWS.
* **Precisão de Referência:** O NotebookLM se mostrou extremamente preciso ao linkar as fontes diretamente aos capítulos dos livros digitais, evitando alucinações comuns em outros LLMs.

---

## 📖 Miniguia de Estudos: Conceitos Básicos de Cloud (Entrega Final)

### 1. Resumos Estruturados dos Conceitos Chave

#### A Evolução Pendular da TI
* **Mainframes (Centralização):** O poder estava focado em computadores gigantescos e muito caros. O foco era máxima eficiência de uso do hardware; a flexibilidade para o usuário era quase nula.
* **Cliente/Servidor (Descentralização):** Com a chegada dos PCs e redes locais, o processamento foi distribuído. Trouxe flexibilidade, mas gerou subutilização de hardware e alta complexidade de gerenciamento.
* **Cloud Computing (Centralização + Flexibilidade):** A nuvem junta o melhor dos dois mundos. Centraliza o processamento físico em gigantescos Datacenters (gerando economia de escala), mas mantém a flexibilidade de acesso e elasticidade total pela internet.

#### CAPEX vs. OPEX e Elasticidade
* **CAPEX (Capital Expenditure):** Gastos com bens físicos (comprar servidores, construir datacenters). Exige alto investimento inicial e gera desperdício quando o servidor fica ocioso.
* **OPEX (Operational Expenditure):** Despesas operacionais. Na nuvem, você paga apenas pelo uso do serviço (pague-pelo-uso), eliminando o custo de entrada.
* **Elasticidade:** A capacidade de crescer ou diminuir recursos em tempo real de acordo com a demanda real (evitando gastos desnecessários com servidores ligados sem uso nos finais de semana, por exemplo).

---

### 2. Glossário de Termos

* **IaaS (Infrastructure as a Service):** O provedor entrega o hardware virtualizado (servidores, redes, armazenamento). Exemplo: *AWS EC2*. O cliente gerencia o Sistema Operacional e as aplicações.
* **PaaS (Platform as a Service):** O provedor entrega o sistema operacional e as ferramentas de desenvolvimento prontos. O cliente foca apenas em escrever o código. Exemplo: *AWS Elastic Beanstalk* ou *Heroku*.
* **SaaS (Software as a Service):** O software é entregue pronto para uso via browser ou app, 100% gerenciado pelo provedor. Exemplo: *Google Docs* ou *Netflix*.
* **Virtualização:** Tecnologia base que permite dividir um servidor físico em várias Máquinas Virtuais (VMs) independentes através de um *Hypervisor*.
* **Nuvem Híbrida:** Modelo que combina infraestrutura local (on-premises ou nuvem privada) com serviços de nuvem pública, permitindo o tráfego de dados entre elas.

---

### 3. Prompts Reutilizáveis para Revisões Futuras

* *"Explique o modelo de Responsabilidade Compartilhada de Segurança na nuvem para IaaS e PaaS usando uma analogia simples do dia a dia."*
* *"Quais são as 5 características essenciais da Computação em Nuvem segundo a definição do NIST e dê um exemplo prático de cada uma?"*
* *"Como a virtualização difere da computação em nuvem? Explique a relação de dependência entre as duas."*
