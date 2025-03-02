# Previsão do Tempo - Atualização Automática

Este projeto busca informações de previsão do tempo, como temperatura e umidade, de uma cidade específica (São Paulo) e salva esses dados em uma planilha Excel. A interface gráfica é construída usando o `Tkinter` e os dados são extraídos automaticamente do site [Climatempo](https://www.climatempo.com.br/) com a ajuda da biblioteca `Selenium`.

## Funcionalidades

- **Interface Gráfica (GUI):** Utiliza `Tkinter` para criar uma interface simples e interativa.
- **Busca de Dados:** O script acessa o site Climatempo, usando o Selenium WebDriver, para obter as informações de temperatura e umidade de São Paulo.
- **Armazenamento de Dados:** As informações coletadas são salvas em uma planilha Excel, utilizando a biblioteca `openpyxl`.
- **Atualização de Planilha:** Cada vez que o script é executado, a planilha é atualizada com a data/hora da consulta, a temperatura e a umidade.

## Como Usar

### Pré-requisitos

- Python 3.x instalado.
- As bibliotecas `selenium`, `openpyxl`, e `tkinter` instaladas.

### Passos para Execução

1. Instale as dependências:
    ```bash
    pip install selenium openpyxl tk
    ```

2. Tenha o navegador Chrome instalado no computador ou qualquer um de sua preferência mas certifique-se de trocar na linha 14 do arquivo clima.py o webdriver.seunavegadoraqui()

3. Clone este repositório:
    ```bash
    git clone https://github.com/vinyciosnavarro07/Atualizador-de-planilha-climatica.git
    ```

4. Navegue até o diretório do projeto:
    ```bash
    cd seu-repositorio
    ```

5. Execute o script:
    ```bash
    python previsao_tempo.py
    ```

6. Na interface gráfica que será aberta, clique no botão **"Buscar Previsão"** para atualizar a previsão do tempo e salvar os dados na planilha `temperatura.xlsx`.

## Tecnologias Utilizadas

- **Tkinter**: Para a criação da interface gráfica.
- **Selenium**: Para automação de navegação no site Climatempo e extração de dados.
- **openpyxl**: Para manipulação de planilhas Excel.
- **datetime**: Para registrar a data e hora da consulta.

## Créditos

A previsão do tempo é obtida a partir do site [Climatempo](https://www.climatempo.com.br/), que fornece informações meteorológicas de diversas cidades no Brasil.
