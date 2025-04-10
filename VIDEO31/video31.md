# CSS Media Queries
		
	- Used for making responsive designs and websites
	- Can use a certain style for different purposes (screen, speech etc)
	- Break points are provided for the websites to give responses according to it
	
	Example: 
    body{
	            background-color: aquamarine;
	        }
	        @media screen and (orientation: landscape){
	            body{
	                border: 2px solid purple;
	            }
	        }
	        @media only screen and (max-width: 455px){
	            body{
	                background-color: blue;
	            }
	            .boxes{
	                flex-direction: column;
	            }
	        }
	        .boxes{
	            display: flex;
	        }
	        .box{
	            width: 344px;
	            height: 344px;
	            background-color: blanchedalmond;
	            padding: 0px;
	            margin: 0;
	        }
