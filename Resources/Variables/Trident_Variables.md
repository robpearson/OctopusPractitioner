- Connection String For Database Deployments
    - Name: Project.Connection.String
    - Value: Server=#{Project.Database.Server.Name};Integrated Security=true;Database=#{Project.Database.Name}
    - Type: Text
- Report Path Variable
    - Name: Project.Database.Report.Path
    - Value: C:\DatabaseReports\\#{Octopus.Environment.Name}
    - Type: Text
- Connection String Variable For Configuration Transform
    - Name: ConnectionStrings:Database
    - Value: #{Project.Connection.String}
    - Type: Text
- Database Name Variable
    - Name: Project.Database.Name     
    - Value: Trident (Production Scoping)
    - Value: Trident_#{Octopus.Environment.Name}
    - Type: Text
- Database Server Variable
    - Name: Project.Database.Server.Name    
    - Value: (localdb)\MSSQLLocalDB
    - Type: Text

This is a change.
