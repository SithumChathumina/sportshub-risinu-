# NSBM SportsHub

Sports club management system for the NSBM Web and Mobile Application Development final project (Topic 3).
Built with HTML, CSS, JavaScript (Bootstrap), PHP and MySQL.

## What it does

**Students**
- Register and log in
- Browse and join sports clubs
- See training schedules and match fixtures
- Register for tournaments and matches
- See match results and standings
- Book training facilities and equipment
- See their own participation history

**Admins**
- Log in to a separate admin panel
- Add, edit and delete clubs, and approve or reject membership requests
- Schedule training sessions and matches
- Create tournaments and record match results
- Approve or reject facility and equipment bookings
- Participation and performance reports (can be downloaded as CSV)

## How to run it (XAMPP)

1. Copy this folder into `C:/xampp/htdocs/` (the folder can have any name, for example `sportshub3.3`).
2. Start Apache and MySQL in the XAMPP control panel.
3. Open `http://localhost/phpmyadmin` and import `database/sportshub.sql`. This creates the database `sportshub3_db` with some sample data.
4. Open `http://localhost/<your folder name>/index.php`, for example `http://localhost/sportshub3.3/index.php`.

The database settings are in `config/database.php`.
For hosting (for example InfinityFree) import `database/sportshub_hosting.sql` instead, because hosting does not let you create or choose the database name in the SQL file.
The site finds its own folder name automatically (`BASE_PATH` in `includes/init.php`), so nothing needs changing when the folder is renamed.

## Sample logins

Students must register with an `@nsbm.ac.lk` email. Admin accounts are added directly in the database, so they can use any email (the sample admin uses `admin@nsbm.lk`).

| Role | Email | Password |
| --- | --- | --- |
| Admin | admin@nsbm.lk | Admin@123 |
| Student | student@nsbm.ac.lk | Student@123 |

## Folder structure

```
index.php, clubs.php, club.php, fixtures.php, results.php   public pages
login.php, register.php, logout.php                          login and registration
student/       pages for logged-in students
admin/         pages for the admin panel
includes/      header, footer, menus and shared functions
config/        database connection settings
database/      sportshub.sql (tables and sample data)
assets/        css, javascript and images
```

## Team

| Member | Part of the system |
| --- | --- |
| Member 1 | (fill in) |
| Member 2 | (fill in) |
| Member 3 | (fill in) |
| Member 4 | (fill in) |
| Member 5 | (fill in) |
| Member 6 | (fill in) |
