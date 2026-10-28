# Aurora — Landing page de apresentação

Landing page estática para apresentar a Aurora, um estúdio criativo fictício. O projeto demonstra como organizar uma página institucional moderna usando somente HTML e CSS: sem JavaScript, frameworks ou etapa de build.

## Visão geral

A página conduz o visitante por uma apresentação do estúdio, uma seleção ilustrativa de projetos, os serviços oferecidos e um convite para contato. O layout se adapta a telas grandes, tablets e celulares.

## Tecnologias

- **HTML5** para estrutura semântica e conteúdo.
- **CSS3** para identidade visual, layout, responsividade e interações leves.
- **Google Fonts** para as famílias Manrope e DM Sans.
- **Unsplash** para as fotografias demonstrativas.

Não há dependências para instalar nem compilação necessária.

## Estrutura do projeto

```text
LandingPage/
├── index.html   # Conteúdo, estrutura e metadados da página
├── style.css    # Estilos, componentes e regras responsivas
└── README.md    # Documentação do projeto
```

## Como visualizar

1. Abra `index.html` diretamente em um navegador; ou
2. Abra a pasta no VS Code e use uma extensão de servidor local, como Live Server, para recarregar a página automaticamente durante a edição.

Como o projeto é estático, qualquer servidor HTTP simples também pode servi-lo. Não é preciso executar comandos de instalação.

## Seções da página

1. **Cabeçalho:** marca e navegação por âncoras.
2. **Apresentação:** mensagem principal e imagem de destaque.
3. **Sobre:** propósito e posicionamento do estúdio.
4. **Projetos:** três trabalhos ilustrativos com fotografias.
5. **Serviços:** estratégia de marca, identidade visual e experiência digital.
6. **Contato:** link `mailto:` para iniciar uma conversa.
7. **Rodapé:** assinatura e atalho para o início da página.

## Responsividade

O CSS parte de um layout para telas amplas e usa media queries para reorganizar os elementos em telas menores:

- **Até 900 px:** reduz espaçamentos e ajusta a composição das seções.
- **Até 640 px:** empilha conteúdo e projetos, reorganiza a navegação e ajusta tipografia e margens para celular.

As larguras são valores de referência. O layout também utiliza unidades flexíveis, `min()`, `clamp()` e CSS Grid para se adaptar entre os pontos de quebra.

## Acessibilidade e boas práticas

- Documento em português (`lang="pt-BR"`) e viewport configurado para dispositivos móveis.
- Regiões semânticas, hierarquia de títulos e rótulo na navegação.
- Texto alternativo nas imagens de conteúdo; elementos decorativos são ocultados de tecnologias assistivas.
- Links com indicação de foco visível para navegação por teclado.
- Respeito à preferência do sistema por movimento reduzido.
- Carregamento tardio (`loading="lazy"`) nas imagens abaixo da primeira dobra.

## Personalização

- Edite textos, títulos, links e descrições em `index.html`.
- Ajuste cores, fontes, espaçamentos e breakpoints em `style.css`. As cores principais estão centralizadas em variáveis CSS no início do arquivo.
- Substitua as URLs das imagens do Unsplash por fotografias próprias ou por imagens cuja licença permita o uso pretendido.
- Atualize o endereço `oi@aurora.studio` para o canal de contato real antes de publicar.
- Revise o nome fictício, os textos e os projetos de demonstração para refletir a identidade da organização.

## Imagens e recursos externos

As fotografias são carregadas do CDN do Unsplash e as fontes do Google Fonts. Por isso, esses recursos dependem de conexão com a internet. Para publicação, verifique os termos de uso e atribuição aplicáveis aos recursos escolhidos; se necessário, hospede imagens autorizadas localmente e atualize os caminhos no HTML.

## Observação

Aurora, os projetos e as informações de contato são conteúdo demonstrativo. Este repositório não implementa envio de formulário, analytics ou integração com serviços externos.
