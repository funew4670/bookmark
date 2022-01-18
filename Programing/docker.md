
https://hub.docker.com/_/mysql <br/>
https://gitlab.com/GammaRayStudio/DevDoc/-/blob/master/DevTool/001-1.docker-mysql.md <br/>

docker pull nouchka/sqlite3 <br/>
docker run --name sqlite -it nouchka/sqlite3 <br/>
docker stop sqlite <br/>

##啟動images 然後連結輸入輸出-i -a <br/>
docker start -ai sqlite    <br/>

##複製db <br/>
docker cp F:\download\finance.sqlite\finance.sqlite sqlite:/finance.sqlite <br/>

## <br/>
sqlite> .help <br/>
sqlite> .open /root/db/finance.sqlite <br/>
sqlite> .tables <br/>
sqlite> select * from xxx limit 10 <br/>
