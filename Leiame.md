TEMA DO TRABALHO: Jogo da Memória
Participantes: Erik Kaue Paroline - RA: 20960545 - GITHUB: https://github.com/bercolis/JogodaMemomria
Fernanda Umberto - RA: 20943426 - GITHUB: https://github.com/fe-umb/crud-game
Guilherme Rodrigues - RA: 20996393 - GITHUB: https://github.com/GuilhermeRodMiranda/JogoMemoria
Matheus Marques - RA: 20981531 - GITHUB: https://github.com/Debrastak/Jogo-mem-ria
Milena Basso - RA: 20956610 - GITHUB: https://github.com/mlnbss/Desenvolvimento-de-Software-Para-Web

-----------------------------------

NOME DO BANCO DE DADOS: bdjogodamemoria
CREATE TABLE aluno (
 ra varchar(8) NOT NULL,
 senha varchar(20) NOT NULL,
 nome varchar(20) NOT NULL,
 sobrenome varchar(50) NOT NULL,
 email varchar(100) NOT NULL,
 PRIMARY KEY (ra)
) 
CREATE TABLE pergunta (
 id int(11) NOT NULL AUTO_INCREMENT,
 enunciado varchar(100) NOT NULL,
 alternativa1 varchar(100) NOT NULL,
 alternativa2 varchar(100) NOT NULL,
 alternativa3 varchar(100) NOT NULL,
 alternativa4 varchar(100) NOT NULL,
 alternativacorreta int(11) NOT NULL,
 ra varchar(8) NOT NULL,
 PRIMARY KEY (id)
) 
CREATE TABLE professor (
 ra varchar(8) NOT NULL,
 senha varchar(20) NOT NULL,
 nome varchar(20) NOT NULL,
 sobrenome varchar(50) NOT NULL,
 email varchar(100) NOT NULL,
 PRIMARY KEY (ra)
)

-----------------------------------

População do banco:

INSERT INTO aluno

	VALUES('100960545', 'admin', 'Erik Kaue', 'dos Santos', 'erikaotop@hotmail.com');

INSERT INTO aluno
	VALUES('20943426', 'bolo', 'Fernanda', 'Umberto', 'feumb@hotmail.com');
    
INSERT INTO aluno
	VALUES('20996393', '123', 'Guilherme', 'Rodrigues', 'guizao@hotmail.com');
    
INSERT INTO aluno
	VALUES('20981531', 'wesley', 'Matheus', 'Marques', 'matheus@hotmail.com');
    
INSERT INTO aluno
	VALUES('20956610', 'sucodeuva', 'Milena', 'Basso', 'mibasso@hotmail.com');

INSERT INTO professor
	VALUES('12345678', 'paulotopdemais', 'Paulo', 'Nietto', 'paulonietto@hotmail.com');
    
INSERT INTO professor
	VALUES('87654321', 'frontendgod', 'Marcos', 'Cavalhieri', 'mc@hotmail.com');
    
INSERT INTO professor
	VALUES('99999999', 'fibonacci', 'Lukas', 'Farias', 'lukao@hotmail.com');
    
INSERT INTO professor
	VALUES('09876789', 'esqueci', 'Roberta', 'Aragon', 'raragon@hotmail.com');

INSERT INTO pergunta(enunciado, alternativa1, alternativa2, alternativa3, alternativa4,alternativacorreta, ra)
	VALUES('Qual desses é um BD não relacional?', 'SQL Server', 'MySQL', 'Postgre', 'MongoDB', 4, '87654321');
    
INSERT INTO pergunta(enunciado, alternativa1, alternativa2, alternativa3, alternativa4,alternativacorreta, ra)
	VALUES('Qual desses comandos em linux permite obter privilégios de outro usuário?', 'admin', 'apt', 'sudo', 'get', 3, '87654321');
    
INSERT INTO pergunta(enunciado, alternativa1, alternativa2, alternativa3, alternativa4,alternativacorreta, ra)
	VALUES('A World Wide Web (WWW) foi concebida em qual laboratório de pesquisa?', 'UCLA', 'DARPA', 'CERN', 'MIT', 3, '87654321');
    
INSERT INTO pergunta(enunciado, alternativa1, alternativa2, alternativa3, alternativa4,alternativacorreta, ra)
	VALUES('Em CSS, para definir a apresentação de um texto em negrito, utiliza se a propriedade', 'font style', 'font weight', 'bold', 'text style', 2, '87654321');
    
INSERT INTO pergunta(enunciado, alternativa1, alternativa2, alternativa3, alternativa4,alternativacorreta, ra)
	VALUES('Para inserir um arquivo de JS em uma página web, deve se utilizar o parâmetro:', 'script', 'href', 'style', 'link', 1, '87654321');
