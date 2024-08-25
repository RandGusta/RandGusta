CREATE DATABASE Bio;

USE bio;

CREATE TABLE About_me(

  idBio INT NOT NULL AUTO_INCREMENT,
  
  name VARCHAR(20) NOT NULL,

  nationality VARCHAR(20) NOT NULL,
  
  pronouns ENUM('ele\dele') NOT NULL,
  
  graduation VARCHAR(25) NOT NULL,

  semester ENUM('1°', '2°', '3°', '4°', '5°', '6°', '7°', '8°'),

  languages VARCHAR(40),

  program_languages VARCHAR(50),
  
  PRIMARY KEY(idbio)
);

INSERT INTO About_me

(idBio, name, nationality, pronouns, graduation, semester, languages, program_languages)

VALUES

(DEFAULT, 'Gustavo Randi', 'Brazilian', 'ele\dele', 'Software Engineers', '2°', 'English and Portuguese', 'Python, SQL');
