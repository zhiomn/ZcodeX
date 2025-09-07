# 📊 Diretório de Diagramas

Esta pasta armazena recursos visuais que complementam a documentação do ZcodeX.

## 🎯 Diagramas Criados

1.  **arquitetura-zcodex.mmd**
    -   Mapa completo da estrutura do framework
    -   Visualiza todas as componentes e suas relações

2.  **fluxo-protocolo-cat.mmd**  
    -   Fluxograma do protocolo CAT passo a passo
    -   Inclui verificações e tratamentos de erro

3.  **mapa-mental-lexico.mmd**
    -   Mapa mental dos termos do léxico
    -   Organização visual dos conceitos

## 🛠️ Como Visualizar

Os arquivos `.mmd` são do Mermaid.js. Podem ser visualizados em:

-   Editores online: Mermaid Live Editor, GitHub
-   VS Code com extensão Mermaid
-   GitHub: os diagramas renderizam automaticamente

## 🔗 Uso na Documentação

Referencie os diagramas assim:

    ```mermaid
    --8<-- "assets/diagrams/arquitetura-zcodex.mmd"
    ```

## 📋 Próximos Diagramas Sugeridos

- [ ] Fluxo completo Breeze→Groundpath→Log
- [ ] Diagrama de sequência do Guardião (Coagula)
- [ ] Arquitetura de monorepo
- [ ] Processo de depuração

---

**Nota:** Execute `mermaid-cli` para gerar PNG/SVG dos arquivos .mmd
