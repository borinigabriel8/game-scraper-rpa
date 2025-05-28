# Projeto RPA de Data Scraping - Jogos Nuvem.com

## Descrição

Este projeto é um robô RPA desenvolvido em UiPath para realizar data scraping no site de jogos Nuuvem. O robô:

- Solicita via input dialog o nome do jogo que deseja buscar.
- Abre o site nuvem.com.
- Realiza a busca dos jogos informados.
- Extrai as informações dos jogos encontrados.
- Armazena os dados coletados em uma planilha Excel.
- Também registra os dados em um banco de dados SQLite local.

---

## Funcionalidades principais

- Conexão com banco SQLite para armazenamento de dados.
- Busca dinâmica de jogos baseada no input do usuário.
- Salvamento dos resultados em arquivo Excel para fácil consulta.
- Organização e estruturação dos dados no banco de dados local.

---

## Estrutura do projeto

- `Main.xaml` — fluxo principal do robô.
- Arquivo SQLite (`.sqlite` ou `.db`) usado para persistência dos dados.
- Planilha Excel gerada com os resultados da busca.

---

## Importante: Configuração dos caminhos (Paths)

No arquivo `Main.xaml`, existem variáveis que armazenam os **caminhos absolutos** para:

- O arquivo SQLite (banco de dados local).
- A tabela ou arquivo da planilha Excel onde os dados são salvos.

> **Atenção:** Esses caminhos são específicos para o ambiente onde o projeto foi desenvolvido/testado.  
> Portanto, **ao utilizar o projeto em outro computador**, você deve ajustar esses caminhos para os diretórios correspondentes na máquina local, para evitar erros de execução.

---

## Como configurar os caminhos

1. Abra o `Main.xaml` no UiPath Studio.
2. Localize as variáveis ou argumentos que armazenam os caminhos (ex: `dbFilePath`, `excelFilePath`).
3. Atualize esses valores para os caminhos corretos no seu computador.
4. Salve as alterações e execute o fluxo.

---

## Requisitos

- UiPath Studio instalado.
- Banco de dados SQLite (arquivo `.sqlite` ou `.db`).
- Conexão à internet para acesso ao site nuvem.com.

---

## Como executar

1. Abra o projeto no UiPath Studio.
2. Ajuste os caminhos conforme descrito acima.
3. Execute o fluxo principal `Main.xaml`.
4. Informe o nome do jogo no input dialog.
5. Aguarde o robô realizar a busca e salvar os dados.

---

