## To kill existing Python3 webserver process in Linux:

`ps -fA | grep "python3\|http.server" | awk -F ' ' '{print $2}' | head -1`

Use to get process ID of existing python server, if it exists. If such a process does not exist, it will simply output the process of this command.

Then use `kill <process-id>` to kill process.

---

The reason why pages might look different using `http` versus using `https` might be due to the website not loading the stylesheets (CSS). In my case, my stylesheet used a Yahoo API over `http` which was not allowed.

Link: https://teamtreehouse.com/community/http-vs-https-same-page-looks-different
