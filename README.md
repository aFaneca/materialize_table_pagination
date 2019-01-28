# materializecss-table-pagination
Plugin to paginate html tables, using materializecss.
Since the original repository is no longer being updated and its JS support is already broken and deprecated, I thought it could be benefitial to release an updated and tweaked version of the library. Works great in coordination with MaterializeCSS and as a standalone too.

## Basic Usage
Import all css and js dependencies


```
<!--Import Google Icon Font-->
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
<!--Import materialize.css-->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/materialize/0.98.2/css/materialize.min.css">
<!--Import jquery.css-->
<script type="text/javascript" src="https://code.jquery.com/jquery-2.1.1.min.js"></script>
<!--Import materialize.js-->
<script src="https://cdnjs.cloudflare.com/ajax/libs/materialize/0.98.2/js/materialize.min.js"></script>
<!--Import pagination.js this is the plugin-->
<script type="text/javascript" src="js/pagination.js"></script>
```


If you have a table named myTable, initialize the table with:

```
$(document).ready(function(){
	$('#myTable').pageMe({
	  pagerSelector:'#myPager',
	  activeColor: 'green',
	  prevText:'Anterior',
	  nextText:'Siguiente',
	  entriesRecordedText: 'entries recorded',
	  showPrevNext:true,
	  hidePageNumbers:false,
	  perPage:10
	});
});
```


## Options

```
pagerSelector:'#myPager',                // the name of the materialize pager
activeColor: 'green',		         // color of the active page
prevText:'Previous',		         //  'previous page' text
nextText:'Next',                         //  'next page' text
entriesRecordedText: 'entries recorded', // '%s entries recorded' text
showPrevNext:true,                       // show previous and next buttons
hidePageNumbers:false,                   // hide page numbers
perPage:10			         // number of rows to show
```

### Demo

View pagination.html to see the code to use pagination plugin.
