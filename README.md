# UiPath-How-to-AccessDBFile-Querying

## 1. Set-up Microsoft Access database engine 2010  [Official Download](https://www.microsoft.com/ko-kr/download/details.aspx?id=13255)
 (**_Caution!_** Must be check Office bit-version)

## 2. Add-on UiPath-Database-Activities Package

## 3. use Connect Activity         
```xaml activity properties
   Activity Properties
   ConnectionString = "Provider=Microsoft.ACE.OLEDB.12.0;Data Source=['File Path']"
   ProviderName     = "System.Data.OleDb"
   Output           = Variable - UiPath.Database.DatabaseConnection
```

## 4. use Execute query Activity   
```xaml activity properties 
   Activity Properties
   ExistingDbConnection = exist before Output
   Sql                  = use Access query
   DataTable            = Variable - System.Data.DataTable
```
## That's It! You Can Run Access DB File querying

## FYI My Sameple Source

                            
