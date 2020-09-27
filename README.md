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
```sql
CREATE TABLE IF NOT EXISTS pacientes (
	pac_code SERIAL NOT NULL PRIMARY KEY,
	pac_nome VARCHAR(125),
	pac_nascimento DATE,
	PAC_RG VARCHAR (25),
	PAC_TELEFONE VARCHAR (15),
	pac_rua VARCHAR (135),
	pac_cep VARCHAR (20),
	pac_complemento VARCHAR (50),
	pac_bairro_fkey INT REFERENCES bairro (baicode)
	);
```
