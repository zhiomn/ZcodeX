# Tópico 02: A Regra Anti-Aninhamento ⚠️ CRÍTICO

## ⚠️ A REGRA É ABSOLUTA

**É ESTRITAMENTE PROIBIDO** o uso de "fences" de markdown (```) dentro de um bloco `cat`. 

**VIOLAÇÃO DESTA REGRA QUEBRARÁ INEXORAVELMENTE O CODEBLOCK E INVALIDARÁ A RESPOSTA COMPLETA.**

## 🚨 MÉTODO CORRETO OBRIGATÓRIO

Para representar código ou qualquer bloco de formatação dentro do arquivo que está sendo criado, use **INDENTAÇÃO COM 4 ESPAÇOS**.

## ❌ EXEMPLO DE VIOLAÇÃO (PROIBIDO - GARANTIDO QUEBRAR)

    cat << 'EOF' > arquivo.md
    ```
    function exemplo() {  # VIOLAÇÃO: Fences dentro de cat
      return 'erro'
    }
    ```
    EOF

## ✅ EXEMPLO DE CONFORMIDADE (OBRIGATÓRIO - FUNCIONARÁ)

    cat << 'EOF' > arquivo.md
        function exemplo() {
          return 'sucesso'
        }
    EOF

## 🔥 JUSTIFICATIVA DA CRITICIDADE

As "fences" (```) quebram o parsing do bloco `cat` atual de forma **IRREVERSÍVEL**. Isso:
1.  **Corrompe a operação** inteira de escrita do arquivo
2.  **Torna o código inexecutável**
3.  **Exige retrabalho completo**
4.  **Ciclos de debugging desnecessários**

A indentação com 4 espaços é universalmente reconhecível e mecanicamente sólida.

## 🎯 REGRA MNEMÔNICA

**"4 ESPAÇOS DENTRO, 'EOF' FORA - SEMPRE FUNCIONA, NUNCA QUEBRA"**

---

**Próximo:** Veja [Justificativas e Exemplos Adicionais](topico_03.justificativa_exemplos.md).
