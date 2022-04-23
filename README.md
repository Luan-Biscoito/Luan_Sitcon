# Luan_Sitcon
 
<!-- Criacao tabelas do bd -->

CREATE SCHEMA `new_schema` ;


CREATE TABLE `hospital_ipatinga`.`tbprocedimentos` (
`idProcedimento` INT NOT NULL,
  `NomeProcedimento` VARCHAR(150) NOT NULL,
  `ValorProcedimento` VARCHAR(15) NOT NULL,
  `Descricao` VARCHAR(100) NULL,
  PRIMARY KEY (`idProcedimento`));


CREATE TABLE `hospital_ipatinga`.`tbcotacao` (
`idcota` INT NOT NULL,
  `idProcedimento` INT NOT NULL,
  `NomeFornecedor` VARCHAR(70) NOT NULL,
  `Valor` VARCHAR(15) NULL,
  PRIMARY KEY (`idcota`));