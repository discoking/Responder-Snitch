# Responder-Snitch
Windows agent to detect when Responder is being run on a network

There are Linux scripts that can be used to detect responder, but no open source programs that can do it on Windows. The attempt of this project is to create a windows agent using the win32 api. It will send out random canary LLMNR requests, if a response is recieved then we know that someone is running responder, and we can send an alert to the logs, email, splunk, etc.
