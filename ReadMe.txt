API of home assignment

1. @GetMapping("/task_of_the_day")
   Task of the day

Response:
{
	"activity": "Learn Express.js",
	"accessibility": 0.25,
	"type": "education",
	"participants": 1,
	"price": 0.1,
	"link": "https://expressjs.com/",
	"key": "3943506"
} 

2.  @GetMapping("/get_type?type=:type")
    Task by type

Response:	
{
	"activity": "Learn how to play a new sport",
	"accessibility": 0.2,
	"type": "recreational",
	"participants": 1,
	"price": 0.1,
	"link": "",
	"key": "5808228"
}

3.  @GetMapping("/get_participants?participants=:participants")
	Task by participants
Response:	
{
	"activity": "Learn how to play a new sport",
	"accessibility": 0.2,
	"type": "recreational",
	"participants": 1,
	"price": 0.1,
	"link": "",
	"key": "5808228"
}

4. @GetMapping("/get_type_and_participants?type=:type&participants=:participants")	
   Task by type and participants
Response:	
{
	"activity": "Learn how to play a new sport",
	"accessibility": 0.2,
	"type": "recreational",
	"participants": 1,
	"price": 0.1,
	"link": "",
	"key": "5808228"
}

5. @GetMapping("/get_all_tasks")   
   List of all user's tasks
Response:	
[{
	"activity": "Learn how to play a new sport",
	"accessibility": 0.2,
	"type": "recreational",
	"participants": 1,
	"price": 0.1,
	"link": "",
	"key": "5808228",
	"taskmark": "WISH_LIST",
	"rating": 1
}]   

6. @GetMapping("/get_wish_tasks")
	List of all user's tasks from WISH_LIST
Response:	
[{
	"activity": "Learn how to play a new sport",
	"accessibility": 0.2,
	"type": "recreational",
	"participants": 1,
	"price": 0.1,
	"link": "",
	"key": "5808228",
	"taskmark": "WISH_LIST",
	"rating": 1
}]  

7. @GetMapping("/get_completed_tasks")
	List of all user's tasks from COMPLETED
Response:	
[{
	"activity": "Learn how to play a new sport",
	"accessibility": 0.2,
	"type": "recreational",
	"participants": 1,
	"price": 0.1,
	"link": "",
	"key": "5808228",
	"taskmark": "COMPLETED",
	"rating": 2
}]  

8. @PutMapping("/task_mark?key=:key&mark=:mark")
	Set a WISH_LIST or COMPLETED mark to a task with a key 
Response:	
{
	"activity": "Learn how to play a new sport",
	"accessibility": 0.2,
	"type": "recreational",
	"participants": 1,
	"price": 0.1,
	"link": "",
	"key": "5808228",
	"taskmark": "COMPLETED",
	"rating": 2
}  	

9. @DeleteMapping("/task_delete?key=:key")
	Delete a task with a key 
Response:	
{
	"activity": "Learn how to play a new sport",
	"accessibility": 0.2,
	"type": "recreational",
	"participants": 1,
	"price": 0.1,
	"link": "",
	"key": "5808228",
	"taskmark": "COMPLETED",
	"rating": 2
}  		
	
10.@GetMapping("/task_get>key=:key")
	Get a task with a key 
Response:	
{
	"activity": "Learn how to play a new sport",
	"accessibility": 0.2,
	"type": "recreational",
	"participants": 1,
	"price": 0.1,
	"link": "",
	"key": "5808228",
	"taskmark": "COMPLETED",
	"rating": 2
}  		

11.@GetMapping("/task_by_rating")
	Get task by rating
Response:	
{
	"activity": "Learn how to play a new sport",
	"accessibility": 0.2,
	"type": "recreational",
	"participants": 1,
	"price": 0.1,
	"link": "",
	"key": "5808228",
	"taskmark": "COMPLETED",
	"rating": 2
}  	

What could be improved or added:

1. Data base 
2. Authorization and authentification
3. Verification of parameters	
4. Logs
	