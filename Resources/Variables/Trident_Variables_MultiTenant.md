- Connection String For Database Deployments
    - Name: Project.Connection.String
    - Value: Server=#{Project.Database.Server.Name};Integrated Security=true;Database=#{Project.Database.Name}
    - Type: Text
- Report Path Variable
    - Name: Project.Database.Report.Path
    - Value: C:\DatabaseReports\\#{CommonTenantVariables.TenantAbbr}\\#{Octopus.Environment.Name}
    - Type: Text
- Connection String Variable For Configuration Transform
    - Name: ConnectionStrings:Database
    - Value: #{Project.Connection.String}
    - Type: Text
- Database Name Variable
    - Name: Project.Database.Name     
    - Value: Trident_#{CommonTenantVariables.TenantAbbr} (Production Scoping)
    - Value: Trident_#{CommonTenantVariables.TenantAbbr}Development (Development Scoping)
    - Value: Trident_#{CommonTenantVariables.TenantAbbr}Staging (Development Scoping)
    - Value: Trident_#{CommonTenantVariables.TenantAbbr}Test (Development Scoping)
    - Type: Text
- Database Server Variable
    - Name: Project.Database.Server.Name    
    - Value: (localdb)\MSSQLLocalDB
    - Type: Text
