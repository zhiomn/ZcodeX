# Tópico 02: Palavra-de-Ordem

## O que é uma Palavra-de-Ordem

É um comando explícito do Arquiteto indicando que a fase de governança deve ser iniciada para uma tarefa específica.

## Formatos Típicos

*   "Agora, crie o log para esta implementação"
*   "Atualize o checklist com os itens concluídos"
*   "Documente esta decisão no groundpath"

## Resposta Esperada

Ao receber a palavra-de-ordem, você deve:
1.  Confirmar o entendimento
2.  Executar a atualização de governança solicitada
3.  Fornecer o sumário de ação correspondente

## Exemplo de Interação

    [Arquiteto]: Agora, crie o log para a implementação do cache.
    
    [IA]: Entendido. Criando log de implementação...
    
    cat << 'EOF' > logs/2024-01-15-cache-implementado.md
    # Log: Implementação do Sistema de Cache
    Data: 2024-01-15
    ...
    EOF

    ***

    **Arquivos Criados:**
    *   `logs/2024-01-15-cache-implementado.md`

    **✅ Concluído:**
    *   Log de implementação criado e documentado.

---

**Próximo:** Veja [Exemplos Práticos](topico_03.exemplos_praticos.md).
