# 🤖 Cadastro de Produtos com Python

> 📦 **Leia os dados de um CSV e automatize o preenchimento de um formulário no navegador.**

Projeto de automação de interface que combina PyAutoGUI e pandas para inserir registros de produtos.

## ✨ Funcionalidades

- 📄 Carrega os registros de `produtos.csv` com pandas.
- 🌐 Abre o Chrome e navega até o formulário configurado no script.
- ⌨️ Preenche os campos do formulário com os dados de cada produto.

## 🧰 Requisitos

- Windows e Google Chrome
- Python 3
- Bibliotecas PyAutoGUI e pandas

Instale as dependências:

```bash
python -m pip install pyautogui pandas
```

## ▶️ Como executar

Na pasta do projeto, confira os dados e as configurações do formulário e rode:

```bash
python bagui.py
```

O CSV precisa estar na mesma pasta e conter as colunas esperadas pelo script: `codigo`, `marca`, `tipo`, `categoria`, `preco_unitario`, `custo` e `obs`.

## ⚠️ Antes de executar

- O script interage com a tela usando coordenadas fixas. A resolução, o zoom e o layout da página podem afetar os cliques.
- Revise o endereço e o fluxo de login configurados no código.
- Substitua os dados de demonstração por um método seguro. Não armazene nem publique senhas reais no código ou no CSV.
- Teste com poucos registros e em um ambiente apropriado antes de processar uma lista completa.

## 📁 Arquivos

- `bagui.py` — automação do navegador e preenchimento.
- `produtos.csv` — dados de entrada para o cadastro.

## 📄 Licença

Nenhuma licença foi definida até o momento.
