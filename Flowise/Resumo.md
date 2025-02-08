# Flowise - Plataforma No-Code/Low-Code

O **Flowise** é uma plataforma no-code/low-code projetada para automatizar fluxos de trabalho, permitindo a integração fácil de APIs e ferramentas de Inteligência Artificial. Serve pra criar processos automatizados sem precisar escrever código complexo, agiliza tarefas.

---

## Memórias: Buffer e Cache

### Buffer Memory
A **Buffer Memory** é uma memória temporária que salva o histórico das mensagens trocadas entre a IA e o usuário. Isso ajuda a IA a "lembrar" do contexto da conversa e oferecer respostas mais contextuais.

### Cache
O **Cache** também é uma memória temporária, mas em vez de guardar o histórico das mensagens, ele armazena dados que a IA pode precisar acessar rapidamente mais tarde, como resultados de cálculos ou informações requisitadas com frequência.

---

## Ferramentas (Tools)

O Flowise oferece uma série de **ferramentas** para otimizar e personalizar a plataforma, adaptando-a às suas necessidades.

### Ferramentas Personalizadas
Uma das funcionalidades mais interessantes do Flowise é a criação de **ferramentas personalizadas**. Você pode adicionar novas ferramentas escrevendo um nome e uma descrição, que será usada como um **prompt** para a IA. Isso ajuda a IA a identificar quando e como utilizar a ferramenta, baseada no que o usuário disser ou nas interações que ocorrerem.

- **Exemplo**: Você pode criar uma ferramenta de "calculo de imposto" e configurar a IA para usá-la sempre que o usuário falar sobre questões fiscais.
  
Além disso, é possível integrar essas ferramentas com **endpoints** ou inserir um código JavaScript para fazer a plataforma se comportar de acordo com suas necessidades específicas.

---

## Assistente e Agente

### Assistente
O **Assistente** no Flowise é mais voltado para interações simples, como chatbots, em que o foco é uma conversa direta e rápida com o usuário.

### Agente
Já o **Agente** é mais completo e robusto. Ele é composto por dois elementos principais:
- **Supervisor**: O supervisor gerencia os **Workers** (trabalhadores), controlando e distribuindo as tarefas.
- **Workers**: Os workers executam essas tarefas.

Você conecta o chatModel apenas ao **Supervisor**, que gerencia os workers que executam as tarefas específicas, e eles 
utilizam o mesmo modelo.

---

## Configurações e Personalização

### Temperatura no ChatModel
A **Temperatura** do ChatModel é um ajuste que define a criatividade e a imprevisibilidade das respostas da IA. 

| Temperatura      | Características                                      |
|------------------|------------------------------------------------------|
| **Alta**         | Respostas mais criativas, variadas e menos previsíveis. |
| **Baixa**        | Respostas mais diretas, precisas e robóticas.        |

### Embed em Outros Sites
O Flowise permite que você **embed** a plataforma em outros sites, o que significa que você pode integrar suas funcionalidades de IA em diversas plataformas externas como se fosse uma API.
