**Here is your detailed guide to getting the Student Wellness Hub running on your machine.**

**Phase 1: Prepare the Environment**
Launch XAMPP: Open the XAMPP Control Panel.

Start Services: Click "Start" for Apache and MySQL.

**Phase 2: Folder Setup**
Open your file explorer and go to C:\xampp\htdocs.

Ensure your project folder is named exactly: group_4-Buarao-Guilingen-Boston-Zamora.

Inside that folder, you should see your files (e.g., index.php, database.sql, etc.).

**Phase 3: Database Import (phpMyAdmin)**
Open your browser and go to http://localhost/phpmyadmin/.

Create Database: * Click New on the left.

Enter name: if0_40312270_db_userdata (This must match what is in your PHP code).

Click Create.

Import Data:

Click the database name you just created.

Click the Import tab.

Click Choose File and navigate to: C:\xampp\htdocs\group_4-Buarao-Guilingen-Boston-Zamora\database.sql

Click Go at the bottom.

**Phase 4: Update the Connection File**


Because your folder name is different from the one originally mentioned in the "Access" instructions, you must ensure the PHP code points to the right database.

Open your project folder.

Search for a file named db_connect.php, connection.php, or config.php.

Open it in a text editor (like Notepad++ or VS Code) and ensure it looks like this:

PHP

$servername = "localhost";
$username = "root";
$password = ""; // XAMPP default is empty
$dbname = "if0_40312270_db_userdata";

$conn = mysqli_connect($servername, $username, $password, $dbname);


**Phase 5: Access the Project**
To view your website, you will now use this specific local URL:

URL: http://localhost/group_4-Buarao-Guilingen-Boston-Zamora/

Admin Credentials
Username: admin2@gmail.com

Password: Admin123

Registration Code: SWHub2025
