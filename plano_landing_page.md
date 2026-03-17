# Plano de Implementação: Nova Landing Page Start Cripto

## 1. Visão Geral (Epic)
Criar uma nova Landing Page para o produto "Start Cripto" utilizando a estrutura narrativa de conversão validada do documento "arremate - combo.pdf", aplicando os textos atuais do arquivo `startcripto (1).html` e o pacote de identidade visual/branding extraído do JSON fornecido.

## 2. Especificações de Design e Branding (Baseado no JSON)
O design deve transmitir uma imagem "professional", de energia "medium", focada em "investors and financial professionals".

*   **Tema Geral:** Dark Mode (Fundo escuro, estilo sofisticado).
*   **Color Scheme:**
    *   Primary: `#031922` (Azul/Preto extremamente profundo)
    *   Accent: `#00080C`
    *   Background: `#000A0F`
    *   Text Primary: `#000A0F` (Nota: Como o tema é dark, garantir legibilidade usando branco/gelo para textos em fundos escuros. A cor `#000A0F` deve ser usada onde o contraste exigir texto escuro).
*   **Tipografia:**
    *   Títulos (Headings): `Be Vietnam Pro`
    *   Corpo de texto (Body): `Be Vietnam Pro`
    *   Tamanhos Base: H1 = 16px (Ajustar com clamp responsivo se necessário), H2 = 24px, Body = 24px.
*   **Styling Base (Spacing & Componentes):**
    *   Border Radius Global: `0px` (Elementos e pontas 100% "quadrados" para um look premium e agressivo).
*   **Botoes (CTA):**
    *   **Primário:** Fundo `#00080C`, Texto `#333333` (Nota da PM: avaliar acessibilidade de contraste e trocar texto para branco/claro caso o fundo seja muito escuro na prática), Border Radius `0px`, Sem Sombra (shadow: "none"). Sugestão de Copy: "GARANTIR MINHA VAGA AGORA".
    *   **Secundário:** Fundo `#FFFFFF`, Texto `#333333`, Border Radius `0px`, Sem sombra. Sugestão de Copy: "QUERO PROTEGER MEU PATRIMÔNIO".

## 3. Estrutura da Página (Mapeamento Arremate PDF -> Copy Start Cripto)

A nova página deve seguir RIGOROSAMENTE as seguintes seções (na mesma ordem visual do template "Arremate"):

### 3.1. Hero Section (Dobra Principal)
*   **Barra/Aviso Topo:** Tarja de oferta por tempo limitado (fundo accent ou destaque).
*   **Título e Subtítulo:** Puxado do HTML atual ("Comece no mercado de criptomoedas em 30 minutos...").
*   **Mockup Visual:** Computador e/ou Celular renderizando a plataforma do Start Cripto (utilizar os mocks ou placeholders do HTML de cripto). Efeitos de iluminação de fundo (ex: gradiente radial escuro).
*   **CTA Primário:** Botão quadrado sem sombra usando o estilo Primário.

### 3.2. Prova Social (Depoimentos)
*   **Header:** "Veja o que nossos alunos estão falando..."
*   **Visual:** Prints no estilo de conversas de WhatsApp simulando ganhos ou mensagens reais de quem já investe em cripto através do método.

### 3.3. Público-Alvo / Para quem é ("Target Audience")
*   **Estrutura do Arremate:** Cards escuros (agora baseados nas cores `#031922`) acompanhados de ícones SVGs limpos e diretos (sem emojis). Border Radius `0px`. Sem sombras excessivas.
*   **Copy (de Start Cripto):** "Para quem quer começar do zero em cripto", "Para quem quer proteger patrimonio", etc.

### 3.4. O que você recebe / Entregáveis (Trilha Prática)
*   Visualizar as seções ("O que você vai aprender") em blocos com mockups/ícones.
*   Uso da tipografia "Be Vietnam Pro" evidenciando o valor dos módulos.

### 3.5. Bônus Especial
*   Blocos quadrados minimalistas descrevendo e-books, planilhas de cripto, lives, etc (extraído do HTML atual de Start Cripto).

### 3.6. Resumo e Oferta (Ancoragem de Preço)
*   **Conteúdo:** Tudo que o usuário leva + Preço Original riscado -> Preço Black/Novo.
*   **Action:** Botão CTA principal gigante. Cores `#000A0F` ou o contraste escolhido para o Botão Primário do design system.

### 3.7. Autoridade (O Especialista)
*   **Foto do Especialista:** Fundo removido/escuro integrando à página (mesmo conceito de Bruna Antiqueira).
*   **Bio/Texto:** Especialista de Cripto e Investimentos do Start Cripto.

### 3.8. Garantia + FAQ Retrátil + Suporte via WhatsApp
*   Selo de garantia com design sério e quadrado alinhado com o nicho de mercado financeiro.
*   Sanfona/Accordion com as perguntas frequentes.
*   Box direito no FAQ ancorando o suporte pelo WhatsApp (conforme template original de leilões).

## 4. Acceptance Criteria (Critérios de Aceite para o Dev)

*   [ ] O arquivo gerado deve ser HTML/CSS/JS contido num único arquivo ou modularizado conforme padrões do projeto, construído DO ZERO baseando-se no novo Design System.
*   [ ] As fontes do Google (`Be Vietnam Pro`) devem estar importadas e aplicadas globalmente em headings e body.
*   [ ] Elementos arredondados do HTML anterior devem ser substituidos por quinas retas (`border-radius: 0px`).
*   [ ] Esquema de cores e iluminações baseados estritamente na paleta (Primary: `#031922`, Accent: `#00080C`, Background: `#000A0F`). O Dev deve assegurar o bom contraste dos textos.
*   [ ] Emojis devem ser abandonados, priorizar ícones em SVG limpos.
*   [ ] Mobile First: Acessibilidade perfeita em dispositivos móveis, como a landing page do "Arremate".

## 5. Próximo Passo
Delegar esta especificação ao agente dev focado em frontend (`@dev`) ou (`@qa` caso já exista um template) para a codificação da LP, utilizando este documento de guia.
