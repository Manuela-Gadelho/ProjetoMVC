
# 🎓 Sistema de Gestão Acadêmica - Arquitetura MVC

Este projeto é uma aplicação desktop acadêmica desenvolvida em **Java**, com interface gráfica baseada em **Swing** e persistência de dados usando **MySQL**. A estrutura segue os princípios da arquitetura **MVC (Model-View-Controller)** para garantir organização, clareza e facilidade de manutenção.

## 📌 Objetivo

O sistema tem como foco o gerenciamento completo de dados acadêmicos, incluindo:
- Cadastro e manutenção de alunos;
- Associação de cursos por campus e período;
- Registro de desempenho escolar (notas e faltas);
- Consulta e emissão de boletins organizados e claros.

## ⚙️ Funcionalidades Principais

- Criar, visualizar, atualizar e remover registros de alunos;
- Relacionar alunos com seus respectivos cursos;
- Lançar notas e controlar frequência por disciplina e semestre;
- Gerar boletins escolares;
- Validar entradas e evitar duplicidade de dados;
- Interface gráfica amigável com menus intuitivos:
  - Menu Aluno
  - Menu Notas e Faltas
  - Menu Ajuda

## 🧱 Estrutura MVC

- **Modelo (Model):**  
  Contém as classes `Aluno`, `Curso`, `Disciplina` e `Desempenho`, que representam diretamente as tabelas do banco de dados.

- **Visão (View):**  
  Conjunto de telas criadas com Swing, organizadas por abas e menus, proporcionando uma navegação acessível e organizada ao usuário.

- **Controle (Controller):**  
  Classes DAO como `AlunoDAO` e `DesempenhoDAO` fazem a ponte entre a interface e o banco de dados, centralizando as regras de acesso e persistência.

## 🔌 Conexão com Banco de Dados

Para gerenciamento de conexões, o projeto utiliza a classe `ConnectionFactory`, que:

- Cria e configura a conexão com o banco de dados MySQL;
- Encapsula informações como URL, usuário e senha;
- Fecha conexões e libera recursos após o uso;
- Facilita reutilização de código e segurança.

Essa abordagem garante maior modularidade e facilidade de manutenção no código.

## ▶️ Como Executar

### Requisitos

- Java 17 ou superior
- IDE Java (preferencialmente Eclipse)

### Passos

1. Clone este repositório:
   ```bash
   git clone https://github.com/ManuelaExemplo/Projeto-MVC.git
   ```
2. Importe o projeto na sua IDE.
3. Compile e execute a classe `Tela.java`.

## 🖼️ Capturas de Tela

| Funcionalidade        | Exemplo de Tela             |
|-----------------------|-----------------------------|
| Dados do Aluno        | ![Dados Pessoais](caminho)  |
| Informações do Curso  | ![Curso](caminho)           |
| Notas e Faltas        | ![Notas](caminho)           |
| Boletim Escolar       | ![Boletim](caminho)         |
| Menu Aluno            | ![Menu Aluno](caminho)      |
| Menu Notas e Faltas   | ![Menu Notas](caminho)      |
| Menu Ajuda            | ![Ajuda](caminho)           |

*(Substitua `caminho` pelos links ou caminhos corretos das imagens caso deseje incluir)*
