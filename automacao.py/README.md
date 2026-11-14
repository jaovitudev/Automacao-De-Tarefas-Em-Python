# 🤖 Python Task Automation

> 📦 **Automatize o cadastro de produtos a partir de um arquivo CSV.**

Este projeto reduz o trabalho repetitivo de copiar dados de produtos manualmente para um formulário web. O script lê uma linha por produto e preenche os campos correspondentes no navegador.

## ⚙️ Como funciona

1. 🐼 Carrega `produtos.csv` com pandas.
2. 🌐 Abre o Chrome e acessa o formulário configurado.
3. 🔐 Executa o fluxo de login definido no script.
4. 🔁 Preenche código, marca, tipo, categoria, preço, custo e observação para cada registro.
5. ✅ Envia cada cadastro e passa ao próximo produto.

## 🧰 Requisitos

- Windows e Google Chrome
- Python 3
- PyAutoGUI e pandas

```bash
python -m pip install pyautogui pandas
```

## ▶️ Como executar

Mantenha `produtos.csv` junto ao script e execute:

```bash
python automacao.py
```

O CSV deve conter as colunas `codigo`, `marca`, `tipo`, `categoria`, `preco_unitario`, `custo` e `obs`.

## ⚠️ Antes de executar

- O script usa coordenadas fixas da tela; resolução, zoom ou mudanças no formulário podem afetar os cliques.
- Confira o endereço e o fluxo de login antes de iniciar.
- Não salve nem publique senhas reais no código ou no CSV. Use credenciais de teste e um método seguro para autenticação.
- Faça um teste com poucos registros antes de processar uma lista completa.

## 📄 Licença

Nenhuma licença foi definida até o momento.
