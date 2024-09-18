# Sistema de Gestão das Olimpíadas

## Descrição do Sistema
Com a chegada das Olimpíadas, um novo sistema de gestão é necessário para coordenar os diferentes aspectos do evento. Este sistema deve permitir o gerenciamento de competições, inscrições de atletas, alocação de locais para as provas e controle de resultados.

- Vinícius Salles de Oliveira
- David Dias

## Regras de Negócio

### 1. Cadastro de Competições
- O sistema deve permitir o cadastro de competições, que incluem:
  - Nome da modalidade
  - Data
  - Horário
  - Local
  - Lista de atletas inscritos

### 2. Inscrição de Atletas
- Atletas de diferentes países devem se inscrever em competições específicas.
- Cada atleta pode participar de várias competições, mas só pode representar um país em cada modalidade.

### 3. Alocação de Locais
- Os locais para as competições devem ser alocados de forma a evitar conflitos de horário.
- Um local só pode abrigar uma competição por vez.

### 4. Controle de Resultados
- Após a realização das competições, os resultados devem ser registrados, determinando:
  - O atleta vencedor
  - Os classificados em segundo e terceiro lugares

### 5. Relatórios de Medalhas
- O sistema deve gerar relatórios de medalhas, mostrando o desempenho de cada país com base nas medalhas de:
  - Ouro
  - Prata
  - Bronze conquistadas

---

# Histórias de Usuário

## US01: Cadastro de Competições

**Como** administrador,  
**Quero** cadastrar novas competições,  
**Para que** eu possa gerenciar as competições com todas as informações necessárias.

### Critérios de Aceitação:
- Deve ser possível inserir o nome da modalidade.
- Deve ser possível selecionar a data e o horário da competição.
- Deve ser possível escolher o local onde a competição ocorrerá.
- Deve ser possível cadastrar uma lista de atletas para a competição.
- O sistema deve validar se todos os campos obrigatórios foram preenchidos corretamente.


## US02: Inscrição de Atletas

**Como** atleta,  
**Quero** me inscrever em competições específicas,  
**Para que** eu possa participar das Olimpíadas representando meu país.

### Critérios de Aceitação:
- O sistema deve permitir que o atleta escolha a competição na qual deseja se inscrever.
- O atleta só pode se inscrever em competições em que ainda haja vagas.
- O sistema deve garantir que o atleta represente apenas um país por modalidade.
- Deve haver uma confirmação de inscrição com os detalhes da competição e o país representado.


## US03: Alocação de Locais

**Como** administrador,  
**Quero** alocar locais para cada competição,  
**Para que** eu possa garantir que não haverá conflitos de horários entre as competições.

### Critérios de Aceitação:
- O sistema deve permitir selecionar locais disponíveis para cada competição.
- O sistema deve impedir que dois eventos sejam agendados no mesmo local e horário.
- Deve exibir uma lista de locais disponíveis e seus horários.


## US04: Controle de Resultados

**Como** administrador,  
**Quero** registrar os resultados das competições,  
**Para que** eu possa determinar os vencedores e classificados.

### Critérios de Aceitação:
- O sistema deve permitir a entrada dos resultados após o término da competição.
- Deve haver campos para registrar o atleta vencedor e os classificados em segundo e terceiro lugares.
- O sistema deve associar os resultados registrados à competição e aos atletas participantes.


## US05: Geração de Relatórios de Medalhas

**Como** administrador,  
**Quero** gerar relatórios de medalhas,  
**Para que** eu possa visualizar o desempenho de cada país com base nas medalhas conquistadas.

### Critérios de Aceitação:
- O sistema deve gerar um relatório que mostre a quantidade de medalhas de ouro, prata e bronze conquistadas por cada país.
- O relatório deve ser atualizado automaticamente conforme os resultados são registrados.
- O relatório deve permitir exportação em formato PDF ou CSV.

