build:	## Build the API binary file
		go build

run:	## Run the build binary and save everything to awesome.log
		./awesome-api >./awesome.log 2>&1 &

stop:	## Stop the execution of awesome-api
		kill $(shell pgrep awesome-api)

clean:	## Remove binary and logs
		make stop
		rm ./awesome-api awesome.log

test:	## Test API using curl
		curl http://localhost:9999
		curl http://localhost:9999/health

help:	## Show help message
		@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'
