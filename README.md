# Trabalho Prático - Programação e Desenvolvimento Web
## **Caça ao Tesouro Cultural**

- **Tema Social:** Patrimônio cultural e educação.
- **Narrativa:** O jogador explora um ambiente virtual em busca de artefatos culturais. Cada artefato revela a história e o significado cultural por trás dele, ensinando ao jogador sobre tradições e patrimônios locais ou globais.
- **Conexão com Games for Change:** Preservação do patrimônio cultural e educação sobre tradições e valores culturais ao redor do mundo.

----------------------------
## Requisitos do projeto

Para o desenvolvimento do jogo, há alguns **componentes obrigatórios** que devem ser implementados com qualidade e organização. Esses elementos são cruciais para criar uma experiência de jogo envolvente e permitir que os jogadores interajam de forma contínua e competitiva. A seguir, apresentamos instruções detalhadas para cada componente:

---

### **1. Ranking (Classificação Global)**

O **ranking** serve para organizar os jogadores com base em sua performance, criando um sistema de comparação entre eles. É fundamental para jogos que envolvem pontuações ou tempo, criando competição e motivação.

### **Instruções para Implementação**:

- **Armazenamento**: Use uma base de dados (por exemplo, Firebase ou MongoDB) para armazenar os dados de cada jogador, como nome de usuário, pontuação, e data do registro.
- **Exibição**: Apresente o ranking em uma página ou área específica do jogo, ordenada pela pontuação dos jogadores, em ordem decrescente.
- **Atualização em Tempo Real**: Sempre que um jogador atinge uma nova pontuação, o ranking deve ser atualizado. Utilize tecnologias como **WebSockets** ou **API REST** para garantir que as mudanças sejam refletidas em tempo real.
- **Componentização**: Crie um componente React exclusivo para o ranking, que possa ser reutilizado em diferentes partes do jogo.
- **Paginação**: Se houver muitos jogadores, implemente a paginação ou um limite de visualização (como mostrar os "Top 10 jogadores") para melhorar o desempenho.

---

### **2. Scoreboard (Quadro de Pontuação)**

O **scoreboard** é uma funcionalidade mais local e dinâmica que mostra a pontuação dos jogadores durante o jogo. Ele é vital para manter os jogadores informados sobre seu desempenho em tempo real.

### **Instruções para Implementação**:

- **Posicionamento na Interface**: Coloque o scoreboard em um local visível da interface do jogo, como no canto superior direito ou em um HUD (Heads-Up Display).
- **Atualização em Tempo Real**: Sempre que o jogador ganhar ou perder pontos, a pontuação deve ser atualizada imediatamente. Utilize o estado do React para gerenciar as mudanças na pontuação.
- **Layout**: Mantenha um layout limpo e direto, mostrando claramente a pontuação atual do jogador, além de outros detalhes como tempo restante ou vidas, dependendo da mecânica do jogo.
- **Design Responsivo**: Certifique-se de que o scoreboard funcione bem em diferentes resoluções de tela, seja no desktop ou em dispositivos móveis.
- **Reset**: Quando o jogador reiniciar o jogo, o scoreboard deve ser reiniciado corretamente. Isso pode ser feito manipulando o estado do componente React.

---

### **3. UI Information (Informações da Interface do Usuário)**

A **interface de usuário (UI)** deve fornecer informações essenciais sobre o progresso do jogador, instruções, status e feedback do jogo, garantindo uma experiência clara e agradável.

### **Instruções para Implementação**:

- **Instruções do Jogo**: A UI deve conter instruções claras de como jogar, seja na forma de tutoriais, dicas ou uma seção de ajuda. Isso pode ser implementado em um modal ou tela inicial.
- **Feedback Visual**: Use elementos visuais para mostrar o progresso do jogador, como barras de vida, medidores de energia, ou níveis de dificuldade. Estes componentes podem ser representados visualmente (ex.: barras de progresso) e devem ser atualizados conforme o jogador avança no jogo.
- **Feedback de Ações**: Mostre mensagens de feedback imediato após ações importantes, como ganho ou perda de pontos, conclusão de fases ou erros cometidos. Use transições visuais para dar clareza, como flashes ou efeitos de fade.
- **Consistência**: A interface deve ser intuitiva e manter uma consistência de design em todas as telas, com tipografia, cores e botões padronizados.
- **Acessibilidade**: Garanta que todos os elementos importantes da UI sejam acessíveis, incluindo cores que contrastem bem e informações textuais claras. Considere também a navegação com teclado.

### **Publicação do Jogo num Servidor Gratuito**

Os alunos devem publicar o jogo online utilizando um servidor gratuito. Aqui estão algumas opções:

### **1. GitHub Pages**

- **Descrição**: Serviço gratuito que permite hospedar sites diretamente a partir de um repositório GitHub.
- **Como usar**: Após criar o repositório, basta ativar o GitHub Pages nas configurações e apontar para a branch correta (geralmente `main` ou `gh-pages`).
- **Link**: [GitHub Pages](https://pages.github.com/)

### **2. Netlify**

- **Descrição**: Plataforma gratuita para publicar projetos web. Suporta fácil integração com repositórios GitHub.
- **Como usar**: Faça login no Netlify, conecte o repositório GitHub, e Netlify fará a publicação automática quando houver alterações.
- **Link**: [Netlify](https://www.netlify.com/)

### **3. Vercel**

- **Descrição**: Outra opção popular para hospedar aplicações React. Simples de configurar e suporta atualizações automáticas via GitHub.
- **Como usar**: Conecte o repositório GitHub, escolha o projeto e Vercel cuidará do resto.
- **Link**: [Vercel](https://vercel.com/)
----------------------------
Ideia: 
