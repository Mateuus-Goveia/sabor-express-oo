# 🍽️ Sistema de Restaurantes

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![Status](https://img.shields.io/badge/status-Em%20Desenvolvimento-yellow)]()
[![Alura](https://img.shields.io/badge/Curso-Alura-blueviolet)](https://www.alura.com.br/)

Projeto desenvolvido durante o curso **"Python: aplicando a Orientação a Objetos"** da [Alura](https://www.alura.com.br/).

O sistema simula o cadastro e a avaliação de restaurantes, aplicando os princípios da **Programação Orientada a Objetos (POO)**.

---

## 📘 Sobre o Projeto

O objetivo é praticar os fundamentos de **classes**, **atributos**, **métodos**, **encapsulamento** e **instâncias** em Python.

O sistema permite:
✅ Cadastrar restaurantes com nome e categoria  
✅ Ativar ou desativar um restaurante  
✅ Registrar avaliações de clientes (de 1 a 5 estrelas)  
✅ Exibir uma listagem com média das avaliações e status  

---

## 🧩 Estrutura do Projeto

```

📂 projeto_restaurantes
┣ 📜 app.py
┣ 📜 restaurante.py
┣ 📜 avaliacao.py
┗ 📁 modelos/

````

---

## 🧠 Principais Classes

### 🏛️ `class Restaurante`
Responsável por representar um restaurante e suas avaliações.

**Principais métodos:**
- `listar_restaurantes()` → exibe todos os restaurantes cadastrados  
- `receber_avaliacao(cliente, nota)` → registra uma nova avaliação  
- `media_avaliacoes` → retorna a média das notas  
- `alternar_estado()` → ativa/desativa o restaurante  

---

### ⭐ `class Avaliacao`
Representa a avaliação feita por um cliente.

```python
class Avaliacao:
    def __init__(self, cliente, nota):
        self._cliente = cliente
        self._nota = nota
````

---

## 🧩 Exemplo de Uso (`app.py`)

```python
from modelos.restaurante import Restaurante

restaurante_praca = Restaurante('Praça', 'Gourmet')
restaurante_praca.receber_avaliacao('Gui', 5)
restaurante_praca.receber_avaliacao('Lais', 4)
restaurante_praca.receber_avaliacao('Emy', 1)

def main():
    Restaurante.listar_restaurantes()

if __name__ == '__main__':
    main()
```

---

## 💻 Exemplo de Saída no Terminal

```bash
Nome do Restaurante         | Categoria do Restaurante     | Avaliação                | Status do Restaurante
Praça                       | GOURMET                     | 3.3                      | ☐
```

---

## 🚀 Como Executar o Projeto

1. Clone este repositório:

   ```bash
   git clone https://github.com/Mateuus-Goveia/oo-sabor-express
   ```

2. Acesse a pasta:

   ```bash
   cd oo-sabor-express
   ```

3. Execute o projeto:

   ```bash
   python app.py
   ```

---

## 🧩 Conceitos Utilizados

* Programação Orientada a Objetos (POO)
* Encapsulamento e propriedades (`@property`)
* Métodos de classe (`@classmethod`)
* Boas práticas de modelagem e formatação de código

---

## 🧑‍💻 Autor

**[Matheus Goveia](https://github.com/Mateuus-Goveia)**
📚 Projeto desenvolvido durante o curso da [Alura](https://www.alura.com.br/)

[![GitHub](https://img.shields.io/badge/GitHub-000?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/seu-usuario)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge\&logo=linkedin\&logoColor=white)](https://www.linkedin.com/in/matheus-goveia)