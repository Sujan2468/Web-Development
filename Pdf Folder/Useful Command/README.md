# Some Useful Terminal Command while working in VSCode using CMD

## 1. How to create multiple directory using single command
>**mkdir "Frontend" "Backend" "Database"**
>**Note:** This is used to create directory with name Frontend, Backend and Database
## 2. How to create single directory 
>**mkdir "Frontend"**
>**Note:** This is used to create directory with name Frontend
## 3. How to remove folder containing sub-folder or files or empty folder
>**rmdir /s /q "Frontend"**
> /s represent delete all subfolders and files
> /q represents quiet mode (no confirmation prompts)
>**Note:** This remove folder name Frontend either empty or not without displaying prompt message. If /q is not return then, terminal asked whether to delete or not prompt message.
## 4. How to create file inside Directory with content
>**echo This is a message >"Frontend\new.txt"**
>**Note:** This create new.txt file with content as **This is a message** inside Frontend directory 
## 5. How to create empty file inside Directory
>**echo. >"Frontend\index.html"**
>**type nul>"Frontend\index.html"**
>**Note:** This create index.html file inside Frontend directory 
## 6. How to delete file 
>**del "Frontend\index.html"** 
>**Note:** This delete index.html file inside Frontend directory.
>**del "new.txt"**
>**Note:** This delete new.txt file
## 7. How to view content of file.
>**type "new.txt"**
>**Note:** View content of new.txt file.
## 8. How to move file inside one directory to another
>**move "Backend\app.js" "Frontend"**
>**Note:** This move app.js from Backend Folder to Frontend Folder
## 9. How to move Sub-directory inside one to another
>**move "Backend\Middleware" "Frontend**
>**Note:** This move Middleware sub-directory from Backend to Frontend directory
## 10. How to copy file from one directory to another
>**copy "Frontend\Middleware\app.html" "Backend"**
>**Note** This copy app.html file present in Middleware sub-directory to Backend directory. copy command is used to copy only file but not folder.
## 11. How to copy folder from one directory to another
>**xcopy "Frontend\Middleware" "Backend\Middleware" /E /I /Y**
>-   `/E` – copies all subfolders (even empty ones)
>-   `/I` – assumes destination is a folder   
>-   `/Y` – suppresses overwrite prompts
>**Note**. This copy Middleware folder to Backend\Middleware folder. we should specify sub-folder named even in destination folder even if sub-directory is not present. E.g: Backend directory donot contain Middleware as sub directory but we mentioned it in command.
## 11. How to rename File or Folder name 
>**rename "Frontend" "frontend"**
>**Note:** This rename Frontend to frontend