# polyglot-service
A micro service for small natural language processing, powered by Polyglot.

# About Polyglot
- https://github.com/aboSamoor/polyglot
- http://polyglot.readthedocs.io/

# Launch example

`docker build -t polyglot .`

making available on port 80 allows for http traffic
(if using aws ec2 instance, traffic must also be allowed on the port)
`docker run -dp 80:80 --name polyglot_container polyglot`


I set up a crontab to restart the container every day because I was having issues with it becoming nonresponsive.

`crontab -e`
`0 */6 * * * docker restart polyglot_container`