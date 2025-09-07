# Tópico 03: Exemplos Práticos

## Exemplo 1: Criação de Log

    [Arquiteto]: Implemente a validação de email no utils.
    
    [IA]: [Implementa a validação...]
    
    [Arquiteto]: Agora, crie o log desta implementação.
    
    [IA]: cat << 'EOF' > logs/2024-01-15-validacao-email.md
    # Log: Implementação Validação de Email
    Data: 2024-01-15
    Implementada função validarEmail no utils.
    Regex de validação de email padrão RFC 5322.
    EOF

    ***

    **Arquivos Criados:**
    *   `logs/2024-01-15-validacao-email.md`

## Exemplo 2: Atualização de Checklist

    [Arquiteto]: Marque os itens 1, 2 e 5 como concluídos no checklist.
    
    [IA]: cat << 'EOF' > groundpaths/projeto-alpha/checklist.md
    - [x] 1. Configuração inicial do Vue
    - [x] 2. Sistema de roteamento
    - [ ] 3. Gerenciamento de estado
    - [ ] 4. Testes unitários
    - [x] 5. Integração com API
    EOF

    ***

    **Arquivos Modificados:**
    *   `groundpaths/projeto-alpha/checklist.md`

## Exemplo 3: Criação de Groundpath

    [Arquiteto]: Crie um groundpath para o novo módulo de analytics.
    
    [IA]: cat << 'EOF' > groundpaths/modulo-analytics.md
    # Groundpath: Módulo de Analytics
    ## Objetivo: Implementar tracking de eventos...
    EOF

    ***

    **Arquivos Criados:**
    *   `groundpaths/modulo-analytics.md`

---

**Próximo:** Retorne ao [Índice de Protocolos](../_indice.*.md).
