# 🍕 Pizzeria del Gatito – Web 3.0

Projeto experimental de **visualização 3D interativa** inspirado no mini-game **Pizzatron 3000**, do Club Penguin.

O objetivo do projeto é recriar a experiência de uma pizzaria dentro de um **ambiente tridimensional estilo metaverso**, explorando interação com objetos, scripts e mecânicas simples de jogo utilizando a **Unity**.

A proposta une **nostalgia + tecnologia**, transformando um ambiente clássico da infância em uma experiência interativa em 3D.

---

# ✨ Objetivo

- 🎮 Criar uma experiência 3D inspirada no mini-game **Pizzatron 3000**
- 🌐 Explorar conceitos iniciais de **metaverso e ambientes virtuais**
- 🛠️ Utilizar a **Unity** como motor gráfico
- 🧩 Desenvolver **mecânicas básicas de interação**

---

# 📂 Estrutura do Projeto

O projeto está organizado em pastas que representam os principais elementos do ambiente, como por exemplo:

### 🏠 `Materials/Cenario/`
Materiais e texturas do ambiente da pizzaria.

### ⚙️ `Materials/Objetos/Esteira`
Modelos e materiais da esteira de produção de pizzas.

### 🍕 `Materials/Objetos/Pizzas`
Materiais relacionados à massa e estrutura das pizzas.

### 🖼️ `Materials/Objetos/QuadrosDeInspiracoes`
Referências visuais utilizadas no desenvolvimento.

### ⏰ `Materials/Objetos/Relogio`
Modelo e materiais do relógio presente no ambiente.

Arquivos utilizados no projeto:
- `.mat` → materiais da Unity  
- `.png / .jpg` → texturas  
- `.fbx` → modelos 3D  

---

# 🚀 Como Executar

### 1️⃣ Clonar o repositório
```bash
git clone https://github.com/Difalls/WEB3
```

### 2️⃣ Abrir o projeto na Unity
**Versão recomendada:** Unity 2021 ou superior

### 3️⃣ Abrir o arquivo de solução
Abra o arquivo: `WEB 3.0 (Pizzeria del Gatito).sln`

### 4️⃣ Explorar o ambiente
Abra a **cena principal** e explore os assets presentes na pasta: `Assets`

---

# 🐧 Inspiração

Este projeto é inspirado no mini-game **Pizzatron 3000**, presente no **Club Penguin**.
A proposta é recriar essa experiência em um ambiente tridimensional, explorando conceitos modernos como:
- ambientes virtuais  
- interação em 3D  
- metaverso  

---

# 📌 Status do Projeto

| Status | Descrição |
|------|------|
| ✅ | Estrutura inicial do ambiente 3D |
| ✅ | Organização de materiais e modelos |
| ✅ | Implementação inicial da esteira |
| 🔄 | Mecânicas de interação em desenvolvimento |
| 🎯 | Futuro: expansão do ambiente |

---

# ⚙️ Evolução e Dificuldades de Desenvolvimento
Durante o desenvolvimento surgiram algumas dificuldades técnicas relacionadas à **manipulação de texturas, scripts e integração com VR**.

---

## 🧩 Animação da esteira
Inicialmente foi tentado utilizar o **Animator da Unity** para criar o movimento da esteira.
No entanto, o Animator é mais adequado para animar **transformações de objetos**, como:

- posição  
- rotação  
- escala  

Para resolver isso foi criado um **script em C#** que altera o **offset da textura ao longo do tempo**, simulando o movimento contínuo da esteira.
Essa abordagem permitiu criar a sensação de **linha de montagem em funcionamento**.

---

## 🕶️ Execução no Meta XR Simulator
Outra dificuldade foi executar o projeto utilizando o **Meta XR Simulator** para testes em realidade virtual.
Durante a configuração surgiram **conflitos entre plugins VR**, impedindo que o simulador carregasse corretamente em algumas tentativas.
Mesmo após ajustes, alguns **warnings da Unity permaneceram**, indicando possíveis conflitos de configuração.
Apesar disso, foi possível realizar **testes básicos dentro do ambiente virtual**.

---

## 🧱 Importação de modelos 3D
Também surgiram dificuldades ao importar modelos 3D e aplicar texturas corretamente.
Alguns arquivos **FBX já possuíam materiais configurados internamente**, fazendo com que as texturas fossem aplicadas automaticamente ao importar o modelo.
Ao tentar recriar manualmente essas configurações dentro da Unity, percebeu-se que algumas informações de **mapeamento de textura** estão definidas diretamente no software de modelagem 3D.

---

# 🚧 Desafios Avançados
Durante o **módulo avançado do desenvolvimento do metaverso**, foram implementadas novas mecânicas de interação dentro do ambiente.

---

## 🖲️ Sistema de botão interativo
Foi desenvolvido um **botão físico interativo** responsável por ligar a esteira de produção.
Inicialmente o método responsável por ativar o botão **não aparecia no sistema de eventos da Unity**.
Isso ocorreu porque o script não possuía um método público configurado para interação.
A solução foi criar o método:

```csharp
Interagir()
```

Após isso, o método passou a aparecer corretamente no Inspector da Unity, podendo ser conectado ao sistema de eventos.

Quando o botão é ativado:
- Botão executa uma animação de pressionamento
- Esteira é acionada
- Ambiente responde à interação do usuário

Essa implementação marcou o início das mecânicas interativas do ambiente.

---

### 🔮 Etapas Futuras do Projeto
Algumas melhorias estão planejadas para fases mais avançadas.

### 🍕 Movimento da pizza na esteira
Fazer com que as pizzas acompanhem o movimento da esteira.

### ♻️ Loop de produção de pizzas
Criar um sistema de geração contínua de pizzas.

### 🥫 Materiais de confecção das pizzas
Adicionar ingredientes e elementos interativos relacionados à montagem da pizza.

### 📏 Ajustes de altura do ambiente
Possíveis ajustes na escala do ambiente para melhorar a interação em realidade virtual.

---

# 👤 Autor
Pedro V. (@DiFalls)
> "Minha aspiração é criar uma visualização 3D inspirada em um jogo da minha infância."

🔗 Repositório  
https://github.com/DiFalls/WEB3

