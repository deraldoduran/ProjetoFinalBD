```SQL
CREATE TABLE IF NOT EXISTS medico(
	num_med SERIAL NOT NULL PRIMARY KEY,
	nome VARCHAR(250),
	especialidade VARCHAR(50),
	crm INT

);
```
```SQL
CREATE TABLE IF NOT EXISTS usuarios (
	usu_code SERIAL NOT NULL PRIMARY KEY,
	uso_nome VARCHAR(125),
	usu_senha VARCHAR(15),
	usu_tipo VARCHAR (20)
	);
```
```sql
CREATE TABLE IF NOT EXISTS BAIRRO (
	baicode SERIAL NOT NULL PRIMARY KEY,
	bainome VARCHAR(125)
	
	);
```
