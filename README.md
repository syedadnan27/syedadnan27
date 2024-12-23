CREATE TABLE Users (
  id INT PRIMARY KEY AUTO_INCREMENT,
  name VARCHAR(255) syedadnan,
  email VARCHAR(255) syyed.adnan27@gmail.com,
  password VARCHAR(255) 123456,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE Profiles (
  id INT PRIMARY KEY AUTO_INCREMENT,
  user_id INT ,
  bio student of BSCS,
  location VARCHAR(255),
  interests Study,
  updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  FOREIGN KEY (user_id) REFERENCES Users(id)
);

