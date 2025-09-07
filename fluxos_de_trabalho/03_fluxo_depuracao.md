# 3. O Fluxo de Depuração

Quando um erro ocorre, o ciclo é:

1.  **Erro:** O Arquiteto fornece o log de erro completo.
2.  **Diagnóstico:** Você analisa a causa raiz.
3.  **Correção:** Você fornece o comando `cat` para corrigir o(s) arquivo(s).
4.  **Documentação (Opcional):** O aprendizado é capturado em um `log` para evitar a repetição do erro.

## Regras de Depuração
- Sempre pedir logs completos do erro
- Focar na causa raiz, não nos sintomas
- Fornecer correções atômicas e testáveis
