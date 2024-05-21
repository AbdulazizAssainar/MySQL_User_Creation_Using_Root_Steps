# MySQL_User_Creation_Using_Root_Steps

1. **Open Command Line:**
   Open your command line interface.

2. **Sign in to MySQL:**
   Type the command to sign in to MySQL using the root user:
   ```
   mysql -u root -p
   ```
   You'll be prompted to enter the root password.

3. **Create a New User:**
   Use the following SQL command to create a new user:
   ```sql
   CREATE USER 'new_username'@'localhost' IDENTIFIED BY 'new_password';
   ```
   Replace `'new_username'` with the desired username and `'new_password'` with the desired password.

4. **Grant Privileges:**
   Grant the necessary privileges to the new user with the following SQL command:
   ```sql
   GRANT ALL PRIVILEGES ON *.* TO 'new_username'@'localhost';
   ```
   Replace `'new_username'` with the username you created.

5. **Flush Privileges:**
   After granting privileges, flush the privileges to ensure they are applied immediately:
   ```sql
   FLUSH PRIVILEGES;
   ```

6. **Exit MySQL:**
   Exit MySQL by typing:
   ```
   exit
   ```
   Then press Enter.

These steps will guide you through creating a new user with all privileges in MySQL.
