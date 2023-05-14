![First start the machine](1.png) First start the machine
![yo](1.1.png)
Then ping it to see it it's working or not
![yo](2.png) Check the server by just typing the ip address on the browser
![ctf](3.png)check for the page source on the browser like this I found this
![ctf](3-1.png) check for the website vulurnerablity on NMAP I found 2 open ports ssh and html
![ctf](4.png) for the directory bruteforce I used common.txt wordlist
![ctf](6.png) by using gobuster directory bruteforce we found that there is /sitemap let's try what it have.
![ctf](5.png) the web site /sitemap is like this I found nothing on it so let's bruteforce again by specifying /sitemap
![ctf](7.png) like this
![ctf](8.png) and here we found /.ssh so let's try this
![ctf](9.png) the .ssh result is like this let's check what id_rsa have
![ctf](10.png) wow and here we got the private key therefor we can attempt to login with this
![ctf](11.png) first let's save the file
![ctf](12.png) we just loged in with the id_rsa the next mission is to find user_flag we'll just use the find command for that
![ctf](13.png) as you can see here we found the user_flag on documents directory let's check what's in it
![ctf](14.png) here the .txt file got the user_flag so let's just copy and paste it to tryhackme and mission 1 is completed.
![ctf](15.png) here I found that I can access root without the need to know the password as it say's right there so let's do it
![ctf](16.png) let's create a listening port and wait in the other terminal
![ctf](17.png) by using this we got the root_flag on the listner let's copy and paste that on the tryhackme
![ctf](18.png) done Mission completed 