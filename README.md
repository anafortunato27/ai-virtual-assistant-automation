# 🤖 Sofia — Assistente Virtual com IA e Automação

Assistente virtual desenvolvida para automatizar atendimentos de uma clínica fictícia, utilizando Inteligência Artificial, automação de processos, webhooks e integrações entre diferentes serviços.

A assistente se chama **Sofia** e representa a clínica fictícia **Clínica Fortunato**.

O objetivo do projeto é demonstrar, de forma prática, como Inteligência Artificial e automação podem ser utilizadas para criar fluxos de atendimento mais inteligentes, organizados e escaláveis.

---

## 🏥 Sobre a Clínica Fortunato

A **Clínica Fortunato** é uma clínica fictícia criada exclusivamente para fins de demonstração deste projeto.

Ela serve como cenário para simular situações reais de atendimento, permitindo que a assistente virtual **Sofia** interaja com usuários, interprete mensagens e encaminhe solicitações para diferentes fluxos automatizados.

---

## 👩‍💻 Sobre a Sofia

A **Sofia** é uma assistente virtual baseada em Inteligência Artificial.

Ela foi desenvolvida para receber mensagens em linguagem natural, interpretar a intenção do usuário e responder de acordo com o contexto da conversa.

Dependendo da solicitação, a assistente pode direcionar o atendimento para diferentes fluxos automatizados.

Entre as possibilidades de interação estão:

- iniciar um atendimento;
- responder dúvidas;
- apresentar informações sobre a clínica;
- orientar o usuário durante a conversa;
- interpretar diferentes tipos de solicitação;
- encaminhar a solicitação para o fluxo correspondente;
- retornar respostas automaticamente pelo WhatsApp.

---

# 📱 Teste a Sofia

A assistente pode ser testada diretamente pelo WhatsApp.

### Número

**+55 (81) 7628-6617**

Para iniciar a conversa, basta enviar uma mensagem como:

```text
Olá
````

ou:

```text
Oi, Sofia!
```

---

## 💬 Exemplos de mensagens

Algumas mensagens que podem ser utilizadas para testar a assistente:

```text
Olá
```

```text
Quais serviços a clínica oferece?
```

```text
Gostaria de fazer um agendamento.
```

```text
Preciso de informações sobre a clínica.
```

```text
Como posso ser atendido?
```

```text
Oi, Sofia! Pode me ajudar?
```

---

# 🧠 Como funciona

De forma simplificada, o funcionamento da aplicação segue o fluxo:

```text
Usuário
   │
   ▼
WhatsApp
   │
   ▼
Webhook
   │
   ▼
n8n
   │
   ▼
Inteligência Artificial
   │
   ▼
Interpretação da solicitação
   │
   ▼
Seleção do fluxo correspondente
   │
   ▼
APIs / Automações
   │
   ▼
Geração da resposta
   │
   ▼
WhatsApp
   │
   ▼
Usuário
```

A mensagem enviada pelo usuário é recebida pelo sistema e encaminhada para o fluxo de automação.

A Inteligência Artificial é utilizada para compreender a solicitação e auxiliar na tomada de decisão sobre qual ação deve ser executada.

Após o processamento, a resposta é enviada novamente ao usuário por meio do WhatsApp.

---

# ⚙️ Arquitetura da solução

O projeto utiliza uma arquitetura baseada em integração entre diferentes serviços.

```text
┌──────────────────┐
│      Usuário     │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│     WhatsApp     │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│      Webhook     │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│       n8n        │
│  Orquestração    │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│ Inteligência     │
│ Artificial       │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│ Identificação da │
│ intenção         │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│ APIs e fluxos    │
│ automatizados    │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│ Geração da       │
│ resposta         │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│     WhatsApp     │
└──────────────────┘
```

---

# 🛠️ Tecnologias utilizadas

O projeto envolve principalmente as seguintes tecnologias:

* **Inteligência Artificial**
* **n8n**
* **Docker**
* **APIs REST**
* **Webhooks**
* **WhatsApp**
* **JSON**
* **Automação de processos**
* **Integração entre sistemas**
* **Prompt Engineering**

---

# 🔄 n8n

O **n8n** é utilizado como ferramenta principal para a orquestração dos fluxos.

Ele é responsável por conectar as diferentes partes da aplicação, como:

* recebimento das mensagens;
* webhooks;
* processamento dos dados;
* chamadas de APIs;
* integração com Inteligência Artificial;
* lógica de decisão;
* execução de automações;
* envio das respostas.

A utilização do n8n permite organizar diferentes etapas do atendimento em workflows independentes e reutilizáveis.

---

# 🤖 Inteligência Artificial

A Inteligência Artificial é utilizada principalmente para interpretar as mensagens enviadas pelos usuários.

Em vez de depender apenas de comandos fixos, a Sofia consegue receber solicitações escritas de diferentes formas e identificar o contexto da conversa.

Por exemplo, mensagens como:

```text
Quero marcar uma consulta.
```

```text
Gostaria de fazer um agendamento.
```

```text
Tem horário disponível?
```

podem representar intenções semelhantes, mesmo sendo escritas de maneiras diferentes.

A IA permite que o sistema trabalhe com linguagem natural e torne a interação mais próxima de um atendimento convencional.

---

# 🔗 Webhooks e APIs

Os **webhooks** permitem que a aplicação receba eventos e mensagens em tempo real.

Já as **APIs** são utilizadas para realizar a comunicação entre os diferentes serviços integrados ao fluxo.

Esse tipo de arquitetura permite que uma mesma automação seja expandida futuramente para integrar:

* sistemas de agendamento;
* bancos de dados;
* sistemas de atendimento;
* plataformas de mensagens;
* calendários;
* sistemas internos;
* CRMs;
* serviços externos.

---

# 🐳 Docker

O Docker é utilizado para facilitar a execução e o gerenciamento dos serviços envolvidos no projeto.

Entre as principais vantagens estão:

* isolamento do ambiente;
* facilidade de configuração;
* padronização;
* portabilidade;
* simplificação da implantação dos serviços.

---

# 🎯 Objetivos do projeto

Este projeto foi desenvolvido com o objetivo de explorar na prática conceitos relacionados a:

* Inteligência Artificial aplicada a atendimento;
* automação de processos;
* integração entre APIs;
* utilização de webhooks;
* automação com n8n;
* integração com WhatsApp;
* interpretação de linguagem natural;
* criação de fluxos automatizados;
* arquitetura de integração entre sistemas.

---

# 📚 Principais aprendizados

Durante o desenvolvimento do projeto, foram trabalhados conceitos como:

### Automação

Criação de fluxos capazes de executar ações automaticamente a partir de eventos ou mensagens recebidas.

### Integração entre sistemas

Comunicação entre diferentes aplicações utilizando APIs, webhooks e estruturas de dados.

### Inteligência Artificial

Uso de modelos de IA para interpretação de mensagens e geração de respostas.

### Prompt Engineering

Estruturação de instruções para orientar o comportamento da assistente e melhorar a consistência das respostas.

### Tratamento de dados

Manipulação e organização de informações recebidas e enviadas entre diferentes serviços.

### Arquitetura de workflows

Organização de fluxos no n8n para facilitar manutenção, leitura e expansão da aplicação.

---

# 🚀 Possíveis evoluções

Algumas funcionalidades que podem ser adicionadas futuramente incluem:

* integração com Google Calendar;
* agendamento automático de consultas;
* confirmação e cancelamento de horários;
* envio automático de lembretes;
* armazenamento do histórico de atendimentos;
* integração com banco de dados;
* integração com CRM;
* painel administrativo;
* transferência do atendimento para uma pessoa;
* análise das principais solicitações recebidas;
* classificação automática dos atendimentos;
* geração de relatórios.

---

# 🔐 Privacidade e segurança

O repositório possui finalidade de **demonstração e portfólio**.

Por isso, informações sensíveis da aplicação não são disponibilizadas publicamente.

Não são publicados:

* chaves de API;
* tokens de autenticação;
* credenciais;
* senhas;
* URLs privadas;
* configurações internas;
* dados de usuários;
* workflows contendo informações sensíveis.

O número disponibilizado neste README deve ser utilizado apenas para testar a demonstração da assistente.

---

# ⚠️ Observação

A **Clínica Fortunato é fictícia** e foi criada exclusivamente como cenário para demonstração do projeto.

A Sofia não representa uma clínica real e não fornece orientação médica.

O projeto tem finalidade educacional, técnica e de portfólio.

---

# 📂 Sobre este repositório

Este repositório funciona como uma apresentação do projeto.

O código, as credenciais e os workflows completos não são disponibilizados publicamente, pois a solução utiliza integrações e configurações privadas.

O objetivo deste repositório é apresentar:

* o funcionamento da aplicação;
* as tecnologias utilizadas;
* a arquitetura da solução;
* os conceitos aplicados;
* uma demonstração funcional da assistente.

---

# 👩‍💻 Desenvolvido por

**Ana Clara Fortunato de Souza**

Estudante de Engenharia de Computação
Universidade Federal de Goiás — UFG

Interesses:

`Desenvolvimento de Software` • `Inteligência Artificial` • `Automação` • `Sistemas Embarcados`

---

## ⭐ Sobre o projeto

Se você chegou até aqui, experimente conversar com a Sofia pelo WhatsApp:

**+55 (81) 7628-6617**

Envie:

```text
Olá, Sofia!
```

e conheça a demonstração da **Clínica Fortunato**.

```

Eu só faria **uma mudança antes de publicar**: confirme como esse número aparece no WhatsApp. O número que você me passou, `8176286617`, tem **10 dígitos com DDD**, enquanto celulares brasileiros normalmente aparecem com 11 dígitos após o código do país por causa do nono dígito. Então deixei exatamente como `+55 (81) 7628-6617`, mas vale conferir se não seria algo como `+55 (81) 9XXXX-XXXX`.

Também recomendo colocar no topo do README uma **captura bonita de uma conversa com a Sofia**. Isso faria o repositório ficar muito mais chamativo no LinkedIn.
```
