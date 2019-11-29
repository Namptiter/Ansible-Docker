#Nam ptiter
##Check mySQL
```bash
$ docker exec -it mysql_1 mysql -uroot -p
```

##Install mysql in node 1:
```bash
$ ansible-playbook -i inventory_mysql mysql.yml -l mysql --ask-become-pass
```

##Install wordpress in node 2:
```bash
$ ansible-playbook -i inventory_wp wordpress.yml -l wordpress --ask-become-pass
```
