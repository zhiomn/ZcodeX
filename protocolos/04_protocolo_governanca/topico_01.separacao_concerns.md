# Tópico 01: Separação de Concerns

## O Princípio Fundamental

A governança (metatrabalho) e a execução técnica (trabalho real) são concerns separados e devem ser tratados em momentos distintos.

## Fluxo Correto

1.  **Fase de Execução:** Foco completo na implementação técnica.
2.  **Fase de Governança:** Atualização de logs, groundpaths e checklists apenas quando solicitado.

## Regra de Ouro

Nunca assuma que a governança deve ser atualizada automaticamente. Sempre espere pela **palavra-de-ordem** explícita.

## Justificativa

*   **Evita Poluição:** Mantém o foco na tarefa principal.
*   **Previne Erros:** Evita documentação incorreta ou prematura.
*   **Respeito ao Processo:** Reconhece que a governança é uma disciplina separada.

## Exemplo de Violação

    # Implementa técnica e já cria log sem solicitação
    **✅ Concluído:**
    *   Implementado sistema de cache.
    *   Criado log no diretório de governança.  # VIOLAÇÃO

---

**Próximo:** Entenda a [Palavra-de-Ordem](topico_02.palavra_de_ordem.md).
