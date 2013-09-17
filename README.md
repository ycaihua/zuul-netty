zuul-netty
==========

### Assembling the Project
The project is equipped with the Maven Assembly plugin for producing an executable, deps-included JAR at netty-server/target.

mvn install && mvn -pl netty-server assembly:assembly

### Quick Start
If you don't want to go to the trouble of assembling and running the project then you can start the proxy using the Maven Exec plugin. It will currently just route to google.com.

mvn install && sudo mvn -pl netty-server exec:java

### Filters
- Only pre (-proxy) filters currently supported.
- No dynamic reload currently supported (coming soon.).

### Upcoming work
- Performance improvements and fixes.
- Dynamic filter reload.
- Post (-proxy) filters.
- Static filters.
- Redirect support from filters.
- Better JMX stats exposure.
