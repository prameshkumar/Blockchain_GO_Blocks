# Code your own blockchain with Go!

### Tutorial

Since we’re going to write our code in Go, we assume you have had some experience with Go. After installing and configuring Go, we’ll also want to grab the following packages:

go get github.com/davecgh/go-spew/spew

Spew allows us to view structs and slices cleanly formatted in our console. This is nice to have.

go get github.com/gorilla/mux

Gorilla/mux is a popular package for writing web handlers. We’ll need this.

go get github.com/joho/godotenv

Gotdotenv lets us read from a .env file that we keep in the root of our directory so we don’t have to hardcode things like our http ports. We’ll need this too.

Let’s also create a .env file in the root of our directory defining the port that will serve http requests. Just add one line to this file:

ADDR=8080

Create a main.go file. Everything from now on will be written to this file and will be less than 200 lines of code. Let’s get coding!


### Check out Part 1: 
Deployment steps:
- `git clone https://github.com/prameshkumar/Blockchain_GO_Blocks.git`
- navigate to this directory and rename the example file `mv example.env .env`
- `go run main.go`
- open a web browser and visit `http://localhost:8080/`
- to write new blocks, send a `POST` request (I like to use [Postman](https://www.getpostman.com/apps)) to `http://localhost:8080/` with a JSON payload with `BPM` as the key and an integer as the value. For example:
```
{"BPM":10}
```
- Send as many requests as you like and refresh your browser to see your blocks grow! 

### Screenshot

![screen](https://user-images.githubusercontent.com/15616604/35492333-2829f690-0461-11e8-8c1f-8a0258d370e8.png)



