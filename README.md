# NomesIBGE 🇧🇷

---

Este repositório contém um web app simples desenvolvido em Python utilizando **Streamlit** que permite consultar a frequência de nomes registrados no Brasil por década, utilizando a API de Nomes do IBGE.

## Funcionalidades

* **Consulta de Nomes:** Insira um nome e veja a quantidade de vezes que ele foi registrado em diferentes décadas.
* **Dados Detalhados:** Visualize a frequência dos nomes em uma tabela.
* **Gráfico de Evolução:** Observe a evolução da popularidade do nome ao longo do tempo através de um gráfico de linha interativo.
* **Fonte de Dados Confiável:** Todos os dados são obtidos diretamente da API oficial de Nomes do IBGE.

## Como Usar

### Pré-requisitos

Certifique-se de ter o Python 3.7 ou superior instalado em sua máquina.

### Instalação

1.  Clone este repositório:
    ```bash
    git clone https://github.com/zeer0e1/nome_ibge_curso_azimov.git
    ```
2.  Navegue até o diretório do projeto:
    ```bash
    cd nomes-ibge
    ```
3.  Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```
    (Se o arquivo `requirements.txt` não existir, crie-o com o seguinte conteúdo:)
    ```
    pandas
    requests
    streamlit
    ```

### Executando o Web App

1.  Execute o script principal:
    ```bash
    streamlit run seu_script.py
    ```
    (Substitua `seu_script.py` pelo nome do seu arquivo Python, por exemplo, `main.py` ou `app.py`).
2.  O web app será aberto automaticamente em seu navegador padrão. Se não abrir, copie o URL fornecido no terminal (geralmente `http://localhost:8501`) e cole-o no navegador.

---

## Estrutura do Código

* `fazer_request(url, params=None)`: Função auxiliar para realizar requisições HTTP à API do IBGE, incluindo tratamento de erros.
* `pegar_nome_por_decada(nome)`: Função que consome a API do IBGE para obter a frequência de um dado nome por década e retorna os dados em um dicionário.
* `main()`: Função principal do aplicativo Streamlit, responsável por criar a interface do usuário, chamar as funções de consulta e exibir os resultados.

---

## Fonte dos Dados

Os dados utilizados neste projeto são provenientes da API de Nomes do IBGE. Você pode encontrar mais informações sobre a API na documentação oficial: [https://servicodados.ibge.gov.br/api/docs/nomes?versao=2](https://servicodados.ibge.gov.br/api/docs/nomes?versao=2)

---

## Contribuição

Contribuições são bem-vindas! Se você tiver alguma sugestão, melhoria ou encontrar algum bug, sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.

---

## Licença

Este projeto está licenciado sob a [MIT License](https://opensource.org/licenses/MIT).