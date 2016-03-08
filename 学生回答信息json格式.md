# 学生回答信息json格式
- 用于记录某个学生对某一题的回答情况
- 当前保存在ibm gitlab上，路径为teacher/answer

teacher/answer路径说明:
- 数据的路径格式为`{email.md5[-2:]}/{username}/{q_number}/{q_number}.json`
- `email.md5[-2:]`表示对email取md5编码的最后两位
- 对于一个学生（ email=test@test.com,username=student），其对于题号为101的题目(q_number=101)的回答情况json的路径为`52/student/101/101.json`

## Json格式说明

|字段|说明|备注|
|---|---|---|
|knowledge|知识点,为字符串数组|必选|

### 实例

```json
    {
        "student":{
        
        }
    }
```
