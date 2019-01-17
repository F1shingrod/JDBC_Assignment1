# JDBC_Assignment1

CREATE DATABASE `sqlandjava`;


CREATE TABLE `sqlandjava`.`people` (
  `person_id` INT NOT NULL,
  `firstname` VARCHAR(45) NOT NULL,
  `lastname` VARCHAR(45) NOT NULL,
  PRIMARY KEY (`person_id`));

    INSERT INTO `sqlandjava`.`people` (`person_id`, `firstname`, `lastname`) VALUES ('1', 'Anna', 'Andersson');
  INSERT INTO `sqlandjava`.`people` (`person_id`, `firstname`, `lastname`) VALUES ('2', 'Berit', 'Bolt');
  INSERT INTO `sqlandjava`.`people` (`person_id`, `firstname`, `lastname`) VALUES ('3', 'Carl', 'Carlsson');
  INSERT INTO `sqlandjava`.`people` (`person_id`, `firstname`, `lastname`) VALUES ('4', 'David', 'Druid');
  
  CREATE USER super@localhost IDENTIFIED BY 'password';
  GRANT SELECT ON sqlandjava.people TO user@localhost;
