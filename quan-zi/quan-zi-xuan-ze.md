* 圈子选择使用场景：

  1. 用户注册后的圈子时的选择

  2. 用户添加圈子时的选择

* 接口地址：/section/select

* 提交方式：POST

* 接口参数：

  * register：1，场景1的时候则补充本字段，且字段值为1；场景2的时候则忽略本字段。

* 接口返回：

* 场景1的返回数据结构

* ```json
  {
      "code": 1,
      "data": [
          {
              "section_id": 1,
              "section_name": "33Talk",
              "section_avatar": "http://om4mfzope.bkt.clouddn.com/2017-03-24-15-12-28840?imageView2/2/w/200"
          },
          {
              "section_id": 2,
              "section_name": "TOKIO",
              "section_avatar": "http://om4mfzope.bkt.clouddn.com/2017-03-24-16-25-08127?imageView2/2/w/200"
          }
      ]
  }
  ```
* 场景2的返回数据结构

* ```json
  {
      "code": 1,
      "data": {
          "section_follow": [ //已经关注的圈子
              {
                  "section_id": 18,
                  "section_name": "AKB48",
                  "section_avatar": "http://om4mfzope.bkt.clouddn.com/2017-03-27-10-33-36759?imageView2/2/w/100"
              }
          ],
          "section_hot": [ //热门圈子
              {
                  "section_id": 423,
                  "section_name": "吐槽区",
                  "section_avatar": "http://om4mfzope.bkt.clouddn.com/2017-03-27-18-00-51514?imageView2/2/w/100",
                  "is_follow": 0
              },
              {
                  "section_id": 425,
                  "section_name": "面基区",
                  "section_avatar": "http://om4mfzope.bkt.clouddn.com/2017-03-27-17-59-19604?imageView2/2/w/100",
                  "is_follow": 0
              }
          ],
          "section_category": [ //圈子分类
              {
                  "section_category_id": 1,
                  "section_category_name": "band",
                  "section_avatar": "http://om4mfzope.bkt.clouddn.com/category_1.jpg"
              },
              {
                  "section_category_id": 2,
                  "section_category_name": "musician",
                  "section_avatar": "http://om4mfzope.bkt.clouddn.com/category_2.jpg"
              }
          ]
      }
  }
  ```



