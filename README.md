# Documentando passo a passo sobre o uso do MySQL

## Login

Para conectar no **MySQL**, tem mais de uma forma, mas o contarei da maneira que o criador do _README_ conseguiu fazer.

Primeiramente, tem que acessar o **Xampp Control Panel**, nele, justamente, terá uma opção para acessar o **MySQL**, ativando-o e clicando 'Start', vai abrir o terminal especifico aos comandos do **MySQL**.
>O espaço escrito 'MySQL', vai ficar verde se devidamente ativo.

Quando estiver devidamente logado, tem que digitar logo em sequencia `mysql -u root` para conectar devidamente.

## Comandos

> [!IMPORTANT]
> Nunca esqueça de usar o ';' para o fim de cada comando
 
### Create database _( nome )_
Cria uma 'base de dados', para servir de principio para o uso dos bancos de dados.

### Show databases
Exibe todos os Bancos de dados para uso.

### Use _( nome do Database )_
Seleciona o _database_ escolhido para haver as modificações ou a inicialização de um novo.

### CREATE TABLE _(NOME)_ ( _Outros comandos_ )
Cria a tabela do _database_ para começar a registrar as informações conforme os comandos definidos, além de integrar itens com valores específicos:
- **INT**: valores numéricos;
- **VARCHAR ( )**: valores escritos, o () representa o limite de caracteres;
- **TEXT**: também registra caracteres mas em maior quantidade;
- **DATE**: Registra datas e horas;
- **BOOLEAN**( _ou TINYINT_ ): Verdadeiro ou falso.
### Desc (_databese_)
Exibir a tabela de informações quando o _database_ já estiver com os códigos de armazenar definidos.

### Insert into ( _database_ )
integrar/inserir um dado conforme as regras/valores estabelecidas para a tabela.

### Select
Seleciona um dado ja existente para consultar, mas precisa ser especificado:
- Select * From ( _tabela_ ): o * consulta todas as colunas;
(EXEMPLO)
```
SELECT * FROM formulas;
```
- Select ( _dado_ ) From ( _tabela_ ): tem que ser escrito com 'Where  (_infromação_ ) = _colocação_' para funcionar justamente para consultar algo especifico.
(EXEMPLO)
```
SELECT info FROM arquivo
WHERE pasta = 1;
```
### Update
Corrigir/Atualizar um dado especifico (WHERE e obrigatorio)
(EXEMPLO)
```
UPDATE alunos
SET responsavel = 'Luna'
WHERE matricula = 4
```

### Delete
Deleta dados/colunas conforme o exemplo: `DELETE FROM info WHERE pasta = 1;`
