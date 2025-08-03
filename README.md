# 🧠 NAXUS AI – AimAssist por IA para FPS modernos (CS2, Valorant, Apex)

> AimAssist avançado com inteligência artificial baseado em YOLOv11-seg, usando ONNX Runtime e inferência de alta performance.  
> Detecta inimigos em tempo real, ajusta a mira de forma natural e modular para múltiplos jogos.

---

## 🚀 Recursos

- 🎯 Detecção por segmentação com **YOLOv11m/l-seg.onnx**
- 🧠 Processamento local com **ONNX Runtime (CUDA, DirectML ou CPU)**
- 🎮 Suporte a múltiplos jogos: CS2, Valorant, Apex, Fortnite, etc.
- 📸 Captura otimizada via DXGI ou GDI
- 🎯 Mira com FOV, suavização (smooth), prioridade e delay configuráveis
- ⚙️ Interface WPF leve e moderna
- 🔒 Totalmente offline – privacidade garantida
- 🧩 Estrutura modular para fácil personalização

---

## 🖥️ Requisitos

- ✅ Windows 10 ou 11 x64
- ✅ .NET 8.0 SDK (https://dotnet.microsoft.com)
- ✅ Visual Studio 2022+
- ✅ GPU com suporte a DirectML ou CUDA (opcional)
- ✅ Drivers de GPU atualizados

---

## 📁 Estrutura do Projeto

NEXUS-AI/
├── Models/
│ ├── cs2/
│ │ └── yolov11m-seg_cs2.onnx
│ ├── valorant/
│ │ └── yolov11l-seg_val.onnx
│ └── ...
├── Configs/
│ ├── cs2_config.json
│ └── valorant_config.json
├── Core/
│ ├── AIManager.cs
│ ├── MouseControl.cs
│ └── CaptureManager.cs
├── UI/
│ └── MainWindow.xaml
├── Assets/
│ └── Logo, ícones e imagens
├── NexusAI.csproj
├── NexusAI.sln
└── README.md

yaml
Copiar
Editar

---

## 🎯 Como usar

1. **Clone o repositório:**
```bash
git clone https://github.com/NexusAI-BR/NEXUS-AI.git
Abra no Visual Studio:

Abra NexusAI.sln

Compile em Release x64

Execute o programa:

O app carregará a interface do NAXUS AI

Escolha o jogo, configure sua mira e pressione Iniciar

⚙️ Configurações
As configurações são específicas por jogo e ficam na pasta /Configs. Exemplo (cs2_config.json):

json
Copiar
Editar
{
  "fov": 3.0,
  "smooth": 28,
  "delay": 15,
  "priority": "nearest",
  "target": "head",
  "switch_target": true,
  "aim_key": "F4"
}
Você pode customizar cada jogo separadamente.

📦 Modelos ONNX
Modelos treinados ou convertidos para YOLOv11-seg devem ficar na pasta /Models/[jogo]/.

Nome sugerido: yolov11m-seg_cs2.onnx

Suporte a quantização (FP16, INT8) para mais desempenho

Pode ser treinado com Ultralytics YOLOv11

🧠 Créditos
Desenvolvido por Rodrigo Jaca com foco em precisão, privacidade e inteligência artificial aplicada a jogos FPS.
Projeto 100% voltado para aprendizado, pesquisa e uso pessoal.

📜 Licença
Distribuído sob a licença MIT.
Você é livre para estudar, modificar e usar o projeto, respeitando os termos.

🧠 “O futuro da mira inteligente é real. Bem-vindo ao NAXUS AI.”