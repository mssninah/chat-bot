# chat-bot
S5- PROJECT 


docker start oracle-xe-11g
docker exec -it oracle-xe-11g bash
sqlplus system/oracle@XE

	docker cp "/home/ninah/cluster/chat-bot/base.dmp" oracle-xe-11g:/tmp/base.dmp


sqlplus system/oracle@XE
  CREATE USER gallois IDENTIFIED BY gallois;
    GRANT DBA TO gallois;


sqlplus gallois/gallois
	imp gallois/gallois@localhost:1521/xe FILE=/tmp/base.dmp FULL=YE