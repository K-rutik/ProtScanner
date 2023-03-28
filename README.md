# ProtScanner
The code you provided is a Python script for performing port scanning on a target host.

The script imports the socket module which is used for creating network sockets, and defines two functions:

conScan function: It creates a TCP socket and tries to establish a connection to the target host and port. If the connection is successful, it prints a message indicating that the port is open, and closes the socket. If the connection fails, it prints a message indicating that the port is closed.

portScan function: It takes the target host and a list of target ports as input parameters. The function first resolves the IP address of the target host using the gethostbyname function. It then uses the gethostbyaddr function to try to resolve the hostname of the target IP address. If it is unable to resolve the hostname, it prints the IP address instead.

The function then loops through each target port in the list, and calls the conScan function to try to establish a connection to the target host and port.

Finally, the script calls the portScan function with the target host 'google.com' and a list of four ports [80, 22, 21, 443] to perform the port scanning.

Note that port scanning without permission is generally considered unethical and could potentially be illegal. It's important to obtain permission before conducting any type of port scanning activity.
