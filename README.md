> #### This is repository was created for the purpose of saving my thoughts during my study aspnet to understand all underwater rocks and setting up my configuration well. Of course all code i took from the internet and AI

## For the future:

#### ./appsettings.json - must be in Git Secret, it contains a DB login information.

It must contain:

    ConnectionStrings:DefaultConnection
    Host=127.0.0.1;Port=5432;Database=todo_db;Username=todo_user;Password=...

---

Notes:

1. Setting up:

        dotnet-sdk-8.0 aspnet-runtime-8.0, aspnet-targeting-pack-8.0
    

        dotnet tool install --global dotnet-ef


        sudo -iu postgres
        initdb -D /var/lib/postgres/data
        exit

        sudo systemctl start postgresql
        sudo systemctl enable postgresql


        dotnet ef migrations add InitialCreate

1. First run:
    
        dotnet restore 
        dotnet run