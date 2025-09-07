# Tópico 02: Posicionamento

## Regra de Posicionamento

A lista de arquivos **deve** ser posicionada imediatamente após o bloco `cat`, sem nenhum conteúdo intermediário.

## Estrutura Correta

    cat << 'EOF' > caminho/do/arquivo.ext
    conteúdo do arquivo
    EOF

    ***

    **Arquivos Atualizados:**

    *   `caminho/do/arquivo.ext`

## Justificativa

O posicionamento imediato garante:
1.  **Associação Clara**: A lista refere-se claramente ao bloco `cat` anterior.
2.  **Prevenção de Ambiguidades**: Elimina confusão sobre qual operação a lista documenta.
3.  **Leitura Robótica**: Facilita o parsing automatizado por ferramentas.

## Exemplo de Violação

    cat << 'EOF' > arquivo.txt
    conteúdo
    EOF

    Aqui foi atualizado o arquivo X...  # VIOLAÇÃO: conteúdo intermediário
    ***

    **Arquivos Atualizados:**
    *   `arquivo.txt`

---

**Próximo:** Veja [Exemplos Práticos](topico_03.exemplos_praticos.md).
