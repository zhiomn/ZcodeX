# Termos de Arquitetura

## Toolbox (Floema)
Nossa biblioteca interna e compartilhada de código (`source/shared/`). Contém utilitários e componentes reutilizáveis.

## Contrato de Dados (Schema)
A definição formal da estrutura de um arquivo `.json`. Garante consistência e interoperabilidade.

## Componente Atômico
A prática de separar um componente Vue em arquivos `.html`, `.ts` e `.css`. Promove modularidade e reuso.

## Monorepo
A arquitetura de nosso projeto, contendo múltiplos subprojetos (workspaces) em um único repositório.

## Guardião (Coagula)
O serviço centralizado responsável por todas as operações de escrita no sistema de arquivos.
