Este projeto simula a criação e gerenciamento de um banco de dados relacional para uma escola. Ele abrange entidades como alunos, professores, disciplinas, turmas e notas. É ideal para fins educacionais e práticas com SQL.

## 📦 Estrutura do Projeto

| Tabela              | Descrição                                                                 |
|---------------------|--------------------------------------------------------------------------|
| `alunos`            | Armazena os dados pessoais dos estudantes                               |
| `professores`       | Dados sobre os professores da escola                                     |
| `disciplinas`       | Disciplinas ofertadas e seus professores responsáveis                    |
| `turmas`            | Turmas formadas em um determinado ano letivo                             |
| `turma_disciplina`  | Associa disciplinas às turmas                                            |
| `turma_alunos`      | Associa alunos às turmas em que estão matriculados                      |
| `notas`             | Registro de notas dos alunos nas disciplinas                             |

## 🛠️ Funcionalidades

- Criação de tabelas com chaves primárias e estrangeiras
- Inserção de dados simulados em massa
- Relacionamentos N:N entre turmas x disciplinas e turmas x alunos
- Registro de notas por aluno e disciplina
- Consultas simples para verificação de dados

## 📊 Exemplos de Consultas

```sql
-- Verificar alunos ordenados por nome
SELECT * FROM alunos ORDER BY nome_aluno;

-- Disciplinas com mais de 40h de carga horária
SELECT * FROM disciplinas WHERE carga_horaria > 40;

-- Notas entre 6 e 8
SELECT * FROM notas WHERE valor_nota > 6 AND valor_nota < 8;
