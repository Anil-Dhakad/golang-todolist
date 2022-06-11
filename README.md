## STEPS for running code:

1. install all packages by running command **go get -u ./...**
2. command to run project **go run todolist.go**

## Database query router commands:

1. Check health check of server running proper **curl -i localhost:8000/healthz**
2. Create todo **curl -X POST -d "description=Play football" localhost:8000/todo**
3. Update todo **curl -X POST -d "completed=true" localhost:8000/todo/{id}**
4. Delete todo **curl -X DELETE localhost:8000/todo/{id}**
5. Get completed todo list **curl -X GET localhost:8000/todo-completed**
6. Get in-complete todo list **curl -X GET localhost:8000/todo-incomplete**
