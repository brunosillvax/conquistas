# Template para Galaxy Brain - Vue Discussions

## Pergunta: "Como usar computed properties?"

## Resposta Template:

### Solucao

Baseado na sua pergunta sobre **computed properties**, aqui esta uma abordagem que pode ajudar:

### Implementacao
`javascript
// Vue 3 Composition API
import { ref, computed } from 'vue'

export default {
  setup() {
    const firstName = ref('Joao')
    const lastName = ref('Silva')
    
    // Computed property
    const fullName = computed(() => {
      return firstName.value + ' ' + lastName.value
    })
    
    return {
      firstName,
      lastName,
      fullName
    }
  }
}
`

`javascript
// Vue 2 Options API
export default {
  data() {
    return {
      firstName: 'Joao',
      lastName: 'Silva'
    }
  },
  computed: {
    fullName() {
      return this.firstName + ' ' + this.lastName
    }
  }
}
`

### Explicacao
- **Por que funciona:** Computed properties sao cacheadas e reativas
- **Alternativas:** Methods para funcoes que nao precisam de cache
- **Consideracoes:** Use computed para valores derivados

### Proximos Passos
1. Teste os exemplos acima
2. Considere usar computed para valores derivados
3. Leia sobre reatividade no Vue

### Recursos Adicionais
- [Documentacao oficial do Vue](https://vuejs.org/guide/essentials/computed.html)
- [Guia de reatividade](https://vuejs.org/guide/extras/reactivity-in-depth.html)

---

**Espero que ajude! Se tiver duvidas, estou aqui.**

**Dica:** Se esta resposta foi util, considere marca-la como aceita!
