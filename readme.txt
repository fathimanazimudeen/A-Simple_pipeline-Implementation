A Simple pipeline implementation using Python
------------------------------------


Language: Python
Tool/Environment: Jupyter Notebook


The goal is to create a simple data pipeline.
Input: A log file which contains each client request sent to a web server.
Output: A CSV file with the extracted data from the log file and its analysis

Each entry in the log follows the below convention:
$remote_addr - $remote_user [$time_local] "$request" $status $body_bytes_sent "$http_referer" "$http_user_agent"

•	$remote_addr — the ip address of the client making the request to the server.
•	$remote_user — if the client authenticated with basic authentication, this is the user name. Blank in the first log line.
•	$time_local — the local time when the request was made. 09/Mar/2017:01:15:59 +0000 in the first line.
•	$request — the type of request, and the URL that it was made to. GET /blog/assets/css/jupyter.css HTTP/1.1 in the first line.
•	$status — the response status code from the server. 200 in the first line.
•	$body_bytes_sent — the number of bytes sent by the server to the client in the response body. 30294 in the first line.
•	$http_referrer — the page that the client was on before sending the current request. http://www.dataquest.io in the first line.
•	$http_user_agent — information about the browser and system of the client. Mozilla/5.0 (Windows CE) AppleWebKit/5332 (KHTML, like Gecko) Chrome/13.0.864.0 Safari/5332 in the first line.

The sequence of tasks in pipeline include:
1.	Reading the log file, splitting each entry and extracting fields
2.	Formatting the entries and writing it into a csv file
3.	Running analysis on the csv file (eg:countting unique request types)



Please contact me for any more information at
fathimanazimudeen@gmail.com