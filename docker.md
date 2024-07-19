### Docker

Docker is a platform that helps developers build, share and run applications with the containers.
Docker basically works for problems like:

### Problem 1
```
 At Developer end:
	Developer made an application which uses services like node, java,etc. That application runs perfectly at developers end. Developer send that application to Testing team for final check before producion phase.

 At Tester end: 
	Tester insatlled that application after around 6months or lets take it as a year. We all know services update their versions with some minor bug fixes and improvements. When the tester 
installed the application it installed with updated version of it services because of which it start creating some issues in application.  
```

### Problem 2
``` 
 At developer and tester end:
	Developer made an application which uses services like node, java,etc. Now that application working perfectly at developer's end. Simultaneously tester also installed that application in same time with 
same version of services as developer was using. Now it will send it to servers for production.

 At Server's end: 
	Servers got the application after like a year. Servers are all ways stays up to date. Again problem occurs that services got latest versions which results in issues in application.
```

There are many more problem occurs for which now almost every company either big or small uses docker.

### Container
A docker container have everything about the project like liberaries, runtime, tools, wuth sepcification version, code.

