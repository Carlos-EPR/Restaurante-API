# Aplicação de Consumo e Filtragem de Dados de uma API

Este projeto consiste em uma aplicação em Python que consome dados de uma API de restaurantes, filtra esses dados com base em critérios especificados pelo usuário e os salva em arquivos JSON.

## Estrutura do Projeto

- `app.py`: Contém o código para consumir os dados da API, filtrar os dados e salvar os resultados em arquivos JSON.
- `main.py`: Configura uma API usando FastAPI para fornecer endpoints para acessar os dados dos restaurantes e cardápios.

## Funcionalidades

### 1. Consumo de Dados da API
   - A aplicação faz uma requisição HTTP GET para a URL da API de restaurantes.
   - Os dados da resposta são processados e convertidos para o formato JSON.

### 2. Filtragem de Dados
   - O usuário pode especificar o nome de um restaurante para visualizar o cardápio daquele restaurante.
   - Os dados são filtrados com base no nome do restaurante fornecido pelo usuário.

### 3. Salvamento em Arquivos JSON
   - Os dados filtrados são salvos em arquivos JSON com o nome do restaurante como identificador.

## Utilização

### Execução da Aplicação
1. Execute o arquivo `main.py` para iniciar o servidor FastAPI.
2. Acesse os endpoints fornecidos pelo FastAPI para consumir os dados da API e filtrá-los conforme necessário.

## Endpoints do FastAPI

- `/api/hello`: Endpoint que exibe uma mensagem incrível do mundo da programação.
- `/api/restaurantes/`: Endpoint para visualizar os cardápios dos restaurantes. Aceita um parâmetro opcional `restaurante` para filtrar os dados por restaurante.

## Pré-requisitos
- Python 3.x instalado no sistema.
- Instalação dos pacotes necessários, como `fastapi` e `requests`.

## Execução
1. Abra um terminal.
2. Navegue até o diretório onde os arquivos do projeto estão localizados.
3. Execute o seguinte comando para iniciar o servidor FastAPI:
   ```
   uvicorn main:app --reload
   ```

## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir um problema ou enviar um pull request para sugerir melhorias ou correções.

## Autores
Carlos Eduardo Peres Rocha

## Licença
Este projeto está licenciado sob a [Licença MIT](https://opensource.org/licenses/MIT).