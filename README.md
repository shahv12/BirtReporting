# BirtReporting

Details for the source reporting is as follows: Reports of type pdf and xls can be generated.

The source contains the following structure

 src
    -com
      -reports
	-contants 		  :constants.
  	-controller		  :request interceptors.
	-exception		  :customized exception classes.	
	-generator		  :report generator.
	
WebContent
    -generated_reports		  : stores the generated reports in the appropriated folders.
    -jsp	                  : status message is directory here.
    -report_design		  : report design files are stored here.
    -WEB-INF
	-lib			  : jars files are  stored.
	-classes
	-springapp-servlet.xml    : all bean definitions are placed here.
	-web.xml		  : configuration for the app.


STEPS TO CONFIGURE.
1. Unzip and export the project to the eclipse.
2. Export to a war file.
3. start the server eg apache-tomcat
4. There are 2 sample design files stored. They are : employee.rptdesign and customers.rptdesign.
	
5: To generate the xls report the url is:
   http://host:8080/Reporting/xls/employee or http://host:8080/Reporting/xls/customers


6: To generate the pdf report the url is:
   http://host:8080/Reporting/pdf/employee or http://host:8080/Reporting/pdf/customers


7. Reports are generated with the name "report" and appended by the timestamp.

8. Reports are stored in the generated_reports directory under the web content folder.

9. Test cases have not been completed.

