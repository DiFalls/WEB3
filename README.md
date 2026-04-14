# 🍕 Pizzeria del Gatito — Web 3.0

![Unity](https://img.shields.io/badge/Unity-2021%2B-black?logo=unity&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?logo=c-sharp&logoColor=white)
![Meta XR](https://img.shields.io/badge/Meta%20XR-Simulator-blue?logo=meta&logoColor=white)
![Status](https://img.shields.io/badge/Status-Em%20desenvolvimento-yellow)

Experiência 3D interativa estilo metaverso, inspirada no mini-game **Pizzatron 3000** do Club Penguin. Um ambiente virtual construído em Unity que une nostalgia e tecnologia.

> "Minha aspiração é criar uma visualização 3D inspirada em um jogo da minha infância." — Pedro V. (@DiFalls)

---

## ✨ Sobre o projeto

O objetivo é recriar a experiência da pizzaria em um **ambiente tridimensional**, explorando interação com objetos, scripts e mecânicas simples de jogo. A proposta explora conceitos de metaverso e ambientes virtuais com uma estética familiar e nostálgica.

| Motor gráfico | Linguagem | Plataforma alvo | Inspiração |
|---|---|---|---|
| Unity 2021+ | C# | VR (Meta XR) | Pizzatron 3000 |

---

## 🚀 Como executar

**1. Clone o repositório**
```bash
git clone https://github.com/Difalls/WEB3
```

**2. Abra o projeto na Unity 2021 ou superior**

**3. Abra o arquivo de solução**
```
WEB 3.0 (Pizzeria del Gatito).sln
```

**4. Explore o ambiente**
Carregue a cena principal e explore os assets na pasta `Assets/`.

---

## 📂 Estrutura do projeto

Os principais assets estão organizados em `Materials/`:

| Pasta | Conteúdo |
|---|---|
| `Materials/Cenario/` | Texturas e materiais do ambiente |
| `Materials/Objetos/Esteira` | Modelos e materiais da esteira |
| `Materials/Objetos/Pizzas` | Massa e estrutura das pizzas |
| `Materials/Objetos/QuadrosDeInspiracoes` | Referências visuais do projeto |
| `Materials/Objetos/Relogio` | Modelo do relógio do ambiente |

**Formatos utilizados:** `.mat` · `.png / .jpg` · `.fbx`

---

## 🧩 Desafios técnicos

### Animação da esteira
O Animator da Unity não era adequado para deslocar texturas — ele lida bem com transformações de posição, rotação e escala, mas não com offset de material. A solução foi um script em C# que altera o **offset da textura ao longo do tempo**, simulando o movimento contínuo da linha de montagem.

### Botão interativo
O método de ativação não aparecia no sistema de eventos da Unity por não ser público. A solução foi expor o método `Interagir()` no script, conectando-o ao Inspector. Ao pressionar o botão:
- O botão executa animação de pressionamento
- A esteira é acionada
- O ambiente responde à interação do usuário

### Meta XR Simulator
Conflitos entre plugins VR impediram o carregamento correto do simulador em algumas tentativas. Mesmo após ajustes, alguns warnings da Unity permaneceram, indicando possíveis conflitos de configuração. Ainda assim, foi possível realizar testes básicos dentro do ambiente virtual.

### Importação de modelos FBX
Alguns arquivos já traziam materiais configurados internamente, aplicando texturas automaticamente na importação. Recriar manualmente o mapeamento de texturas exigiu atenção ao pipeline de modelagem 3D, pois algumas configurações estão definidas diretamente no software de origem.

---

## 📌 Status do projeto

| | Funcionalidade |
|---|---|
| ✅ | Estrutura inicial do ambiente 3D |
| ✅ | Organização de materiais e modelos |
| ✅ | Implementação da esteira com script de offset |
| ✅ | Botão interativo ligando a esteira |
| 🔄 | Mecânicas de interação em desenvolvimento |
| 🎯 | Movimento das pizzas na esteira |
| 🎯 | Loop de produção contínua de pizzas |
| 🎯 | Ingredientes e montagem interativa |
| 🎯 | Ajustes de escala para VR |

---

## 👤 Autor

**Pedro Victor** · [@DiFalls](https://github.com/DiFalls)

🔗 [github.com/DiFalls/WEB3](https://github.com/DiFalls/WEB3)
