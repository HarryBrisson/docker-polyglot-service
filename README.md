# polyglot-service
A micro service for small natural language processing, powered by Polyglot.

# About Polyglot
- https://github.com/aboSamoor/polyglot
- http://polyglot.readthedocs.io/

# Launch example

`docker build -t polyglot .`

making available on port 80 allows for http traffic
(if using aws ec2 instance, traffic must also be allowed on the port)
`docker run -dp 80:80 polyglot`


