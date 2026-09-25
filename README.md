# InvestView

Interface de um painel rápido de investimentos, desenvolvida como atividade prática da disciplina **Web Mobile** do curso de Tecnologia em Análise e Desenvolvimento de Sistemas (Mackenzie).

O objetivo foi aplicar o conceito de **Mobile First**: construir a interface pensando primeiro no celular e, a partir dela, adaptar o layout para telas maiores usando media queries — sem duplicar a estrutura do zero para cada tamanho de tela.

## O que muda entre os tamanhos de tela

**Mobile (até 768px)**
- Ocupa 100% da altura da tela (`100dvh`), sem bordas arredondadas
- Fundo sólido
- Menu de ações (Aportar / Resgatar / Extrato) fixo na parte inferior, como uma barra de navegação de app nativo

**Desktop (acima de 768px)**
- Fundo da página com gradiente
- O painel vira um cartão centralizado, com largura limitada, bordas arredondadas e sombra
- Menu de ações vira uma barra lateral (sidebar) à esquerda do conteúdo

## Tecnologias

- HTML5 semântico
- CSS3
  - Flexbox (alinhamentos e distribuição de espaço)
  - CSS Grid (estrutura de colunas no desktop e grade de botões de ação)
  - Custom Properties (variáveis de cor centralizadas em `:root`)
  - Media Queries (responsividade Mobile First)
- Ícones em SVG inline (sem uso de imagens externas)

## Estrutura do projeto

```
investview/
├── index.html
└── css/
    └── style.css
```

## Como visualizar

Não há dependências ou build — é só abrir o `index.html` diretamente no navegador.

Para testar a responsividade, recomenda-se usar o modo de dispositivo do DevTools (F12 → ícone de celular/tablet) e redimensionar a janela em torno de 768px de largura, que é o breakpoint definido entre a versão mobile e a desktop.

## Autor

Desenvolvido por **Tiago Farias**, estudante de Análise e Desenvolvimento de Sistemas.