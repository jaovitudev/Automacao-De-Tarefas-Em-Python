#  Automação de Tarefas em Python

> **Menos tarefas repetitivas. Mais Python em ação.**
>
> Repositório de mini projetos que automatizam tarefas no computador com Python e PyAutoGUI — do preenchimento de formulários à navegação no navegador.

##  Projetos

###  Cadastro de Produtos
Lê os produtos de um arquivo CSV e preenche automaticamente um formulário no navegador. O projeto usa pandas para processar os dados e PyAutoGUI para controlar a interface.

 Pasta: `automacao.py/`

###  GitHub Scroll Pilot
Abre o Google Chrome, acessa o perfil do GitHub configurado e percorre a página com rolagens automatizadas.

 Pasta: `GitHubScrollPilot.py/`

##  Tecnologias

- Python 3
- PyAutoGUI — controle de mouse e teclado
- pandas — leitura dos dados CSV
- CSV — lista de produtos

## Instalação

Instale as dependências usadas pelos projetos:

```bash
python -m pip install pyautogui pandas
```

O cadastro de produtos requer Windows e Google Chrome. O GitHub Scroll Pilot também foi configurado para abrir o Chrome no Windows.

## Como executar

Execute cada automação a partir da raiz do repositório:

```bash
python automacao.py/bagui.py
```

```bash
python GitHubScrollPilot.py/main.py
```

Antes de iniciar o cadastro, confira o arquivo `automacao.py/produtos.csv` e os campos esperados pelo formulário.

## Como funciona o cadastro

1. O pandas carrega os produtos do CSV.
2. O PyAutoGUI abre o navegador e acessa o formulário configurado no código.
3. O script preenche os dados de cada produto e envia o formulário.
4. O processo se repete para as linhas restantes do arquivo.

## Cuidados importantes

- As automações controlam mouse e teclado. Evite usar o computador enquanto elas estiverem rodando.
- O cadastro usa coordenadas fixas da tela; alterações de resolução, zoom ou layout podem afetar os cliques.
- Revise o endereço e o fluxo de login antes de executar.
- Não publique senhas ou chaves reais no código. Use credenciais de teste e mantenha informações de acesso protegidas.
- Faça um teste com poucos registros antes de processar uma lista maior.

## Estrutura

```text
.
├── automacao.py/
│   ├── bagui.py
│   └── produtos.csv
├── GitHubScrollPilot.py/
│   └── main.py
└── README.md
```

## 👨‍💻 Autor

Criado por [jaovitudev](https://github.com/jaovitudev).

## Licença

Nenhuma licença foi definida para este repositório.
