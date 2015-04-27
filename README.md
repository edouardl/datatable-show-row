Show Row : a DataTable plugin
==================

This simple plugin works with the new API of the jQuery [DataTables](http://datatables.net) table enhancer.

It permits to search a row and display the right page of DataTable to show it. For example after a new row creation or row content update.

Could be chained to the DataTable Rows API, like that : 

var table = jQuery('#example_table').DataTable();

// Show that row
    
    table.row( '#row_example' ).r_show();

// Update row and show it after reorder
    
    table.row( '#row_example' ).data({ [some data] }).r_show();

// Create a row and show it after drawing
    
    table.row.add({ [some data] }).r_show();