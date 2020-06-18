# Desafio_Serasa
Desafio Serasa 06/2020

Dependências do projeto:
- Ionic v4+;
- Angular v7+;
- XAMPP ou software similar;
- MySQL;
- Extensão "Moessif Origins & CORS Changer";
- Google Chrome;

Configurar ambiente para testes:
- Descompactar .rar, mover o conteúdo pasta backend para o diretório definido no XAMPP (por padrao xampp/htdocs) de modo que o caminho fique xampp/htdocs/serasa;
- Descompactar .rar, mover o conteúdo da pasta frontend para o diretório desejado;
- Inicializar o XAMPP;
- Abrir o Google Chrome, ativar a extensão "Moessif Origins & CORS Changer";
- Abrir o prompt de comando e encaminhar para dentro da pasta frontend, executar o comando "ionic cordova run browser";


Os fontes relevantes estao dentro do .rar, nas pastas frontend/src e backend/serasa;


Scripts de MySQL necessarios:
CREATE DATABASE `db_serasa`;
CREATE TABLE empresa (
	id INTEGER PRIMARY KEY AUTO_INCREMENT,
	nome VARCHAR(255)
);

CREATE TABLE nota (
	id INTEGER PRIMARY KEY AUTO_INCREMENT,
	descricao VARCHAR(255),
	empresa INTEGER NOT NULL,
	FOREIGN KEY (empresa) REFERENCES empresa(id)
);

INSERT INTO empresa (nome) VALUES ('Empresa 1');
INSERT INTO empresa (nome) VALUES ('Empresa 2');
INSERT INTO empresa (nome) VALUES ('Empresa 3');
INSERT INTO empresa (nome) VALUES ('Empresa 4');
INSERT INTO empresa (nome) VALUES ('Empresa 5');

Arquivo de modelo para upload de notas esta no repositorio.
