# mona-linux-extract-inforamtion-5



Questions -

1.Extract log.tar.gz

2.Look for unauthorized connection attempts

3.Extract the usernames an attacker tried to use

4.Create a file containing these names(and make it orgnized)

5.use tools you've learned about to explore and process the log

Solutions - ~/Documents/Exercise Files$ tar -xvf log.tar.gz ~/Documents/Exercise Files$ cat auth.log | grep "input_userauth_request |awk '{print $9}' | sort -u > users.txt
