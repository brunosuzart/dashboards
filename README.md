# dashboards
#The file Modelo.xlsm is a spreadsheet model that I've create to solve a specific problem about knowledge of commercial information. This model is used to fullfill the entire broker's needs about information.
#The file functions, is a module from Access VBA, that explain and show how you build individuals dashboard for specific persons (in my case is Insurance brokers) in an automated process mirrored in a sample file as I sad above.
#It's important to name specific ranges in excel: 

Example: 

''This code means that you're trying to export an specific Query to an excel which have a specific Path in an specific range
  DoCmd.TransferSpreadsheet acExport, acSpreadsheetTypeExcel12Xml, "Inadimplência", xlsxpath, True, Range:="tbinadimplencia"
  
  DoCmd.TransferSpreadsheet Type of exportation, Type of the spredsheet, Access table or Query name, _
  & The File Path that you would like to export with the completely name of the file and his .extension, If it has fields name (True / False), _
& And the range in the excel, range means the name of an specific range of value, and you must declare in in your own model as I did in my own
and it always will be preced by the name Range:="your_range_name"
  
  