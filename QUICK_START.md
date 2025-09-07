# ZcodeX - Guia de Início Rápido ⚡

## 🚀 Primeiros 5 Minutos

### 1. Estrutura Básica
    mkdir -p meu-projeto/{src,docs,logs}
    cd meu-projeto

### 2. Primeiro Arquivo
    cat << 'EOF' > src/app.js
        console.log('Hello ZcodeX!')
    EOF

### 3. Lista de Arquivos
    ***

    **Arquivos Criados:**
    *   `src/app.js`

### 4. Sumário de Ação
    **✅ Concluído:**
    *   Arquivo principal da aplicação criado.

    **▶️ Próximos Passos (Até 5):**
    *   Configurar package.json
    *   Adicionar configuração do ESLint
    *   Criar estrutura de componentes Vue

## 📋 Regras de Ouro

### 🚫 NUNCA Faça
    # ❌ PROIBIDO - Isso QUEBRARÁ tudo
    cat << EOF > arquivo.js
    function erro() {  # Faltam aspas no EOF
      return 'falha'
    }
    EOF

### ✅ SEMPRE Faça  
    # ✅ CORRETO - Isso FUNCIONARÁ
    cat << 'EOF' > arquivo.js
        function sucesso() {
          return 'funciona'
        }
    EOF

## 🆘 Socorro! Quebrei Algo

### Sintomas:
- Bloco `cat` não funciona
- Arquivo corrompido
- Erros de parsing

### Solução:
1.  Verifique se usou `<< 'EOF'` (com aspas simples)
2.  Confirme indentação de 4 espaços no conteúdo
3.  Remova qualquer ```` do conteúdo interno
4.  Execute novamente

## 🔗 Próximos Passos

1.  Leia [Protocolos de Comunicação](protocolos/_indice.*.md)
2.  Explore [Exemplos Práticos](exemplos/_indice.*.md)
3.  Use [Templates](modelos/_indice.*.md) para iniciar rapidamente

---

**Dica:** Execute `find zcodex-framework -name "*.md" | head -10` para ver a estrutura!
