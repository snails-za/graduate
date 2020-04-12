# 熊猫之家（原型爱彼迎APP）接口文档



### base_url:

### 1、获取短信验证码接口

| URL    | METHOD | PARAMS |
| ------ | ------ | ------ |
| /code/ | GET    | phone  |

#### 短信发送成功：

###### 	{'state': 0, 'msg':'' 验证码已发送''}

#### 短信发送失败：

##### 	{'state': 1,    'msg': '手机号不能为空'}

##### 	{'state': 2,    'msg': '获取验证码失败'}

### 2、用户注册接口

| URL        | METHOD | PARAMS               |
| ---------- | ------ | -------------------- |
| /register/ | POST   | name ,phone,password |





### 3、普通用户升级为会员用户接口

| URL                | METHOD | PARAMS |
| ------------------ | ------ | ------ |
| /become_superuser/ | GET    | token  |



### 4、用户修改密码接口

| URL               | METHOD | PARAMS                                |
| ----------------- | ------ | ------------------------------------- |
| /modify_password/ | POST   | new_password_str，password_str，token |



### 5、用户注销接口

| URL         | METHOD | PARAMS |
| ----------- | ------ | ------ |
| /login_out/ | POST   | token  |



### 6、用户头像上传接口

| URL           | METHOD | PARAMS     |
| ------------- | ------ | ---------- |
| /upload_head/ | POST   | head,token |



### 7、更新用户信息接口

| URL               | METHOD | PARAMS |
| ----------------- | ------ | ------ |
| /detail_resource/ | POST   | token  |



### 8、用户积分查询接口

| URL        | METHOD | PARAMS |
| ---------- | ------ | ------ |
| /integral/ | GET    | null   |



### 9、关于我们接口

| URL            | METHOD | PARAMS |
| -------------- | ------ | ------ |
| /about_pandas/ | GET    | token  |





### 10、查看合同接口

| URL            | METHOD | PARAMS |
| -------------- | ------ | ------ |
| /get_contract/ | GET    | token  |



### 11、查看交易记录接口

| URL           | METHOD | PARAMS |
| ------------- | ------ | ------ |
| /traderecord/ | GET    | token  |



### 12、查看订单接口

| URL         | METHOD | PARAMS |
| ----------- | ------ | ------ |
| /get_order/ | GET    | token  |



### 13、查看代金券接口

| URL    | METHOD | PARAMS |
| ------ | ------ | ------ |
| /cash/ | GET    | token  |



### 14、首页轮播图接口

| URL     | METHOD | PARAMS |
| ------- | ------ | ------ |
| /slide/ | GET    | token  |



### 15、首页房屋展示接口

| URL             | METHOD | PARAMS |
| --------------- | ------ | ------ |
| /house_display/ | GET    | token  |



### 16、房屋详细信息页接口

| URL            | METHOD | PARAMS |
| -------------- | ------ | ------ |
| /house_detail/ | GET    | token  |



### 17、收藏房屋接口

| URL                 | METHOD | PARAMS   |
| ------------------- | ------ | -------- |
| /insert_collection/ | POST   | house_id |



### 18、查询收藏房屋信息接口

| URL              | METHOD | PARAMS |
| ---------------- | ------ | ------ |
| /get_collection/ | GET    | token  |



### 19、添加订单接口

| URL     | METHOD | PARAMS                                                       |
| ------- | ------ | ------------------------------------------------------------ |
| /order/ | POST   | user_id,house_id,hire_price,cash_price,enter_time,enter_time,exit_tiem |



### 20、删除订单接口

| URL         | METHOD | PARAMS              |
| ----------- | ------ | ------------------- |
| /del_order/ | POST   | token, order_number |



### 21、全部订单接口

| URL         | METHOD | PARAMS |
| ----------- | ------ | ------ |
| /all_order/ | GET    | token  |





### 22、添加评论接口

| URL           | METHOD | PARAMS                 |
| ------------- | ------ | ---------------------- |
| /add_comment/ | POST   | token,content,house_id |





### 23、删除评论接口

| URL           | METHOD | PARAMS           |
| ------------- | ------ | ---------------- |
| /del_comment/ | POST   | token,comment_id |





### 24、添加投诉接口

| URL             | METHOD | PARAMS                               |
| --------------- | ------ | ------------------------------------ |
| /add_complaint/ | POST   | token，order_id，phone,content,email |





### 25、删除投诉接口

| URL             | METHOD | PARAMS            |
| --------------- | ------ | ----------------- |
| /del_complaint/ | POST   | token,fadeback_id |



### 26、发布房屋接口

| URL   | METHOD | PARAMS                                               |
| ----- | ------ | ---------------------------------------------------- |
| /add/ | POST   | image，name,type,address,price,area,descrition,token |





### 27、删除房源信息接口

| URL         | METHOD | PARAMS         |
| ----------- | ------ | -------------- |
| /del_house/ | POST   | token,house_id |



### 28、编辑房源信息接口

| URL                 | METHOD | PARAMS                                                       |
| ------------------- | ------ | ------------------------------------------------------------ |
| /change_house_info/ | POST   | image,name,type,address, price,area,description,token,house_id |









### 29、查看房东房源信息

| URL           | METHOD | PARAMS |
| ------------- | ------ | ------ |
| /list_houses/ | GET    | token  |



### 30、查看所有房源信息接口

| URL               | METHOD | PARAMS |
| ----------------- | ------ | ------ |
| /list_all_houses/ | GET    | token  |





### 31、查看房屋详情接口

| URL      | METHOD | PARAMS |
| -------- | ------ | ------ |
| /detail/ | GET    | token  |





### 





