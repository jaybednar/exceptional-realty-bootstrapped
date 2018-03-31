Exceptional Realty Website (Bootstrapped Version) 

Example using Twitter Bootstrap v4 framework, with FontAwesome. 

More info on Bootstrap: http://getbootstrap.com 

More info on FontAwesome: http://fontawesome.com

---------

Use --- container --- class to wrap your content to center it.  You have a choice of fixed width or fluid

<div class="container"> </div>

<div class="container-fluid"></div>  =(stretches the whole screen) 

---------

Use --- row --- to wrap columns.  To create vertical separation.

<div class="container">
	<div class="row">
		
	</div>
</div>


---------

Use --- col- --- classes to separate content horizontally.  The default grid allows for 12 columns. So as seen below, a col- ending in a -4 would take 1/3 of the screen.  (You could also have a col-sm-8 (2/3 screen) with a col-sm-4 (1/3) or a col-sm-6 (1/2) with another col-sm-6 (1/2) etc etc.)

	The col- class is followed by either xs, sm, md, or lg.  These indicate the sizes (extra-small, small, mediumd, large) -- which effect the CSS media query break points (how many pixels the columns start to stack vertically instead of horizontally. lg: 1200px, md: 992px, sm: 768px, xs: always horizontal)  

<div class="container">
	<div class="row">
		<div class="col-sm-4"></div>
		<div class="col-sm-4"></div>
		<div class="col-sm-4"></div>
	</div>
</div>

---------

Use --- -offset --- class to shift columns over to the right.  So col-sm-offset-4 will offset the column 4 spaces.  See the code below will push two separate col-sm-4 over to the middle and right region.  

<div class="container">
	<div class="row">
		<div class="col-sm-4 col-sm-offset-4"></div>
		<div class="col-sm-4"></div>
	</div>
</div>

---------

Use --- -push and -pull ---

You can change to the conventional order of the columns by using push and pull classes. Push will push columns to the right and pull will pull columns to the left.  You can use a number to indicate how many column spaces to push or pull. 

<div class="container">
	<div class="row">
		<div class="col-sm-8 col-sm-push-4"></div>
		<div class="col-sm-4 col-sm-pull-8"></div>
	</div>
</div>

---------

--- Nesting Columns --- 

Columns can be nested inside one another by inserting a row inside a column and then inserting additional columns inside of the inner row.  

(nested columns will take up their appropriate portion of the column they are nested inside of. ie. below the nested columns of col-sm-4 will take up 1/3 of the col-sm-8 column.)

<div class="container">
	<div class="row">
		<div class="col-sm-8"></div>
			<div class="row">
				<div class="col-sm-4"></div>    
				<div class="col-sm-4"></div>
				<div class="col-sm-4"></div>
			</div>
		<div class="col-sm-4 col-sm-pull-8"></div>
	</div>
</div>






















