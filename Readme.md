## API Specification

| Route  	                | Method  	|  Description 	        |  Middleware 	        |
|---	                    |---	    |---	                |---	                |
| /users  	                |  POST 	|   	                |   	                |
| /user/{id}  	            |  GET 	    |   	                |   	                | 
| /user/{id}  	            |  PUT 	    |   	                |   	                |
| - 	                    |   	    |   	                |   	                |
| /vendor/create 	        |  POST 	|   	                | Auth | Admin	        |
| /vendor/{id} 	            |  GET 	    |   	                | Auth  	            |
| /vendor/{id}/order 	    |  GET 	    |   	                | Auth  	            |
| -	                        |   	    |   	                |   	                |
| /order/{id} 	            |  GET 	    |   	                | Auth  	            |
| /order/{id}/approve 	    |  POST 	|   	                | Auth | Vendor {Owner} |
| /order/{id}/decline 	    |  POST 	|   	                | Auth | Vendor {Owner} |
| -                   	    |        	|   	                |          	            |
| /savings 	                |  GET 	    |   	                | Auth  	            |
| /save 	                |  POST 	| Save via Xend SDK     | Auth  	            |
| /withdraw 	            |  POST 	| Unstake via Xend SDK  | Auth  	            |