### questions
# POST
curl http://127.0.0.1:5000/questions -F "content=1111" -F "created_by=222" -F "updated_by=3333" -F "state=0" -F "created_at=8888" -F "updated_at=9999"

curl http://127.0.0.1:5000/questions -F "content=問題投稿" -F "created_by=himejima" -F "updated_by=投稿者" -F "state=0" -F "created_at=2014/13/31 11:13:99" -F "updated_at=2022/11/21"

# new version
curl http://127.0.0.1:5000/questions -F "content=問題の中身" -F "created_by=himejima" -F "updated_by=投稿者" -F "state=0" 
curl http://127.0.0.1:5000/questions -F "content=問題の中身2" -F "created_by=himejima2" -F "updated_by=投稿者2" -F "state=1" 

# DELETE
$ curl http://localhost:5000/questions/1 -X DELETE

# PUT
$ curl http://localhost:5000/questions/2 -X PUT -F "content=update問題" -F "state=1" -F "created_by=up_himejima" -F "updated_by=poster_up" -F "created_at=2013/12/11" -F "updated_at=2011/03/22"
$ curl http://localhost:5000/questions/2 -X PUT -F "content=update問題1" -F "state=0" -F "updated_by=アップデーター1"


### operations
# POST
curl http://127.0.0.1:5000/operations -F "username=username1" -F "password=password1" -F "state=0"
curl http://127.0.0.1:5000/operations -F "username=username2" -F "password=password2" -F "state=1"

# PUT
curl http://127.0.0.1:5000/operations/1 -X PUT -F "username=update_username1" -F "password=update_password1" -F "state=1"

# DELETE
$ curl http://localhost:5000/operations/1 -X DELETE

### answers
# POST
curl http://127.0.0.1:5000/answers/1 -F "content=解答1" -F "state=0" -F "created_by=himejima1" -F "updated_by=himejima"

# PUT
curl http://127.0.0.1:5000/answers/1/1 -X PUT -F "content=解答1www" -F "state=1" -F "updated_by=updater"

# DELETE
$ curl http://localhost:5000/answers/1/1 -X DELETE

### informations
# POST
curl http://127.0.0.1:5000/informations -F "content=contetnwwwww" -F "state=0" -F "created_by=投稿者ll" -F "updated_by=wwwww"

# PUT
curl http://127.0.0.1:5000/informations/1 -X PUT -F "content=update_content_testddd" -F "state=1" -F "updated_by=updaterdesu"

# DELETE
$ curl http://localhost:5000/informations/1 -X DELETE

### responses
# POST
$ curl http://127.0.0.1:5000/responses -F "type=ok" -F "content=contetnwwwww" -F "state=0" -F "created_by=投稿者ll" -F "updated_by=wwwww"

# PUT
$ curl http://127.0.0.1:5000/responses/1 -X PUT -F "type=ng" -F "content=update_content_testddd" -F "state=1" -F "updated_by=updaterdesu"

# DELETE
$ curl http://localhost:5000/responses/1 -X DELETE


# curlにいろいろ
http://d.hatena.ne.jp/thata/20100207/1265554365

