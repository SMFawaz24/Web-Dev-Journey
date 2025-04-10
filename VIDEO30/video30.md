# CSS Variables
											
	- Can be used to provide styling of all under one variable
	- Variables will be called in order to provide styling
	
 Example: 
      
      <style>
	
	        :root{
	            --color:rgb(65, 111, 112);
	            --seccolor:rgb(127, 236, 240);
	        }
	        *{
	            margin: 0;
	            padding: 0;
	        }
	        .nav{
	            background-color:var(--color);
	        }
	
	        ul{
	            display: flex;
	        }
	
	        ul li:first-child{
	            --color:rgb(43, 161, 55);
	            background-color: var(--color);
	        }
	
	        ul li{
	            list-style-type: none;
	            padding: 50px;
	        }
	        .container{
	            background-color: var(--seccolor);
	        }
	    </style>
