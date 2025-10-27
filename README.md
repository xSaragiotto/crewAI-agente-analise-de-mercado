# 🧠 Projeto de Análise de Mercado com Crew AI

Este é um projeto de **análise de dados de mercado**, desenvolvido com **Crew AI** e uma arquitetura **multiagente**, que permite dividir as tarefas entre agentes especializados (coleta, análise e relatório).  
O objetivo é analisar dados de um **setor específico fornecido**, identificando padrões, tendências e oportunidades de mercado.

---

## 📊 Por que usar Multiagentes no Crew AI?

No Crew AI, podemos optar por usar **um único agente** ou **vários agentes especializados**.  
A abordagem **multiagente** apresenta diversas vantagens em relação a um único agente:

### 1️⃣ Especialização
Cada agente pode ser configurado para uma **função específica**, por exemplo:

- **Agente A:** Coleta dados de concorrentes  
- **Agente B:** Analisa tendências de preços  
- **Agente C:** Gera gráficos e relatórios  

Com um único agente, ele precisaria conhecer tudo, o que aumenta a complexidade e o risco de erros.

---

### 2️⃣ Paralelismo
- Múltiplos agentes podem executar tarefas **simultaneamente**.  
  - Exemplo: enquanto o Agente A coleta dados, o Agente B já pode analisar dados antigos.  
- Um único agente faz tudo **em sequência**, tornando o processo mais lento.

---

### 3️⃣ Modularidade e Manutenção
- A abordagem multiagente permite **substituir ou atualizar um agente sem afetar os outros**.  
- Um agente centralizado é mais difícil de ajustar e testar.

---

### 4️⃣ Robustez e Resiliência
- Se um agente falhar, os outros podem continuar trabalhando ou assumir parcialmente a tarefa.  
- Com um único agente, qualquer falha interrompe todo o fluxo.

---

### 5️⃣ Colaboração e Raciocínio Combinado
- Agentes podem **trocar informações e insights entre si**, aumentando a qualidade da análise.  
  - Exemplo: o Agente A detecta um padrão de mercado e envia para o Agente B, que avalia sua relevância.  
- Isso simula **trabalho em equipe humano**, com inteligência coletiva.

---

### ✅ Resumo
| Abordagem | Vantagens | Desvantagens |
|------------|------------|---------------|
| **Um só agente** | Simples, rápido de configurar | Mais lento, menos robusto, difícil de manter |
| **Multiagente** | Especializado, modular, rápido, confiável | Requer mais configuração inicial |

---

## ⚙️ Instalação e Execução no VS Code

### 1️⃣ Pré-requisitos

Antes de começar, você precisa ter instalado:

- [Python 3.10+](https://www.python.org/downloads/)
- [Visual Studio Code](https://code.visualstudio.com/)
- Extensão **Python** no VS Code
- **Git** (opcional, mas recomendado)

---

### 2️⃣ Clonar o repositório

Abra o terminal e execute:
```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```

---

### 3️⃣ Criar e ativar o ambiente virtual

No terminal do VS Code, execute:
```bash
python -m venv .venv
```

Depois, ative o ambiente virtual conforme seu sistema operacional:

#### 👉 PowerShell (Windows)
```powershell
.\.venv\Scripts\Activate.ps1
```

Se aparecer erro de permissão, execute:
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

#### 👉 CMD (Prompt de Comando)
```cmd
.venv\Scripts\activate.bat
```

#### 👉 Linux ou macOS
```bash
source .venv/bin/activate
```

---

### 4️⃣ Instalar dependências

Com o ambiente virtual ativo, execute:
```bash
pip install -r requirements.txt
```

---