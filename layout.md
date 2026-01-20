# Layout Specification - Workshop Ecossistema Google Jurídico 2077

## Linguagem Visual (Extraída do Design System 2077)

### Cores
- **Background (Void Black):** `#020205` - Fundo principal.
- **Surface (Dark Plate):** `#0a0b14` - Cards e seções secundárias.
- **Primary (Neon Cyan):** `#00f3ff` - Destaques, botões, brilhos.
- **Secondary (Electric Blue):** `#0066ff` - Gradientes, acccents profundos.
- **Accent (Cyber Purple):** `#bc13fe` - Detalhes especiais, hovers.
- **Text White:** `#ffffff` - Títulos e textos de alto contraste.
- **Text Gray:** `#8b9bb4` - Texto de corpo.
- **Error:** `#ff5f56` - Indicadores negativos (comparativo).
- **Success:** `#27c93f` - Indicadores positivos.

### Tipografia
- **Display/Headlines:** 'Orbitron', sans-serif.
  - Pesos: 700 (Bold), 900 (Black).
  - Transform: Uppercase.
  - Line-height: 1.1.
- **Body/Content:** 'Rajdhani', sans-serif.
  - Pesos: 400 (Regular), 500 (Medium), 600 (SemiBold).
  - Line-height: 1.6.

### Espaçamentos e Estrutura
- **Container:** Max-width 1280px.
- **Padding Seção:** 8rem (128px) vertical.
- **Gap Padrão:** 2rem (32px) a 4rem (64px).
- **Border Radius:** 
  - Cards: 8px (visual "tech" levemente quadrado).
  - Botões: Clip-path poligonal (não arredondado).

### Efeitos Globais
- **Glow Cyan:** `0 0 10px rgba(0, 243, 255, 0.5)`.
- **Neon Border:** `1px solid rgba(0, 243, 255, 0.2)`.
- **Glassmorphism:** Backgorund `rgba(10, 11, 20, 0.8)` + `backdrop-filter: blur(10px)`.
- **Clip-path:** Cortes angulares em botões e containers (estilo Cyberpunk).

---

## Seção 1: Hero (Definida em index.html)

### Conteúdo
- **Badge:** "Online e ao vivo | 28/02 | 09h30 - 17h"
- **Title:** "Workshop Ecossistema Google Jurídico na Prática"
- **Headline:** "Domine em 1 dia o Ecossistema Google (NotebookLM + Gemini)"
- **Subheadline:** "Análise Processual, Petições Automatizadas, Pareceres, Estudos Jurídicos. Integre o poder de análise de provas do NotebookLM com a capacidade de redação do Gemini. Uma metodologia segura, validada por magistrados e premiada internacionalmente, para multiplicar a eficiência da sua atuação jurídica com ética e precisão."
- **CTA:** "QUERO ADQUIRIR AGORA"

### Layout
- **Alinhamento:** Centralizado.
- **Background:** Grid infinito `hero-bg-grid` + Glow central `hero-glow`.
- **Badge:** Topo do conteúdo, estilo tech-tag.
- **Title:** Grande destaque com `text-gradient`.

### Tipografia
- **Title:** Orbitron, 900, clamp(2.5rem, 5vw, 5rem).
- **Headline:** Rajdhani, 600, 1.5rem, cor White.
- **Subheadline:** Rajdhani, 500, 1.1rem, cor Gray, max-width 700px.

### Animações
- **Background:** Grid move infinitamente (20s linear).
- **Elementos de Texto:** Fade-up escalonado (0s, 0.2s, 0.4s).
- **Scroll Indicator:** Chevron animado (loop infinito).

### Interatividade
- **CTA:** Glitch effect no hover (transform random de 2px).

---

## Seção 2: Problema (Definida em index.html)

### Conteúdo
- **Headline:** "O Fim do trabalho braçal no Direito e inteligência estratégica para todos os atores jurídicos."
- **Texto:** "Não importa se você redige sentenças, petições ou pareceres. O volume processual explodiu, mas o seu tempo continua o mesmo. Nesta imersão, você dominará o Ecossistema Google para delegar à IA a leitura exaustiva e a formatação repetitiva."
- **CTA:** "QUERO ADQUIRIR AGORA"

### Layout
- **Grid:** 2 Colunas (Texto à esquerda, Visual Cyber-Card à direita).
- **Visual:** "Cyber Card" simulando interface de terminal/sistema com erro de sobrecarga.
- **Background:** Surface (`#0a0b14`).
- **Divisor:** Linha neon gradient no topo (`section-problema::before`).

### Animações
- **Terminal:** Linhas de código "digitando" (`animation: typing`).
- **Barra de Progresso:** Preenchimento animado vermelho/verde.
- **Entrada:** AOS `fade-right` (texto) e `fade-left` (visual).

---

## Seção 3: Público Alvo

### Conteúdo
- **Headline:** "Quem deve participar" (Implícito)
- Items:
  1. **Juízes, Desembargadores e Assessores:** Celeridade no gabinete com segurança decisória.
  2. **Promotores e Procuradores:** Análise processual ágil e pareceres mais robustos.
  3. **Advogados:** Mais teses vencedoras em menos tempo.
  4. **Defensores Públicos:** Atendimento mais eficiente à população.
  5. **Servidores da Justiça e Notários:** Eficiência na triagem e análise de dados.
  6. **Estudantes de Direito:** Preparação diferenciada para o mercado.

### Layout
- **Estilo:** Grid de 3 colunas x 2 linhas.
- **Cards:** "Holo-Cards". Cards transparentes com borda fina e brilho no hover.
- **Iconografia:** Ícones abstratos geométricos ou Phosphor Icons futuristas (tamanho 48px, cor Cyan).

### Tipografia Específica
- **Role (Título do Card):** Orbitron, 700, 1.25rem, cor White.
- **Benefício (Texto do Card):** Rajdhani, 400, 1rem, cor Gray.

### Cores Específicas
- **Card Background:** `rgba(255, 255, 255, 0.02)`.
- **Card Border:** `1px solid rgba(139, 155, 180, 0.1)`.
- **Hover Border:** `1px solid #00f3ff`.

### Animações
- **Cards:** `data-aos="fade-up"`, delay escalonado (100ms por card).
- **Hover:** Glow interno acende (`box-shadow: inset 0 0 20px rgba(0, 243, 255, 0.1)`).

---

## Seção 4: Solução (Como a IA Revoluciona)

### Conteúdo
- **Headline:** "Como a IA e o Ecossistema Google Revoluciona a Produção Jurídica"
- **Subheadline:** "A união do NotebookLM com o Gemini cria o 'Gabinete Digital' perfeito..."
- **CTA:** "QUERO ADQUIRIR AGORA"
- **Features:**
  1. **Análise de Prova (NotebookLM):** Audita autos, depoimentos e documentos em segundos.
  2. **Redação Jurídica (Gemini):** Estrutura a minuta baseada na análise.
  3. **Segurança Técnica:** Método validado para blindar contra erros.

### Layout
- **Estrutura:** Feature Row com ícones grandes ou diagramática.
- **Central:** Imagem/Diagrama esquemático conectando "NotebookLM" + "Gemini" = "Resultado". (Se não houver imagem, fazer com CSS shapes - dois círculos orbitando).
- **Features:** Dispostas ao redor ou abaixo do diagrama.

### Tipografia
- **Feature Title:** Orbitron, 600, 1.5rem, Cyan.
- **Feature Text:** Rajdhani, 1.1rem.

### Elementos Visuais
- **Conector:** Linhas pontilhadas brilhantes conectando os cards.

---

## Seção 5: Transformação & Benefícios

### Conteúdo
- **Headline:** "Como o Ecossistema Google Transforma Sua Rotina Jurídica"
- **Items:**
  1. Análise Rápida de Precedentes.
  2. Gestão Inteligente de Contratos.
  3. Construção de Argumentos Precisos.
  4. Organização Avançada de Dados.
- **CTA:** "QUERO ADQUIRIR AGORA"

### Layout
- **Estilo:** Bento Grid (Grid assimétrico).
- **Card 1 (Grande):** "Análise Rápida" - Foco visual.
- **Cards 2, 3, 4 (Menores):** Grid lateral.

### Estilo dos Cards (Bento)
- Background: Gradiente linear muito sutil (`linear-gradient(135deg, rgba(255,255,255,0.03) 0%, rgba(255,255,255,0.01) 100%)`).
- Borda: Esquerda colorida (Cyan para card 1, Blue para card 2, Purple para card 3).
- Padding: 2rem.

---

## Seção 6: Cronograma

### Conteúdo
- **Data:** 28 de fevereiro de 2025 | Online e ao vivo
- Steps:
  - 09h30: Início do Workshop
  - 12h00: Pausa para o almoço
  - 14h30: Retorno das atividades
  - 17h00: Encerramento
- **CTA:** "QUERO ADQUIRIR AGORA"

### Layout
- **Estilo:** Linha do Tempo Vertical (Cyber Timeline).
- **Linha:** Linha central neon (`width: 4px`, `box-shadow: 0 0 10px Cyan`).
- **Nodes:** Círculos brilhantes nos horários.
- **Cards:** Alternados (Esquerda/Direita).

### Interatividade
- **Scroll:** A linha "enche" de luz conforme o scroll desce (usando script simples ou apenas CSS attachment fixed illusion).
- **Hover no Node:** O card expande levemente.

---

## Seção 7: Comparativo (Quem usa vs Quem não usa)

### Conteúdo
- **Headline:** "Quem usa o Ecossistema Google vs Quem Não Usa"
- **Items:**
  - Gestão de Documentos (Dossiês Digitais vs Arquivos Dispersos)
  - Análise de Provas (Interrogatório dos Autos vs Leitura Linear)
  - Redação (Minutas Prontas vs Tela em Branco)
  - Audiências (Análise Multimodal vs Trabalho Manual)
  - Segurança (Grounding vs Risco Ético)
  - Pesquisa (Jurimetria Pessoal vs Pesquisa Lenta)
  - Produtividade (Estratégia vs Enxugar Gelo)
  - Carreira (Autoridade Tech vs Obsoletismo)
- **CTA:** "QUERO ADQUIRIR AGORA"

### Layout
- **Tableless Comparison:** Grid de 3 Colunas.
  - Col 1: "Quem Não Usa" (Estilo: Opaco, Monocromático, Borda Vermelha no hover, Texto cinza escuro).
  - Col 2: Tópicos (Centralizado, Texto Bold White).
  - Col 3: "Quem Usa" (Estilo: Brilhante, Borda Verde/Cyan, Glow).
- **Mobile:** Empilhado (Tópico -> Ruim -> Bom).

### Detalhes
- **Ícones:** "X" vermelho na esquerda, "Check" verde neon na direita.
- **Background Coluna Boa:** `rgba(0, 243, 255, 0.05)`.

---

## Seção 8: O que vai aprender & Instrutores

### Conteúdo (Aprender)
- 7 itens numerados (NotebookLM, Gestão, Auditoria, Redação, Prompt, Curadoria, Casos).

### Conteúdo (Instrutores)
- Felipe Damous (Especialista em IA Jurídica)
- Rodrigo Terças (Programador & Especialista em IA)

### Layout
- **Container Dividido:**
  - Lado Esquerdo: Lista "O que vai aprender" (Checklist tech).
  - Lado Direito: Cards dos Instrutores.
- **Instrutores Cards:** Design hexagonal ou com "corte" no canto da foto.
  - Foto em P&B com filtro duotone Cyan/Blue.
  - Nome em Orbitron.
  - Texto bio pequeno (0.9rem).

---

## Seção 9: Oferta

### Conteúdo
- **Data/Hora/Local:** Destaque.
- **Preço:** "De R$ ??? por R$ 47,00".
- **CTA:** "QUERO ADQUIRIR AGORA".
- **Aviso:** Valor promocional lote 0.

### Layout
- **Mega Card:** O elemento mais chamativo da página.
- **Borda:** "Neon Pulse" animation (borda pulsando luz).
- **Preço:**
  - "De R$ ???": Riscado, opaco.
  - "R$ 47,00": Gigante (4rem), Orbitron, Gradient Text Cyan-Blue.
- **Fundo:** Textura de circuito impresso sutil (opacity 0.1).

### Animações
- **Botão CTA:** Maior que os outros, com efeito de "onda de choque" (ring animation) constante.

---

## Seção 10: Depoimentos, FAQ e Footer

### Depoimentos
- Carrossel horizontal simples. Cards com aspas gigantes em marca d'água.

### FAQ
- Accordion Style.
- Perguntas: Texto branco, fundo escuro.
- Ao abrir: Borda esquerda fica Cyan e conteúdo desliza.

### Footer CTA
- **Headline:** "Vagas Limitadas - Garanta a Sua Agora Mesmo!"
- **CTA:** "GARANTA SUA VAGA AGORA!"
- Background: Gradiente radial forte vindo de baixo (`radial-gradient(circle at bottom, #001f3f, #020205)`).
- Copyright simples no fim.

---

## Micro-interações e Fatores Uau

1.  **Cursor Personalizado (Opcional):** Um anel fino Cyan que segue o mouse com delay (se não prejudicar UX).
2.  **Highlight nos Textos:** Palavras chave na copy devem ter a classe `.text-highlight` (Cyan) ou `.text-gradient`.
3.  **Scroll Animations:** Todos os títulos de seção devem ter `data-aos="fade-right"`. Todos os cards `data-aos="fade-up"`.
4.  **Botões:** Todos com clip-path e efeito hover de preenchimento ou glitch.

---
**Fim da Especificação. Arquivo pronto para implementação via `/desenvolver`.**
