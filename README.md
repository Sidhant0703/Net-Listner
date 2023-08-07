# Net-Listner
A simple python programed alternative for netcat. Net-Listner is an networking utility with the help of TCP/IP protocol which reads and writes data across network connections. It is built as a secure back-end tool and can be used to send files from a client to a server and back directly with other programmes and scripts.

# How To Install
git clone https://github.com/Sidhant0703/Net-Listner.git

# Usage
>> python3 net-listner.py -h
 
usage: net-listner.py [-h] [-c] [-e EXECUTE] [-l] [-p PORT] [-t TARGET]
                      [-u UPLOAD}

optional arguments:
  -h, --help            show this help message and exit
  
  
  -c, --command         command shell
 
  
  -e EXECUTE, --execute EXECUTE
                        execute specified command
  
  
  
  -l, --listen          listen
 
  
  
  -p PORT, --port PORT  specified port
 
  
  
  -t TARGET, --target TARGET
                        specified IP

  
  
  -u UPLOAD, --upload UPLOAD
                        upload file

# Example:
net-listner.py -t 192.8.7.11 -p 1234 -l -c # command shell



net-listner.py -t 192.8.7.11 -p 1234 -l -u=mytest.txt # upload to file



net-listner.py -t 192.8.7.11 -p 1234 -l -e="cat /etc/passwd" # execute command


echo 'ABC' | ./net-listner.py -t 192.8.7.11 -p 1234 -l -c # echo text to server port 135


net-listner.py -t 192.8.7.11 -p 1234 # connect to server
