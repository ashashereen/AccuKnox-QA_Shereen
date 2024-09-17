How the Script Works:
Import the requests Library: This library is used to make HTTP requests.

Define the check_application_status Function:

It sends a GET request to the specified URL.
Based on the HTTP status code received, it determines if the application is up or down:
Status code 200 generally indicates that the application is functioning correctly.
Status codes like 400, 401, 403, 404, 500, 502, 503, and 504 typically indicate issues with the application or server problems.
If the request fails (e.g., network issues, invalid URL), it catches the exception and returns 'DOWN'.
Run the Script:

The script checks the status of the application specified in application_url and prints the result.
Note : Customize application_url to the URL you want to monitor.
