# Exemplo de Fluxo de Depuração

## Cenário: Erro na Validação de Email

### Erro Reportado
    Error: Invalid email validation regex
    at validarEmail (utils/validadores.js:15:23)

### Diagnóstico
A regex atual não valida corretamente emails com domínios complexos.

### Correção
    cat << 'EOF' > src/utils/validadores.js
    export function validarEmail(email) {
      return /^[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*$/.test(email)
    }
    EOF

### Documentação (Opcional)
    # Log: Correção Validação Email
    Data: 2024-01-15
    Corrigida regex de validação de email para suportar domínios complexos.
    Regex atualizada segue padrão mais abrangente.
