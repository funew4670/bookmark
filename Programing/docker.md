
https://hub.docker.com/_/mysql <br/>
https://gitlab.com/GammaRayStudio/DevDoc/-/blob/master/DevTool/001-1.docker-mysql.md <br/>

docker pull nouchka/sqlite3
docker run --name sqlite -it nouchka/sqlite3
docker stop sqlite

##啟動images 然後連結輸入輸出-i -a
docker start -ai sqlite   

##複製db
docker cp F:\download\finance.sqlite\finance.sqlite sqlite:/finance.sqlite

##
sqlite> .help
sqlite> .open /root/db/finance.sqlite
sqlite> .tables
sqlite> select * from xxx limit 10
