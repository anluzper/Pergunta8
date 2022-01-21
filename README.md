# Pergunta8
-- Create table Dogs
CREATE TABLE dogs (
id INTEGER NOT NULL PRIMARY KEY,
name VARCHAR(50) NOT NULL
  );

--Create table Cats
CREATE TABLE cats(
id INTEGER NOT NULL PRIMARY KEY,
name VARCHAR(50) NOT NULL
  );

-- Inserir na tabela dogs
insert into dogs VALUES
(1,'TOM');
insert into dogs VALUES
(2,'MAX');
insert into dogs VALUES
(3,'ALEX');

-- Inserir na tabela cats
insert into cats VALUES
(1,'TOMY');
insert into cats VALUES
(2,'MASSON');
insert into cats VALUES
(3,'MISU');
  
-- Consulta na tabela 
  SELECT d.id, d.name dogs, c.name cats
  FROM dogs d, cats c
  where d.id = c.id;
