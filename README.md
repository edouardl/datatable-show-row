# Show Row : a DataTable plugin
==================

This simple plugin works with the new API of the jQuery [DataTables](http://datatables.net) table enhancer (API introduce in version 1.10).

It permits to search a row and display the right page of DataTable to show it. For example after a new row creation or row content update.

Could be chained to the DataTable Rows API, see examples below : 


## Example

var table = jQuery('#example_table').DataTable();

// Show a selected row
    
    table.row( '#row_example' ).show().draw(false);

// Update row and show it after reorder
    
    table.row( '#row_example' ).data({ [some data] }).draw().show().draw(false);

// Create a row and show it after drawing
    
    table.row.add({ [some data] }).draw().show().draw(false);


## Changelog

Version 1.0
* Remove the "r_" prefix
* Remove the calling of "draw()" function inside the show() method to be consistent with the rest of the API
