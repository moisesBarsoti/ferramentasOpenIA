# Explorando o Copiloto e Ferramentas da OpenAI

## 🎯 Objetivos do Projeto
- ✔️ Aplicar conceitos de IA generativa na prática  
- 📝 Documentar processos técnicos de forma clara e estruturada  
- 🤖 Explorar recursos do GitHub Copilot e ferramentas OpenAI  
- 📚 Compartilhar aprendizados através do GitHub  

## 🛠 Tecnologias Utilizadas
| Tecnologia | Uso Principal |
|------------|---------------|
| GitHub Copilot | Geração assistida de código |
| OpenAI API | Processamento de linguagem natural |
| Python | Exemplos e automações |
| Markdown | Documentação técnica |

## 💻 Exemplos Práticos

### 1. Geração de Código com Copilot
```python
# Função para verificar números primos (gerada com Copilot)
def is_prime(n: int) -> bool:
    """
    Verifica se um número é primo
    
    Args:
        n (int): Número a ser verificado
        
    Returns:
        bool: True se for primo, False caso contrário
    """
    if n <= 1:
        return False
    if n <= 3:
        return True
    if n % 2 == 0 or n % 3 == 0:
        return False
    i = 5
    while i * i <= n:
        if n % i == 0 or n % (i + 2) == 0:
            return False
        i += 6
    return True
