
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
| Dados do Aluno        | ![Dados Pessoais](![{9FDA83C6-9308-452A-A167-2706807B89D1}](https://github.com/user-attachments/assets/6f5b795c-c0b7-4385-9651-be9b91bbe52e)
)  |
| Informações do Curso  | ![Curso](![{EE5286D9-B124-4511-9D25-8706F057EE02}](https://github.com/user-attachments/assets/3f4ddb23-9a16-4bdd-8f34-e4c58520834f)
)           |
| Notas e Faltas        | ![Notas](![{F6FF91FD-6DF3-4490-8056-FC26020291F9}](https://github.com/user-attachments/assets/e20a5be5-f54f-4b8d-949e-52b86678f476)
)           |
| Boletim Escolar       | ![Boletim](![{5182953C-CA1F-47FD-BEE3-6BF3D1EF5BF0}](https://github.com/user-attachments/assets/31b36493-72cb-4c87-85db-12266e9b4d89)
)         |
| Menu Aluno            | ![Menu Aluno](![image](https://github.com/user-attachments/assets/db4db690-3abb-4df2-8b70-b1ee0aa1cd2e)
)      |
| Menu Notas e Faltas   | ![Menu Notas](![{994E2965-0CF7-492B-9529-A8591A17FA60}](https://github.com/user-attachments/assets/83a765f0-7b08-4f30-b508-671326842d2a)
)      |
| Menu Ajuda            | ![Ajuda](![{BB2EA1C8-FE29-4DB1-A2CB-03415D141E92}](https://github.com/user-attachments/assets/eade8fce-902a-4217-9972-b1eb1e90e1bf)
)           |

