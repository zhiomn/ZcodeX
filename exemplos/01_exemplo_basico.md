# Exemplo Básico de Uso do ZcodeX

## Cenário: Criar um Componente de Botão

### Fase 1: Breeze (Brisa)
"Precisamos de um botão reutilizável com temas claro e escuro."

### Fase 2: Groundpath (Plano de Ação)
    # Groundpath: Componente Botão
    ## Checklist:
    - [ ] Template HTML do botão
    - [ ] Lógica TypeScript com props
    - [ ] Estilos CSS com variáveis de tema
    - [ ] Testes unitários básicos
    - [ ] Documentação de uso

### Fase 3: Implementação
    cat << 'EOF' > src/components/Botao/Botao.vue
    <template>
      <button :class="['botao', `tema-${tema}`]" @click="handleClick">
        <slot></slot>
      </button>
    </template>

    <script setup lang="ts">
    defineProps<{
      tema: 'claro' | 'escuro'
    }>()

    const emit = defineEmits<{
      (e: 'clique'): void
    }>()

    const handleClick = () => {
      emit('clique')
    }
    </script>

    <style scoped>
    .botao {
      padding: 12px 24px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-weight: 600;
    }

    .tema-claro {
      background-color: var(--cor-primaria-claro);
      color: var(--cor-texto-claro);
    }

    .tema-escuro {
      background-color: var(--cor-primaria-escuro);
      color: var(--cor-texto-escuro);
    }
    </style>
    EOF

### Fase 4: Log (Registro)
    # Log: Implementação Componente Botão
    Data: 2024-01-15
    Implementado componente Botão com suporte a temas claro e escuro.
    Utilizadas variáveis CSS para theming.
