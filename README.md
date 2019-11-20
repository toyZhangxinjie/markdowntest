# markdowntest

<details>
<summary>前台接口</summary>

### 行业

</details>

region { 前台接口

**所有前台接口的`headers`中`Cookie(SMM_auth_token)`和`X-API-KEY`表示登录token  
`SMM_auth_token`为pc端使用  
`X-API-KEY`为移动端或小程序使用**

  region { 行业
    region { 查询所有启用的行业列表
      **接口描述**

查询所有启用状态的行业列表；

`启用` 用户可选； `禁用` 用户不可选，行业不可用；该属性优先`显示`、`隐藏`

`显示` 前台可以看到； `隐藏` 作为查询条件时不显示，但是作为表单内条件时可以显示。如完善名片时可以显示隐藏的行业，但是查询名片时行业的选择列表中不会有隐藏的行业

**请求描述**

**GET**  industry/enable/list



**响应描述**

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 5,
            "industry_name": "测试003",
            "status": 2, // 1显示 2隐藏
            "disable": 1, // 1启用 2禁用
            "card_num": 0,
            "sort": 1,
            "create_admin": "test@smm.cn",
            "update_admin": "test@smm.cn",
            "create_time": 1568701331,
            "update_time": 1568701887
        }
    ]
}
```
    }
  }
  region { 企业店铺
    region { 获取企业店铺
    
    }
  }
}
