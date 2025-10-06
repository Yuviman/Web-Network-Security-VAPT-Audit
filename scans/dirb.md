# dirb
Since we found out that there is a http service running in the mercury virtual machine lets try directory busting the http service
- dirb http://192.168.56.102:8080
- dirb http://192.168.56.102:8080 -X .txt

Here we can even specifically mention to only search for text files with the help of .txt extension by using the flag -X.

Then we find out that there is a robots.txt file that none of the directories, thus we cant crawl into any pages of the website.

(Add Screenshot)
