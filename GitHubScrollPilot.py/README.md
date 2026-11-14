# 🧭 GitHub Scroll Pilot

> 🚀 **Automatize a abertura e a navegação de um perfil do GitHub com Python.**

Este mini projeto usa PyAutoGUI para abrir o Chrome, acessar o perfil configurado e rolar a página.

## ✨ Funcionalidades

- 🪟 Abre o menu Iniciar do Windows.
- 🌐 Inicia o Chrome e acessa `github.com/jaovitudev/`.
- 🖥️ Coloca o navegador em tela cheia.
- 🖱️ Posiciona o cursor e percorre a página com rolagens.

## 🧰 Requisitos

- Windows com Google Chrome instalado
- Python 3
- PyAutoGUI

```bash
python -m pip install pyautogui
```

## ▶️ Como executar

```bash
python GitHubScrollPilot.py
```

O script controla teclado e mouse durante a execução. Para interromper, mova rapidamente o cursor para um canto da tela, acionando o mecanismo de segurança do PyAutoGUI.

## ⚙️ Personalização

Altere no arquivo `GitHubScrollPilot.py` o endereço, os tempos de espera e os valores de rolagem.

## 📄 Licença

Nenhuma licença foi definida até o momento.
