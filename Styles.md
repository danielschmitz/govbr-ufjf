# Styles

<!-- vscode-markdown-toc -->
	* 1. [Documentação de Classes CSS (core.css)](#DocumentaodeClassesCSScore.css)
	* 2. [**Cores e Temas**](#CoreseTemas)
	* 3. [**Layout e Display**](#LayouteDisplay)
	* 4. [**Espaçamento (Margin e Padding)**](#EspaamentoMarginePadding)
	* 5. [**Tipografia**](#Tipografia)
	* 6. [**Bordas, Sombras e Opacidade**](#BordasSombraseOpacidade)
	* 7. [**Animações e Transições**](#AnimaeseTransies)
	* 8. [**Ícones (Font Awesome)**](#conesFontAwesome)
	* 9. [**Classes de Componentes e Elementos HTML**](#ClassesdeComponenteseElementosHTML)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->



###  1. <a name='DocumentaodeClassesCSScore.css'></a>Documentação de Classes CSS (core.css)

Este documento descreve as principais classes CSS de utilidade e de componentes presentes no arquivo `core.css`, que faz parte do sistema de design GOVBR-DS.

---

###  2. <a name='CoreseTemas'></a>**Cores e Temas**

As cores são definidas usando variáveis CSS (`--{cor}-{tonalidade}`). As classes de utilidade para cores seguem o padrão `bg-{cor}-{tonalidade}`, `text-{cor}-{tonalidade}`, e `border-{cor}-{tonalidade}`.

* **Tonalidades de Azul (`blue`)**: Variam de `blue-90` (mais escuro) a `blue-5` (mais claro). Inclui variações como `blue-cool` e `blue-warm`, e tonalidades vívidas como `blue-vivid`, `blue-cool-vivid`, `blue-warm-vivid`.
    * Exemplo: `.bg-blue-50`, `.text-blue-vivid-60`, `.border-blue-cool-10`.
* **Tonalidades de Ciano (`cyan`)**: Variam de `cyan-90` a `cyan-5`, com uma variação vívida (`cyan-vivid`).
* **Tonalidades de Dourado (`gold`)**: Variam de `gold-90` a `gold-5`, com uma variação vívida (`gold-vivid`).
* **Tonalidades de Cinza (`gray`)**: Variam de `gray-90` a `gray-1`, com variações `gray-cool` e `gray-warm`.
* **Tonalidades de Verde (`green`)**: Variam de `green-90` a `green-5`, com variações `green-cool`, `green-warm`, e tonalidades vívidas.
* **Tonalidades de Índigo (`indigo`)**: Variam de `indigo-90` a `indigo-5`, com variações `indigo-cool`, `indigo-warm`, e tonalidades vívidas.
* **Tonalidades de Magenta (`magenta`)**: Variam de `magenta-90` a `magenta-5`, com uma variação vívida (`magenta-vivid`).
* **Tonalidades de Menta (`mint`)**: Variam de `mint-90` a `mint-5`, com variações `mint-cool` e tonalidades vívidas.
* **Tonalidades de Laranja (`orange`)**: Variam de `orange-90` a `orange-5`, com variações `orange-warm` e tonalidades vívidas.
* **Tonalidades Puras (`pure`)**: `pure-100` (preto) e `pure-0` (branco).
* **Tonalidades de Vermelho (`red`)**: Variam de `red-90` a `red-5`, com variações `red-cool`, `red-warm`, e tonalidades vívidas.
* **Tonalidades de Violeta (`violet`)**: Variam de `violet-90` a `violet-5`, com variações `violet-warm` e tonalidades vívidas.
* **Tonalidades de Amarelo (`yellow`)**: Variam de `yellow-90` a `yellow-5`, com uma variação vívida (`yellow-vivid`).
* **Cores Interativas e de Status**:
    * `.bg-interactive`, `.text-interactive`, `.border-interactive`: Cores para elementos interativos.
    * `.bg-danger`, `.text-danger`, `.border-danger`: Cores para indicar perigo/erro.
    * `.bg-warning`, `.text-warning`, `.border-warning`: Cores para indicar aviso.
    * `.bg-success`, `.text-success`, `.border-success`: Cores para indicar sucesso.
    * `.bg-info`, `.text-info`, `.border-info`: Cores para indicar informação.
* **Cores Primárias e Secundárias do Design System**:
    * `bg-primary-pastel-01` a `bg-primary-darken-02`, `text-primary-pastel-01` a `text-primary-darken-02`, `border-primary-pastel-01` a `border-primary-darken-02`.
    * `bg-secondary-01` a `bg-secondary-09`, `text-secondary-01` a `text-secondary-09`, `border-secondary-01` a `border-secondary-09`.
* **Cores de Suporte**: `bg-support-01` a `bg-support-11`, `text-support-01` a `text-support-11`, `border-support-01` a `border-support-11`.

---

###  3. <a name='LayouteDisplay'></a>**Layout e Display**

* **Display Utilitaries**:
    * `.d-none`: `display: none;`
    * `.d-block`: `display: block;`
    * `.d-flex`: `display: flex;`
    * `.d-inline`: `display: inline;`
    * `.d-inline-block`: `display: inline-block;`
    * `.d-inline-flex`: `display: inline-flex;`
    * Classes responsivas para display (ex: `d-sm-block`, `d-md-flex`, `d-lg-none`, `d-xl-inline-block`).
* **Flexbox**:
    * `flex-row`, `flex-row-reverse`, `flex-column`, `flex-column-reverse`: Direção do flex container.
    * `justify-content-start`, `justify-content-end`, `justify-content-center`, `justify-content-between`, `justify-content-around`, `justify-content-evenly`: Alinhamento no eixo principal.
    * `align-items-start`, `align-items-end`, `align-items-center`, `align-items-baseline`, `align-items-stretch`: Alinhamento no eixo cruzado.
    * `align-self-start`, `align-self-end`, `align-self-center`, `align-self-baseline`, `align-self-stretch`: Alinhamento individual de itens.
    * `flex-fill`, `flex-grow-1`, `flex-grow-0`, `flex-shrink-1`, `flex-shrink-0`: Propriedades de flex item.
    * `flex-wrap`, `flex-nowrap`, `flex-wrap-reverse`: Quebra de linha dos itens.
    * `order-0` a `order-12`: Ordem visual dos itens.
    * `align-content-start`, `align-content-end`, `align-content-center`, `align-content-between`, `align-content-around`, `align-content-evenly`, `align-content-stretch`: Alinhamento de linhas em um flex container.
    * Classes responsivas para todas as utilidades flexbox (ex: `flex-sm-row`, `justify-content-md-center`).
* **Grid (Colunas)**:
    * `.col`, `col-auto`, `col-1` a `col-12`: Define a largura das colunas em um sistema de grid.
    * Classes responsivas para colunas (ex: `col-sm-6`, `col-md-4`, `col-lg-3`, `col-xl-2`).
* **Contêineres**:
    * `.container`, `.container-fluid`, `.container-sm`, `.container-md`, `.container-lg`, `.container-xl`: Contêineres com larguras máximas definidas para diferentes breakpoints.
* **Linhas do Grid**:
    * `.row`: Cria uma linha de grid com espaçamento entre as colunas (`--grid-gutter`).
* **Overflow**:
    * `overflow-auto`: `overflow: auto;`
    * `overflow-hidden`: `overflow: hidden;`
    * Classes responsivas para overflow (ex: `overflow-sm-auto`).

---

###  4. <a name='EspaamentoMarginePadding'></a>**Espaçamento (Margin e Padding)**

Classes utilitárias para `margin` e `padding`. O formato é `{propriedade}-{lado}-{escala}` ou `{propriedade}-{eixo}-{escala}`. As escalas de espaçamento são baseadas em variáveis CSS.

* **Margin (`m-`)**:
    * `m-0` (0px)
    * `m-half` (4px)
    * `m-base` (8px)
    * `m-baseh` (12px)
    * `m-1` a `m-6` (escalas pré-definidas)
    * `m-2x` a `m-10x` (escalas de 16px a 80px)
    * `m-2xh` a `m-10xh` (escalas de 20px a 84px)
    * `m-auto`: `margin: auto;`
    * Variações para eixos: `mx-` (horizontal), `my-` (vertical).
    * Variações para lados: `mt-` (top), `mr-` (right), `mb-` (bottom), `ml-` (left).
    * Variações negativas: `m-nhalf`, `mt-nbase`, etc.
    * Classes responsivas (ex: `m-sm-2x`, `mx-md-auto`).
* **Padding (`p-`)**:
    * `p-0` (0px)
    * `p-half` (4px)
    * `p-base` (8px)
    * `p-baseh` (12px)
    * `p-1` a `p-6` (escalas pré-definidas)
    * `p-2x` a `p-10x` (escalas de 16px a 80px)
    * `p-2xh` a `p-10xh` (escalas de 20px a 84px)
    * Variações para eixos: `px-` (horizontal), `py-` (vertical).
    * Variações para lados: `pt-` (top), `pr-` (right), `pb-` (bottom), `pl-` (left).
    * Variações negativas: `p-nhalf`, `pt-nbase`, etc.
    * Classes responsivas (ex: `p-sm-2x`, `px-md-auto`).

---

###  5. <a name='Tipografia'></a>**Tipografia**

* **Estilos de Texto**:
    * `text-center`, `text-justify`, `text-left`, `text-right`: Alinhamento do texto.
    * `text-wrap`, `text-nowrap`: Quebra de linha.
    * `text-truncate`: Trunca o texto com reticências.
    * `text-break`: Permite quebrar palavras longas.
    * `text-lowercase`, `text-uppercase`, `text-capitalize`: Transformação do texto.
* **Pesos de Fonte (`font-weight`)**:
    * `text-thin`, `text-weight-thin` (100)
    * `text-extra-light`, `text-weight-extra-light` (200)
    * `text-light`, `text-weight-light` (300)
    * `text-regular`, `text-weight-regular` (400)
    * `text-medium`, `text-weight-medium` (500)
    * `text-semi-bold`, `text-weight-semi-bold` (600)
    * `text-bold`, `text-weight-bold` (700)
    * `text-extra-bold`, `text-weight-extra-bold` (800)
    * `text-black`, `text-weight-black` (900)
* **Tamanhos de Fonte (`font-size`)**:
    * `text-base` (14px)
    * `text-down-01` a `text-down-03` (escalas menores)
    * `text-up-01` a `text-up-11` (escalas maiores)
* Classes responsivas para todas as utilidades de texto (ex: `text-sm-center`, `text-md-bold`, `text-lg-up-02`).

---

###  6. <a name='BordasSombraseOpacidade'></a>**Bordas, Sombras e Opacidade**

* **Bordas (`border-`)**:
    * `border-solid-none`, `border-solid-sm`, `border-solid-md`, `border-solid-lg`: Bordas sólidas com diferentes espessuras.
    * `border-dashed-none`, `border-dashed-sm`, `border-dashed-md`, `border-dashed-lg`: Bordas tracejadas com diferentes espessuras.
    * `border-top`, `border-right`, `border-bottom`, `border-left`: Aplica bordas a lados específicos.
* **Arredondamento de Bordas (`rounder-`)**:
    * `rounder-none` (0px)
    * `rounder-sm` (4px)
    * `rounder-md` (8px)
    * `rounder-lg` (16px)
    * `rounder-pill` (999em)
* **Opacidade (`opacity-`)**:
    * `opacity-none` (0)
    * `opacity-default` (1)
    * `opacity-xs` (0.16)
    * `opacity-sm` (0.3)
    * `opacity-md` (0.45)
    * `opacity-lg` (0.65)
    * `opacity-xl` (0.85)
* **Sombras (`shadow-`)**:
    * `shadow-none`
    * `shadow-sm`, `shadow-md`, `shadow-lg`, `shadow-xl`: Sombras para baixo com diferentes offsets.
    * `shadow-sm-inset`, `shadow-md-inset`, `shadow-lg-inset`, `shadow-xl-inset`: Sombras internas para cima.
    * `shadow-sm-up`, `shadow-md-up`, `shadow-lg-up`, `shadow-xl-up`: Sombras para cima.
    * `shadow-sm-inset-up`, `shadow-md-inset-up`, `shadow-lg-inset-up`, `shadow-xl-inset-up`: Sombras internas para baixo.
    * `shadow-sm-right`, `shadow-md-right`, `shadow-lg-right`, `shadow-xl-right`: Sombras para a direita.
    * `shadow-sm-inset-right`, `shadow-md-inset-right`, `shadow-lg-inset-right`, `shadow-xl-inset-right`: Sombras internas para a esquerda.
    * `shadow-sm-left`, `shadow-md-left`, `shadow-lg-left`, `shadow-xl-left`: Sombras para a esquerda.
    * `shadow-sm-inset-left`, `shadow-md-inset-left`, `shadow-lg-inset-left`, `shadow-xl-inset-left`: Sombras internas para a direita.
* **Camadas (Z-index)**:
    * `layer-0` a `layer-4`: Diferentes níveis de z-index.

---

###  7. <a name='AnimaeseTransies'></a>**Animações e Transições**

* **Funções de Animação (`ease-`)**:
    * `ease`: `cubic-bezier(0.25, 0.1, 0.25, 1)`
    * `ease-in`: `cubic-bezier(0.42, 0, 1, 1)`
    * `ease-out`: `cubic-bezier(0, 0, 0.58, 1)`
    * `ease-in-out`: `cubic-bezier(0.42, 0, 0.58, 1)`
    * `ease-linear`: `cubic-bezier(0, 0, 1, 1)`
* **Duração da Animação (`-fast`)**:
    * `very-fast` (0.1s)
    * `fast` (0.3s)
    * `moderate` (0.5s)
    * `slow` (0.8s)
    * `very-slow` (1s)

---

###  8. <a name='conesFontAwesome'></a>**Ícones (Font Awesome)**

* Classes base para ícones: `.svg-inline--fa`, `.fa`, `.fab`, `.fad`, `.fal`, `.far`, `.fas`.
* **Tamanhos de Ícone**:
    * `fa-xs` (8px)
    * `fa-sm` (12px)
    * `fa-lg` (20px)
    * `fa-2x` a `fa-10x` (32px a 160px)

---

###  9. <a name='ClassesdeComponenteseElementosHTML'></a>**Classes de Componentes e Elementos HTML**

* **Elementos HTML Padrão**: Estilos para `body`, `p`, `a`, `button`, `img`, `h1` a `h6`, `ul`, `ol`, `blockquote`, `table`, `th`, `td`, `label`, `fieldset`, `legend`, `::placeholder`, `input`, `textarea`, `code`, `pre`, `mark`.
* **`.highlight`**: Estilo para destaque de texto.
* **Estados (`disabled`, `dragged`, etc.)**:
    * `[disabled]`, `.disabled`: Define estilos para elementos desabilitados.
    * `.dragged`: Estilo para elementos sendo arrastados.
* **`.dropdown`**: Componente de dropdown.
* **`.br-accordion`**: Componente de acordeão.
    * `.item`: Item do acordeão.
    * `.header`: Cabeçalho do item.
    * `.content`: Conteúdo do item.
    * `[negative]`: Variação de estilo negativo.
* **`.br-avatar`**: Componente de avatar.
    * `.content`, `.image`, `.letter`: Conteúdo do avatar.
    * `small`, `medium`, `large`: Variações de tamanho.
    * `.br-avatar-action`: Botão de ação do avatar.
* **`.br-breadcrumb`**: Componente de breadcrumb.
    * `.crumb-list`: Lista de itens.
    * `.crumb`: Item individual.
    * `.home`, `.menu-mobil`: Botões de navegação.
    * `.br-card`: Card para menus suspensos.
* **`.br-button`**: Componente de botão.
    * `block`, `block-sm`, `block-md`, etc.: Botões de largura total (responsivos).
    * `auto`, `auto-sm`, `auto-md`, etc.: Botões com largura automática (responsivos).
    * `circle`, `xsmall`, `small`, `medium`, `large`: Variações de forma e tamanho.
    * `primary`, `secondary`, `danger`, `success`, `warning`, `info`: Variações de cor e estilo.
    * `active`, `loading`: Estados do botão.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-card`**: Componente de card.
    * `.card-content`, `.card-header`, `.card-footer`: Áreas do card.
    * `h-fixed`: Altura fixa com scroll.
    * `hover`: Efeito de hover.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-carousel`**: Componente de carrossel.
    * `.carousel-stage`: Área visível do carrossel.
    * `.carousel-page`: Página individual do carrossel.
    * `.carousel-content`, `.carousel-title`: Conteúdo da página.
    * `.carousel-step`: Indicadores de passo/navegação.
    * `.carousel-button`, `.carousel-btn-next`, `.carousel-btn-prev`: Botões de navegação.
    * `[data-stage=in]`, `[data-stage=out]`, `[data-stage=hibh]`, `[data-stage=hibw]`: Variações do stage.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-checkbox`**: Componente de checkbox.
    * `hidden-label`: Esconde o label.
    * `invalid`, `valid`: Estados de validação.
    * `small`: Variação de tamanho.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-radio`**: Componente de rádio button.
    * `invalid`, `valid`: Estados de validação.
    * `small`: Variação de tamanho.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-cookiebar`**: Componente de barra de cookies.
    * `default`: Estilo padrão da barra.
    * `.entry-text`, `.info-text`, `.main-content`, `.complementary-content`, `.actions`: Áreas da barra.
    * `.br-modal-header`, `.br-modal-title`, `.last-update`: Cabeçalho do modal de cookies.
    * `.br-modal-body`: Corpo do modal de cookies.
    * `.group-name`, `.cookies-checked`, `.group-size`: Informações dos grupos de cookies.
    * `.always-active`: Cookies sempre ativos.
    * `.cookie-term`, `.notes`: Termos e notas.
* **`.br-divider`**: Componente de divisor horizontal.
    * `content`: Divisor com conteúdo centralizado.
    * `vertical`: Divisor vertical.
    * `sm`, `md`, `lg`: Variações de espessura.
    * `dashed`: Estilo tracejado.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-header`**: Componente de cabeçalho.
    * `.header-top`, `.header-bottom`: Áreas do cabeçalho.
    * `.header-logo`, `.header-sign`: Logo e assinatura.
    * `.header-actions`: Ações do cabeçalho (links, funções, login, avatar, busca).
    * `.header-menu`: Menu principal.
    * `small`, `medium`, `large`, `compact`: Variações de tamanho e estilo.
    * `[data-sticky]`: Cabeçalho fixo ao rolar.
    * `[data-no-links]`, `[data-no-functions]`, `[data-no-login]`, `[data-no-search]`, `[data-no-logo]`, `[data-no-sign]`, `[data-no-subtitle]`: Oculta elementos específicos.
* **`.br-input`**: Componente de campo de entrada de texto.
    * `input-inline`: Input e label na mesma linha.
    * `.input-group`: Grupo de input.
    * `.input-icon`: Ícone dentro do input.
    * `.br-button`: Botão dentro do input.
    * `input-highlight`: Estilo de destaque.
    * `.br-list`: Lista de sugestões.
    * `success`, `danger`, `warning`, `info`: Estados de validação.
    * `small`, `medium`, `large`: Variações de tamanho.
    * `inverted`, `dark-mode`: Variações de tema.
    * `.feedback`: Mensagem de feedback.
* **`.br-item`**: Componente de item de lista genérico, usado em outros componentes.
    * `[data-toggle]`: Habilita funcionalidade de toggle.
    * `[data-toggle=selection]`: Habilita seleção.
    * `.content`: Área de conteúdo do item.
    * `primary-lighten-01` a `support-08`: Variações de cor.
    * `selected`, `active`: Estados de seleção/ativação.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-list`**: Componente de lista.
    * `horizontal`: Lista horizontal.
    * `.header`: Cabeçalho da lista.
    * `[data-one-line]`, `[data-two-lines]`, `[data-three-lines]`: Número de linhas para itens.
* **`.br-menu`**: Componente de menu de navegação.
    * `.menu-container`, `.menu-scrim`, `.menu-panel`: Elementos estruturais do menu.
    * `.menu-header`, `.menu-title`: Cabeçalho do menu.
    * `.menu-body`, `.menu-folder`, `.drop-menu`: Corpo e tipos de menu.
    * `.menu-footer`, `.menu-logos`, `.menu-links`, `.social-network`, `.menu-social`, `.menu-info`: Rodapé do menu.
    * `small`, `medium`, `large`: Variações de tamanho dos itens do menu.
    * `push`, `contextual`: Tipos de comportamento do menu.
* **`.loading`, `.br-loading`**: Componentes de carregamento.
    * `[data-progress]`: Indicador de progresso (0% a 100%).
    * `loading-mask`, `loading-fill`: Elementos para o círculo de progresso.
    * `medium`: Variação de tamanho.
* **`.br-magic-button`**: Componente de botão mágico.
    * `small`, `medium`, `large`: Variações de tamanho.
* **`.br-message`**: Componente de mensagem (feedback).
    * `.content`, `.message-title`, `.message-body`: Conteúdo da mensagem.
    * `icon`: Ícone da mensagem.
    * `close`: Botão para fechar a mensagem.
    * `success`, `danger`, `info`, `warning`: Variações de status.
* **`.feedback`**: Mensagens de feedback, geralmente usadas com inputs.
    * `success`, `danger`, `info`, `warning`: Variações de status.
* **`.br-modal`**: Componente de modal.
    * `.modal-title`, `.br-modal-header`, `.br-modal-body`, `.br-modal-footer`: Áreas do modal.
    * `xsmall`, `small`, `medium`, `large`, `auto`: Variações de tamanho.
    * `.terms`: Área para termos e condições.
* **`.br-notification`**: Componente de notificação.
    * `.notification-header`, `.notification-body`: Áreas da notificação.
    * `.status`: Indicador de status dentro do item.
* **`.br-pagination`**: Componente de paginação.
    * `.page`: Item de página.
    * `active`: Página ativa.
    * `pagination-ellipsis`: Indicador de páginas omitidas.
    * `pagination-information`, `pagination-per-page`, `pagination-go-to-page`: Informações e controles de paginação.
    * `pagination-arrows`: Botões de navegação.
    * `small`, `medium`, `large`: Variações de tamanho.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-scrim`**, **`.br-scrim-util`**: Componentes de scrim (camada sobre o conteúdo).
    * `foco`: Scrim para foco.
    * `inibicao`: Scrim para inibição.
    * `legibilidade`: Scrim para legibilidade.
    * `active`: Scrim ativo.
* **`.br-select`**: Componente de select (dropdown).
    * `.br-input`, `.br-list`: Elementos do select.
    * `selected`, `highlighted`: Estados de seleção/destaque.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-sign-in`**: Componente de botão de login/autenticação.
    * Variações de tamanho e estilo de `br-button`.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-skiplink`**: Componente de link de atalho.
    * `full`: Variação de estilo.
* **`.br-step`**: Componente de progresso em passos.
    * `.step-progress`: Barra de progresso.
    * `.step-progress-btn`: Botão de passo.
    * `.step-icon`: Ícone do passo.
    * `.step-alert`: Alerta do passo.
    * `vertical`: Orientação vertical.
    * `[data-label=bottom]`, `[data-label=top]`, `[data-label=left]`, `[data-label=right]`: Posição do label.
    * `[data-type=void]`, `[data-type=simple]`, `[data-type=text]`: Tipos de passo.
    * `[scroll]`: Permite scroll.
    * `success`, `info`, `warning`, `danger`: Cores de alerta.
    * `active`: Passo ativo.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-switch`**: Componente de switch (toggle).
    * `right`, `top`: Posição do label.
    * `small`, `medium`, `large`: Variações de tamanho.
    * `icon`: Com ícone.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-table`**: Componente de tabela.
    * `responsive`: Tabela responsiva.
    * `.column-collapse`, `.column-checkbox`: Colunas especiais.
    * `.table-header`, `.top-bar`, `.table-title`, `.actions-trigger`: Cabeçalho da tabela.
    * `.search-bar`: Barra de busca.
    * `.selected-bar`, `.selection-bar`: Barra de seleção.
    * `.info`, `.text`, `.count`: Informações da barra de seleção.
    * `.footer`, `.table-footer`: Rodapé da tabela.
    * `small`, `medium`, `large`: Variações de tamanho das linhas da tabela.
    * `no-hover`: Desabilita o hover das linhas.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-tab`**: Componente de abas (tabs).
    * `.tab-nav`: Navegação das abas.
    * `.tab-item`: Item de aba.
    * `is-active`, `active`: Aba ativa.
    * `.results`: Contador de resultados.
    * `[data-counter=true]`: Habilita contador.
    * `.tab-content`, `.tab-panel`: Conteúdo das abas.
    * `small`, `medium`, `large`: Variações de tamanho.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-tag`**: Componente de tag.
    * `interaction`, `interaction-select`: Tags interativas/selecionáveis.
    * `status`, `count`, `icon`: Tipos de tags.
    * `small`, `medium`, `large`: Variações de tamanho.
    * Cores de suporte (ex: `support-01` a `support-11`).
    * Cores primárias/secundárias (ex: `primary-pastel-01`).
    * `success`, `danger`, `warning`, `info`: Cores de status.
* **`.br-tag-input`**: Componente de input com tags.
    * `.input-tag`: O input de texto dentro do componente.
* **`.br-textarea`**: Componente de textarea.
    * `small`, `medium`, `large`: Variações de tamanho.
    * `success`, `danger`, `warning`, `info`: Estados de validação.
    * `inverted`, `dark-mode`: Variações de tema.
* **`.br-tooltip`**: Componente de tooltip.
    * `[data-show]`: Mostra o tooltip.
    * `[popover]`: Estilo de popover.
    * `success`, `error`, `warning`, `info`: Cores de status.
    * `.arrow`: Seta do tooltip.
    * `[data-popper-placement^=top]`, `[data-popper-placement^=bottom]`, `[data-popper-placement^=left]`, `[data-popper-placement^=right]`: Posição do tooltip.
    * `.text`, `.subtext`, `.link`: Conteúdo do tooltip.
    * `.popover-header`, `.popover-image`, `.popover-icon`, `.popover-body`, `.popover-footer`: Estrutura do popover.
    * `close`: Botão para fechar o tooltip.
* **`.br-upload`**: Componente de upload de arquivos.
    * `input`: Input de arquivo (oculto).
    * `.upload-button`: Botão de upload.
    * `.upload-list`: Lista de arquivos.
    * `success`, `danger`, `warning`, `info`: Estados de validação.
    * `dragging`: Estado de arrastar arquivo.
* **`.br-wizard`**: Componente de wizard (passos).
    * `.wizard-progress`: Barra de progresso.
    * `.wizard-progress-btn`: Botão de passo.
    * `.info`: Informação do passo.
    * `[collapsed]`: Estado de colapsado.
    * `.wizard-form`: Formulário do wizard.
    * `.wizard-panel`: Painel de passo.
    * `[active]`: Passo ativo.
    * `.wizard-panel-content`: Conteúdo do painel.
    * `.wizard-panel-btn`, `.wizard-btn-next`, `.wizard-btn`, `.wizard-btn-prev`, `.wizard-btn-canc`: Botões de navegação.
    * `[vertical]`: Orientação vertical.
    * `[scroll]`: Permite scroll.
    * `inverted`, `dark-mode`: Variações de tema.

---