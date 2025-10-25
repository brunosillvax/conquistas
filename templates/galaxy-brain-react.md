# Template para Galaxy Brain - React Discussions

## Pergunta: "Como usar useState corretamente?"

## Resposta Template:

### Solucao

Baseado na sua pergunta sobre **useState**, aqui esta uma abordagem que pode ajudar:

### Implementacao
`javascript
import React, { useState } from 'react';

function Exemplo() {
  // Estado simples
  const [count, setCount] = useState(0);
  
  // Estado com objeto
  const [user, setUser] = useState({
    name: '',
    email: ''
  });
  
  // Estado com array
  const [items, setItems] = useState([]);
  
  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={() => setCount(count + 1)}>
        Incrementar
      </button>
    </div>
  );
}
`

### Explicacao
- **Por que funciona:** useState retorna um array com [valor, setter]
- **Alternativas:** useReducer para estado complexo
- **Consideracoes:** Evite mutacoes diretas do estado

### Proximos Passos
1. Teste o exemplo acima
2. Considere useReducer para estado complexo
3. Leia sobre otimizacao com useMemo/useCallback

### Recursos Adicionais
- [Documentacao oficial do useState](https://reactjs.org/docs/hooks-state.html)
- [Guia completo de Hooks](https://reactjs.org/docs/hooks-intro.html)

---

**Espero que ajude! Se tiver duvidas, estou aqui.**

**Dica:** Se esta resposta foi util, considere marca-la como aceita!
