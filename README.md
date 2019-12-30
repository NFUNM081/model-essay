# PRD_model-essay App

| 发布日期 | 2019-12-3 |
| --------   | -----:  |
| 史诗 | 范文 | 
| 文件状态 | 基本完成 | 
| 文件主人 | 吴玮馨 | 
| 领头的设计师  | 吴玮馨 | 
| 领头的开发者  | 吴玮馨 | 
| 领头的测试者  | 吴玮馨 | 

## 一、价值主张设计
### 1. 加值宣言
中学时期，老师每次批改完作文，总会想要拿一些优秀同学的优秀作文来向大家展示，供大家学习参考。但是作文是同学们手写的，字体可能会不太好看，而且只有一份。老师评讲的时候如果复印一人一份又会浪费很多纸张。这个app运用了百度-手写文字识别API和百度-文章分类API。用户把手写版文章的照片上传到app，通过手写文字识别API，对图片中的手写中文、手写数字进行检测和识别，针对不规则的手写字体进行专项优化，将手写的文字转化成电子版文字，再通过文章分类API，对文章按照内容类型进行自动分类。从而让用户节省了要复印的纸张，和省下了手打成电子版文字的时间，也方便了用户寻找不同类型的优秀范文。

优先级：依托百度优秀的图像处理技术和海量优质数据，通过百度-手写文字识别API，对图片中的手写中文、手写数字进行检测和识别，支持识别各种不规则手写字体，并对字迹潦草、模糊等情况进行专项优化。

次优先：文章分类服务对文章内容进行深度分析，输出文章的主题一级分类、主题二级分类，如娱乐、社会、音乐、人文、科学、历史、军事、体育、科技、教育等分类结果。通过百度-文章分类API，对文章按照内容类型进行自动分类。

### 2. 核心价值
本产品着眼于解决用户手打文字浪费时间的问题，用户不知道去哪里寻找不同类型的范文的问题，以及浪费纸张的问题。

### 3. 用户
需要寻找不同类别的范文作为参考的人，以及需要不想浪费打文字时间的用户。

### 4.使用场景 

- 老师评讲作文的时候，不想要打印全班人的份数，将范文拍照，识别成电子版，发布到APP上。
- 老师评讲作文的时候，没有好的范文，在APP上按照不同的类别寻找范文。
- 学生写作文遇到瓶颈的时候，在APP上按照不同的类别寻找范文，以供学习。

### 5. 核心价值与用户痛点
- 老师要评讲作文，要帮每位同学都复印一份范文，浪费很多纸张。
- 老师即使帮每位同学都复印一份范文,范文的字体可能并不那么端正，同学们看得不太清晰。
- 老师讲范文逐字打成电子版要浪费很多时间。
- 同学们寻找不同类型的范文，不知道要去哪个地方全部找得到。

### 6. 人工智能概率性与用户痛点
#### 百度文字识别技术-手写文字识别，有二个保证：
- 准确率高:依托百度优秀的图像处理技术和海量优质数据，支持识别各种不规则手写字体，并对字迹潦草、模糊等情况进行专项优化，手写中文识别准确率可达90%以上。
- 服务稳定:依托百度云技术实力，提供高可靠性、弹性可伸缩、高并发承载的文字识别服务，服务可用性高达99.99%。

#### 百度自然语言处理技术-文章分类，有三个保证：
- 整体精度高：基于大数据的深度学习，自动学习深层次的语义及语序特征，文章主题分类的精确度高。
- 覆盖率高：文章主题分类对网络文章覆盖率可达95%。
- 粒度完整：文章主题分类包含一级分类和二级分类两种粒度，层次清晰，满足各类应用需求。

#### 所以，该产品利用了手写文字识别通过拍出来的图片识别书图片中的手写文字，文章分类通过对文章按照内容类型进行自动分类。这两个功能技术转换精确率较高，都达到了90%，甚至95%，普遍情况下都可以使用。
### 7. 需求列表与人工智能API加值
| 用户案例	| API接口	| 重要程度 |
| -- | -- | -- |
| 用户不想输入很多的文字 	| 手写文字识别 	| 重要 |
| 用户字体不太端正，想让别的用户看得更加清楚	| 手写文字识别	| 重要 |
| 用户想要寻找不同类型的范文	| 文章分类	| 重要 |
| 用户不想复印很多纸张，避免浪费 	| 手写文字识别 	| 次重要 |

## 二、原型

### [原型文档交互展示](https://nfunm081.github.io/prototype-model-essay/)
### [原型文档下载区](https://github.com/NFUNM081/prototype-model-essay)


### 1. 产品流程图
![范文APP产品流程图](https://images.gitee.com/uploads/images/2019/1230/161438_158db02e_1922090.jpeg "范文APP产品流程图.jpg")

### 2. 产品功能结构图
![范文APP功能结构图](https://images.gitee.com/uploads/images/2019/1222/035837_bebf3a76_1922090.png "范文APP功能结构图.png")

### 3. 产品信息结构图
![范文APP信息结构图](https://images.gitee.com/uploads/images/2019/1222/035852_1b084f5f_1922090.png "范文APP信息结构图.png")

## 三、API 产品使用关键AI或机器学习之API的输出入展示
### 1. 使用水平
1. 百度API：
计算机视觉-文字识别——手写文字识别
- 接口描述：对手写中文汉字、数字进行识别
- HTTP 方法：POST
- 请求URL： https://aip.baidubce.com/rest/2.0/ocr/v1/handwriting
- 输入
```
代码示例
import json
import requests
import base64
import urllib.parse

APP_ID = '17992576'
API_KEY ='aYZxrzH8qGVBcwSAZOVdhivS'
SECRECT_KEY = 'U206MT7Kjb22dGvFWIU1zHDQE2YxLaFZ'

# 获取token
url = 'https://aip.baidubce.com/oauth/2.0/token'
body = {'grant_type': 'client_credentials',
        'client_id': API_KEY,
        'client_secret': SECRECT_KEY
        }

req = requests.post(url=url, data=body)
token = json.loads(req.content)['access_token']

# 获取百度api识别结果
ocr_url = 'https://aip.baidubce.com/rest/2.0/ocr/v1/general_basic?access_token=%s'%token
headers = {'Content-Type': 'application/x-www-form-urlencoded'}

# 读取图片并进行base64加密
body = base64.b64encode(open('./handwrite.png' ,'rb').read())
# 进行urlencode
data = urllib.parse.urlencode({'image': body})

# post请求
r = requests.post(url=ocr_url, headers=headers, data=data)

# 输出请求结果
print('请求码为: %s' %r.status_code)
res_words = json.loads(r.content)['words_result'][0]['words']
print('识别结果为: %s' % res_words)
```
- 输出
```
请求码为: 200
识别结果为: 《演讲的力量》
```
需要逐行输出

2. 百度API：
自然语言处理——文章分类
- 接口描述：对文章按照内容类型进行自动分类
- HTTP 方法：POST
- （通用版）请求URL: https://aip.baidubce.com/rpc/2.0/nlp/v2/comment_tag
- 输入
```
import urllib, urllib.request, sys
import ssl

# client_id 为官网获取的AK， client_secret 为官网获取的SK
host = 'https://aip.baidubce.com/oauth/2.0/token?grant_type=client_credentials&client_id=aYZxrzH8qGVBcwSAZOVdhivS&client_secret=U206MT7Kjb22dGvFWIU1zHDQE2YxLaFZ'
request = urllib.request.Request(host)
request.add_header('Content-Type', 'application/json; charset=UTF-8')
response = urllib.request.urlopen(request)
content = response.read()
if (content):
    print(content)
```
```
import json
{
"title":"欧洲冠军联赛",
"content": "欧洲冠军联赛是欧洲足球协会联盟主办的年度足球比赛，代表欧洲俱乐部足球最高荣誉和水平，被认为是全世界最高素质、最具影响力以及最高水平的俱乐部赛事，亦是世界上奖金最高的足球赛事和体育赛事之一。"
}
request_url = "https://aip.baidubce.com/rpc/2.0/ai_custom/v1/text_cls/orgclassify"
params = json.dumps({"text":text,"top_num": 6}).encode("utf-8")

access_token = '24.d10428f4f1c00f70b467c81f55779680.2592000.1578586839.282335-17992576’
request_url = 'https://aip.baidubce.com/rpc/2.0/ai_custom/v1/text_cls/orgclassify?access_token=24.d10428f4f1c00f70b467c81f55779680.2592000.1578586839.282335-17992576'
request = urllib.request.Request(url=request_url, data=params)
request.add_header('Content-Type', 'application/json')
response = urllib.request.urlopen(request)
content = response.read()
if content:
    resu=eval(str(content,'utf-8'))
    
    print (resu['results'][0]['name'],resu['results'][0]['score'])
    print(resu['results'])
```
- 输出
```
{
    "log_id": 3591049593939822907,
    "item": {
        "lv2_tag_list": [
            {
                "score": 0.877436,
                "tag": "足球"
            },
            {
                "score": 0.793682,
                "tag": "国际足球"
            },
            {
                "score": 0.775911,
                "tag": "英超"
            }
        ],
        "lv1_tag_list": [
            {
                "score": 0.824329,
                "tag": "体育"
            }
        ]
    }
}
```


### 2. 使用比较分析
#### 手写文字识别
- 百度-手写文字识别API
![百度价格](https://images.gitee.com/uploads/images/2019/1230/223516_2cea3ab9_1922090.png "5e986e009f7b013005180a3188b2220.png")

- 讯飞-手写文字识别API
![讯飞价格](https://images.gitee.com/uploads/images/2019/1230/223601_e14edb86_1922090.png "bf19b66b7266d43edec40ab76ad81a3.png")

| 调用量\价格 | 百度价格            | 讯飞价格|
| ----------- | ------------------- | ----- |
| 1万         | 0.01*10000=100      | 350   |
| 10万        | 0.0065*100000=650   | 3200  |
| 100万       | 0.0045*1000000=4500 | 30000 |

在调用难度上来说，都有明确的调用文档说明以及步骤。在价格上来说，百度比讯飞便宜很多。所以，该项目选择的是百度的API。


### 3. 使用后风险报告
- 手写文字识别中，虽然针对不规则的手写字体进行专项优化，手写中文识别准确率可达90%以上，但是仍然有识别错误的可能，此时会需要用户手动修改识别到的文章错误内容。而且需要逐行输出识别内容，可能需要的时间会长一些。
- 文章分类中，输出文章的主题一级分类、主题二级分类，如一级分类是体育，二级分类是足球、国际足球、英超。能识别出的二级分类较多，若一篇文章里不止提到一种分类，不论一级还是二级，难以识别最主要的类别。

