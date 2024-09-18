# Sistema de Gestão de Inventário de Veículos

Este é um projeto de gestão de inventário de veículos desenvolvido em TypeScript. O sistema permite adicionar, listar e remover veículos em um estacionamento. Os dados são armazenados no `localStorage` do navegador, e a interface do usuário é manipulada através do DOM.

## Funcionalidades

- **Adicionar Veículo**: Permite adicionar um novo veículo com nome, placa e horário de entrada.
- **Listar Veículos**: Exibe a lista de veículos no estacionamento, com informações sobre o nome, placa e horário de entrada.
- **Remover Veículo**: Remove um veículo da lista e solicita confirmação com o tempo que o veículo permaneceu no estacionamento.

## Tecnologias Utilizadas

- **TypeScript**: Linguagem de programação que adiciona tipagem estática ao JavaScript.
- **HTML**: Estrutura da página.
- **CSS**: Estilização da interface (não incluído neste projeto, mas pode ser adicionado conforme necessário).

## Estrutura do Projeto

- **interface Veiculo**: Define a estrutura dos objetos de veículo.
- **funções principais**:
  - `calcTempo(mil: number)`: Calcula o tempo de permanência do veículo no estacionamento.
  - `patio()`: Função principal que gerencia o armazenamento e a exibição dos veículos.
  - `ler()`: Lê os veículos armazenados no `localStorage`.
  - `salvar(veiculo: Veiculo[])`: Salva a lista de veículos no `localStorage`.
  - `adicionar(veiculo: Veiculo, salva?: boolean)`: Adiciona um veículo à lista e opcionalmente salva no `localStorage`.
  - `remover(placa: string)`: Remove um veículo da lista e solicita confirmação ao usuário.
  - `render()`: Atualiza a interface do usuário com a lista de veículos.

## Instruções de Uso

1. **Clone o Repositório**
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
