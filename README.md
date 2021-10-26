# ElsaDemo
Steps to run and test workflows
1. Run as DocumentManagement.Web instead of IIS Express
2. Run following commands in powershell:

	For SMTP: docker run -p 3000:80 -p 2525:25 rnwood/smtp4dev:linux-amd64-3.1.0-ci0856
	
	For Elsa Dashboard: docker run -t -i -e ELSA__SERVER__BASEADDRESS=http://localhost:5000 -p 14000:80 elsaworkflows/elsa-dashboard:latest
3. Open following links in the browser other than http://localhost:5001
  
	For SMTP: http://localhost:3000/
  
	For Elsa Dashboard: http://localhost:14000/


Reference: https://sipkeschoorstra.medium.com/building-workflow-driven-net-applications-with-elsa-2-part-1-44e08a9ba94b
