build:	## Build the API binary file
		make lint
		go build

run:	## Runs the build binary and save everything to awesome.log
		./awesome-api >./awesome.log 2>&1 &

stop:	## Stop the execution of awesome-api
		kill $(shell pgrep awesome-api)

clean:	## Remove binary and logs
		-make stop
		-rm ./awesome-api awesome.log

test:	## Test API using curl
		curl http://localhost:9999
		curl http://localhost:9999/health

lint:	## Lints all the go files using golangci-lint
		golangci-lint run

unit-tests:		## run unit tests using go test
		go test -v -short -coverprofile=coverage-units.out

help:	## Show help message
		@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'
