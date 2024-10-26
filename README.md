# golangecom

### Run the Commands:

##### Build the Project:
go build -o bin/ecom cmd/main.go

##### Run Tests:
go test -v ./...

##### Run the Application:
- After building, execute the application:
.\bin\ecom

##### Create a New Migration File
- download migrate tool 
go get github.com/golang-migrate/migrate/v4/cmd/migrate@latest

- Replace <name_of_migration> with the desired migration name
migrate create -ext sql -dir cmd/migrate/migrations <name_of_migration>
- Note: You might need to add migrate to your PATH or use its full path if it isn’t recognized.

##### Run Migrations Up
go run cmd\migrate\main.go up

##### Run Migrations Down
go run cmd\migrate\main.go down
