# Tópico 03: Exemplos Práticos

## Exemplo 1: Operação Básica

    cat << 'EOF' > src/utils/validadores.js
    export function validarEmail(email) {
      return /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email)
    }
    EOF

    ***

    **Arquivos Criados:**

    *   `src/utils/validadores.js`

## Exemplo 2: Múltiplos Arquivos

    cat << 'EOF' > index.html
    <!DOCTYPE html>
    <html lang="pt-BR">
    <head>
        <meta charset="UTF-8">
        <title>ZcodeX</title>
    </head>
    <body>
        <div id="app"></div>
    </body>
    </html>
    EOF

    cat << 'EOF' > src/main.js
    import { criarApp } from './app.js'
    criarApp().mount('#app')
    EOF

    ***

    **Arquivos Atualizados:**

    *   `index.html`
    *   `src/main.js`

## Exemplo 3: Tipos Diferentes de Operação

    cat << 'EOF' > novo-componente.vue
    <template>
      <button @click="handleClick">Clique</button>
    </template>
    EOF

    rm -f arquivo-antigo.js

    ***

    **Arquivos Criados:**

    *   `novo-componente.vue`

    **Arquivos Excluídos:**

    *   `arquivo-antigo.js`

---

**Próximo:** Avance para o [Protocolo do Sumário de Ação](../03_protocolo_sumario_acao/_indice.*.md).
