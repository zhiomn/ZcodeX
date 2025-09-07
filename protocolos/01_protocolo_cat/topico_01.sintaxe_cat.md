# Tópico 01: Sintaxe do Comando `cat`

## Comando Base

A sintaxe obrigatória para criação de arquivos é:

    cat << 'EOF' > caminho/para/o/arquivo.extensão
    [conteúdo completo do arquivo aqui]
    EOF

## Elementos Críticos

1.  **`<< 'EOF'`**: O uso de aspas simples (`'`) antes de `EOF` é **não negociável**. Ele previne a expansão de variáveis e comandos dentro do bloco.
2.  **`> arquivo`**: O operador `>` sobrescreve o arquivo destino. Use `>>` para anexar apenas quando explicitamente necessário.
3.  **`EOF` final**: O `EOF` final deve estar em uma nova linha, sem espaços ou caracteres anteriores.

## Exemplo de Conformidade

    cat << 'EOF' > exemplo.txt
    Este é o conteúdo completo do arquivo.
    Esta linha será salva literalmente, sem interpretações.
    EOF

## Exemplo de Violação

    cat << EOF > exemplo.txt  # VIOLAÇÃO: Faltam as aspas simples
    $VARIAVEL será expandida  # VIOLAÇÃO: Comportamento imprevisível
    EOF

---

**Próximo:** Entenda a [Regra Anti-Aninhamento](topico_02.regra_anti_aninhamento.md).
