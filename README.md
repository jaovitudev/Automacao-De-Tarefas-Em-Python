# 🤖 Cadastro de Produtos com Python

> 📦 **Transforme uma planilha CSV em cadastros preenchidos automaticamente no navegador.**

Este projeto automatiza o preenchimento de um formulário de produtos. Ele ajuda a reduzir o trabalho repetitivo de copiar os dados de cada item manualmente, usando um arquivo CSV como fonte.

## 🎯 Problema que resolve

Cadastrar muitos produtos um por um pode consumir tempo e aumentar a chance de erros de digitação. A automação lê os registros de `produtos.csv` e preenche os campos correspondentes no formulário do navegador, repetindo o processo para cada linha.

## ⚙️ Como funciona

1. 📄 O pandas abre `produtos.csv` e carrega os dados em uma tabela.
2. 🌐 O PyAutoGUI abre o Chrome e acessa o endereço do formulário configurado no script.
3. 🔐 O script realiza o fluxo de login configurado.
4. 🔁 Para cada linha do CSV, seleciona os campos e digita código, marca, tipo, categoria, preço, custo e observação.
5. ✅ Envia o formulário e segue para o próximo produto.

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

O arquivo CSV precisa estar na mesma pasta e conter as colunas esperadas pelo script: `codigo`, `marca`, `tipo`, `categoria`, `preco_unitario`, `custo` e `obs`.

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
