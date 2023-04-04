# LearnAzure

// All telemetry for Operation ID: <**************************>
union *
// Apply filters
| where timestamp > datetime("2023-03-07T18:38:00.686Z") and timestamp < datetime("2023-03-09T18:38:00.686Z")
| where operation_Id == "<**************************>"

Get the exception detail with ID
exceptions
| where operation_Id == '<**************************>'

# Azure DB CLI
Importing Azure SQL\
sqlpackage /Action:Import /tsn:tcp:<sql-server>.database.windows.net,1433 /tdn:<sqldb-new> /tu:<admin-name> /tp:<password> /sf:<local-DB.bacpac>\
Exporting Azure SQL\
sqlpackage /Action:Import /tsn:tcp:<sql-server>.database.windows.net,1433 /tdn:<sqldb-new> /tu:<admin-name> /tp:<password> /tf:<local-DB.bacpac>
