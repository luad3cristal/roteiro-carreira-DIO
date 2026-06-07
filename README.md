# 🚀 Repositório de Orientação de Carreira & Roadmap Tech Personalizado

Este repositório documenta o processo completo de mentoria de carreira assistida por IA, simulando a interação entre dois agentes especializados: um **Agente Entrevistador de Perfil** e um **Agente Planejador de Roadmaps**. 

O objetivo deste projeto é mapear competências, diagnosticar cenários de transição ou inserção no mercado e consolidar um plano de estudos de 90 dias focado no ecossistema **Fullstack Web com Integração de Inteligência Artificial**.

---

## 🎯 Contexto e Objetivos

O mercado de tecnologia exige cada vez mais especificidade e direcionamento estratégico dos profissionais em início de carreira. Este repositório foi construído para simular uma esteira automatizada de orientação profissional, idealizada para:
* **Mapear Perfis Individuais:** Coletar objetivos de carreira, limitações de tempo e afinidades de código/dados por meio de uma entrevista estruturada.
* **Mitigar Gaps de Aprendizado:** Analisar competências existentes (ex: bagagem acadêmica em Análise e Desenvolvimento de Sistemas e estágio em Mobile/Flutter) para impulsionar a transição para posições Fullstack.
* **Viabilizar Cronogramas Reais:** Estruturar um guia prático adaptado para rotinas restritas (4 horas semanais concentradas nos fins de semana), priorizando a constância sobre o volume.

---

## 📚 Curadoria de Fontes e Engenharia de Prompts

O ecossistema foi projetado utilizando a dinâmica de múltiplos agentes inteligentes atuando em etapas complementares (Triagem de Perfil e Planejamento de Carreira). 

As diretrizes estruturais, personas e regras críticas utilizadas para configurar os agentes deste projeto foram integralmente extraídas e adaptadas do repositório oficial de prompts da comunidade:

* 🔗 **Fonte dos Prompts:** [digitalinnovationone/copilot-prompts](https://github.com/digitalinnovationone/copilot-prompts)

A partir dessa base de engenharia de prompts, o sistema foi capaz de interpretar restrições severas de tempo (menos de 5 horas semanais) e aplicar uma regra de **otimização para o essencial**, removendo excessos teóricos e focando na entrega de um único projeto prático integrador.

---

## 🗺️ Análise Estratégica da Rota de Carreira

A escolha da rota de **Desenvolvedora Fullstack Web** com viés em **IA** apresenta uma sinergia agressiva e inteligente com o seu perfil atual por três motivos principais:

1. **Aproveitamento de Bagagem (Efeito Alavanca):** Você não está começando do zero. O conhecimento de ciclo de vida de componentes, consumo de APIs assíncronas e gerência de estado que você já domina por causa do **Flutter/Mobile** se traduz quase que perfeitamente para o ecossistema do **React**. Você muda a interface (de app para tela web), mas a lógica de engenharia permanece a mesma.
2. **Diferencial Competitivo no Mercado Júnior:** O mercado para desenvolvedores juniores tradicionais está altamente concorrência. No entanto, o profissional que sabe construir o sistema de ponta a ponta (Fullstack) e ainda possui a capacidade técnica de **plugar e consumir APIs de Inteligência Artificial** (tirando os modelos da teoria e transformando-os em produtos reais) destaca-se imediatamente em processos seletivos.
3. **Maximização do Tempo Restrito:** Como sua rotina permite apenas 4 horas de estudo focadas no fim de semana, unificar o aprendizado no ecossistema **JavaScript/TypeScript** (usando React no Frontend e Node.js no Backend) reduz drasticamente a sobrecarga cognitiva. Você domina uma única linguagem para governar toda a aplicação.

---

## 🎓 Miniguia de Estudo: Plano de Ação Consolidado

Abaixo está o plano prático gerado com base no cruzamento do seu diagnóstico com a matriz de decisão dos agentes.

### 📅 Roadmap de 90 Dias: Desenvolvedora Fullstack Web
*Foco: Otimização de tempo (4h semanais nos finais de semana)*

#### MÊS 1 - Fundamentos e Alinhamento Backend
* **Semanas 1-2:** Revisar a arquitetura MVC; consolidação de rotas e controllers com Node.js e Express. Configuração de conexões de banco de dados relacionais via ORM (Prisma/Sequelize).
* **Semanas 3-4:** Implementação de autenticação segura com JWT (*JSON Web Tokens*), criptografia de senhas e validação de dados de entrada contra injeções.

#### MÊS 2 - Integração Frontend e IA
* **Semanas 5-6:** Conexão do ecossistema React ao Backend em Node.js; gerenciamento de estados globais e tratamentos de erro de rede na interface.
* **Semanas 7-8:** Estudo e consumo assíncrono da API da OpenAI no Backend para processamento de rotinas inteligentes.

#### MÊS 3 - Portfólio e Preparação para Processo Seletivo
* **Semanas 9-10:** Finalização de estilização responsiva, deploy prático (Vercel/Render) e documentação detalhada da arquitetura no GitHub.
* **Semanas 11-12:** Simulação de testes técnicos, revisão de conceitos teóricos de engenharia de software e otimização de perfil no LinkedIn/Currículo destacando a bagagem de estágio.

---

### 🚀 Projeto de Portfólio: SmartTask
* **O que é:** Um Gerenciador de Tarefas Inteligente com Insights de IA. O sistema executa o CRUD tradicional de tarefas, mas possui um botão de otimização que aciona modelos de linguagem para sugerir quebras de subtarefas, estimativas de prazos ou níveis de priorização.
* **Entregáveis:** Repositório organizado com commits semânticos, API operando com banco de dados PostgreSQL e interface responsiva com loaders visuais para requisições assíncronas.
* **💡 Dica de Execução:** Devido ao tempo restrito nos fins de semana, isole o teste da API de IA em um arquivo simples de script no início do Mês 2 antes de acoplá-la na arquitetura principal do projeto.

---

### 💬 Roteiro de Entrevistas (Preparação Técnica)

#### Pergunta 1: Como você gerencia o estado da aplicação no React ao integrar com uma API assíncrona?
> **Como Responder:** *"Eu isolo as requisições em services ou hooks customizados. Utilizo o `useEffect` para buscar os dados iniciais e controlo os estados de carregamento (`loading`), sucesso e erro usando o `useState`. Para aplicações maiores, prefiro utilizar ferramentas como Context API ou bibliotecas de server-state como React Query para evitar o prop-drilling e cachear os dados."*

#### Pergunta 2: Como você garante a segurança das rotas no seu ecossistema Backend em Node.js?
> **Como Responder:** *"Eu utilizo uma estratégia baseada em Middlewares. Após o usuário fazer o login, o servidor gera um JWT. Para as rotas protegidas, intercepto a requisição com um middleware que valida o token enviado no cabeçalho (Header Authorization). Se o token for válido e não estiver expirado, a requisição prossegue; caso contrário, retorno um status HTTP 401 Unauthorized."*

#### Pergunta 3: Você já trabalhou com Flutter e agora estuda Fullstack Web. Como sua experiência com mobile te ajuda no desenvolvimento Web?
> **Como Responder:** *"O Flutter me deu uma base sólida sobre ciclo de vida de componentes, consumo de APIs assíncronas e gerenciamento de estado estruturado, conceitos que se aplicam diretamente ao React. Além disso, trabalhar com mobile me trouxe uma preocupação nativa com performance, consumo de dados e responsividade, garantindo que eu crie aplicações web otimizadas para qualquer tela."*

---

### 📖 Glossário de Conceitos Aprendidos

| Conceito | Definição |
| :--- | :--- |
| **Handoff** | O processo de transferência de dados e contexto coletados por um sistema/agente para o próximo estágio operacional. |
| **Ramp-up** | O período de tempo necessário para que um profissional adquira a proficiência necessária para se tornar produtivo em uma nova função ou tecnologia. |
| **JWT (JSON Web Token)** | Um padrão de mercado (RFC 7519) usado para criar tokens de acesso compactos e seguros para autenticação de requisições. |
| **Commit Semântico** | Convenção de escrita para mensagens de versionamento de código (ex: `feat:`, `fix:`, `docs:`) que organiza o histórico de evolução do software. |
| **Server-State** | Estado de dados que persistem no lado do servidor e necessitam de chamadas assíncronas para sincronização no cliente (ex: dados guardados em banco). |

---

### 🎓 Trilha de Estudo Recomendada (Plataforma DIO)
* **Curso:** *Bootcamp Coding The Future Claro - Desenvolvimento Fullstack Node.js & React*
* **Justificativa:** Conecta o aprendizado pontual feito nos fins de semana a uma trilha linear com o ecossistema JavaScript unificado, validando os conceitos cobrados pelo mercado em vagas juniores.

---

🤖 *Este README foi produzido com o auxílio do Gemini (Google), sintetizando a lógica estrutural da entrevista, consumindo as diretrizes de prompts da comunidade e mapeando a rota estratégica de carreira do usuário.*
