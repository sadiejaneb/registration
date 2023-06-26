# registration

# add phpmyadmin for database configuration

# tables setup

# CREATE TABLE users (
    id INT PRIMARY KEY AUTO_INCREMENT,
    username VARCHAR(255),
    password VARCHAR(255)
);

CREATE TABLE pokemon_sprites (
    id INT PRIMARY KEY AUTO_INCREMENT,
    user_id INT,
    sprite_url VARCHAR(255),
    FOREIGN KEY (user_id) REFERENCES users(id)
);

# change hostname, username, password, database for your codd
