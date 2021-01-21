# ASP .NET Core

## Copy row

Create a [command column with a custom button](https://js.devexpress.com/Documentation/Guide/Widgets/DataGrid/Columns/Column_Types/Command_Columns/#Create_a_Column_with_Custom_Buttons). The [rowCopy](../jQuery/index.js#L2) function in the [jQuery](../jQuery) sample shows how to implement the button's onClick event.

The function will copy the current row data into a pasteable format for Excel. This will allow the end-user to paste the row data into their Excel application.

## Copy via Export

Create a custom button in the DataGrid's [onToolbarPreparing](https://js.devexpress.com/Documentation/ApiReference/UI_Widgets/dxDataGrid/Configuration/#onToolbarPreparing) event. The [copyViaExcelExport](../jQuery/index.js#L31) function in the [jQuery](../jQuery) sample shows how to implement the button's onClick event.

The function will use the DataGrid's [exportDataGrid](https://js.devexpress.com/Documentation/ApiReference/Common/Utils/excelExporter/#exportDataGridoptions) method for Excel. The [customizeCell](https://js.devexpress.com/Documentation/ApiReference/Common/Object_Structures/ExcelExportDataGridProps/#customizeCell) callback is used to copy the DataGrid's data into a pasteable format for Excel. This will allow the end-user to paste the entire DataGrid into their Excel application.

This function can also be used for different tasks. For example, copying the summary rows or copying a certain column.