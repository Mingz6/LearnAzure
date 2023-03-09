# LearnAzure

// All telemetry for Operation ID: <**************************>
union *
// Apply filters
| where timestamp > datetime("2023-03-07T18:38:00.686Z") and timestamp < datetime("2023-03-09T18:38:00.686Z")
| where operation_Id == "<**************************>"

Get the exception detail with ID
exceptions
| where operation_Id == '<**************************>'
