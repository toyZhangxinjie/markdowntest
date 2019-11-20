# 商机后端接口文档

 商机2.0接口是在1.0版本的基础上改的，所以有些接口如果链接相同则以2.0的文档为准。

Postman接口文档地址：https://www.getpostman.com/collections/6f49e3cfa39a28a72b4b

* [前台接口](#item_qiantaijiekou_659925000)

	* [行业](#item_xingye_659973000)

		* [查询所有启用的行业列表](#industry.enable.list)

		* [查询所有启用且显示的行业](#industry.show.list)

		* [查询单个行业](#industry.info.id)

	* [企业店铺](#item_qiyedianpu_660004000)

		* [获取企业店铺](#vipCompany.info)

		* [判断当前用户是否是企业管理员](#vipCompany.isAdmin)

		* [设置企业图片](#vipCompany.pic.setting)

		* [获取系统默认企业背景图](#vipCompany.background.system)

		* [最新开通店铺的企业](#vipCompany.latest)

		* [设置企业主题简介等](#vipCompany.edit)

		* [前台用户开通店铺](#vipCompany.openshop)

		* [根据分类获取对应的企业店铺](#vipCompany.category)

		* [分类页](#vipCompany.category)

	* [商友圈](#item_shangyouquan_660719000)

		* [根据圈子名称获取圈子ID](#club.by_name)

		* [按条件查询圈子列表](#club.list)

		* [热门圈子列表](#club.hot.list)

		* [圈子详情](#club.info.club_id)

		* [圈子成员列表](#club.members)

		* [编辑圈子logo](#club.logo.edit)

		* [编辑圈子背景图](#club.background.edit)

		* [圈主同意加圈请求](#club.join.approve)

		* [圈主拒绝加圈请求](#club.join.reject)

		* [圈主踢成员出圈](#club.member.clean_out)

		* [编辑圈子简介](#club.edit)

		* [编辑加圈是否需要圈主审核](#club.audit.edit)

		* [加入圈子](#club.join_apply)

		* [用户退出圈子](#club.leave)

		* [申请建圈子](#club.create_apply)

		* [查询公告列表](#club.notice)

		* [批量更新圈子成员数](#load_club_member_amount)

		* [批量更新圈内帖子数](#load_club_post_amount)

		* [圈子sitmap列表](#club.sitmap.list)

		* [获取企业所有圈子](#club.company.list)

		* [分类页圈子列表](#club.category)

	* [分类](#item_fenlei_661517000)

		* [查询分类属性](#category.query_attribute_list)

		* [根据分类获取关系关联的分类](#category.relation_category_list)

		* [获取用户历史选择的分类列表](#category.history.list)

		* [获取所有分类（多级嵌套结构）](#category.nesting.all.list)

		* [获取所有一级分类下所有后代的推荐分类](#category.recommend.list)

		* [根据子级分类ID获取所有父级列表](#category.parent.list)

		* [根据关键词搜索最后一级分类](#category.last_level.list)

		* [获取企业所有分类](#category.company.list)

		* [获取分类详情](#category.info.category_id)

		* [根据分类名称查询分类ID](#category.by_name)

		* [根据分类获取同级别的其他分类](#category.other.list)

	* [名片 ](#item_mingpian_661680000)

		* [根据用户ID获取名片](#usercard.info)

		* [完善名片信息](#usercard.completed)

		* [递名片](#usercard.submit)

		* [名片墙](#usercard.wall)

		* [名片夹](#usercard.clip)

		* [搜索名片](#usercard.search)

		* [名片请求列表](#usercard.request)

		* [同意递名片（加好友）请求](#usercard.agree)

		* [添加名片分组](#usercard.group.add)

		* [根据分组获取名片夹名片](#usercard.group)

		* [获取登录用户的名片分组](#usercard.group.list)

		* [编辑名片分组](#usercard.group.edit)

		* [删除名片分组](#usercard.group.del)

		* [设置名片夹名片分组](#usercard.group.set)

		* [ocr识别名片](#usercard.ocr)

		* [查看其他人名片详情/usercard/look](#usercard.look)

		* [谁看过我列表](#usercard.look_me)

		* [获取通讯录](#usercard.address.book)

		* [根据企业店铺获取联系人名片列表](#usercard.list.company)

		* [根据批量用户ID获取名片或用户中心的头像和名称](#usercard.info_by_user_ids)

		* [金属产业链-根据分类关联行业查询名片](#user_card.company_by_category)

		* [邀请用户加入有色名片](#user_card.invite_join)

		* [名片识别并切割](#usercard.ocr_crop)

	* [帖子信息](#item_tiezixinxi_663582000)

		* [圈子主页帖子列表](#post.club)

		* [分类主页](#post.category.list)

		* [按条件查询帖子列表](#post.list)

		* [帖子详情](#post.info.post_id)

		* [帖子详情推荐帖子](#post.recommend)

		* [设置帖子在圈子中置顶](#post.settle.top)

		* [取消置顶圈子中的帖子](#post.cancel.top)

		* [设置公告帖子信息](#post.settle.notice)

		* [取消公告帖子信息](#post.cancel.notice)

		* [修改帖子报价](#post.alter.price)

		* [刷新帖子时间](#post.refresh.time)

		* [删除帖子](#post.delete.id)

		* [发布帖子信息](#post.publish)

		* [编辑帖子信息](#post.edit)

		* [帖子模版](#post.template)

		* [m站推荐详情](#app.recommend.info)

		* [帖子sitmap列表](#post.sitmap.list)

		* [企点获取用户最新修改的5条帖子](#post.latest)

		* [根据用户ID获取最新的n条帖子](#post.exclude.latest)

		* [商机首页最新商品](#post.product.latest)

		* [首页企业动态](#post.other.vip)

		* [IP白名单获取帖子列表](#inner.post.list)

		* [个人主页搜索我的信息](#post.person)

		* [手机端](#post.app.my_club)

		* [获取信息关键词](#post.keywords)

	* [分享兑换](#item_fenxiangduihuan_667519000)

		* [获取当前登录用户可使用的兑换份额](#exchange.unused)

		* [分享份额兑换商机vip](#exchange)

		* [获取分享页兑换内容列表](#share.exchange.content)

		* [获取分享好友助力榜](#share.friend.boost)

		* [获取兑换记录列表](#exchange.list)

	* [其他 ](#item_qita_667646000)

		* [地区列表](#province)

		* [个人信息](#user.info)

		* [查询用户圈子角色](#user.club_role)

		* [获取用户圈子列表](#user.club_list)

		* [获取我的圈子列表](#my.club_list)

		* [获取关键词列表](#key_word_list)

		* [查询n天内发帖数量最多的m个用户](#active.user.list)

		* [获取新帖榜](#new.post.list)

		* [获取推荐用户榜](#recommend.user.list)

		* [前台上传图片](#upload.img)

		* [发送留言](#send.message)

		* [发送沟通请求](#send.communication)

		* [有色网首页商机板块](#clubcenter)

		* [有色网首页商机板块导航标签数据](#clubcenter.label_list.navID)

		* [有商推荐](#recommend.company)

		* [根据经纬度获取省市](#get_area)

		* [手机端商圈洽谈](#app.chat)

		* [为用户中心提供数据](#card_and_post)

	* [搜索](#item_sousuo_668602000)

		* [搜索圈子列表](#search.club_list)

		* [搜索圈子列表](#app.search.club_list)

		* [批量更新搜索帖子数据](#search.load_all_post)

		* [批量更新搜索圈子数据](#search.load_all_club)

		* [搜索帖子列表](#search.post_list)

		* [搜索帖子列表](#search.posts)

		* [企点根据关键词搜索帖子](#search.post.qidian)

		* [根据帖子标题搜索帖子重的公司](#search.company_list)

		* [搜索关键词列表](#search.key_word_list)

		* [批量更新关键词](#search.load_all_key_word)

	* [前台例子](#)

* [后台接口](#item_houtaijiekou_669071000)

	* [行业](#item_xingye_669132000)

		* [添加/保存行业](#admin.industry.save)

		* [查询行业列表](#admin.industry.list)

		* [禁用或启用行业](#admin.industry.disable)

		* [获取单个行业信息](#admin.industry.info.id)

		* [将行业名片迁移至其他行业](#admin.industry.migrate)

		* [手动同步行业关联名片数](#admin.industry.sync.card_num)

		* [批量保存行业排序](#admin.industry.batch_order)

	* [分类管理](#item_fenleiguanli_669198000)

		* [查询分类列表](#admin.category.get_category_list)

		* [保存分类](#admin.category.save_category)

		* [查询分类详情](#admin.category.get_category_info)

		* [启用/禁用分类](#admin.category.batch_disabled)

		* [显示/隐藏分类](#admin.category.batch_hide)

		* [设置获取消推荐分类](#admin.category.batch_recommend)

		* [迁移分类](#admin.category.migrate_category)

		* [查询分类属性列表](#admin.category.get_category_attribute_list)

		* [保存分类属性](#admin.category.save_category_attribute)

		* [查询分类关系列表](#admin.category.get_category_relation_list)

		* [保存分类关系](#admin.category.save_category_relation)

		* [批量删除分类关系](#admin.category.del_category_relation)

		* [查询分类关系详情](#admin.category.get_category_relation_info)

		* [查询关系类型列表](#admin.category.get_relation_list)

		* [保存关系](#admin.category.save_relation)

		* [删除关系类型](#admin.category.del_relation)

		* [查询关系类型详情](#admin.category.get_relation_info)

		* [批量保存分类排序](#admin.category.batch_order)

	* [圈子管理](#item_quanziguanli_669491000)

		* [查询圈子列表](#admin.club.list)

		* [添加/编辑圈子](#admin.club.add_or_edit)

		* [启用圈子](#admin.club.enable)

		* [禁用圈子](#admin.club.disable)

		* [设置推荐圈子](#admin.club.settle.recommend)

		* [取消推荐圈子](#admin.club.cancel.recommend)

		* [圈内成员列表](#admin.club.members)

		* [批量禁止或启用圈内成员](#admin.club.member.disable)

		* [获取所有加过圈子的用户](#admin.club.users)

		* [根据用户获取加入的圈子列表](#admin.club.list_by_member)

	* [名片管理](#item_mingpianguanli_669834000)

		* [获取审核名片列表](#admin.usercard.approval.list)

		* [获取单个名片审核记录](#admin.usercard.approval.info)

		* [批量审核名片](#admin.usercard.batch.approval)

		* [审核并编辑名片](#admin.usercard.approval)

		* [获取名片列表](#admin.usercard.list)

		* [根据用户ID获取名片](#admin.usercard.info)

		* [添加/编辑名片信息](#admin.usercard.save)

		* [获取某个名片的名片夹里的所有名片](#admin.usercard.relationship)

	* [会员管理](#item_huiyuanguanli_670137000)

		* [会员管理列表](#admin.vip.list)

		* [根据账号查询用户](#admin.vip.user)

		* [添加/编辑会员](#admin.vip.save)

		* [后台开通店铺](#admin.vip.openshop)

	* [店铺管理](#item_dianpuguanli_670211000)

		* [获取企业列表](#admin.vipCompany.list)

		* [编辑企业店铺信息](#admin.vipCompany.edit)

		* [获取企业图片审核列表](#admin.vipCompany.pic.list)

		* [批量审核企业图片](#admin.vipCompany.batch.pic)

		* [编辑企业图片](#admin.vipCompany.edit.pic)

		* [授权店铺编辑权限](#admin.vipCompany.auth.edit)

	* [分享管理](#item_fenxiangguanli_670275000)

		* [分享列表](#admin.share.list)

	* [搜索日志](#item_sousuorizhi_670304000)

		* [搜索日志](#admin.search.log.list)

	* [兑换列表](#item_duihuanliebiao_670327000)

		* [查询兑换记录列表](#admin.exchange.list)

	* [帖子管理](#item_tieziguanli_670349000)

		* [查询帖子列表](#admin.post.list)

		* [设置推荐帖子](#admin.post.settle.recommend)

		* [取消推荐帖子](#admin.post.cancel.recommend)

		* [删除帖子](#admin.post.delete)

		* [批量删除帖子](#admin.post.batch.delete)

		* [批量迁移帖子](#admin.post.batch.migrate)

		* [批量刷新](#admin.post.batch.refresh)

		* [全局刷新](#admin.post.global.refresh)

		* [获取待审核帖子列表](#admin.post.approval.list)

		* [批量审核帖子](#admin.post.batch.approval)

		* [编辑帖子并审核通过](#admin.post.save)

		* [查询帖子详情](#admin.post.info.id)

	* [其他](#item_qita_670735000)

		* [获取关键词列表](#admin.key_word_list)

		* [删除关键词](#admin.product_words.delete)

		* [设置商机首页推荐用户榜](#admin.recommend.user.setting)

		* [获取商机首页推荐用户ID](#admin.recommend.user.ids)

		* [后台上传图片](#admin.upload.pic)

		* [获取商机各个模块审核数据总数](#admin.approval.num.count)

	* [数据修复](#item_shujuxiufu_670850000)

		* [初始化所有老用户的名片](#admin.usercard.init.old)

		* [将导航和标签转换成分类](#admin.navbar_label.transfer.category)

		* [生成所有名片图片为空的名片图片](#admin.generate.user_card_url)

		* [导入商机用户名片](#admin.import.smm_user)

	* [例子](#admin)

* [内网接口](#item_neiwangjiekou_671436000)

	* [购买会员成功回调](#vip.pay_success)

	* [用户从分享连接注册回调](#share.reg)

	* [使用优惠券兑换商机会员](#coupon.use)

* [调用其他服务接口](#item_diaoyongqitafuwujiekou_671604000)

	* [[用户中心]查询企业列表/usercenter/inner/get_paged_company_list](#usercenter.inner.get_paged_company_list)

	* [[用户中心]获取用户信息/usercenter/inner/get_filter_user_and_company_list](#usercenter.inner.get_filter_user_and_company_list)

	* [大数据首页今日访客/get_flow_view_count](#get_flow_view_count)

	* [[用户中心]获取企业详情](#usercenter.inner.get_company_detail)

	* [获取企点用户/qidiancenter/get_users?user_ids=804792](#qidiancenter.get_users)

	* [分页获取通讯录](#inner.cards.list)

	* [用户通讯录名片](#inner.user_share_url)

	* [邀请用户加入有色名片短信vcode_center](#vcodecenter.inner.v3.send_csy_sms)

	* [云盾校验](#vcodecenter.inner.v3.check_validate_common)

	* [名片全能王](#BCRService.BCR_Crop)

	* [查询短信发送记录](#vcodecenter.inner.v3.get_notify_sms_send_log)

	* [名片全能王](#BCRService.BCR_VCF2)

	* [获取用户评论总数](#inner.comment.count)



### <a id="item_qiantaijiekou_659925000">前台接口</a>

**所有前台接口的`headers`中`Cookie(SMM_auth_token)`和`X-API-KEY`表示登录token  
`SMM_auth_token`为pc端使用  
`X-API-KEY`为移动端或小程序使用**

### <a id="item_xingye_659973000">行业</a>



---

#### <a id="industry.enable.list">API: 查询所有启用的行业列表</a>

**接口描述**

查询所有启用状态的行业列表；

`启用` 用户可选； `禁用` 用户不可选，行业不可用；该属性优先`显示`、`隐藏`

`显示` 前台可以看到； `隐藏` 作为查询条件时不显示，但是作为表单内条件时可以显示。如完善名片时可以显示隐藏的行业，但是查询名片时行业的选择列表中不会有隐藏的行业

**请求描述**

**GET**  industry/enable/list



<details>
<summary>响应描述</summary>

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
</details>

---

#### <a id="industry.show.list">API: 查询所有启用且显示的行业</a>

**接口描述**

查询所有启用状态的行业列表；

`启用` 用户可选； `禁用` 用户不可选，行业不可用；该属性优先`显示`、`隐藏`

`显示` 前台可以看到； `隐藏` 作为查询条件时不显示，但是作为表单内条件时可以显示。如完善名片时可以显示隐藏的行业，但是查询名片时行业的选择列表中不会有隐藏的行业

**请求描述**

**GET**  industry/show/list



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 6,
            "industry_name": "测试004",
            "status": 1, // 1显示 2隐藏
            "disable": 1, // 1启用 2禁用
            "card_num": 0,
            "sort": 1,
            "create_admin": "test@smm.cn",
            "update_admin": "test@smm.cn",
            "create_time": 1568701433,
            "update_time": 1568701879
        }
    ]
}
```
</details>

---

#### <a id="industry.info.id">API: 查询单个行业</a>

**接口描述**

查询所有启用状态的行业列表；

`启用` 用户可选； `禁用` 用户不可选，行业不可用；该属性优先`显示`、`隐藏`

`显示` 前台可以看到； `隐藏` 作为查询条件时不显示，但是作为表单内条件时可以显示。如完善名片时可以显示隐藏的行业，但是查询名片时行业的选择列表中不会有隐藏的行业

**请求描述**

**GET**  industry/info/:id

**参数描述**

path:

名称|类型|描述
---|---|---
id|int|行业ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "id": 3,
        "industry_name": "食品加工、销售",
        "status": 1, // 1显示 2隐藏
        "disable": 1, // 1启用 2禁用
        "card_num": 6, // 关联的名片数
        "sort": 222,
        "create_admin": "test@smm.cn",
        "update_admin": "test@smm.cn",
        "create_time": 1568701141,
        "update_time": 1568701938
    }
}
```
</details>

### <a id="item_qiyedianpu_660004000">企业店铺</a>



---

#### <a id="vipCompany.info">API: 获取企业店铺</a>

**请求描述**

**GET**  vipCompany/info

**参数描述**

query:

名称|类型|描述
---|---|---
company_id|int|企业ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "id": 24,
        "company_id": 1001150,
        "status": 2, // 店铺状态 0未开通 1过期 2服务中 3关闭
        "status_desc": "服务中",
        "year_base": 10, // 店铺服务年限
        "start_date": 1561910400, // 店铺开通开始时间
        "end_date": 1596124800, // 店铺开通结束时间
        "background_pic": "https://imgqn.smm.cn/production/club/company/system/picTkGMs20190712162917.png",
        "admin_email": "test@smm.cn",
        "open_person": "", // 店铺开通用户ID或后台管理员
        "update_time": 1569314408,
        "style_config": "{\"hide_title\":false,\"theme\":\"default\"}",
        "description": "定时发放",
        "style": {
            "theme": "default",
            "hide_title": false
        },
        "employee_list": [
            {
                "id": 804472,
                "email": "111@smm.cn",
                "cellphone": "13564317032",
                "role_name_list": [
                    "管理员",
                    "财务管理员",
                    "仓单操作员",
                    "业务员",
                    "财务操作员"
                ],
                "user_name": "SMM1511423497TO",
                "status": 0,
                "real_name": "wmn111",
                "position": "产品经理",
                "external_cellphone": "13564317039",
                "qidian_wpa_url": ""
            },
            {
                "id": 808115,
                "email": "",
                "cellphone": "15221119163",
                "role_name_list": [
                    "业务员"
                ],
                "user_name": "SMM1561338037Jl",
                "status": 0,
                "real_name": "王甜",
                "position": "",
                "external_cellphone": "15221119163",
                "qidian_wpa_url": ""
            },
            {
                "id": 808216,
                "email": "",
                "cellphone": "15692102049",
                "role_name_list": [
                    "业务员"
                ],
                "user_name": "SMM1562809427hc",
                "status": 0,
                "real_name": "许国军",
                "position": "",
                "external_cellphone": "15692102049",
                "qidian_wpa_url": ""
            }
        ], // 企业员工列表，只包含 角色为‘业务员’和‘企业职员’的员工
        "description_pic": "https://test-imgqn.smm.cn/test/b/image/VLKBVoBufysVOnTVkxRV20190722114655.jpg",
        "post_count": 126, // 发布信息总数
        "prod_count": 118, // 发布商品数
        "other_count": 8, // 发布帖子数
        "company_detail_info": {
            "id": 1001150,
            "city_info": {
                "id": 47,
                "name": "苏州市",
                "qidian_code": "53"
            },
            "province_info": {
                "id": 12,
                "name": "江苏",
                "qidian_code": "13106"
            },
            "status": 1,
            "name": "张家港中集圣达因低温装备有限公司",
            "province": "江苏",
            "city": "苏州市",
            "province_id": 12,
            "city_id": 47,
            "registered_capital": "",
            "employee_number": "500人以上",
            "business_duration": "三年以内",
            "company_site": "",
            "company_logo": "https://test-imgqn.smm.cn/test/userweb/userverify/UHAhQELKBxrxVNCiLdby20190611050824.jpg",
            "company_desc": "上海有色网信息科技股份有限公司拥有50万注册用户，日均超过20万企业访问, 已经成为世界范围的垂直门户。 主要运营金属行业网站 www.smm.cn, 商城 mall.smm.cn, 国际网站 www.metal.com，手机站 m.smm.cn，APP 掌上有色，官方认证的微信公众账号“上海有色网”亦广受好评。\n我们热诚为客户提供交易服务、安全支付、仓储物流监管、供应链融资、行业大数据及营销服务。上海有色网致力于构建全球金属经营者社群。上海有色网信息科技股份有限公司拥有50万注册用户，日均超过20万企业访问, 已经成为世界范围的垂直门户。 主要运营金属行业网站 www.smm.cn, 商城 mall.smm.cn, 国际网站 www.metal.com，手机站 m.smm.cn，APP 掌上有色，官方认证的微信公众账号“上海有色网”亦广受好评。 \n我们热诚为客户提供交易服务、安全支付、仓储物流监管、供应链融资、行业大数据及营销服务。上海有色网致力于构建全球金属经营者社群。上海有色网信息科技股份有限公司拥有50万注册用户，日均超过20万企业访问, 已经成为世界范围的垂直门户。 主要运营金属行业网站 www.smm.cn, 商城 mall.smm.cn, 国际网站 www.metal.com，手机站 m.smm.cn，APP 掌上有色，官方认证的微信公众账号“上海有色网”亦广受好评。 \n我们热诚为客户提供交易服务、安全支付、仓储物流监管、供应链融资、行业大数据及营销服务。上海有色网致力于构建全球金属经营者社群。上海有色网信息科技股份有限公司拥有50万注册用户，日均超过20万企业访问, 已经成为世界范围的垂直门户。 主要运营金属行业网站 www.smm.cn, 商城 mall.smm.cn, 国际网站 www.metal.com，手机站 m.smm.cn，APP 掌上有色，官方认证的微信公众账号“上海有色网”亦广受好评。 \n我们热诚为客户提供交易服务、安全支付、仓储物流监管、供应链融资、行业大数据及营销服务。上海有色网致力于构建全球金属经营者社群。上海有色网信息科技股份有限公司拥有50万注册用户，日均超过20万企业访问, 已经成为世界范围的垂直门户。 主要运营金属行业网站 www.smm.cn, 商城 mall.smm.cn, 国际网站 www.metal.co",
            "license_no": "12340300726198175M",
            "license_photo": "https://test-imgqn.smm.cn/test/userweb/userverify/ccFBoMhPqMNyrUfdRmUE20171124020804.jpg",
            "org_photo": "",
            "tax_reg_photo": "",
            "account_open_cert": "",
            "proxy_cert": "https://test-imgqn.smm.cn/test/userweb/userverify/CQwGtFTEtwmQwecAzPcM20171124021346.jpg",
            "company_property": "企业",
            "company_type": "加工企业",
            "license_type": 1,
            "buy_product": "",
            "buy_product_list": [],
            "sell_product": "",
            "sell_product_list": [],
            "contact_person": "123",
            "contact_addr": "峨山路20号",
            "contact_phone": "13500000001",
            "contact_email": "",
            "qq": "",
            "fax": "",
            "bank": "工商银行",
            "bank_card_no": "123456",
            "receipt_addr": "张家港低温装备有限公司",
            "taxpayer_no": "ZJGZJSDY0012345",
            "receipt_phone": "12345678901",
            "company_status": 1,
            "pay_status": 0,
            "create_time": "2017-11-24 14:08:49",
            "org_no": "",
            "businessentity_is_admin": 1,
            "businessentity_type": "中国大陆",
            "businessentity_name": "娜娜",
            "businessentity_front": "https://test-imgqn.smm.cn/test/userweb/userverify/pbTHyNlVNXBagFHJmajv20171124021327.jpg",
            "businessentity_back": "https://test-imgqn.smm.cn/test/userweb/userverify/oOMpQOTthcvBRKGDAKIQ20171124021330.jpg",
            "businessentity_no": "42068319941212526",
            "businessentity_id_islongterm": 1,
            "businessentity_id_endtime": "",
            "proxyadmin_name": "娜娜",
            "proxyadmin_no": "42068319941212526",
            "proxyadmin_front": "",
            "proxyadmin_back": "",
            "proxyadmin_id_endtime": "",
            "proxyadmin_id_islongterm": 0,
            "verify_level": 2,
            "license_islongterm": 0,
            "license_start_time": "2017-11-16",
            "license_end_time": "2018-01-01",
            "verify_time": "2017-11-24 14:08:49",
            "main_product": "黄铜、黄铜板、黄铜棒、黄铜管、黄铜带、黄铜排、黄铜箔、紫铜板、紫铜棒、紫铜管、紫铜带、紫铜排、紫铜箔、铝板、铝棒、铝管、铝带、铝排、铝线、铝型材、铜板、铜棒、铝青铜板、铝青铜棒、铝青铜箔、铝青铜带、铝",
            "admin_list": null,
            "user_list": null,
            "invite_code": "23523",
            "registered_capital_amount": 5000000000,
            "certification_list": [
                {
                    "id": 243,
                    "company_id": 1001150,
                    "image_name": "证书名",
                    "image_url": "https://test-imgqn.smm.cn/test/user/image/LzwCuyeXfwLyaGQqLzZF20190617041752.jpg"
                },
                {
                    "id": 254,
                    "company_id": 1001150,
                    "image_name": "证书名",
                    "image_url": "https://test-imgqn.smm.cn/test/user/image/bciVbooqywaowuwFEHjl20190620103023.jpg"
                },
                {
                    "id": 255,
                    "company_id": 1001150,
                    "image_name": "证书名",
                    "image_url": "https://test-imgqn.smm.cn/test/user/image/svhphjGXPLzPCLGIzMAe20190620103024.jpg"
                },
                {
                    "id": 256,
                    "company_id": 1001150,
                    "image_name": "证书名",
                    "image_url": "https://test-imgqn.smm.cn/test/user/image/rzzWiBoHnkZfdkdWfjGY20190620103030.gif"
                }
            ],
            "staff_number": 4
        } // 用户中心企业信息
    }
}
```
</details>

---

#### <a id="vipCompany.isAdmin">API: 判断当前用户是否是企业管理员</a>

**接口描述**

该接口必须登录，判断当前登录的用户是否是指定`company_id`的企业管理员或企业职员

**请求描述**

**GET**  vipCompany/isAdmin

**参数描述**

query:

名称|类型|描述
---|---|---
company_id|int|企业ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "is_admin": false // true:企业管理员或企业职员 false:不是
    }
}
```
</details>

---

#### <a id="vipCompany.pic.setting">API: 设置企业图片</a>

**接口描述**

参数`auth_key`存在时可以不用登录，否则必须登录后才能设置企业图片

**请求描述**

**POST**  vipCompany/pic/setting

**参数描述**

body:

名称|类型|描述
---|---|---
company_id|int|店铺ID
pic_url|string|图片链接
pic_type|int|`1` 背景图 `2`企业简介图
auth_key|string|字符串，后台管理授权编辑码，此参数可忽略店铺管理员权限



<details>
<summary>响应描述</summary>

```json

```
</details>

---

#### <a id="vipCompany.background.system">API: 获取系统默认企业背景图</a>

**请求描述**

**GET**  vipCompany/background/system



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        "https://imgqn.smm.cn/production/club/company/system/picmBgGz20190712162241.png",
        "https://imgqn.smm.cn/production/club/company/system/picTkGMs20190712162917.png",
        "https://imgqn.smm.cn/production/club/company/system/picOXsAG20190712162953.png",
        "https://imgqn.smm.cn/production/club/company/system/picDjMEH20190712163009.png",
        "https://imgqn.smm.cn/production/club/company/system/picwhYGs20190712163023.png",
        "https://imgqn.smm.cn/production/club/company/system/picaoUIJ20190712163042.png",
        "https://imgqn.smm.cn/production/club/company/system/piclWFYN20190712163056.png",
        "https://imgqn.smm.cn/production/club/company/system/picMYMuY20190712163110.png",
        "https://imgqn.smm.cn/production/club/company/system/picqFGpB20190712163124.png",
        "https://imgqn.smm.cn/production/club/company/system/picVfUUz20190724094838.png",
        "https://imgqn.smm.cn/production/club/company/system/picUjYCp20190724094954.png",
        "https://imgqn.smm.cn/production/club/company/system/picZWiKW20190724095029.png"
    ]
}
```
</details>

---

#### <a id="vipCompany.latest">API: 最新开通店铺的企业</a>

**接口描述**

最多返回10条数据

**请求描述**

**GET**  vipCompany/latest



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 24,
            "company_id": 1001150,
            "company_name": "张家港中集圣达因低温装备有限公司",
            "status": 2, // 店铺状态 0未开通 1已过期 2服务中 3关闭
            "status_desc": "服务中",
            "year_base": 9, // 店铺服务年限
            "start_date": 1561910400, // 店铺开通开始时间戳
            "end_date": 1596124800, // 店铺开通结束时间戳
            "background_pic": "", // 店铺背景图
            "admin_email": "test@smm.cn",
            "open_person": "", // 店铺开通用户ID或后台管理员
            "update_time": 1573548679,
            "style_config": "{\"hide_title\":false,\"theme\":\"blue\"}",
            "description": "测试修改没修改成功？",
            "style": {
                "theme": "",
                "hide_title": false
            },
            "company_district": ""
        }
    ]
}
```
</details>

---

#### <a id="vipCompany.edit">API: 设置企业主题简介等</a>

**接口描述**

参数`auth_key`存在时可以不用登录，否则必须登录后才能设置企业图片

**请求描述**

**POST**  vipCompany/edit

**参数描述**

body:

名称|类型|描述
---|---|---
company_id|int|
description|string|企业简介
style_config|string|`hide_title` 是否隐藏公司名称; `theme` 公司样式主题;  例如:{"hide_title":false,"theme":"default"}
auth_key|string|临时授权码



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="vipCompany.openshop">API: 前台用户开通店铺</a>

**请求描述**

**GET**  vipCompany/openshop



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="vipCompany.category">API: 根据分类获取对应的企业店铺</a>

**请求描述**

**GET**  vipCompany/category

**参数描述**

query:

名称|类型|描述
---|---|---
category_id|int|分类ID
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 26,
            "company_id": 1001764,
            "status": 2, // 店铺状态 0未开通 1已过期 2服务中 3关闭
            "status_desc": "",
            "year_base": 6, // 店铺服务年限
            "start_date": 1564329600, // 店铺开通开始时间戳
            "end_date": 1667180800, // 店铺开通结束时间戳
            "background_pic": "",
            "admin_email": "test@smm.cn",
            "open_person": "", // 店铺开通用户ID或后台管理员
            "update_time": 1569746848,
            "style_config": "{\"hide_title\":false,\"theme\":\"default\"}",
            "description": "定时发放",
            "style": {
                "theme": "",
                "hide_title": false
            },
            "main_product": "",
            "province": "上海",
            "city": "浦东新区",
            "address": ""
        }
    ]
}
```
</details>

---

#### <a id="vipCompany.category">API: 分类页</a>

**接口描述**

默认返回6条

分类下 的 付费帖子 且 有company_id大于0 按更新时间倒排 取指定数量店铺

**请求描述**

**GET**  vipCompany/category

**参数描述**

query:

名称|类型|描述
---|---|---
category_id|int|分类ID
limit|int|查询数据条数



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 20,
            "company_id": 1001530,
            "status": 2, // 店铺状态 0未开通 1已过期 2服务中 3关闭
            "status_desc": "",
            "year_base": 5, //店铺服务年限
            "start_date": 1561910400, // 店铺开通开始时间戳
            "end_date": 1601308800, // 店铺开通结束时间戳
            "background_pic": "",
            "admin_email": "test@smm.cn",
            "open_person": "test@smm.cn", // 店铺开通用户ID或后台管理员
            "update_time": 1570781633,
            "style_config": "{\"hide_title\":false,\"theme\":\"green\"}",
            "description": "定时发放第三方第三方第三方第三方",
            "style": {
                "theme": "",
                "hide_title": false
            },
            "company_name": "link的企业",
            "main_product": "我啥都卖",
            "province": "福建",
            "city": "福州市",
            "address": ""
        }
    ]
}
```
</details>

### <a id="item_shangyouquan_660719000">商友圈</a>



---

#### <a id="club.by_name">API: 根据圈子名称获取圈子ID</a>

**接口描述**

精确匹配

**请求描述**

**GET**  club/by_name

**参数描述**

query:

名称|类型|描述
---|---|---
club_name|string|圈子名称



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": 625 // 圈子ID
}
```
</details>

---

#### <a id="club.list">API: 按条件查询圈子列表</a>

**请求描述**

**GET**  club/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|页数
limit|int|数据条数
filter|string|`my_club`：我的圈子，必须登录<br/>`hot`：推荐圈子<br/>`category`：根据分类ID查询圈子，category_id必填
category_id|int|分类ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 51,
        "club_list": [
            {
                "id": 420,
                "user_id": 808117,
                "name": "鼓风机",
                "introduction": "",
                "logo": "",
                "h5_background": "",
                "web_background": "",
                "is_recommend": 1, // 是否推荐 1是 0否
                "disabled": 0, // 是否禁用 1禁用 0正常
                "updated_time": 1573630862,
                "created_time": 1562205875,
                "members_amount": 5, // 圈内成员数
                "post_amount": 1872, // 圈内信息数
                "today_post_amount": 0, // 今日圈内信息数
                "admin_email": "test@smm.cn",
                "is_audit": 0,
                "user_role": "guest", // 如果传用户token，则该字段代表该用户在此圈的角色；master：圈主，member：成员，其他都是未加圈
                "user_info": { // 用户中心的圈主信息
                    "real_name": "",
                    "user_name": "SMM1561341959pu",
                    "nickname": "135****2056",
                    "description": "",
                    "cellphone": "13585952056",
                    "email": "fj@smm.cn",
                    "id": 808117,
                    "company_name": "CCtest",
                    "company_id": 1001629,
                    "company_status": 1,
                    "avatar": "",
                    "company_verify_level": 2,
                    "position": "",
                    "external_cellphone": "13585952056" // 对外联系方式
                },
                "category_list": [ //关联的商机分类
                    {
                        "id": 3,
                        "name_cn": "铜棒",
                        "level": 2,
                        "parent_id": 2,
                        "sort": 1,
                        "children_ids": "79",
                        "post_num": 18, // 分类下的信息数
                        "type": 0,
                        "status": 1, // 是否显示 1显示 2隐藏
                        "is_disabled": 0, // 是否禁用 1禁用 0启用
                        "industry_id": 0,
                        "img_url": "",
                        "is_recommend": 1, // 是否推荐 0正常 1推荐
                        "create_admin": "test@smm.cn",
                        "create_time": 1571202327,
                        "update_admin": "test@smm.cn",
                        "update_time": 1572331972
                    }
                ]
            }
        ]
    }
}
```
</details>

---

#### <a id="club.hot.list">API: 热门圈子列表</a>

**接口描述**

只返回15条；按今日、所有帖子数量排序，数量越多越靠前

**请求描述**

**GET**  club/hot/list



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 475,
        "club_list": [
            {
                "id": 420,
                "user_id": 808117,
                "name": "鼓风机",
                "introduction": "",
                "logo": "",
                "h5_background": "",
                "web_background": "",
                "is_recommend": 1,// 是否推荐 1是 0否
                "disabled": 0, // 是否禁用 1禁用 0正常
                "updated_time": 1573630862,
                "created_time": 1562205875,
                "members_amount": 5, // 圈内成员数
                "post_amount": 1872, // 圈内信息数
                "today_post_amount": 0, // 今日圈内信息数
                "admin_email": "test@smm.cn",
                "is_audit": 0,
                "user_role": "", // 如果传用户token，则该字段代表该用户在此圈的角色；master：圈主，member：成员，其他都是未加圈
                "user_info": { // 用户中心的圈主信息
                    "real_name": "",
                    "user_name": "SMM1561341959pu",
                    "nickname": "135****2056",
                    "description": "",
                    "cellphone": "13585952056",
                    "email": "fj@smm.cn",
                    "id": 808117,
                    "company_name": "CCtest",
                    "company_id": 1001629,
                    "company_status": 1,
                    "avatar": "",
                    "company_verify_level": 2,
                    "position": "",
                    "external_cellphone": "13585952056" // 对外联系方式
                },
                "category_list": [
                    {
                        "id": 3,
                        "name_cn": "铜棒",
                        "level": 2,
                        "parent_id": 2,
                        "sort": 1,
                        "children_ids": "79",
                        "post_num": 18, // 分类下的信息数
                        "type": 0,
                        "status": 1, // 是否显示 1显示 2隐藏
                        "is_disabled": 0, // 是否禁用 1禁用 0启用
                        "industry_id": 0,
                        "img_url": "",
                        "is_recommend": 1, // 是否推荐 0正常 1推荐
                        "create_admin": "test@smm.cn",
                        "create_time": 1571202327,
                        "update_admin": "test@smm.cn",
                        "update_time": 1572331972
                    }
                ]
            }
        ]
    }
}
```
</details>

---

#### <a id="club.info.club_id">API: 圈子详情</a>

**请求描述**

**GET**  club/info/:club_id

**参数描述**

path:

名称|类型|描述
---|---|---
club_id|int|圈子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "club_info": {
            "id": 420,
            "user_id": 808117,
            "name": "鼓风机",
            "introduction": "",
            "logo": "",
            "h5_background": "",
            "web_background": "",
            "is_recommend": 1, // 是否推荐 1是 0否
            "disabled": 0, // 是否禁用 1禁用 0正常
            "updated_time": 1573630862,
            "created_time": 1562205875,
            "members_amount": 5, // 圈内成员数
            "post_amount": 1872, // 圈内信息数
            "today_post_amount": 0, // 今日圈内信息数
            "admin_email": "test@smm.cn",
            "is_audit": 0,
            "user_role": "guest", // 如果传用户token，则该字段代表该用户在此圈的角色；master：圈主，member：成员，其他都是未加圈
            "apply_join_amount": 0,
            "category_list": [
                {
                    "id": 3,
                    "name_cn": "铜棒",
                    "level": 2,
                    "parent_id": 2,
                    "sort": 1,
                    "children_ids": "79",
                    "post_num": 18, // 分类下的信息数
                    "type": 0,
                    "status": 1, // 是否显示 1显示 2隐藏
                    "is_disabled": 0, // 是否禁用 1禁用 0启用
                    "industry_id": 0,
                    "img_url": "",
                    "is_recommend": 1, // 是否推荐 0正常 1推荐
                    "create_admin": "test@smm.cn",
                    "create_time": 1571202327,
                    "update_admin": "test@smm.cn",
                    "update_time": 1572331972
                }
            ]
        }
    }
}
```
</details>

---

#### <a id="club.members">API: 圈子成员列表</a>

**请求描述**

**GET**  club/members

**参数描述**

query:

名称|类型|描述
---|---|---
club_id|int|圈子ID
page|int|页数
limit|int|数据条数



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 31,
        "members": [
            {
                "id": 4,
                "user_id": 804472,
                "is_public": 2, // 是否公开名片 1公开 2不公开
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardpnbdV20191101154254.png", // 名片
                "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/bVDZe20190917144835.jpeg", // 用户中心头像
                "real_name": "小小娜",
                "cellphone": "13564317032",
                "telephone": "13564317066",
                "company_type": "贸易商",
                "company_name": "张家港中集圣达因集团有限公司",
                "province_id": 18,
                "city_id": 0,
                "address": "上海浦东新区峨山路",
                "position": "产品经理",
                "main_product": "铜棒",
                "source_channel": 1, // 名片来源渠道 1pc 2app 3wx 4admin
                "admin_email": "test@smm.cn",
                "create_time": 1568704643,
                "update_time": 1572594190,
                "vip_status": 2, // 会员状态 0不是会员 1过期 2服务中 3关闭
                "vip_type": 2, // 会员类型 1月度 2年度 3体验 4季度 5半年
                "relationship": 1, // 当前登录用户和该成员的关系：0没有关系 1已保存该用户 2互为好友 3待对方同意
                "industry_list": [
                    {
                        "id": 16,
                        "industry_name": "国际贸易",
                        "status": 1, // 是否显示 1显示 2隐藏
                        "disable": 1, // 是否禁用 1启用 2禁用
                        "card_num": 21, // 关联的名片数
                        "sort": 1,
                        "create_admin": "test@smm.cn",
                        "update_admin": "test@smm.cn",
                        "create_time": 1571384075,
                        "update_time": 1571646390
                    }
                ]
            }
        ]
    }
}
```
</details>

---

#### <a id="club.logo.edit">API: 编辑圈子logo</a>

**请求描述**

**POST**  club/logo/edit

**参数描述**

body:

名称|类型|描述
---|---|---
club_id|int|圈子ID
pic_url|string|圈子logo



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="club.background.edit">API: 编辑圈子背景图</a>

**请求描述**

**POST**  club/background/edit

**参数描述**

body:

名称|类型|描述
---|---|---
club_id|int|圈子ID
h5_url|string|h5页面背景图
web_url|string|pc端背景图



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="club.join.approve">API: 圈主同意加圈请求</a>

**接口描述**

该接口暂时废弃

**请求描述**

**POST**  club/join/approve

**参数描述**

body:

名称|参考值|描述
---|---|---
club_id|624|圈子ID
user_id|123|用户ID

---

#### <a id="club.join.reject">API: 圈主拒绝加圈请求</a>

**接口描述**

该接口暂时废弃

**请求描述**

**POST**  club/join/reject

**参数描述**

body:

名称|参考值|描述
---|---|---
club_id|624|
user_id|234|

---

#### <a id="club.member.clean_out">API: 圈主踢成员出圈</a>

**请求描述**

**POST**  club/member/clean_out

**参数描述**

body:

名称|类型|描述
---|---|---
club_id|int|圈子ID
user_id|int|要踢出圈的用户ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="club.edit">API: 编辑圈子简介</a>

**请求描述**

**POST**  club/edit

**参数描述**

body:

名称|类型|描述
---|---|---
club_id|int|圈子ID
introduction|string|圈子简介
is_audit|int|加圈是否需要审核 `0`不需要 `1`需要；目前已经废弃 全部不需要审核



<details>
<summary>响应描述</summary>

```json

```
</details>

---

#### <a id="club.audit.edit">API: 编辑加圈是否需要圈主审核</a>

**接口描述**

该接口暂时废弃

**请求描述**

**POST**  club/audit/edit

**参数描述**

body:

名称|参考值|描述
---|---|---
club_id|624|
is_audit|0|加圈是否需要圈主审核，0不需要 1需要；目前没用，全部不需要审核

---

#### <a id="club.join_apply">API: 加入圈子</a>

**请求描述**

**POST**  club/join_apply

**参数描述**

body:

名称|类型|描述
---|---|---
club_id|int|圈子ID
form_id|string|可选，微信小程序form_id



<details>
<summary>响应描述</summary>

```json

```
</details>

---

#### <a id="club.leave">API: 用户退出圈子</a>

**请求描述**

**POST**  club/leave

**参数描述**

body:

名称|类型|描述
---|---|---
club_id|int|圈子ID



<details>
<summary>响应描述</summary>

```json

```
</details>

---

#### <a id="club.create_apply">API: 申请建圈子</a>

**接口描述**

该接口暂时废弃

**请求描述**

**POST**  club/create_apply

**参数描述**

body:

名称|参考值|描述
---|---|---
product|sadf|圈子名称
phone||
company_name||
device_type||发布渠道 1:web 2:h5 3android 4ios 5小程序

---

#### <a id="club.notice">API: 查询公告列表</a>

**请求描述**

**GET**  club/notice

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|页数
limit|int|数据条数
club_id|int|圈子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 4,
        "post_list": [
            {
                "id": 213168,
                "user_id": 808108,
                "company_id": 1001625,
                "title": "发布在自己圈子里面的其他信息设为公告",
                "post_type": 2, // 帖子类型 1:产品信息 2:其他信息
                "price": 0,
                "quantity_unit": 0,
                "province_id": 0,
                "city_id": 0,
                "club_id": 434, // 所属圈子ID
                "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 1是 0否
                "status": 1, // 消息状态: 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1564384635,
                "created_time": 1564384635,
                "post_content_rtf": "",
                "post_content_txt": "三顿饭付付付付过多所过不别的",
                "cover_pic": "",
                "product_pic_set": "",
                "admin_email": "",
                "top": 0 // 置顶标志 1:置顶 0 否
                "is_notice": 1, // 是否是通知 1:是 0否
                "refresh_time": 0,
                "is_offer": 0, // 是否报价 1:是 0否
                "pic_amount": 0,
                "is_crawl": 0,
                "unit": "",
                "area": "",
                "approval_status": 2, // 审核状态: 1待审核 2审核成功 3审核失败
                "reason": "", // 审核失败原因
                "approval_time": 1564384642,
                "approver_email": "test@smm.cn",
                "click_count": 5, // 点击量
                "sale_number": "0", // 可售数量
                "valid_period": 100, // 有效期天数
                "valid_period_time": 1582182175, // 有效期时间戳
                "category_id": 0, // 所属分类顶级ID
                "last_category_id": 0, // 所属分类ID
                "is_vip": 2, // 发布该信息时是否时会员
                "vip_type": 1, // 发布该信息时的会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "", // gps 省份
                "location_city": "", // gps 城市
                "location_gps": "", // gps 地址
                "navbar_name": "铜",
                "club_name": "开发测试用圈",
                "province_name": "",
                "city_name": "",
                "user_info": { // 名片信息,有可能时审核中的名片
                    "id": 10,
                    "user_id": 808108,
                    "is_public": 1, // 是否公开 1公开 2不公开
                    "card_url": "http://card_url.jpg",
                    "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/TEgwp20190703101715.jpeg",
                    "real_name": "商机小号01",
                    "cellphone": "13564317036",
                    "telephone": "13564317037",
                    "company_type": "贸易商",
                    "company_name": "商机测试02有限公司",
                    "province_id": 0,
                    "city_id": 0,
                    "address": "铁岭",
                    "position": "老板",
                    "main_product": "",
                    "source_channel": 1, // 名片来源 1pc 2app 3wx 4admin
                    "admin_email": "test@smm.cn",
                    "create_time": 1569223906,
                    "update_time": 1571034877
                },
                "attribute": [
                	{
                        "attribute_id": 1866,
                        "name": "品牌",
                        "attr_type": 1, // 1单选 2文本
                        "attr_options": "华为,OPPO,vivo,苹果", // 单选时为逗号分隔的选项；文本时为正则
                        "attr_unit": "",
                        "attr_value": "华为"
                    }
            	], // 信息属性
                "company_name": "商机测试01号",
                "vip_company_status": 2, // 店铺状态 0未开通 1过期 2服务中 3关闭
                "vip_company_status_desc": "服务中",
                "vip_year": 2, // 店铺年限
                "qidian_wpa_url": "", // 企点url
                "category_name": "", // 所属顶级分类名称
                "last_category_name": "" // 所属分类名称
            }
        ]
    }
}
```
</details>

---

#### <a id="load_club_member_amount">API: 批量更新圈子成员数</a>

**请求描述**

**GET**  load_club_member_amount

---

#### <a id="load_club_post_amount">API: 批量更新圈内帖子数</a>

**请求描述**

**GET**  load_club_post_amount

---

#### <a id="club.sitmap.list">API: 圈子sitmap列表</a>

**请求描述**

**GET**  club/sitmap/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|页数
limit|int|数据条数
begin_time|int|圈子创建开始时间
end_time|int|圈子创建结束时间



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 475,
        "club_site_map_list": [
            {
                "id": 232, // 圈子ID
                "created_time": 1541583416,
                "updated_time": 1569376070
            }
        ]
    }
}
```
</details>

---

#### <a id="club.company.list">API: 获取企业所有圈子</a>

**接口描述**

获取企业下所有帖子所属的圈子列表

**请求描述**

**GET**  club/company/list

**参数描述**

query:

名称|类型|描述
---|---|---
company_id|int|企业ID
post_type|int|信息类型 `1`商品 `2`帖子



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "club_list": [
            {
                "club_name": "马口铁",
                "club_id": 230
            }
        ]
    }
}
```
</details>

---

#### <a id="club.category">API: 分类页圈子列表</a>

**接口描述**

默认返回3条数据

**请求描述**

**GET**  club/category

**参数描述**

query:

名称|类型|描述
---|---|---
category_id|int|分类ID
limit|int|数据条数
exclude_club_id|int|排除指定商圈
exclude_user_id|int|排除指定用户加入的圈子



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 420,
            "user_id": 808117,
            "name": "鼓风机",
            "introduction": "",
            "logo": "",
            "h5_background": "",
            "web_background": "",
            "is_recommend": 1, // 是否推荐 1是 0否
            "disabled": 0, // 是否禁用 1禁用 0正常
            "updated_time": 1573630862,
            "created_time": 1562205875,
            "members_amount": 5, // 圈内成员数
            "post_amount": 1872, // 圈内信息数
            "today_post_amount": 0, // 今日圈内信息数
            "admin_email": "test@smm.cn",
            "is_audit": 0,
            "user_role": "guest", // 如果传用户token，则该字段代表该用户在此圈的角色；master：圈主，member：成员，其他都是未加圈
            "user_info": { // 用户中心的圈主信息
                "real_name": "",
                "user_name": "SMM1561341959pu",
                "nickname": "135****2056",
                "description": "",
                "cellphone": "13585952056",
                "email": "fj@smm.cn",
                "id": 808117,
                "company_name": "CCtest",
                "company_id": 1001629,
                "company_status": 1,
                "avatar": "",
                "company_verify_level": 2,
                "position": "",
                "external_cellphone": "13585952056" // 对外联系方式
            },
            "category_list": [ //关联的商机分类
                {
                    "id": 3,
                    "name_cn": "铜棒",
                    "level": 2,
                    "parent_id": 2,
                    "sort": 1,
                    "children_ids": "79",
                    "post_num": 18, // 分类下的信息数
                    "type": 0,
                    "status": 1, // 是否显示 1显示 2隐藏
                    "is_disabled": 0, // 是否禁用 1禁用 0启用
                    "industry_id": 0,
                    "img_url": "",
                    "is_recommend": 1, // 是否推荐 0正常 1推荐
                    "create_admin": "test@smm.cn",
                    "create_time": 1571202327,
                    "update_admin": "test@smm.cn",
                    "update_time": 1572331972
                }
            ]
        }
    ]
}
```
</details>

### <a id="item_fenlei_661517000">分类</a>



---

#### <a id="category.query_attribute_list">API: 查询分类属性</a>

**请求描述**

**GET**  category/query_attribute_list

**参数描述**

query:

名称|类型|描述
---|---|---
category_id|int|分类ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "attribute_list": [
            {
                "id": 44,
                "name": "牌号",
                "attr_type": 2, // 1单选 2文本
                "attr_options": "^[0-9]*$", // 文本时为正则表达式
                "attr_unit": "",
                "sort_number": 0,
                "is_lock": 0
            },
            {
                "id": 45,
                "name": "品牌",
                "attr_type": 1,
                "attr_options": "samsung,apple,vivo,mi,sony", // 单选时为逗号分割的选项
                "attr_unit": "",
                "sort_number": 0,
                "is_lock": 0
            }
        ]
    }
}
```
</details>

---

#### <a id="category.relation_category_list">API: 根据分类获取关系关联的分类</a>

**请求描述**

**GET**  category/relation_category_list

**参数描述**

query:

名称|类型|描述
---|---|---
category_id|int|分类ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "relation_id": 3, // 关系ID
            "relation_name": "分类产品", //关系名称
            "category_list": [ // 关系关联的分类
                {
                    "category_id": 85, // 分类ID
                    "category_name": "龙头"
                },
                {
                    "category_id": 86,
                    "category_name": "灯具部件"
                }
            ]
        }
    ]
}
```
</details>

---

#### <a id="category.history.list">API: 获取用户历史选择的分类列表</a>

**请求描述**

**GET**  category/history/list



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 3,
            "name_cn": "铜棒",
            "level": 2,
            "parent_id": 2, // 父级分类ID
            "sort": 1,
            "children_ids": "79",
            "post_num": 18, // 该分类下的信息数
            "type": 0,
            "status": 1, // 是否显示 1显示 2隐藏
            "is_disabled": 0, // 是否禁用 0启用 1禁用
            "industry_id": 0,
            "img_url": "",
            "is_recommend": 1, // 是否推荐 0正常 1推荐
            "create_admin": "test@smm.cn",
            "create_time": 1571202327,
            "update_admin": "test@smm.cn",
            "update_time": 1572331972
        }
    ]
}
```
</details>

---

#### <a id="category.nesting.all.list">API: 获取所有分类（多级嵌套结构）</a>

**接口描述**

缓存8小时

**请求描述**

**GET**  category/nesting/all/list

**参数描述**

query:

名称|类型|描述
---|---|---
status|int|是否显示 `0`全部 `1`显示 `2`隐藏
disable|int|禁用 `-1`全部  `0`正常 `1`禁用



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [ // 多级嵌套结构
        {
            "id": 2,
            "name_cn": "铜",
            "level": 1, // 级别
            "parent_id": 0, // 父级分类ID
            "sort": 1,
            "children_ids": "3,4,5,6",
            "post_num": 36, // 分类下的信息数
            "type": 0,
            "status": 1, // 是否显示 1显示 2隐藏
            "is_disabled": 0, // 是否禁用 0启用 1禁用
            "industry_id": 0,
            "img_url": "",
            "is_recommend": 1, // 是否推荐 0 正常 1 推荐
            "create_admin": "test@smm.cn",
            "create_time": 1571202165,
            "update_admin": "test@smm.cn",
            "update_time": 1571724168,
            "children_list": [ // 子集分类
                {
                    "id": 4,
                    "name_cn": "铜原料",
                    "level": 2,
                    "parent_id": 2,
                    "sort": 1,
                    "children_ids": "8,9,10",
                    "post_num": 7,
                    "type": 0,
                    "status": 1,
                    "is_disabled": 0,
                    "industry_id": 0,
                    "img_url": "",
                    "is_recommend": 1,
                    "create_admin": "test@smm.cn",
                    "create_time": 1571205889,
                    "update_admin": "test@smm.cn",
                    "update_time": 1571724168,
                    "children_list": [
                        {
                            "id": 8,
                            "name_cn": "电解铜",
                            "level": 3,
                            "parent_id": 4,
                            "sort": 1,
                            "children_ids": "",
                            "post_num": 7,
                            "type": 0,
                            "status": 1,
                            "is_disabled": 0,
                            "industry_id": 0,
                            "img_url": "",
                            "is_recommend": 1,
                            "create_admin": "test@smm.cn",
                            "create_time": 1571205969,
                            "update_admin": "test@smm.cn",
                            "update_time": 1571724168,
                            "children_list": []
                        }
                    ]
                }
            ]
        }
    ]
}
```
</details>

---

#### <a id="category.recommend.list">API: 获取所有一级分类下所有后代的推荐分类</a>

**接口描述**

缓存8小时

**请求描述**

**GET**  category/recommend/list



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": { // key为一级分类ID，内容是一级分类下所有后代（包括孙子等）的推荐分类
        "1": [],
        "2": [
            {
                "category_id": 3, // 分类ID
                "category_name": "铜棒"
            },
            {
                "category_id": 4,
                "category_name": "铜原料"
            },
            {
                "category_id": 5,
                "category_name": "铜加工"
            }
        ]
    }
}
```
</details>

---

#### <a id="category.parent.list">API: 根据子级分类ID获取所有父级列表</a>

**请求描述**

**GET**  category/parent/list

**参数描述**

query:

名称|类型|描述
---|---|---
category_id|int|子级分类ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [ // 数组顺序为顶级分离逐级排序
        {
            "id": 2,
            "name_cn": "铜",
            "level": 1, // 级别
            "parent_id": 0, // 父级ID
            "sort": 1,
            "children_ids": "3,4,5,6",
            "post_num": 36, // 信息数
            "type": 0,
            "status": 1, // 是否显示 1显示 2隐藏
            "is_disabled": 0, // 是否禁用 0启用 1禁用
            "industry_id": 0,
            "img_url": "",
            "is_recommend": 1, // 是否推荐 0正常 1推荐
            "create_admin": "test@smm.cn",
            "create_time": 1571202165,
            "update_admin": "test@smm.cn",
            "update_time": 1571724168
        },
        {
            "id": 4,
            "name_cn": "铜原料",
            "level": 2,
            "parent_id": 2,
            "sort": 1,
            "children_ids": "8,9,10",
            "post_num": 7,
            "type": 0,
            "status": 1,
            "is_disabled": 0,
            "industry_id": 0,
            "img_url": "",
            "is_recommend": 1,
            "create_admin": "test@smm.cn",
            "create_time": 1571205889,
            "update_admin": "test@smm.cn",
            "update_time": 1571724168
        }
    ]
}
```
</details>

---

#### <a id="category.last_level.list">API: 根据关键词搜索最后一级分类</a>

**请求描述**

**GET**  category/last_level/list

**参数描述**

query:

名称|类型|描述
---|---|---
keyword|string|分类名称关键词，模糊匹配



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 8,
            "name_cn": "电解铜",
            "level": 3,
            "parent_id": 4,
            "sort": 1,
            "children_ids": "",
            "post_num": 7, // 分类下的信息数
            "type": 0,
            "status": 1, // 是否显示 1显示 2隐藏
            "is_disabled": 0, // 是否禁用 0启用 1禁用
            "industry_id": 0,
            "img_url": "",
            "is_recommend": 1, // 是否推荐 0正常 1推荐
            "create_admin": "test@smm.cn",
            "create_time": 1571205969,
            "update_admin": "test@smm.cn",
            "update_time": 1571724168
        }
    ]
}
```
</details>

---

#### <a id="category.company.list">API: 获取企业所有分类</a>

**请求描述**

**GET**  category/company/list

**参数描述**

query:

名称|类型|描述
---|---|---
company_id|int|分类ID
post_type|int|帖子类型：`1`产品 `2`其他



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "category_list": [
            {
                "category_id": 3,
                "category_name": "铜棒"
            },
            {
                "category_id": 8,
                "category_name": "电解铜"
            }
        ]
    }
}
```
</details>

---

#### <a id="category.info.category_id">API: 获取分类详情</a>

**请求描述**

**GET**  category/info/:category_id

**参数描述**

path:

名称|类型|描述
---|---|---
category_id|int|分类ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "id": 27,
        "name_cn": "铝箔",
        "level": 3,
        "parent_id": 19,
        "sort": 1,
        "children_ids": "",
        "post_num": 0, // 分类下的信息数
        "type": 0,
        "status": 1, // 是否显示 1显示 2隐藏
        "is_disabled": 1, // 是否禁用 0启用 1禁用
        "industry_id": 0,
        "img_url": "",
        "is_recommend": 0, // 是否推荐 0正常 1推荐
        "create_admin": "test@smm.cn",
        "create_time": 1571206178,
        "update_admin": "test@smm.cn",
        "update_time": 1571724168,
        "parent_name": "铝加工",
        "children_list": [
        	{
                "category_id": 18,
                "category_name": "铝原料"
            }	
    	]
    }
}
```
</details>

---

#### <a id="category.by_name">API: 根据分类名称查询分类ID</a>

**请求描述**

**GET**  category/by_name

**参数描述**

query:

名称|类型|描述
---|---|---
name|string|分类名称关键词，精确匹配



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": 84 // 分类ID
}
```
</details>

---

#### <a id="category.other.list">API: 根据分类获取同级别的其他分类</a>

**接口描述**

`limit`不传，则默认为7

**请求描述**

**GET**  category/other/list

**参数描述**

query:

名称|类型|描述
---|---|---
category_id|int| 分类ID
limit|int|数据条数



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 2,
            "name_cn": "铜",
            "level": 1,
            "parent_id": 0,
            "sort": 1,
            "children_ids": "3,4,5,6",
            "post_num": 36, // 分类下的信息数
            "type": 0,
            "status": 1, // 是否显示 1显示 2隐藏
            "is_disabled": 0, // 是否禁用 0启用 1禁用
            "industry_id": 0,
            "img_url": "",
            "is_recommend": 1, // 是否推荐 0正常 1推荐
            "create_admin": "test@smm.cn",
            "create_time": 1571202165,
            "update_admin": "test@smm.cn",
            "update_time": 1571724168
        }
    ]
}
```
</details>

### <a id="item_mingpian_661680000">名片 </a>



---

#### <a id="usercard.info">API: 根据用户ID获取名片</a>

**接口描述**

relationship: 0不是好友关系 1 单向加对方 2互为好友 3待对方确认

**请求描述**

**GET**  usercard/info

**参数描述**

query:

名称|类型|描述
---|---|---
user_id|int|用户ID
approval_status|int|名片状态 1待审核名片 2审核通过的名片



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "id": 7,
        "user_id": 807720,
        "is_public": 2, // 是否公开名片 1公开 2不公开
        "card_url": "https://test-imgqn.smm.cn/test/club/user/cardubpDF20191105173608.png",
        "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/nNaGF20190923194241.jpeg",
        "real_name": "张新杰",
        "cellphone": "13127881017",
        "telephone": "099-123456",
        "company_type": "矿产商",
        "company_name": "上海有色网股份有限公司",
        "province_id": 18,
        "city_id": 0,
        "address": "上海浦东新区峨山路91弄20号陆家嘴软件园9号楼9楼",
        "position": "后端工程师",
        "main_product": "铝合金",
        "source_channel": 4, // 名片来源渠道 1pc 2app 3wx 4admin
        "create_time": 1568788590,
        "update_time": 1572946568,
        "province": "上海",
        "city": "",
        "approval_status": 2, // 名片审核状态：1 待审核 2审核通过 3拒绝
        "reason": "",  // 审核拒绝拒绝原因
        "admin_email": "",
        "industry_list": [ // 关联行业列表
            {
                "id": 5,
                "industry_name": "测试003",
                "status": 2,
                "disable": 1,
                "card_num": 3,
                "sort": 2,
                "create_admin": "test@smm.cn",
                "update_admin": "test@smm.cn",
                "create_time": 1568701331,
                "update_time": 1571646390
            }
        ],
        "vip_status": 2, // 会员状态 0不是会员 1过期 2服务中 3关闭
        "vip_type": 1, // 会员类型 1月度 2年度 3体验 4季度 5半年
        "relationship": 0, // 当前登录用户和该名片的关系：0没有关系 1已保存该用户 2互为好友 3待对方同意
        "group_id": 0,
        "group_name": ""
    }
}
```
</details>

---

#### <a id="usercard.completed">API: 完善名片信息</a>

**接口描述**

该接口是新建和编辑公用接口，每次提交都会产生新的审核记录（如果当前已经有待审核的记录则不生成新记录），后台审核通过后才会更新到名片。审核通过前别人无法看到提交的信息。

**请求描述**

**POST**  usercard/completed

**参数描述**

body:

名称|类型|描述
---|---|---
is_public|int|是否公开 1公开 2需要同意
card_url|string|名片图片链接
real_name|string|真实姓名
cellphone|string|手机号
telephone|string|电话号
company_type|string|企业类型 `贸易商`、`矿产商`、`冶炼企业`、`加工企业`、`生产企业`
company_name|string|企业名称
province_id|int|省份id
city_id|int|城市id
address|string|地址·
position|string|职位
industry_ids|string|逗号分割的行业ID，如：1,2,3
main_product|string|主营产品
source_channel|int|名片来源渠道 `1`pc `2`app `3`wx `4`admin
share_user_id|int|从分享链接进入完善名片的分享人用户ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="usercard.submit">API: 递名片</a>

**请求描述**

**POST**  usercard/submit

**参数描述**

body:

名称|类型|描述
---|---|---
card_id|int|对方名片ID
source|int|添加来源： `1`扫描二维码 `2`商机  `3`通讯录
form_id|string|微信小程序form_id，可选



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="usercard.wall">API: 名片墙</a>

**接口描述**

查询限制：

会员类型|限制数据条数
---|---
非会员|20
体验|100
月度|300
年度|不限

**请求描述**

**GET**  usercard/wall

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|页数
limit|int|数据条数
industry_id|int|行业ID
province_id|int|省份ID
city_id|int|城市ID
position|string|职位 



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 29,
        "page": 1,
        "limit": 3,
        "limit_msg": "", // 超出限制后的提示消息
        "list": [
            {
                "id": 348,
                "user_id": 481389,
                "is_public": 1, // 是否公开名片 1公开 2不公开
                "card_url": "https://test-imgqn.smm.cn/club/user/cardKDVIt20191030103247.png",
                "avatar": "",
                "real_name": "潘东亮",
                "cellphone": "13916144044",
                "telephone": "021-52901122",
                "company_type": "",
                "company_name": "上海坤泰企业发展有限公司",
                "province_id": 0,
                "city_id": 0,
                "address": "中国上海市中山北路2000号8元",
                "position": "副总裁",
                "main_product": "",
                "source_channel": 4, // 名片来源渠道 1pc 2app 3wx 4admin
                "create_time": 1570864138,
                "update_time": 1570864138,
                "province": "",
                "city": "",
                "approval_status": 2, // 名片审核状态：1 待审核 2审核通过 3拒绝
                "reason": "",  // 审核拒绝拒绝原因
                "admin_email": "",
                "industry_list": [ // 关联行业列表
                    {
                        "id": 16,
                        "industry_name": "国际贸易",
                        "status": 1,
                        "disable": 1,
                        "card_num": 21,
                        "sort": 1,
                        "create_admin": "test@smm.cn",
                        "update_admin": "test@smm.cn",
                        "create_time": 1571384075,
                        "update_time": 1571646390
                    }
                ],
                "vip_status": 2, // 会员状态 0不是会员 1过期 2服务中 3关闭
                "vip_type": 1, // 会员类型 1月度 2年度 3体验 4季度 5半年
                "relationship": 0, // 当前登录用户和该名片的关系：0没有关系 1已保存该用户 2互为好友 3待对方同意
                "group_id": 0,
                "group_name": ""
            }
        ]
    }
}
```
</details>

---

#### <a id="usercard.clip">API: 名片夹</a>

**请求描述**

**GET**  usercard/clip

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|页数
limit|int|数据条数
keyword|string|关键字，模糊匹配；手机号/电话号/公司名称/姓名



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 14,
        "page": 1,
        "limit": 10,
        "list": [
            {
                "id": 13,
                "user_id": 808004,
                "is_public": 1, // 是否公开名片 1公开 2不公开
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardoEyZs20191105181929.png",
                "avatar": "https://test-imgqn.smm.cn/test/thirdparty/avatar/OPqay20190805155209.jpeg",
                "real_name": "梁小A",
                "cellphone": "15850225218",
                "telephone": "",
                "company_type": "冶炼企业",
                "company_name": "CUACON.广告器材。超市",
                "province_id": 12,
                "city_id": 0,
                "address": "上海陆家嘴软件园",
                "position": "老板",
                "main_product": "啥都卖",
                "source_channel": 4,  // 名片来源渠道 1pc 2app 3wx 4admin
                "create_time": 1569383630,
                "update_time": 1572950082,
                "province": "江苏",
                "city": "",
                "approval_status": 2, // 名片审核状态：1 待审核 2审核通过 3拒绝
                "reason": "",  // 审核拒绝拒绝原因
                "admin_email": "",
                "industry_list": [ // 关联行业列表
                    {
                        "id": 12,
                        "industry_name": "物流运输",
                        "status": 1,
                        "disable": 1,
                        "card_num": 18,
                        "sort": 1,
                        "create_admin": "test@smm.cn",
                        "update_admin": "test@smm.cn",
                        "create_time": 1571384052,
                        "update_time": 1571646390
                    },
                    {
                        "id": 14,
                        "industry_name": "井巷工程",
                        "status": 1,
                        "disable": 1,
                        "card_num": 18,
                        "sort": 1,
                        "create_admin": "test@smm.cn",
                        "update_admin": "test@smm.cn",
                        "create_time": 1571384064,
                        "update_time": 1571646390
                    }
                ],
                "vip_status": 0, // 会员状态 0不是会员 1过期 2服务中 3关闭
                "vip_type": 0, // 会员类型 1月度 2年度 3体验 4季度 5半年
                "relationship": 2,// 当前登录用户和该名片的关系：0没有关系 1已保存该用户 2互为好友 3待对方同意
                "group_id": 18, // 该名片所属分组ID
                "group_name": "啦啦啦啦" // 该名片所属分组
            }
        ]
    }
}
```
</details>

---

#### <a id="usercard.search">API: 搜索名片</a>

**接口描述**

查询限制：

会员类型|限制数据条数
---|---
非会员|2
体验|5
月度|10
年度|不限

**请求描述**

**GET**  usercard/search

**参数描述**

query:

名称|类型|描述
---|---|---
page|1|页数
limit|10|数据条数
real_name|张三|姓名
company_name|有色网|公司名称
cellphone|13112345678|手机号



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 208,
        "page": 1,
        "limit": 10,
        "list": [
            {
                "id": 390,
                "user_id": 807848,
                "is_public": 1,  // 是否公开名片 1公开 2不公开
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardMNfOw20191029124119.png",
                "avatar": "",
                "real_name": "张大炮",
                "cellphone": "13112345678",
                "telephone": "1234567",
                "company_type": "矿产商",
                "company_name": "jhigyh",
                "province_id": 28,
                "city_id": 0,
                "address": "上海市杨浦区五角场",
                "position": "员工",
                "main_product": "",
                "source_channel": 1,  // 名片来源渠道 1pc 2app 3wx 4admin
                "create_time": 1573187562,
                "update_time": 1573187562,
                "province": "湖北",
                "city": "",
                "approval_status": 2,
                "reason": "",
                "admin_email": "",
                "industry_list": [ // 关联行业列表
                    {
                        "id": 15,
                        "industry_name": "地质勘探",
                        "status": 1,
                        "disable": 1,
                        "card_num": 19,
                        "sort": 1,
                        "create_admin": "test@smm.cn",
                        "update_admin": "test@smm.cn",
                        "create_time": 1571384070,
                        "update_time": 1571646390
                    }
                ],
                "vip_status": 0, // 会员状态 0不是会员 1过期 2服务中 3关闭
                "vip_type": 0, // 会员类型 1月度 2年度 3体验 4季度 5半年
                "relationship": 0,// 当前登录用户和该名片的关系：0没有关系 1已保存该用户 2互为好友 3待对方同意
                "group_id": 0,
                "group_name": ""
            }
        ]
    }
}
```
</details>

---

#### <a id="usercard.request">API: 名片请求列表</a>

**请求描述**

**GET**  usercard/request



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "with_three_day": [ // 三天内
        	{
                "id": 2,
                "user_id": 807722,
                "is_public": 1, // 是否公开名片 1公开 2不公开
                "card_url": "",
                "avatar": "",
                "real_name": "娃儿",
                "cellphone": "",
                "telephone": "",
                "company_type": "",
                "company_name": "",
                "province_id": 0,
                "city_id": 0,
                "address": "",
                "position": "",
                "main_product": "",
                "source_channel": 1, // 名片来源渠道 1pc 2app 3wx 4admin
                "create_time": 0,
                "update_time": 0,
                "province": "",
                "city": "",
                "approval_status": 0,
                "reason": "",
                "admin_email": "",
                "industry_list": [],
                "vip_status": 0, // 会员状态 0不是会员 1过期 2服务中 3关闭
                "vip_type": 0, // 会员类型 1月度 2年度 3体验 4季度 5半年
                "relationship": 3 // 当前登录用户和该名片的关系：0没有关系 1已保存该用户 2互为好友 3待对方同意
            }	
    	],
        "three_day_ago": [ // 三天前
            {
                "id": 2,
                "user_id": 807722,
                "is_public": 1,
                "card_url": "",
                "avatar": "",
                "real_name": "娃儿",
                "cellphone": "",
                "telephone": "",
                "company_type": "",
                "company_name": "",
                "province_id": 0,
                "city_id": 0,
                "address": "",
                "position": "",
                "main_product": "",
                "source_channel": 1,
                "create_time": 0,
                "update_time": 0,
                "province": "",
                "city": "",
                "approval_status": 0,
                "reason": "",
                "admin_email": "",
                "industry_list": [ // 关联行业列表
                	{
		                "id": 5,
		                "industry_name": "测试003",
		                "status": 2,
		                "disable": 1,
		                "card_num": 3,
		                "sort": 2,
		                "create_admin": "test@smm.cn",
		                "update_admin": "test@smm.cn",
		                "create_time": 1568701331,
		                "update_time": 1571646390
            		}	
            	],
                "vip_status": 0,
                "vip_type": 0,
                "relationship": 3
            }
        ]
    }
}
```
</details>

---

#### <a id="usercard.agree">API: 同意递名片（加好友）请求</a>

**请求描述**

**POST**  usercard/agree

**参数描述**

body:

名称|类型|描述
---|---|---
card_id|int|请求方名片ID
form_id|string|微信小程序form_id，可选



<details>
<summary>响应描述</summary>

```json
{
    "code": 10150,
    "msg": "没有好友请求或已为好友",
    "data": null
}
```
</details>

---

#### <a id="usercard.group.add">API: 添加名片分组</a>

**请求描述**

**POST**  usercard/group/add

**参数描述**

body:

名称|类型|描述
---|---|---
group_name|string|分组名称



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "group_id": 30 // 新添加的分组ID
    }
}
```
</details>

---

#### <a id="usercard.group">API: 根据分组获取名片夹名片</a>

**请求描述**

**GET**  usercard/group

**参数描述**

query:

名称|类型|描述
---|---|---
group_id|int|分组ID，`0`代表未分组的名片
page|int|页数
limit|int|数据条数



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 11,
        "page": 1,
        "limit": 10,
        "list": [
            {
                "id": 64,
                "user_id": 807748,
                "is_public": 1, // 是否公开名片 1公开 2不公开
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardcfLqK20191029145002.png",
                "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/LBVmh20190625135010.jpeg",
                "real_name": "吴梦娜",
                "cellphone": "18512197032",
                "telephone": "18512154782",
                "company_type": "矿产商",
                "company_name": "测试贸易12134",
                "province_id": 18,
                "city_id": 0,
                "address": "峨山路",
                "position": "小职员",
                "main_product": "铜铝铅",
                "source_channel": 1, // 名片来源渠道 1pc 2app 3wx 4admin
                "create_time": 1570863392,
                "update_time": 1573187590,
                "province": "上海",
                "city": "",
                "approval_status": 2,
                "reason": "",
                "admin_email": "",
                "industry_list": [ // 关联行业列表
                    {
                        "id": 16,
                        "industry_name": "国际贸易",
                        "status": 1,
                        "disable": 1,
                        "card_num": 21,
                        "sort": 1,
                        "create_admin": "test@smm.cn",
                        "update_admin": "test@smm.cn",
                        "create_time": 1571384075,
                        "update_time": 1571646390
                    }
                ],
                "vip_status": 2, // 会员状态 0不是会员 1过期 2服务中 3关闭
                "vip_type": 2, // 会员类型 1月度 2年度 3体验 4季度 5半年
                "relationship": 2, // 当前登录用户和该名片的关系：0没有关系 1已保存该用户 2互为好友 3待对方同意
                "group_id": 0, // 分组ID
                "group_name": "" // 分组名称
            }
        ]
    }
}
```
</details>

---

#### <a id="usercard.group.list">API: 获取登录用户的名片分组</a>

**请求描述**

**GET**  usercard/group/list



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [ // 分组列表
        {
            "group_id": 18,
            "group_name": "啦啦啦啦",
            "user_card_count": 1 // 分组下拥有的名片数量
        },
        {
            "group_id": 0, // 未分组ID未 0
            "group_name": "未分组",
            "user_card_count": 11
        }
    ]
}
```
</details>

---

#### <a id="usercard.group.edit">API: 编辑名片分组</a>

**请求描述**

**POST**  usercard/group/edit

**参数描述**

body:

名称|类型|描述
---|---|---
group_id|int|分组ID
group_name|string|分组名称



<details>
<summary>响应描述</summary>

```json

```
</details>

---

#### <a id="usercard.group.del">API: 删除名片分组</a>

**请求描述**

**POST**  usercard/group/del

**参数描述**

body:

名称|类型|描述
---|---|---
group_id|int|要删除的分组ID



<details>
<summary>响应描述</summary>

```json

```
</details>

---

#### <a id="usercard.group.set">API: 设置名片夹名片分组</a>

**请求描述**

**POST**  usercard/group/set

**参数描述**

body:

名称|类型|描述
---|---|---
card_id|int|名片ID
group_id|int|分组ID，未`0`就是将名片移入未分组下



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="usercard.ocr">API: ocr识别名片</a>

**接口描述**

仅识别名片信息

**请求描述**

**GET**  usercard/ocr

**参数描述**

query:

名称|类型|描述
---|---|---
card_url|string|名片网络链接



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "name": "",
            "avatar": "",
            "cover_img": "https://test-imgqn.smm.cn/test/b/image/UjERbUvWbfjFjtmwkHMy20190923074257.jpg",
            "back_img": "",
            "job": "", // 工作
            "company": "理县吉祥谷国际大酒店",
            "profession": "", // 职位
            "city": "",
            "cellphone": "15281502289",
            "telephone": "0837-6826999",
            "email": "",
            "address": "理县杂谷脑镇红叶大道",
            "website": ""
        }
    ]
}
```
</details>

---

#### <a id="usercard.look">API: 查看其他人名片详情/usercard/look</a>

**接口描述**

该接口需要前端在用户查看别人的名片详情时主动调用，目的是为了展示 **谁看过我** 列表

**请求描述**

**GET**  usercard/look

**参数描述**

query:

名称|类型|描述
---|---|---
seen_card_id|int|被查看的名片ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="usercard.look_me">API: 谁看过我列表</a>

**接口描述**

查询限制：

会员类型|限制数据条数
---|---
非会员|0
体验|50
月度|300
年度|不限

**请求描述**

**GET**  usercard/look_me

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|页数
limit|int|数据条数
time_type|string|时间范围，`today` / `week` / `month`  三选一，默认`today`



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 2,
        "page": 1,
        "limit": 2,
        "limit_msg": "",
        "list": [
            {
                "id": 4,
                "user_id": 804472,
                "is_public": 2, // 是否公开名片 1公开 2不公开
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardpnbdV20191101154254.png",
                "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/bVDZe20190917144835.jpeg",
                "real_name": "小小娜",
                "cellphone": "13564317032",
                "telephone": "13564317066",
                "company_type": "贸易商",
                "company_name": "张家港中集圣达因集团有限公司",
                "province_id": 18,
                "city_id": 0,
                "address": "上海浦东新区峨山路",
                "position": "产品经理",
                "main_product": "铜棒",
                "source_channel": 1, // 名片来源渠道 1pc 2app 3wx 4admin
                "admin_email": "test@smm.cn",
                "create_time": 1568704643,
                "update_time": 1572594190,
                "look_time": 1573701438, // 被此人查看的时间
                "relationship": 1 // 当前登录用户和该名片的关系：0没有关系 1已保存该用户 2互为好友 3待对方同意
            }
        ]
    }
}
```
</details>

---

#### <a id="usercard.address.book">API: 获取通讯录</a>

**请求描述**

**GET**  usercard/address/book

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|页数
limit|int|数据条数
keyword|string|关键字，模糊匹配: 姓名/手机号/电话号



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 134,
        "page": 1,
        "limit": 10,
        "list": [
            {
                "id": 3468694785,
                "name": "芭提雅司机",
                "cover_img": "",
                "job": "",
                "company": "",
                "profession": "", // 行业
                "cellphone": "0875735402",
                "telephone": "0875735402",
                "group_id": 10194,
                "group_name": "巴",
                "create_time": 1572854234,
                "user_card_id": 0, // 对应商机的名片ID，为0代表无商机名片
                "is_public": 0, // 商机名片是否公开 1公开 2不公开
                "relationship": -1 // 当前登录用户和该名片的关系：-1没有商机名片 0没有关系 1已保存该用户 2互为好友 3待对方同意
            }
        ]
    }
}
```
</details>

---

#### <a id="usercard.list.company">API: 根据企业店铺获取联系人名片列表</a>

**请求描述**

**GET**  usercard/list/company

**参数描述**

query:

名称|类型|描述
---|---|---
company_id|int|企业ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 7,
            "user_id": 807720,
            "is_public": 2, // 是否公开名片 1公开 2不公开
            "card_url": "https://test-imgqn.smm.cn/test/club/user/cardubpDF20191105173608.png",
            "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/nNaGF20190923194241.jpeg",
            "real_name": "张新杰",
            "cellphone": "13127881017",
            "telephone": "099-123456",
            "company_type": "矿产商",
            "company_name": "上海有色网股份有限公司",
            "province_id": 18,
            "city_id": 0,
            "address": "上海浦东新区峨山路91弄20号陆家嘴软件园9号楼9楼",
            "position": "后端工程师",
            "main_product": "铝合金",
            "source_channel": 4, // 名片来源渠道 1pc 2app 3wx 4admin
            "create_time": 1568788590,
            "update_time": 1572946568,
            "province": "上海",
            "city": "",
            "approval_status": 2,
            "reason": "",
            "admin_email": "",
            "industry_list": [ // 关联行业列表
                {
                    "id": 5,
                    "industry_name": "测试003",
                    "status": 2,
                    "disable": 1,
                    "card_num": 3,
                    "sort": 2,
                    "create_admin": "test@smm.cn",
                    "update_admin": "test@smm.cn",
                    "create_time": 1568701331,
                    "update_time": 1571646390
                }
            ],
            "vip_status": 2, // 会员状态 0不是会员 1过期 2服务中 3关闭
            "vip_type": 1, // 会员类型 1月度 2年度 3体验 4季度 5半年
            "relationship": 0, // 当前登录用户和该名片的关系：0没有关系 1已保存该用户 2互为好友 3待对方同意
            "group_id": 0,
            "group_name": ""
        }
    ]
}
```
</details>

---

#### <a id="usercard.info_by_user_ids">API: 根据批量用户ID获取名片或用户中心的头像和名称</a>

**请求描述**

**GET**  usercard/info_by_user_ids

**参数描述**

query:

名称|类型|描述
---|---|---
user_ids|string|逗号分割的用户ID，如：807720,804472



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "user_id": 807720,
            "avatar": "", // 用户中心头像
            "name": "张三",
            "position": "员工",
            "company_name": "上海蓝天有限公司"
        },
        {
            "user_id": 804472,
            "avatar": "",
            "name": "小小娜",
            "position": "COO",
            "company_name": "张家港中集圣达因集团有限公司"
        }
    ]
}
```
</details>

---

#### <a id="user_card.company_by_category">API: 金属产业链-根据分类关联行业查询名片</a>

**接口描述**

未登录情况下最多返回6条

**请求描述**

**GET**  user_card/company_by_category

**参数描述**

query:

名称|类型|描述
---|---|---
category_id|int|分类ID
page|int|页数
limit|int|数据条数



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 18,
        "page": 1,
        "limit": 10,
        "list": [
            {
                "id": 11,
                "user_id": 808109,
                "is_public": 1, // 是否公开名片 1公开 2不公开
                "card_url": "https://test-imgqn.smm.cn/test/b/image/rZoFUYSJaHQkABDFCXQB20191015014802.jpg",
                "avatar": "",
                "real_name": "Zhangsan",
                "cellphone": "13559669115",
                "telephone": "2570013",
                "company_type": "贸易商",
                "company_name": "商机测试02有限公司",
                "province_id": 15,
                "city_id": 89,
                "address": "芗城区石亭镇石亭东路",
                "position": "商务经理",
                "main_product": "",
                "source_channel": 1, // 名片来源渠道 1pc 2app 3wx 4admin
                "admin_email": "test@smm.cn",
                "create_time": 1569306491,
                "update_time": 1571824850,
                "open_shop": 1, // 是否开通店铺 0未开通 1开通
                "is_vip": 1 // 是否开通会员 0是 1否
            }
        ]
    }
}
```
</details>

---

#### <a id="user_card.invite_join">API: 邀请用户加入有色名片</a>

**接口描述**

发送短信通知；每个手机号最多发送一次

**请求描述**

**GET**  user_card/invite_join

**参数描述**

query:

名称|类型|描述
---|---|---
cellphone|string|手机号



<details>
<summary>响应描述</summary>

```json
{
    "code": 10150,
    "msg": "已邀请过该用户",
    "data": null
}
```
</details>

---

#### <a id="usercard.ocr_crop">API: 名片识别并切割</a>

**接口描述**

识别名片信息，且去除上传图片中名片外多余的内容

**请求描述**

**POST**  usercard/ocr_crop

**参数描述**

body:

名称|类型|描述
---|---|---
file|选择本地文件对象|名片文件



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "name": "纪清然",
        "avatar": "",
        "cover_img": "https://test-imgqn.smm.cn/test/club/user/cardzvshk20191114114034.png",
        "back_img": "",
        "job": "经理助理",
        "company": "上海宸楠贵金属有限公司",
        "profession": "经理助理",
        "city": "上海",
        "cellphone": "18611226703",
        "telephone": "02161406653",
        "email": "16012410@qq.com",
        "address": "上海曹杨路505号尚城国际大厦1001 室",
        "website": "www.ychmetal.com"
    }
}
```
</details>

### <a id="item_tiezixinxi_663582000">帖子信息</a>

> 该模块下所有接口中说的`帖子`（老版本叫法）无特殊说明都代表一条普通的信息，每条信息的属性`post_type`有`1`（商品）和`2`（帖子，新版本叫法）的区分。  

---|post记录|`post_type`(1)|`post_type`(2)
---|---|---|---
老版本|帖子|产品|其他
新版本|信息|商品|帖子


---

#### <a id="post.club">API: 圈子主页帖子列表</a>

**请求描述**

**GET**  post/club

**参数描述**

query:

名称|类型|描述
---|---|---
club_id|int|圈子ID 必填
post_type|int|帖子类型 `0`全部 `1`商品 `2`帖子/其他
page|int|页数
limit|int|数据条数



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 6,
        "post_list": [
            {
                "id": 212362,
                "user_id": 808117, // 用户ID
                "company_id": 1001629, // 企业/店铺ID
                "title": "专业回收银焊条13580887176现金收购银焊片，银焊环",
                "post_type": 1, // 信息类型 1商品 2帖子
                "price": 0,
                "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
                "province_id": 12,
                "city_id": 51,
                "club_id": 111,
                "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 0正常 1推荐
                "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1570867564,
                "created_time": 1561619403,
                "post_content_rtf": "<p>宏锦金银回收有限公司面向全国高价回收<br />\n金废料：金盐，钯盐，金水，镀金，金膏，金丝，氯化钯；</p>\n\n<p>银废料：银浆，银浆罐，擦银布，银胶，银膏，银焊条，银触点，氯化银，硫化银，925银。<br />\n&nbsp;<br />\n钌废料：钌浆，废钌，粗钌，工业钌，钌催化剂，钌碳</p>\n\n<p>钯废料：氧化钯，胶体钯，钯水，钯盐，钯粉，钯浆，钯碳，钯催化剂，线路板钯水，钯块，钯片，钯板，废料钯&nbsp;</p>\n\n<p>&nbsp;全国免费上门，现场看货，现金支付 24小时热线：13580887176 陈生</p>\n", // 富文本内容
                "post_content_txt": "", // 纯文本内容
                "cover_pic": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 封面
                "product_pic_set": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 图片集合
                "admin_email": "",
                "top": 1, // 是否置顶 0否 1是
                "is_notice": 0, // 是否通知 0否 1是
                "refresh_time": 0, // 最后一次刷新时间
                "is_offer": 0, // 是否报价 0否 1是
                "pic_amount": 1, // 图片总数
                "is_crawl": 0, // 是否爬虫抓取 0否 1是
                "unit": "",
                "area": "",
                "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
                "reason": "", // 审核拒绝原因
                "approval_time": 0, // 审核时间
                "approver_email": "",
                "click_count": 7, // 点击量
                "sale_number": "0", // 可售数量
                "valid_period": 100, // 有效期（天）
                "valid_period_time": 1582182175, // 有效期时间戳
                "category_id": 0, // 所属顶级分类ID
                "last_category_id": 0, // 所属分类
                "is_vip": 2, // 发布人是否会员 1是 2否
                "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "", // gps 省份
                "location_city": "", // gps 城市
                "location_gps": "", // GPS 经纬度
                "navbar_name": "铜",
                "club_name": "铜棒",
                "province_name": "江苏",
                "city_name": "盐城市",
                "user_info": { // 发布人名片
                    "id": 44, // 名片ID
                    "user_id": 808117,
                    "is_public": 1, 
                    "card_url": "https://test-imgqn.smm.cn/club/user/cardaQEte20191030103235.png",
                    "avatar": "",
                    "real_name": "135****2056",
                    "cellphone": "13585952056",
                    "telephone": "13585952056",
                    "company_type": "",
                    "company_name": "CCtest",
                    "province_id": 0,
                    "city_id": 0,
                    "address": "",
                    "position": "",
                    "main_product": "",
                    "source_channel": 4,
                    "admin_email": "olduser@smm.cn",
                    "create_time": 1570774034,
                    "update_time": 1570774034
                },
                "attribute": [ // 信息属性
                    {
                        "attribute_id": 490,
                        "name": "牌号",
                        "attr_type": 2, // 1单选 2文本
                        "attr_options": "", // 单选时为逗号分隔的选项 文本时为正则表达式
                        "attr_unit": "",
                        "attr_value": "不限"
                    }
                ],
                "company_name": "CCtest",
                "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
                "vip_company_status_desc": "服务中",
                "vip_year": 6, // 店铺服务年限
                "qidian_wpa_url": "", // 企点URL
                "category_name": "",
                "last_category_name": ""
            }
        ]
    }
}
```
</details>

---

#### <a id="post.category.list">API: 分类主页</a>

**请求描述**

**GET**  post/category/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|页数
limit|int|数据条数
category_id|int|分类ID
post_type|int|信息类型：`1`产品 `2`其他
province_id|int|省份ID
low_price|float|最低价 包含
high_price|float|最高价，包含
is_offer|int|是否报价：`-1`全部 `0`议价 `1`是  
attributes|string|属性json，例如:  [{"attribute_id":123,"attr_value":"abc"},{"attribute_id":123,"attr_value":"abc"}]



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 0,
        "post_list": [
        	{
                "id": 212362,
                "user_id": 808117, // 用户ID
                "company_id": 1001629, // 企业/店铺ID
                "title": "专业回收银焊条13580887176现金收购银焊片，银焊环",
                "post_type": 1, // 信息类型 1商品 2帖子
                "price": 0,
                "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
                "province_id": 12,
                "city_id": 51,
                "club_id": 111,
                "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 0正常 1推荐
                "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1570867564,
                "created_time": 1561619403,
                "post_content_rtf": "<p>宏锦金银回收有限公司面向全国高价回收<br />\n金废料：金盐，钯盐，金水，镀金，金膏，金丝，氯化钯；</p>\n\n<p>银废料：银浆，银浆罐，擦银布，银胶，银膏，银焊条，银触点，氯化银，硫化银，925银。<br />\n&nbsp;<br />\n钌废料：钌浆，废钌，粗钌，工业钌，钌催化剂，钌碳</p>\n\n<p>钯废料：氧化钯，胶体钯，钯水，钯盐，钯粉，钯浆，钯碳，钯催化剂，线路板钯水，钯块，钯片，钯板，废料钯&nbsp;</p>\n\n<p>&nbsp;全国免费上门，现场看货，现金支付 24小时热线：13580887176 陈生</p>\n", // 富文本内容
                "post_content_txt": "", // 纯文本内容
                "cover_pic": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 封面
                "product_pic_set": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 图片集合
                "admin_email": "",
                "top": 1, // 是否置顶 0否 1是
                "is_notice": 0, // 是否通知 0否 1是
                "refresh_time": 0, // 最后一次刷新时间
                "is_offer": 0, // 是否报价 0否 1是
                "pic_amount": 1, // 图片总数
                "is_crawl": 0, // 是否爬虫抓取 0否 1是
                "unit": "",
                "area": "",
                "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
                "reason": "", // 审核拒绝原因
                "approval_time": 0, // 审核时间
                "approver_email": "",
                "click_count": 7, // 点击量
                "sale_number": "0", // 可售数量
                "valid_period": 100, // 有效期（天）
                "valid_period_time": 1582182175, // 有效期时间戳
                "category_id": 0, // 所属顶级分类ID
                "last_category_id": 0, // 所属分类
                "is_vip": 2, // 发布人是否会员 1是 2否
                "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "", // gps 省份
                "location_city": "", // gps 城市
                "location_gps": "", // GPS 经纬度
                "navbar_name": "铜",
                "club_name": "铜棒",
                "province_name": "江苏",
                "city_name": "盐城市",
                "user_info": { // 发布人名片
                    "id": 44, // 名片ID
                    "user_id": 808117,
                    "is_public": 1, 
                    "card_url": "https://test-imgqn.smm.cn/club/user/cardaQEte20191030103235.png",
                    "avatar": "",
                    "real_name": "135****2056",
                    "cellphone": "13585952056",
                    "telephone": "13585952056",
                    "company_type": "",
                    "company_name": "CCtest",
                    "province_id": 0,
                    "city_id": 0,
                    "address": "",
                    "position": "",
                    "main_product": "",
                    "source_channel": 4,
                    "admin_email": "olduser@smm.cn",
                    "create_time": 1570774034,
                    "update_time": 1570774034
                },
                "attribute": [ // 信息属性
                    {
                        "attribute_id": 490,
                        "name": "牌号",
                        "attr_type": 2, // 1单选 2文本
                        "attr_options": "", // 单选时为逗号分隔的选项 文本时为正则表达式
                        "attr_unit": "",
                        "attr_value": "不限"
                    }
                ],
                "company_name": "CCtest",
                "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
                "vip_company_status_desc": "服务中",
                "vip_year": 6, // 店铺服务年限
                "qidian_wpa_url": "", // 企点URL
                "category_name": "",
                "last_category_name": ""
            }	
    	]
    }
}
```
</details>

---

#### <a id="post.list">API: 按条件查询帖子列表</a>

**接口描述**

is_vip：1是商机会员 2不是

vip_type：1月度 2年度 3体验

valid_period：有效期 （天）

**请求描述**

**GET**  post/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|页数
limit|int|数据条数
filter|string|搜索类型，必填<br/>`my_club`：我的圈子，必须登录<br/>`hot`：热门推荐<br/>`club`：圈子，`club_id`必填<br/>`user`：个人主页，`user`必填<br/>`my_post`：我的主页，必须登录<br/>`company`：店铺主页，`company_id`必填<br/>`click`：按点击量<br/>`category`：按分类，`category_id`必填<br/>`nearby`：附近，`province_id`必填<br/>`latest`：最新
category_id|int|分类ID
club_id|int|圈子ID
user|int|用户ID
post_type|int|参数`filter`=`company`时有效，`1`商品 `2`帖子
company_id|int|企业ID
province_id|int|省份ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 4,
        "post_list": [
            {
                "id": 212362,
                "user_id": 808117, // 用户ID
                "company_id": 1001629, // 企业/店铺ID
                "title": "专业回收银焊条13580887176现金收购银焊片，银焊环",
                "post_type": 1, // 信息类型 1商品 2帖子
                "price": 0,
                "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
                "province_id": 12,
                "city_id": 51,
                "club_id": 111,
                "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 0正常 1推荐
                "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1570867564,
                "created_time": 1561619403,
                "post_content_rtf": "<p>宏锦金银回收有限公司面向全国高价回收<br />\n金废料：金盐，钯盐，金水，镀金，金膏，金丝，氯化钯；</p>\n\n<p>银废料：银浆，银浆罐，擦银布，银胶，银膏，银焊条，银触点，氯化银，硫化银，925银。<br />\n&nbsp;<br />\n钌废料：钌浆，废钌，粗钌，工业钌，钌催化剂，钌碳</p>\n\n<p>钯废料：氧化钯，胶体钯，钯水，钯盐，钯粉，钯浆，钯碳，钯催化剂，线路板钯水，钯块，钯片，钯板，废料钯&nbsp;</p>\n\n<p>&nbsp;全国免费上门，现场看货，现金支付 24小时热线：13580887176 陈生</p>\n", // 富文本内容
                "post_content_txt": "", // 纯文本内容
                "cover_pic": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 封面
                "product_pic_set": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 图片集合
                "admin_email": "",
                "top": 1, // 是否置顶 0否 1是
                "is_notice": 0, // 是否通知 0否 1是
                "refresh_time": 0, // 最后一次刷新时间
                "is_offer": 0, // 是否报价 0否 1是
                "pic_amount": 1, // 图片总数
                "is_crawl": 0, // 是否爬虫抓取 0否 1是
                "unit": "",
                "area": "",
                "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
                "reason": "", // 审核拒绝原因
                "approval_time": 0, // 审核时间
                "approver_email": "",
                "click_count": 7, // 点击量
                "sale_number": "0", // 可售数量
                "valid_period": 100, // 有效期（天）
                "valid_period_time": 1582182175, // 有效期时间戳
                "category_id": 0, // 所属顶级分类ID
                "last_category_id": 0, // 所属分类
                "is_vip": 2, // 发布人是否会员 1是 2否
                "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "", // gps 省份
                "location_city": "", // gps 城市
                "location_gps": "", // GPS 经纬度
                "navbar_name": "铜",
                "club_name": "铜棒",
                "province_name": "江苏",
                "city_name": "盐城市",
                "user_info": { // 发布人名片
                    "id": 44, // 名片ID
                    "user_id": 808117,
                    "is_public": 1, 
                    "card_url": "https://test-imgqn.smm.cn/club/user/cardaQEte20191030103235.png",
                    "avatar": "",
                    "real_name": "135****2056",
                    "cellphone": "13585952056",
                    "telephone": "13585952056",
                    "company_type": "",
                    "company_name": "CCtest",
                    "province_id": 0,
                    "city_id": 0,
                    "address": "",
                    "position": "",
                    "main_product": "",
                    "source_channel": 4,
                    "admin_email": "olduser@smm.cn",
                    "create_time": 1570774034,
                    "update_time": 1570774034
                },
                "attribute": [ // 信息属性
                    {
                        "attribute_id": 490,
                        "name": "牌号",
                        "attr_type": 2, // 1单选 2文本
                        "attr_options": "", // 单选时为逗号分隔的选项 文本时为正则表达式
                        "attr_unit": "",
                        "attr_value": "不限"
                    }
                ],
                "company_name": "CCtest",
                "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
                "vip_company_status_desc": "服务中",
                "vip_year": 6, // 店铺服务年限
                "qidian_wpa_url": "", // 企点URL
                "category_name": "",
                "last_category_name": ""
            }
        ]
    }
}
```
</details>

---

#### <a id="post.info.post_id">API: 帖子详情</a>

**请求描述**

**GET**  post/info/:post_id

**参数描述**

path:

名称|类型|描述
---|---|---
post_id|int|信息ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "post_info": {
            "id": 213389,
            "user_id": 807748, // 用户ID
            "company_id": 1001572, // 企业/店铺ID
            "title": "我这个账号是有企Q的哦",
            "post_type": 1, // 信息类型 1商品 2帖子
            "price": 0,
            "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
            "province_id": 20,
            "city_id": 144,
            "club_id": 22,
            "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
            "is_recommend": 0, // 是否推荐 0正常 1推荐
            "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
            "updated_time": 1571905231,
            "created_time": 1571905231,
            "post_content_rtf": "", // 富文本内容
            "post_content_txt": "", // 纯文本内容
            "cover_pic": "https://test-imgqn.smm.cn/test/b/image/EYcjagsUSDUxKQvYfNlO20191024042026.jpg", // 封面
            "product_pic_set": "https://test-imgqn.smm.cn/test/b/image/kgeKsKmfakQBrFSjkLow20191024042026.jpg;https://test-imgqn.smm.cn/test/b/image/PVnORfRFEwGXPbiWlPFm20191024042026.jpg;https://test-imgqn.smm.cn/test/b/image/EYcjagsUSDUxKQvYfNlO20191024042026.jpg", // 图片集合
            "admin_email": "",
            "top": 0, // 是否置顶 0否 1是
            "is_notice": 0, // 是否通知 0否 1是
            "refresh_time": 0, // 最后一次刷新时间
            "is_offer": 0, // 是否报价 0否 1是
            "pic_amount": 3, // 图片总数
            "is_crawl": 0, // 是否爬虫抓取 0否 1是
            "unit": "",
            "area": "",
            "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
            "reason": "", // 审核拒绝原因
            "approval_time": 1571906970, // 审核时间
            "approver_email": "test@smm.cn",
            "click_count": 11, // 点击量
            "sale_number": "222", // 可售数量
            "valid_period": 100, // 有效期（天）
            "valid_period_time": 1582182175, // 有效期时间戳
            "category_id": 2, // 所属顶级分类ID
            "last_category_id": 8, // 所属分类
            "is_vip": 1, // 发布人是否会员 1是 2否
            "vip_type": 2, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
            "location_province": "", // gps 省份
            "location_city": "", // gps 城市
            "location_gps": "", // GPS 经纬度
            "navbar_name": "铜",
            "club_name": "电解铜",
            "province_name": "广西",
            "city_name": "桂林市",
            "user_info": { // 发布人名片
                "id": 64, // 名片ID
                "user_id": 807748,
                "is_public": 1,
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardcfLqK20191029145002.png",
                "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/LBVmh20190625135010.jpeg",
                "real_name": "吴梦娜",
                "cellphone": "18512197032",
                "telephone": "18512154782",
                "company_type": "矿产商",
                "company_name": "测试贸易12134",
                "province_id": 18,
                "city_id": 0,
                "address": "峨山路",
                "position": "小职员",
                "main_product": "铜铝铅",
                "source_channel": 1,
                "admin_email": "olduser@smm.cn",
                "create_time": 1570863392,
                "update_time": 1573187590
            },
            "attribute": [ // 信息属性
                {
                    "attribute_id": 42,
                    "name": "正则",
                    "attr_type": 2, // 1单选 2文本
                    "attr_options": "^[A-Za-z0-9]+$", // 单选时为逗号分隔的选项 文本时为正则表达式
                    "attr_unit": "",
                    "attr_value": "22"
                }
            ],
            "company_name": "测试贸易12134",
            "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
            "vip_company_status_desc": "服务中",
            "vip_year": 5, // 店铺服务年限
            "qidian_wpa_url": "http://q.url.cn/ABoDYP?_type=wpa&qidian=true", // 企点URL
            "category_name": "铜",
            "last_category_name": "电解铜"
        }
    }
}
```
</details>

---

#### <a id="post.recommend">API: 帖子详情推荐帖子</a>

**请求描述**

**GET**  post/recommend

**参数描述**

query:

名称|类型|描述
---|---|---
post_id|int|信息ID，不包括此ID的同一用户发布的其他帖子



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "author_post_list": [ // 除参数外的其他同一用户信息，最多5条
            {
                "id": 212362,
                "user_id": 808117, // 用户ID
                "company_id": 1001629, // 企业/店铺ID
                "title": "专业回收银焊条13580887176现金收购银焊片，银焊环",
                "post_type": 1, // 信息类型 1商品 2帖子
                "price": 0,
                "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
                "province_id": 12,
                "city_id": 51,
                "club_id": 111,
                "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 0正常 1推荐
                "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1570867564,
                "created_time": 1561619403,
                "post_content_rtf": "<p>宏锦金银回收有限公司面向全国高价回收<br />\n金废料：金盐，钯盐，金水，镀金，金膏，金丝，氯化钯；</p>\n\n<p>银废料：银浆，银浆罐，擦银布，银胶，银膏，银焊条，银触点，氯化银，硫化银，925银。<br />\n&nbsp;<br />\n钌废料：钌浆，废钌，粗钌，工业钌，钌催化剂，钌碳</p>\n\n<p>钯废料：氧化钯，胶体钯，钯水，钯盐，钯粉，钯浆，钯碳，钯催化剂，线路板钯水，钯块，钯片，钯板，废料钯&nbsp;</p>\n\n<p>&nbsp;全国免费上门，现场看货，现金支付 24小时热线：13580887176 陈生</p>\n", // 富文本内容
                "post_content_txt": "", // 纯文本内容
                "cover_pic": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 封面
                "product_pic_set": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 图片集合
                "admin_email": "",
                "top": 1, // 是否置顶 0否 1是
                "is_notice": 0, // 是否通知 0否 1是
                "refresh_time": 0, // 最后一次刷新时间
                "is_offer": 0, // 是否报价 0否 1是
                "pic_amount": 1, // 图片总数
                "is_crawl": 0, // 是否爬虫抓取 0否 1是
                "unit": "",
                "area": "",
                "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
                "reason": "", // 审核拒绝原因
                "approval_time": 0, // 审核时间
                "approver_email": "",
                "click_count": 7, // 点击量
                "sale_number": "0", // 可售数量
                "valid_period": 100, // 有效期（天）
                "valid_period_time": 1582182175, // 有效期时间戳
                "category_id": 0, // 所属顶级分类ID
                "last_category_id": 0, // 所属分类
                "is_vip": 2, // 发布人是否会员 1是 2否
                "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "", // gps 省份
                "location_city": "", // gps 城市
                "location_gps": "", // GPS 经纬度
                "navbar_name": "铜",
                "club_name": "铜棒",
                "province_name": "江苏",
                "city_name": "盐城市",
                "user_info": { // 发布人名片
                    "id": 44, // 名片ID
                    "user_id": 808117,
                    "is_public": 1, 
                    "card_url": "https://test-imgqn.smm.cn/club/user/cardaQEte20191030103235.png",
                    "avatar": "",
                    "real_name": "135****2056",
                    "cellphone": "13585952056",
                    "telephone": "13585952056",
                    "company_type": "",
                    "company_name": "CCtest",
                    "province_id": 0,
                    "city_id": 0,
                    "address": "",
                    "position": "",
                    "main_product": "",
                    "source_channel": 4,
                    "admin_email": "olduser@smm.cn",
                    "create_time": 1570774034,
                    "update_time": 1570774034
                },
                "attribute": [ // 信息属性
                    {
                        "attribute_id": 490,
                        "name": "牌号",
                        "attr_type": 2, // 1单选 2文本
                        "attr_options": "", // 单选时为逗号分隔的选项 文本时为正则表达式
                        "attr_unit": "",
                        "attr_value": "不限"
                    }
                ],
                "company_name": "CCtest",
                "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
                "vip_company_status_desc": "服务中",
                "vip_year": 6, // 店铺服务年限
                "qidian_wpa_url": "", // 企点URL
                "category_name": "",
                "last_category_name": ""
            }
        ],
        "other_post_list": [
        	// 除参数外的其他同一用户同一圈子信息，最多10条，置顶排序
        ]
    }
}
```
</details>

---

#### <a id="post.settle.top">API: 设置帖子在圈子中置顶</a>

**请求描述**

**POST**  post/settle/top

**参数描述**

body:

名称|类型|描述
---|---|---
post_id|int|信息ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="post.cancel.top">API: 取消置顶圈子中的帖子</a>

**请求描述**

**POST**  post/cancel/top

**参数描述**

body:

名称|类型|描述
---|---|---
post_id|int|信息ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="post.settle.notice">API: 设置公告帖子信息</a>

**请求描述**

**POST**  post/settle/notice

**参数描述**

body:

名称|类型|描述
---|---|---
post_id|int|信息ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="post.cancel.notice">API: 取消公告帖子信息</a>

**请求描述**

**POST**  post/cancel/notice

**参数描述**

body:

名称|类型|描述
---|---|---
post_id|int|信息ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="post.alter.price">API: 修改帖子报价</a>

**请求描述**

**POST**  post/alter/price

**参数描述**

body:

名称|类型|描述
---|---|---
post_id|int|信息ID
is_offer|int|是否报价：`1`是 `0`议价
price|float|可小数，价格
quantity_unit|int|单位：`1`吨 `2`千克 `3`组 `4`只



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="post.refresh.time">API: 刷新帖子时间</a>

**请求描述**

**GET**  post/refresh/time

**参数描述**

query:

名称|类型|描述
---|---|---
post_id|int|要刷新时间的帖子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="post.delete.id">API: 删除帖子</a>

**请求描述**

**GET**  post/delete/:id

**参数描述**

path:

名称|类型|描述
---|---|---
id|int|帖子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="post.publish">API: 发布帖子信息</a>

**请求描述**

**POST**  post/publish

**参数描述**

body:

名称|类型|描述
---|---|---
club_id|int|同步到商圈的圈子ID，`post_type`=`1`可选，=`2`必选
title|string|信息标题
post_type|int|信息类型：`1`商品 `2`其他
device_type|int|发布渠道 `1`:web `2`:h5 `3`android `4`ios `5`小程序
product_attr_json|string|帖子属性，例如：[{"id":1,"value":"mi"}]
city_id|int|城市ID
province_id|int|省份ID
product_pic_set|string|帖子图片
cover_pic|string|帖子封面
price|float|价格
quantity_unit|int|单位：`1`：吨 `2`：千克 `3`：组 `4`：只
is_offer|int|是否报价  `0`否 `1`是
post_content_rtf|string|富文本帖子内容
post_content_txt|string|纯文本帖子内容
pic_amount|int|帖子图片数量
sale_number|string|可售数量
valid_period|int|有效期，非VIP会员为`1`，会员可选 `1`、`7`、`30`、`90`
category_id|int|帖子顶级分类ID
last_category_id|int|帖子所属分类ID
location_province|string|GPS所在位置省份，手机端参数
location_city|string|GPS所在位置城市，手机端参数
location_gps|string|GPS所在位置经纬度，纬度在前，经度在后，手机端参数



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "post_id": 213488 // 发布成功的信息ID
    }
}
```
</details>

---

#### <a id="post.edit">API: 编辑帖子信息</a>

**请求描述**

**POST**  post/edit

**参数描述**

body:

名称|类型|描述
---|---|---
post_id|int|信息ID
title|string|信息标题
post_type|int|信息类型：`1`商品 `2`帖子
device_type|int|发布渠道 `1`:web `2`:h5 `3`android `4`ios `5`小程序
city_id|int|城市ID
province_id|int|省份ID
price|float|价格
quantity_unit|int|单位：`1`：吨 `2`：千克 `3`：组 `4`：只
is_offer|int|是否报价 `0`否 `1`是
sale_number|string|可售数量
valid_period|int| 有效期(天)，非VIP会员为`1`，会员可选 `1`、`7`、`30`、`90`
product_pic_set|string|帖子图片
cover_pic|string|帖子封面
location_province|string|GPS所在位置省份，手机端参数
location_city|string|GPS所在位置城市，手机端参数
location_gps|string|GPS所在位置经纬度，纬度在前，经度在后，手机端参数



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="post.template">API: 帖子模版</a>

**请求描述**

**GET**  post/template

**参数描述**

query:

名称|类型|描述
---|---|---
category_id|int|分类ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "template": {
            "attribute": [
                {
                    "id": 42,
                    "name": "正则",
                    "attr_type": 2, // 1单选 2文本
                    "attr_options": "^[A-Za-z0-9]+$", // 单选时为逗号分隔的选项 文本时为正则表达式
                    "attr_unit": "",
                    "sort_number": 0
                },
                {
                    "id": 43,
                    "name": "品牌",
                    "attr_type": 2,
                    "attr_options": "^[A-Za-z0-9]+$",
                    "attr_unit": "",
                    "sort_number": 0
                }
            ],
            "quantity_unit_list": [ // 常量
                {
                    "id": 1,
                    "value": "吨"
                },
                {
                    "id": 2,
                    "value": "千克"
                },
                {
                    "id": 3,
                    "value": "组"
                },
                {
                    "id": 4,
                    "value": "只"
                }
            ]
        }
    }
}
```
</details>

---

#### <a id="app.recommend.info">API: m站推荐详情</a>

**请求描述**

**GET**  app/recommend/info

**参数描述**

query:

名称|类型|描述
---|---|---
post_id|int|信息ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "club_list": [ // 推荐圈子 最多17条
            {
                "id": 111,
                "user_id": 807584,
                "name": "铜棒",
                "introduction": "本圈为铜棒交流圈，可在圈里发布与铜棒相关的买卖信息、最新市场价格行情等", // 圈子简介
                "logo": "https://imgqn.smm.cn/production/b/image/eJFOnGyXasSBAyWQcsjG20181030013937.png",
                "h5_background": "",
                "web_background": "https://imgqn.smm.cn/production/b/image/yYmTNAayLsSmDZGukUaV20181030113602.jpg",
                "is_recommend": 0, // 是否推荐 0否 1推荐
                "disabled": 0, // 是否禁用 0否 1禁用
                "updated_time": 1573007671,
                "created_time": 1540384121,
                "members_amount": 19, // 圈内成员数
                "post_amount": 34, // 圈内信息数
                "today_post_amount": 0, // 今日圈内信息数
                "admin_email": "test@smm.cn",
                "is_audit": 0
            }
        ],
        "post_list": [ // 推荐信息 最多20条
            {
                "id": 212362,
                "user_id": 808117, // 用户ID
                "company_id": 1001629, // 企业/店铺ID
                "title": "专业回收银焊条13580887176现金收购银焊片，银焊环",
                "post_type": 1, // 信息类型 1商品 2帖子
                "price": 0,
                "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
                "province_id": 12,
                "city_id": 51,
                "club_id": 111,
                "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 0正常 1推荐
                "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1570867564,
                "created_time": 1561619403,
                "post_content_rtf": "<p>宏锦金银回收有限公司面向全国高价回收<br />\n金废料：金盐，钯盐，金水，镀金，金膏，金丝，氯化钯；</p>\n\n<p>银废料：银浆，银浆罐，擦银布，银胶，银膏，银焊条，银触点，氯化银，硫化银，925银。<br />\n&nbsp;<br />\n钌废料：钌浆，废钌，粗钌，工业钌，钌催化剂，钌碳</p>\n\n<p>钯废料：氧化钯，胶体钯，钯水，钯盐，钯粉，钯浆，钯碳，钯催化剂，线路板钯水，钯块，钯片，钯板，废料钯&nbsp;</p>\n\n<p>&nbsp;全国免费上门，现场看货，现金支付 24小时热线：13580887176 陈生</p>\n", // 富文本内容
                "post_content_txt": "", // 纯文本内容
                "cover_pic": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 封面
                "product_pic_set": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 图片集合
                "admin_email": "",
                "top": 1, // 是否置顶 0否 1是
                "is_notice": 0, // 是否通知 0否 1是
                "refresh_time": 0, // 最后一次刷新时间
                "is_offer": 0, // 是否报价 0否 1是
                "pic_amount": 1, // 图片总数
                "is_crawl": 0, // 是否爬虫抓取 0否 1是
                "unit": "",
                "area": "",
                "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
                "reason": "", // 审核拒绝原因
                "approval_time": 0, // 审核时间
                "approver_email": "",
                "click_count": 7, // 点击量
                "sale_number": "0", // 可售数量
                "valid_period": 100, // 有效期（天）
                "valid_period_time": 1582182175, // 有效期时间戳
                "category_id": 0, // 所属顶级分类ID
                "last_category_id": 0, // 所属分类
                "is_vip": 2, // 发布人是否会员 1是 2否
                "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "", // gps 省份
                "location_city": "", // gps 城市
                "location_gps": "", // GPS 经纬度
                "navbar_name": "铜",
                "club_name": "铜棒",
                "province_name": "江苏",
                "city_name": "盐城市",
                "user_info": { // 发布人名片
                    "id": 44, // 名片ID
                    "user_id": 808117,
                    "is_public": 1, 
                    "card_url": "https://test-imgqn.smm.cn/club/user/cardaQEte20191030103235.png",
                    "avatar": "",
                    "real_name": "135****2056",
                    "cellphone": "13585952056",
                    "telephone": "13585952056",
                    "company_type": "",
                    "company_name": "CCtest",
                    "province_id": 0,
                    "city_id": 0,
                    "address": "",
                    "position": "",
                    "main_product": "",
                    "source_channel": 4,
                    "admin_email": "olduser@smm.cn",
                    "create_time": 1570774034,
                    "update_time": 1570774034
                },
                "attribute": [ // 信息属性
                    {
                        "attribute_id": 490,
                        "name": "牌号",
                        "attr_type": 2, // 1单选 2文本
                        "attr_options": "", // 单选时为逗号分隔的选项 文本时为正则表达式
                        "attr_unit": "",
                        "attr_value": "不限"
                    }
                ],
                "company_name": "CCtest",
                "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
                "vip_company_status_desc": "服务中",
                "vip_year": 6, // 店铺服务年限
                "qidian_wpa_url": "", // 企点URL
                "category_name": "",
                "last_category_name": ""
            }
        ]
    }
}
```
</details>

---

#### <a id="post.sitmap.list">API: 帖子sitmap列表</a>

**请求描述**

**GET**  post/sitmap/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
begin_time|int|信息更新开始时间
end_time|int|信息更新结束时间



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 7731,
        "post_site_map_list": [
            {
                "id": 205003, // 信息ID
                "created_time": 1547817898,
                "updated_time": 1573713832
            },
            {
                "id": 213474,
                "created_time": 1573634904,
                "updated_time": 1573634985
            }
        ]
    }
}
```
</details>

---

#### <a id="post.latest">API: 企点获取用户最新修改的5条帖子</a>

**请求描述**

**GET**  post/latest

**参数描述**

query:

名称|类型|描述
---|---|---
user_id|int|信息ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "list": [
            {
                "time": "11/07", // 更新日期
                "category": "氧化铝", // 圈子名称
                "content": "tttttt", // 信息标题
                "shopUrl": "https://testb.smm.cn/info/213426" // 信息链接
            },
            {
                "time": "10/08",
                "category": "马达",
                "content": "6瓦沟通调速电机 2IK6RGN-C单相马达异步交",
                "shopUrl": "https://testb.smm.cn/info/206404"
            }
        ],
        "moreUrl": "https://testb.smm.cn/p/807720" // 查看更多链接
    }
}
```
</details>

---

#### <a id="post.exclude.latest">API: 根据用户ID获取最新的n条帖子</a>

**请求描述**

**GET**  post/exclude/latest

**参数描述**

query:

名称|类型|描述
---|---|---
limit|int|数据条数
user_id|int|用户ID
exclude_post_id|int|排除的信息ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 213470,
            "user_id": 807720, // 用户ID
            "company_id": 1001764, // 企业/店铺ID
            "title": "撒地方撒",
            "post_type": 1, // 信息类型 1商品 2帖子
            "price": 0,
            "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
            "province_id": 37,
            "city_id": 0,
            "club_id": 0,
            "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
            "is_recommend": 0, // 是否推荐 0正常 1推荐
            "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
            "updated_time": 1573634453,
            "created_time": 1573634453,
            "post_content_rtf": "<p>是打发时</p>\n", // 富文本内容
            "post_content_txt": "是打发时", // 纯文本内容
            "cover_pic": "https://test-imgqn.smm.cn/test/b/image/ISKYoNOsUBnZMMJRFxFL20191113044045.png", // 封面
            "product_pic_set": "https://test-imgqn.smm.cn/test/b/image/ISKYoNOsUBnZMMJRFxFL20191113044045.png", // 图片集合
            "admin_email": "",
            "top": 0, // 是否置顶 0否 1是
            "is_notice": 0, // 是否通知 0否 1是
            "refresh_time": 0, // 最后一次刷新时间
            "is_offer": 0, // 是否报价 0否 1是
            "pic_amount": 1,
            "is_crawl": 0, // 是否爬虫抓取 0否 1是
            "unit": "",
            "area": "",
            "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
            "reason": "", // 审核拒绝原因
            "approval_time": 1573634517, // 审核时间
            "approver_email": "test@smm.cn",
            "click_count": 6, // 点击量
            "sale_number": "", // 可售数量
            "valid_period": 1, // 有效期（天）
            "valid_period_time": 1573720917, // 有效期时间戳
            "category_id": 61, // 所属顶级分类ID
            "last_category_id": 66, // 所属分类
            "is_vip": 1, // 发布人是否会员 1是 2否
            "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
            "location_province": "", // gps 省份
            "location_city": "", // gps 城市
            "location_gps": "" // GPS 经纬度
        }
    ]
}
```
</details>

---

#### <a id="post.product.latest">API: 商机首页最新商品</a>

**接口描述**

接口有缓存，5分钟；最多返回4条数据

**请求描述**

**GET**  post/product/latest



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
                "id": 212362,
                "user_id": 808117, // 用户ID
                "company_id": 1001629, // 企业/店铺ID
                "title": "专业回收银焊条13580887176现金收购银焊片，银焊环",
                "post_type": 1, // 信息类型 1商品 2帖子
                "price": 0,
                "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
                "province_id": 12,
                "city_id": 51,
                "club_id": 111,
                "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 0正常 1推荐
                "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1570867564,
                "created_time": 1561619403,
                "post_content_rtf": "<p>宏锦金银回收有限公司面向全国高价回收<br />\n金废料：金盐，钯盐，金水，镀金，金膏，金丝，氯化钯；</p>\n\n<p>银废料：银浆，银浆罐，擦银布，银胶，银膏，银焊条，银触点，氯化银，硫化银，925银。<br />\n&nbsp;<br />\n钌废料：钌浆，废钌，粗钌，工业钌，钌催化剂，钌碳</p>\n\n<p>钯废料：氧化钯，胶体钯，钯水，钯盐，钯粉，钯浆，钯碳，钯催化剂，线路板钯水，钯块，钯片，钯板，废料钯&nbsp;</p>\n\n<p>&nbsp;全国免费上门，现场看货，现金支付 24小时热线：13580887176 陈生</p>\n", // 富文本内容
                "post_content_txt": "", // 纯文本内容
                "cover_pic": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 封面
                "product_pic_set": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 图片集合
                "admin_email": "",
                "top": 1, // 是否置顶 0否 1是
                "is_notice": 0, // 是否通知 0否 1是
                "refresh_time": 0, // 最后一次刷新时间
                "is_offer": 0, // 是否报价 0否 1是
                "pic_amount": 1, // 图片总数
                "is_crawl": 0, // 是否爬虫抓取 0否 1是
                "unit": "",
                "area": "",
                "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
                "reason": "", // 审核拒绝原因
                "approval_time": 0, // 审核时间
                "approver_email": "",
                "click_count": 7, // 点击量
                "sale_number": "0", // 可售数量
                "valid_period": 100, // 有效期（天）
                "valid_period_time": 1582182175, // 有效期时间戳
                "category_id": 0, // 所属顶级分类ID
                "last_category_id": 0, // 所属分类
                "is_vip": 2, // 发布人是否会员 1是 2否
                "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "", // gps 省份
                "location_city": "", // gps 城市
                "location_gps": "", // GPS 经纬度
                "navbar_name": "铜",
                "club_name": "铜棒",
                "province_name": "江苏",
                "city_name": "盐城市",
                "user_info": { // 发布人名片
                    "id": 44, // 名片ID
                    "user_id": 808117,
                    "is_public": 1, 
                    "card_url": "https://test-imgqn.smm.cn/club/user/cardaQEte20191030103235.png",
                    "avatar": "",
                    "real_name": "135****2056",
                    "cellphone": "13585952056",
                    "telephone": "13585952056",
                    "company_type": "",
                    "company_name": "CCtest",
                    "province_id": 0,
                    "city_id": 0,
                    "address": "",
                    "position": "",
                    "main_product": "",
                    "source_channel": 4,
                    "admin_email": "olduser@smm.cn",
                    "create_time": 1570774034,
                    "update_time": 1570774034
                },
                "attribute": [ // 信息属性
                    {
                        "attribute_id": 490,
                        "name": "牌号",
                        "attr_type": 2, // 1单选 2文本
                        "attr_options": "", // 单选时为逗号分隔的选项 文本时为正则表达式
                        "attr_unit": "",
                        "attr_value": "不限"
                    }
                ],
                "company_name": "CCtest",
                "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
                "vip_company_status_desc": "服务中",
                "vip_year": 6, // 店铺服务年限
                "qidian_wpa_url": "", // 企点URL
                "category_name": "",
                "last_category_name": ""
            }
    ]
}
```
</details>

---

#### <a id="post.other.vip">API: 首页企业动态</a>

**接口描述**

接口有缓存，有效期30分钟；最多返回5条数据

**请求描述**

**GET**  post/other/vip



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 213470,
            "user_id": 807720, // 用户ID
            "company_id": 1001764, // 企业/店铺ID
            "title": "撒地方撒",
            "post_type": 1, // 信息类型 1商品 2帖子
            "price": 0,
            "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
            "province_id": 37,
            "city_id": 0,
            "club_id": 0,
            "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
            "is_recommend": 0, // 是否推荐 0正常 1推荐
            "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
            "updated_time": 1573634453,
            "created_time": 1573634453,
            "post_content_rtf": "<p>是打发时</p>\n", // 富文本内容
            "post_content_txt": "是打发时", // 纯文本内容
            "cover_pic": "https://test-imgqn.smm.cn/test/b/image/ISKYoNOsUBnZMMJRFxFL20191113044045.png", // 封面
            "product_pic_set": "https://test-imgqn.smm.cn/test/b/image/ISKYoNOsUBnZMMJRFxFL20191113044045.png", // 图片集合
            "admin_email": "",
            "top": 0, // 是否置顶 0否 1是
            "is_notice": 0, // 是否通知 0否 1是
            "refresh_time": 0, // 最后一次刷新时间
            "is_offer": 0, // 是否报价 0否 1是
            "pic_amount": 1,
            "is_crawl": 0, // 是否爬虫抓取 0否 1是
            "unit": "",
            "area": "",
            "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
            "reason": "", // 审核拒绝原因
            "approval_time": 1573634517, // 审核时间
            "approver_email": "test@smm.cn",
            "click_count": 6, // 点击量
            "sale_number": "", // 可售数量
            "valid_period": 1, // 有效期（天）
            "valid_period_time": 1573720917, // 有效期时间戳
            "category_id": 61, // 所属顶级分类ID
            "last_category_id": 66, // 所属分类
            "is_vip": 1, // 发布人是否会员 1是 2否
            "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
            "location_province": "", // gps 省份
            "location_city": "", // gps 城市
            "location_gps": "" // GPS 经纬度
        }
    ]
}
```
</details>

---

#### <a id="inner.post.list">API: IP白名单获取帖子列表</a>

**接口描述**

白名单限制查询所有帖子信息

**请求描述**

**GET**  inner/post/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 7731,
        "page": 1,
        "limit": 1,
        "post_list": [
            {
                "id": 212362,
                "user_id": 808117, // 用户ID
                "company_id": 1001629, // 企业/店铺ID
                "title": "专业回收银焊条13580887176现金收购银焊片，银焊环",
                "post_type": 1, // 信息类型 1商品 2帖子
                "price": 0,
                "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
                "province_id": 12,
                "city_id": 51,
                "club_id": 111,
                "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 0正常 1推荐
                "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1570867564,
                "created_time": 1561619403,
                "post_content_rtf": "<p>宏锦金银回收有限公司面向全国高价回收<br />\n金废料：金盐，钯盐，金水，镀金，金膏，金丝，氯化钯；</p>\n\n<p>银废料：银浆，银浆罐，擦银布，银胶，银膏，银焊条，银触点，氯化银，硫化银，925银。<br />\n&nbsp;<br />\n钌废料：钌浆，废钌，粗钌，工业钌，钌催化剂，钌碳</p>\n\n<p>钯废料：氧化钯，胶体钯，钯水，钯盐，钯粉，钯浆，钯碳，钯催化剂，线路板钯水，钯块，钯片，钯板，废料钯&nbsp;</p>\n\n<p>&nbsp;全国免费上门，现场看货，现金支付 24小时热线：13580887176 陈生</p>\n", // 富文本内容
                "post_content_txt": "", // 纯文本内容
                "cover_pic": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 封面
                "product_pic_set": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 图片集合
                "admin_email": "",
                "top": 1, // 是否置顶 0否 1是
                "is_notice": 0, // 是否通知 0否 1是
                "refresh_time": 0, // 最后一次刷新时间
                "is_offer": 0, // 是否报价 0否 1是
                "pic_amount": 1, // 图片总数
                "is_crawl": 0, // 是否爬虫抓取 0否 1是
                "unit": "",
                "area": "",
                "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
                "reason": "", // 审核拒绝原因
                "approval_time": 0, // 审核时间
                "approver_email": "",
                "click_count": 7, // 点击量
                "sale_number": "0", // 可售数量
                "valid_period": 100, // 有效期（天）
                "valid_period_time": 1582182175, // 有效期时间戳
                "category_id": 0, // 所属顶级分类ID
                "last_category_id": 0, // 所属分类
                "is_vip": 2, // 发布人是否会员 1是 2否
                "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "", // gps 省份
                "location_city": "", // gps 城市
                "location_gps": "", // GPS 经纬度
                "navbar_name": "铜",
                "club_name": "铜棒",
                "province_name": "江苏",
                "city_name": "盐城市",
                "user_info": { // 发布人名片
                    "id": 44, // 名片ID
                    "user_id": 808117,
                    "is_public": 1, 
                    "card_url": "https://test-imgqn.smm.cn/club/user/cardaQEte20191030103235.png",
                    "avatar": "",
                    "real_name": "135****2056",
                    "cellphone": "13585952056",
                    "telephone": "13585952056",
                    "company_type": "",
                    "company_name": "CCtest",
                    "province_id": 0,
                    "city_id": 0,
                    "address": "",
                    "position": "",
                    "main_product": "",
                    "source_channel": 4,
                    "admin_email": "olduser@smm.cn",
                    "create_time": 1570774034,
                    "update_time": 1570774034
                },
                "attribute": [ // 信息属性
                    {
                        "attribute_id": 490,
                        "name": "牌号",
                        "attr_type": 2, // 1单选 2文本
                        "attr_options": "", // 单选时为逗号分隔的选项 文本时为正则表达式
                        "attr_unit": "",
                        "attr_value": "不限"
                    }
                ],
                "company_name": "CCtest",
                "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
                "vip_company_status_desc": "服务中",
                "vip_year": 6, // 店铺服务年限
                "qidian_wpa_url": "", // 企点URL
                "category_name": "",
                "last_category_name": ""
            }
        ]
    }
}
```
</details>

---

#### <a id="post.person">API: 个人主页搜索我的信息</a>

**请求描述**

**GET**  post/person

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
keyword|string|标题关键字，模糊匹配
post_type|int|信息类型：`0`全部 `1`商品信息 `2`帖子
person_id|int|个人主页的用户ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 242,
        "post_list": [
            {
                "id": 212362,
                "user_id": 808117, // 用户ID
                "company_id": 1001629, // 企业/店铺ID
                "title": "专业回收银焊条13580887176现金收购银焊片，银焊环",
                "post_type": 1, // 信息类型 1商品 2帖子
                "price": 0,
                "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
                "province_id": 12,
                "city_id": 51,
                "club_id": 111,
                "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 0正常 1推荐
                "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1570867564,
                "created_time": 1561619403,
                "post_content_rtf": "<p>宏锦金银回收有限公司面向全国高价回收<br />\n金废料：金盐，钯盐，金水，镀金，金膏，金丝，氯化钯；</p>\n\n<p>银废料：银浆，银浆罐，擦银布，银胶，银膏，银焊条，银触点，氯化银，硫化银，925银。<br />\n&nbsp;<br />\n钌废料：钌浆，废钌，粗钌，工业钌，钌催化剂，钌碳</p>\n\n<p>钯废料：氧化钯，胶体钯，钯水，钯盐，钯粉，钯浆，钯碳，钯催化剂，线路板钯水，钯块，钯片，钯板，废料钯&nbsp;</p>\n\n<p>&nbsp;全国免费上门，现场看货，现金支付 24小时热线：13580887176 陈生</p>\n", // 富文本内容
                "post_content_txt": "", // 纯文本内容
                "cover_pic": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 封面
                "product_pic_set": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 图片集合
                "admin_email": "",
                "top": 1, // 是否置顶 0否 1是
                "is_notice": 0, // 是否通知 0否 1是
                "refresh_time": 0, // 最后一次刷新时间
                "is_offer": 0, // 是否报价 0否 1是
                "pic_amount": 1, // 图片总数
                "is_crawl": 0, // 是否爬虫抓取 0否 1是
                "unit": "",
                "area": "",
                "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
                "reason": "", // 审核拒绝原因
                "approval_time": 0, // 审核时间
                "approver_email": "",
                "click_count": 7, // 点击量
                "sale_number": "0", // 可售数量
                "valid_period": 100, // 有效期（天）
                "valid_period_time": 1582182175, // 有效期时间戳
                "category_id": 0, // 所属顶级分类ID
                "last_category_id": 0, // 所属分类
                "is_vip": 2, // 发布人是否会员 1是 2否
                "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "", // gps 省份
                "location_city": "", // gps 城市
                "location_gps": "", // GPS 经纬度
                "navbar_name": "铜",
                "club_name": "铜棒",
                "province_name": "江苏",
                "city_name": "盐城市",
                "user_info": { // 发布人名片
                    "id": 44, // 名片ID
                    "user_id": 808117,
                    "is_public": 1, 
                    "card_url": "https://test-imgqn.smm.cn/club/user/cardaQEte20191030103235.png",
                    "avatar": "",
                    "real_name": "135****2056",
                    "cellphone": "13585952056",
                    "telephone": "13585952056",
                    "company_type": "",
                    "company_name": "CCtest",
                    "province_id": 0,
                    "city_id": 0,
                    "address": "",
                    "position": "",
                    "main_product": "",
                    "source_channel": 4,
                    "admin_email": "olduser@smm.cn",
                    "create_time": 1570774034,
                    "update_time": 1570774034
                },
                "attribute": [ // 信息属性
                    {
                        "attribute_id": 490,
                        "name": "牌号",
                        "attr_type": 2, // 1单选 2文本
                        "attr_options": "", // 单选时为逗号分隔的选项 文本时为正则表达式
                        "attr_unit": "",
                        "attr_value": "不限"
                    }
                ],
                "company_name": "CCtest",
                "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
                "vip_company_status_desc": "服务中",
                "vip_year": 6, // 店铺服务年限
                "qidian_wpa_url": "", // 企点URL
                "category_name": "",
                "last_category_name": ""
            }
        ]
    }
}
```
</details>

---

#### <a id="post.app.my_club">API: 手机端</a>

**请求描述**

**GET**  post/app/my_club

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
order_by|string|排序：`click`热度，`update`更新时间，默认`click`
industry_id|int|行业ID，可选



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 3,
        "post_list": [
            {
                "id": 212362,
                "user_id": 808117, // 用户ID
                "company_id": 1001629, // 企业/店铺ID
                "title": "专业回收银焊条13580887176现金收购银焊片，银焊环",
                "post_type": 1, // 信息类型 1商品 2帖子
                "price": 0,
                "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
                "province_id": 12,
                "city_id": 51,
                "club_id": 111,
                "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 0正常 1推荐
                "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1570867564,
                "created_time": 1561619403,
                "post_content_rtf": "<p>宏锦金银回收有限公司面向全国高价回收<br />\n金废料：金盐，钯盐，金水，镀金，金膏，金丝，氯化钯；</p>\n\n<p>银废料：银浆，银浆罐，擦银布，银胶，银膏，银焊条，银触点，氯化银，硫化银，925银。<br />\n&nbsp;<br />\n钌废料：钌浆，废钌，粗钌，工业钌，钌催化剂，钌碳</p>\n\n<p>钯废料：氧化钯，胶体钯，钯水，钯盐，钯粉，钯浆，钯碳，钯催化剂，线路板钯水，钯块，钯片，钯板，废料钯&nbsp;</p>\n\n<p>&nbsp;全国免费上门，现场看货，现金支付 24小时热线：13580887176 陈生</p>\n", // 富文本内容
                "post_content_txt": "", // 纯文本内容
                "cover_pic": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 封面
                "product_pic_set": "https://imgqn.smm.cn/production/b/image/HckMOIxDudLKYQpBBFfP20190627030958.jpg", // 图片集合
                "admin_email": "",
                "top": 1, // 是否置顶 0否 1是
                "is_notice": 0, // 是否通知 0否 1是
                "refresh_time": 0, // 最后一次刷新时间
                "is_offer": 0, // 是否报价 0否 1是
                "pic_amount": 1, // 图片总数
                "is_crawl": 0, // 是否爬虫抓取 0否 1是
                "unit": "",
                "area": "",
                "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
                "reason": "", // 审核拒绝原因
                "approval_time": 0, // 审核时间
                "approver_email": "",
                "click_count": 7, // 点击量
                "sale_number": "0", // 可售数量
                "valid_period": 100, // 有效期（天）
                "valid_period_time": 1582182175, // 有效期时间戳
                "category_id": 0, // 所属顶级分类ID
                "last_category_id": 0, // 所属分类
                "is_vip": 2, // 发布人是否会员 1是 2否
                "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "", // gps 省份
                "location_city": "", // gps 城市
                "location_gps": "", // GPS 经纬度
                "navbar_name": "铜",
                "club_name": "铜棒",
                "province_name": "江苏",
                "city_name": "盐城市",
                "user_info": { // 发布人名片
                    "id": 44, // 名片ID
                    "user_id": 808117,
                    "is_public": 1, 
                    "card_url": "https://test-imgqn.smm.cn/club/user/cardaQEte20191030103235.png",
                    "avatar": "",
                    "real_name": "135****2056",
                    "cellphone": "13585952056",
                    "telephone": "13585952056",
                    "company_type": "",
                    "company_name": "CCtest",
                    "province_id": 0,
                    "city_id": 0,
                    "address": "",
                    "position": "",
                    "main_product": "",
                    "source_channel": 4,
                    "admin_email": "olduser@smm.cn",
                    "create_time": 1570774034,
                    "update_time": 1570774034
                },
                "attribute": [ // 信息属性
                    {
                        "attribute_id": 490,
                        "name": "牌号",
                        "attr_type": 2, // 1单选 2文本
                        "attr_options": "", // 单选时为逗号分隔的选项 文本时为正则表达式
                        "attr_unit": "",
                        "attr_value": "不限"
                    }
                ],
                "company_name": "CCtest",
                "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
                "vip_company_status_desc": "服务中",
                "vip_year": 6, // 店铺服务年限
                "qidian_wpa_url": "", // 企点URL
                "category_name": "",
                "last_category_name": ""
            }
        ]
    }
}
```
</details>

---

#### <a id="post.keywords">API: 获取信息关键词</a>

**请求描述**

**GET**  post/keywords

**参数描述**

query:

名称|类型|描述
---|---|---
post_id|int|信息ID
limit|int|关键词数量，默认6个



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "post_id": 205010, // 信息ID
            "origin_field": "title", // 关键词来源信息字段
            "score": 1, // 评分
            "word": "高温", // 关键词
            "create_time": 1573026124 // 创建时间
        }
    ]
}
```
</details>

### <a id="item_fenxiangduihuan_667519000">分享兑换</a>



---

#### <a id="exchange.unused">API: 获取当前登录用户可使用的兑换份额</a>

**请求描述**

**GET**  exchange/unused



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "all_used_amount": 5, // 所有可用的兑换名额
        "use_amount": 5 // 已经使用了的兑换名额
    }
}
```
</details>

---

#### <a id="exchange">API: 分享份额兑换商机vip</a>

**请求描述**

**POST**  exchange

**参数描述**

body:

名称|类型|描述
---|---|---
product|int|1月度 2季度 3一年 4两年 



<details>
<summary>响应描述</summary>

```json
{
    "code": 10150,
    "msg": "邀请的好友数不足",
    "data": null
}
```
</details>

---

#### <a id="share.exchange.content">API: 获取分享页兑换内容列表</a>

**请求描述**

**GET**  share/exchange/content



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [ // 后台常量
        {
            "product": 4, // 产品ID
            "product_name": "2年商机VIP",
            "price": "6888元",
            "limit_desc": "邀请50位好友可获得",
            "is_exchange": false // 是否已经兑换过 true是 false否
        },
        {
            "product": 3,
            "product_name": "1年商机VIP",
            "price": "3298元",
            "limit_desc": "邀请30位好友可获得",
            "is_exchange": false
        },
        {
            "product": 2,
            "product_name": "季度商机VIP",
            "price": "998元",
            "limit_desc": "邀请10位好友可获得",
            "is_exchange": false
        },
        {
            "product": 1,
            "product_name": "月度商机VIP",
            "price": "388元",
            "limit_desc": "邀请5位好友可获得",
            "is_exchange": true
        }
    ]
}
```
</details>

---

#### <a id="share.friend.boost">API: 获取分享好友助力榜</a>

**请求描述**

**GET**  share/friend/boost



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [ // 成功分享记录
        {
            "id": 2,
            "user_id": 804792, // 被分享人用户ID
            "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/PHVgQ20190724160900.jpeg",
            "nick_name": "toy",
            "phone": "13127881017",
            "real_name": "张新杰",
            "company_name": "上海大宝剑有限公司",
            "share_user_id": 807720, // 分享人用户ID
            "share_phone": "10001221212", // 分享人手机号
            "reg_time": 1568788591, // 被分享人注册时间
            "card_time": 1568788591, // 被分享人完善名片信息时间
            "admin_email": "",
            "create_time": 1568788591,
            "update_time": 1568788591
        }
    ]
}
```
</details>

---

#### <a id="exchange.list">API: 获取兑换记录列表</a>

**接口描述**

最多返回20条记录

**请求描述**

**GET**  exchange/list



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 2,
            "user_id": 807720,
            "phone": "13127881017",
            "product": 1, // 兑换产品ID
            "product_name": "月度商机VIP",
            "use_amount": 5, // 使用的兑换名额数
            "remain_amount": 0, // 剩余的兑换名额 
            "exchange_time": 1569550326, // 兑换时间
            "nick_name": "toy" // 昵称
        }
    ]
}
```
</details>

### <a id="item_qita_667646000">其他 </a>



---

#### <a id="province">API: 地区列表</a>

**请求描述**

**GET**  province



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "id": 22, // 省份ID
            "name": "北京", // 省
            "city_list": [ // 城市/区列表
                {
                    "id": 401, // 城市/区ID
                    "name": "东城区",
                    "parent_id": 22
                },
                {
                    "id": 402,
                    "name": "西城区",
                    "parent_id": 22
                }
            ]
        }
    ]
}
```
</details>

---

#### <a id="user.info">API: 个人信息</a>

**请求描述**

**GET**  user/info

**参数描述**

query:

名称|类型|描述
---|---|---
user_id|int|优先user_id，不传则根据token查询



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "user_info": { // 用户中心信息
            "real_name": "张新杰",
            "user_name": "SMM1546927067xW",
            "nickname": "toy",
            "description": "",
            "cellphone": "13127881017",
            "email": "",
            "id": 807720, // 用户ID
            "company_name": "上海大宝剑有限公司",
            "company_id": 1001764,
            "company_status": 1,
            "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/nNaGF20190923194241.jpeg",
            "company_verify_level": 2,
            "position": "员工",
            "external_cellphone": "13127881017", // 对外联系方式
            "join_club_amount": 18, // 加入的圈子数
            "post_amount": 242, // 发布的信息数
            "shop_status": 0,
            "shop_logo": "",
            "vip_status": 2, // 会员状态 0为开通 1过期 2服务中 3关闭
            "vip_type": 1, // 会员类型 1月度 2年度 3体验 4季度 5半年
            "vip_status_desc": "服务中",
            "vip_year": 6, // 店铺年限
            "qidian_wpa_url": "", // 企点URL
            "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
            "user_card_status": 2, // 名片状态 0未完善名片 1待审核 2审核通过 3审核拒绝
            "user_card": { // 完善的名片信息
                "id": 7,
                "user_id": 807720,
                "is_public": 2, // 是否公开 1公开 2不公开
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardubpDF20191105173608.png",
                "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/nNaGF20190923194241.jpeg",
                "real_name": "张新杰",
                "cellphone": "13127881017",
                "telephone": "099-123456",
                "company_type": "矿产商",
                "company_name": "上海有色网股份有限公司",
                "province_id": 18,
                "city_id": 0,
                "address": "上海浦东新区峨山路91弄20号陆家嘴软件园9号楼9楼",
                "position": "后端工程师",
                "main_product": "铝合金",
                "source_channel": 4, // 名片信息来源 1pc 2app 3wx 4admin
                "create_time": 1568788590,
                "update_time": 1572946568,
                "province": "上海",
                "city": "",
                "approval_status": 2,
                "reason": "",
                "admin_email": "",
                "industry_list": [ // 关联的行业列表
                    {
                        "id": 5,
                        "industry_name": "测试003",
                        "status": 2,
                        "disable": 1,
                        "card_num": 3,
                        "sort": 2,
                        "create_admin": "test@smm.cn",
                        "update_admin": "test@smm.cn",
                        "create_time": 1568701331,
                        "update_time": 1571646390
                    }
                ],
                "vip_status": 2,
                "vip_type": 1,
                "relationship": 0,
                "group_id": 0,
                "group_name": ""
            },
            "user_card_approval": { // 审核中的名片信息
                "id": 76,
                "user_id": 807720,
                "is_public": 1,
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardubpDF20191105173608.png",
                "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/nNaGF20190923194241.jpeg",
                "real_name": "张新杰",
                "cellphone": "13127881017",
                "telephone": "099-123456",
                "company_type": "矿产商",
                "company_name": "上海有色网股份有限公司",
                "province_id": 18,
                "city_id": 0,
                "address": "上海浦东新区峨山路91弄20号陆家嘴软件园9号楼9楼",
                "position": "后端工程师",
                "main_product": "铝合金",
                "source_channel": 1,
                "create_time": 0,
                "update_time": 0,
                "province": "上海",
                "city": "",
                "approval_status": 3, // 名片审核状态 1待审核 2审核通过 3审核拒绝
                "reason": "阿斯顿发",
                "admin_email": "test@smm.cn",
                "industry_list": [
                    {
                        "id": 8,
                        "industry_name": "电器001",
                        "status": 1,
                        "disable": 1,
                        "card_num": 3,
                        "sort": 4,
                        "create_admin": "test@smm.cn",
                        "update_admin": "test@smm.cn",
                        "create_time": 1571119885,
                        "update_time": 1571646390
                    }
                ],
                "vip_status": 0,
                "vip_type": 0,
                "relationship": 0,
                "group_id": 0,
                "group_name": ""
            }
        }
    }
}
```
</details>

---

#### <a id="user.club_role">API: 查询用户圈子角色</a>

**请求描述**

**GET**  user/club_role

**参数描述**

query:

名称|类型|描述
---|---|---
club_id|int|圈子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "user_role": "master" // master圈主 member成员 其他都是未加圈用户
    }
}
```
</details>

---

#### <a id="user.club_list">API: 获取用户圈子列表</a>

**请求描述**

**GET**  user/club_list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
user_id|int|用户ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 18,
        "club_list": [
            {
                "id": 389, // 圈子ID
                "user_id": 1276401, // 圈主用户ID
                "name": "贵金属圈", // 圈子名称
                "introduction": "",// 圈子简介
                "logo": "",
                "h5_background": "",
                "web_background": "",
                "is_recommend": 1, // 是否推荐 0正常 1推荐
                "disabled": 0, // 是否禁用 0正常 1禁用
                "updated_time": 1569296631,
                "created_time": 1555069168,
                "members_amount": 2, // 圈内成员数量
                "post_amount": 1586, // 圈内信息数
                "today_post_amount": 0,// 今日圈内信息数
                "admin_email": "wangayan@smm.cn",
                "is_audit": 0,
                "user_role": "member", // 圈内角色 master：圈主 member：成员
                "user_info": { // 圈主用户中心信息
                    "real_name": "管理员",
                    "user_name": "SMM1544668516YZ",
                    "nickname": "TestAdminNa",
                    "description": "123acddf456",
                    "cellphone": "10000033580",
                    "email": "10000033580@smm.cn",
                    "id": 807584,
                    "company_name": "测试贸易12134",
                    "company_id": 1001572,
                    "company_status": 1,
                    "avatar": "https://test-imgqn.smm.cn/tradecenter/image/iEHxH20190731134712.gif",
                    "company_verify_level": 2,
                    "position": "销售总监",
                    "external_cellphone": "10000033580" // 对外联系方式
                },
                "category_list": [ // 圈子关联分类列表
                	{
                        "id": 3,
                        "name_cn": "铜棒",
                        "level": 2,
                        "parent_id": 2,
                        "sort": 1,
                        "children_ids": "79",
                        "post_num": 19,
                        "type": 0,
                        "status": 1,
                        "is_disabled": 0,
                        "industry_id": 0,
                        "img_url": "",
                        "is_recommend": 1,
                        "create_admin": "test@smm.cn",
                        "create_time": 1571202327,
                        "update_admin": "test@smm.cn",
                        "update_time": 1572331972
                    }	
            	]
            }
        ]
    }
}
```
</details>

---

#### <a id="my.club_list">API: 获取我的圈子列表</a>

**请求描述**

**GET**  my/club_list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 18,
        "club_list": [
            {
                "id": 389, // 圈子ID
                "user_id": 1276401, // 圈主用户ID
                "name": "贵金属圈", // 圈子名称
                "introduction": "",// 圈子简介
                "logo": "",
                "h5_background": "",
                "web_background": "",
                "is_recommend": 1, // 是否推荐 0正常 1推荐
                "disabled": 0, // 是否禁用 0正常 1禁用
                "updated_time": 1569296631,
                "created_time": 1555069168,
                "members_amount": 2, // 圈内成员数量
                "post_amount": 1586, // 圈内信息数
                "today_post_amount": 0,// 今日圈内信息数
                "admin_email": "wangayan@smm.cn",
                "is_audit": 0,
                "user_role": "member", // 圈内角色 master：圈主 member：成员
                "user_info": { // 圈主用户中心信息
                    "real_name": "管理员",
                    "user_name": "SMM1544668516YZ",
                    "nickname": "TestAdminNa",
                    "description": "123acddf456",
                    "cellphone": "10000033580",
                    "email": "10000033580@smm.cn",
                    "id": 807584,
                    "company_name": "测试贸易12134",
                    "company_id": 1001572,
                    "company_status": 1,
                    "avatar": "https://test-imgqn.smm.cn/tradecenter/image/iEHxH20190731134712.gif",
                    "company_verify_level": 2,
                    "position": "销售总监",
                    "external_cellphone": "10000033580" // 对外联系方式
                },
                "category_list": [ // 圈子关联分类列表
                	{
                        "id": 3,
                        "name_cn": "铜棒",
                        "level": 2,
                        "parent_id": 2,
                        "sort": 1,
                        "children_ids": "79",
                        "post_num": 19,
                        "type": 0,
                        "status": 1,
                        "is_disabled": 0,
                        "industry_id": 0,
                        "img_url": "",
                        "is_recommend": 1,
                        "create_admin": "test@smm.cn",
                        "create_time": 1571202327,
                        "update_admin": "test@smm.cn",
                        "update_time": 1572331972
                    }	
            	]
            }
        ]
    }
}
```
</details>

---

#### <a id="key_word_list">API: 获取关键词列表</a>

**请求描述**

**GET**  key_word_list

**参数描述**

query:

名称|类型|描述
---|---|---
word_type|int|词类型 1:主词 2:相关词
name|string|产品名 模糊匹配
id|int|逗号分割的ID
begin_time|int|更新开始时间
end_time|int|更新结束时间
page|int|
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 61285,
        "key_word_list": [
            {
                "id": 64183,
                "name": "铈钨合金用途",
                "updated_time": 1562292865,
                "created_time": 1562292865,
                "admin_email": "liuzhenli@smm.cn",
                "word_type": 2
            }
        ]
    }
}
```
</details>

---

#### <a id="active.user.list">API: 查询n天内发帖数量最多的m个用户</a>

**接口描述**

该接口缓存5分钟；`club_id`存在的情况下不走缓存

**请求描述**

**GET**  active/user/list

**参数描述**

query:

名称|类型|描述
---|---|---
club_id|int|圈子ID；选填，代表从指定的圈子里查询
day_num|int|天数
limit|int|数据条数



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "user_info": { // 用户中心的用户信息
                "real_name": "wmn111",
                "user_name": "SMM1511423497TO",
                "nickname": "小小娜",
                "description": "我是企业账号，小小娜的账号啦啦啦",
                "cellphone": "13564317032",
                "email": "111@smm.cn",
                "id": 804472,
                "company_name": "张家港中集圣达因低温装备有限公司",
                "company_id": 1001150,
                "company_status": 1,
                "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/bVDZe20190917144835.jpeg",
                "company_verify_level": 2,
                "position": "产品经理",
                "external_cellphone": "13564317032" // 对外联系方式
            },
            "post_count": 13, // 信息发布数
            "id": 213464, // 信息ID
            "user_id": 804472,
            "title": "从圈子里面发布"
        }
    ]
}
```
</details>

---

#### <a id="new.post.list">API: 获取新帖榜</a>

**接口描述**

该接口缓存5分钟；最多返回10条数据，按发布时间倒叙排序

**请求描述**

**GET**  new/post/list



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
         {
            "id": 213470,
            "user_id": 807720, // 用户ID
            "company_id": 1001764, // 企业/店铺ID
            "title": "撒地方撒",
            "post_type": 1, // 信息类型 1商品 2帖子
            "price": 0,
            "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
            "province_id": 37,
            "city_id": 0,
            "club_id": 0,
            "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
            "is_recommend": 0, // 是否推荐 0正常 1推荐
            "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
            "updated_time": 1573634453,
            "created_time": 1573634453,
            "post_content_rtf": "<p>是打发时</p>\n", // 富文本内容
            "post_content_txt": "是打发时", // 纯文本内容
            "cover_pic": "https://test-imgqn.smm.cn/test/b/image/ISKYoNOsUBnZMMJRFxFL20191113044045.png", // 封面
            "product_pic_set": "https://test-imgqn.smm.cn/test/b/image/ISKYoNOsUBnZMMJRFxFL20191113044045.png", // 图片集合
            "admin_email": "",
            "top": 0, // 是否置顶 0否 1是
            "is_notice": 0, // 是否通知 0否 1是
            "refresh_time": 0, // 最后一次刷新时间
            "is_offer": 0, // 是否报价 0否 1是
            "pic_amount": 1,
            "is_crawl": 0, // 是否爬虫抓取 0否 1是
            "unit": "",
            "area": "",
            "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
            "reason": "", // 审核拒绝原因
            "approval_time": 1573634517, // 审核时间
            "approver_email": "test@smm.cn",
            "click_count": 6, // 点击量
            "sale_number": "", // 可售数量
            "valid_period": 1, // 有效期（天）
            "valid_period_time": 1573720917, // 有效期时间戳
            "category_id": 61, // 所属顶级分类ID
            "last_category_id": 66, // 所属分类
            "is_vip": 1, // 发布人是否会员 1是 2否
            "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
            "location_province": "", // gps 省份
            "location_city": "", // gps 城市
            "location_gps": "" // GPS 经纬度
        }
    ]
}
```
</details>

---

#### <a id="recommend.user.list">API: 获取推荐用户榜</a>

**接口描述**

缓存5分钟；获取最新发布信息的用户列表，最多10条

**请求描述**

**GET**  recommend/user/list



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "user_info": {
                "real_name": "张新杰",
                "user_name": "SMM1546927067xW",
                "nickname": "toy",
                "description": "",
                "cellphone": "13127881017",
                "email": "",
                "id": 807720,
                "company_name": "上海大宝剑有限公司",
                "company_id": 1001764,
                "company_status": 1,
                "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/nNaGF20190923194241.jpeg",
                "company_verify_level": 2,
                "position": "员工",
                "external_cellphone": "13127881017" // 对外联系方式
            },
            "post_count": 214, // 发布信息数
            "id": 213470, // 信息ID
            "user_id": 807720,
            "title": "撒地方撒" // 信息标题
        }
    ]
}
```
</details>

---

#### <a id="upload.img">API: 前台上传图片</a>

**请求描述**

**POST**  upload/img

**参数描述**

body:

名称|类型|描述
---|---|---
file|选择本地文件对象|图片文件
code_type|int|`800`：商机九图<br/>`801`：商机富文本图片<br/>`802`：用户上传企业背景图<br/>`803`：系统默认企业背景图<br/>`804`:   用户名片



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": "https://test-imgqn.smm.cn/test/club/company/system/picKMpDF20191115103435.png" // 上传图片的链接
}
```
</details>

---

#### <a id="send.message">API: 发送留言</a>

**接口描述**

有两个必传的header:

name|type|description
---|---|---
captcha_id|string|验证码ID
validate|string|验证码数据

**请求描述**

**POST**  send/message

**参数描述**

body:

名称|类型|描述
---|---|---
post_id|int|信息ID
receive_user_id|int|接收消息的用户ID
message|string|消息内容
contact|string|联系方式



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="send.communication">API: 发送沟通请求</a>

**请求描述**

**POST**  send/communication

**参数描述**

body:

名称|类型|描述
---|---|---
post_id|int|信息ID
receive_user_id|int|接收请求的用户ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="clubcenter">API: 有色网首页商机板块</a>

**接口描述**

缓存5分钟；

**请求描述**

**GET**  clubcenter



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "visitor_today": 0, // 今日访客数
        "updated_today": 1000, // 今日信息更新数
        "recommend_company_list": [ // 推荐企业，来源于后台设置的推荐用户关联企业
            {
                "company_logo": "", // 企业logo
                "company_id": 1001764, // 企业ID
                "company_name": "上海大宝剑有限公司", // 公司名称
                "company_desc": "",
                "main_product": "" // 公司主营
            }
        ],
        "navbar_list": [ // 商机分类列表
            {
                "navbar_id": 2, // 商机分类ID
                "navbar_name": "铜", // 分类名称
                "navbar_icon": "" // 分类默认图
            },
            {
                "navbar_id": 210,
                "navbar_name": "测试2",
                "navbar_icon": ""
            },
            {
                "navbar_id": 112,
                "navbar_name": "测试1",
                "navbar_icon": "https://test-imgqn.smm.cn/test/admin/company/FRFCd20191023154654.png"
            }
        ]
    }
}
```
</details>

---

#### <a id="clubcenter.label_list.navID">API: 有色网首页商机板块导航标签数据</a>

**接口描述**

缓存5分钟

**请求描述**

**GET**  clubcenter/label_list/:navID

**参数描述**

path:

名称|类型|描述
---|---|---
navID|int|商机分类ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": [
        {
            "label_id": 90, // 参数分类的子级商机分类ID
            "label_name": "玩具", // 分类名称
            "post_list": [ // 分类下的信息列表，最多4条
                {
                    "post_id": 205017, // 信息ID
                    "title": "构思屋形糖块包装铁盒 精美马口铁喜糖喜饼收纳金属盒定", // 信息标题
                    "price": 5, // 价格
                    "quantity_unit": 0, // 单位
                    "unit": "个",
                    "province_id": 0,
                    "province": "",
                    "city_id": 0,
                    "city": "",
                    "company_id": 1001717, // 企业ID
                    "company_name": "这个公司名字不太冷", // 企业名称
                    "vip_year": 1, // 店铺服务年限
                    "qidian_wpa_url": "" // 企点URL
                }
            ],
            "club_list": [ // 子级分类列表
                {
                    "id": 91, // 商机分类ID
                    "name": "3#锌合金", // 分类名称
                    "is_recommend": 0,
                    "created_time": 1571367867,
                    "updated_time": 1571367867,
                    "club_id": 91, // 分类ID
                    "label_id": 90 // 父级分类ID
                }
            ]
        }
    ]
}
```
</details>

---

#### <a id="recommend.company">API: 有商推荐</a>

**接口描述**

缓存5分钟；最多返回30条

**请求描述**

**GET**  recommend/company



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "recommend_company_list": [
            {
                "company_id": 1001530,
                "company_name": "link的企业",
                "vip_year": 5, // 企业店铺年限
                "product_count": 130, // 企业下的商品数量
                "other_post": { // 帖子信息
                    "post_id": 213424,
                    "title": "阿里每十年公布一次内部录像，讲述当时发生了什么，公司当时为什么要做这个决定。如果年轻人和",
                    "cover_pic": "",
                    "attribute": null,
                    "category_id": 0,
                    "category_name": ""
                },
                "product_post_list": [ // 商品列表 最多3条
                    {
                        "post_id": 205003,
                        "title": "保健品铁盒   viagra铁盒马口铁礼盒定制",
                        "cover_pic": "https://imgbucket.smm.cn/09d3e7af91c51b1e0c15d6f507bca710.jpg",
                        "attribute": [ // 商品属性列表
                            {
                                "attribute_id": 0,
                                "name": "加工定制",
                                "attr_type": 2,
                                "attr_options": "",
                                "attr_unit": "",
                                "attr_value": "是 "
                            }
                        ],
                        "category_id": 85, // 商品所属分类
                        "category_name": "龙头" // 商品所属分类名称
                    }
                ],
                "category_list": [ // 店铺下发布信息所属的分类列表
                    {
                        "category_id": 3,
                        "category_name": "铜棒"
                    }
                ]
            }
        ]
    }
}
```
</details>

---

#### <a id="get_area">API: 根据经纬度获取省市</a>

**请求描述**

**GET**  get_area

**参数描述**

query:

名称|类型|描述
---|---|---
lng|string|经度
lat|string|纬度



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "province_id": 12,
        "province": "江苏",
        "city_id": 47,
        "city": "苏州市"
    }
}
```
</details>

---

#### <a id="app.chat">API: 手机端商圈洽谈</a>

**请求描述**

**POST**  app/chat

**参数描述**

body:

名称|类型|描述
---|---|---
post_id|int|帖子ID
local_id|string|手机端local_id



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "msg_id": 1486194, // 消息ID
        "local_id": "adkdkfkmehni32"
    }
}
```
</details>

---

#### <a id="card_and_post">API: 为用户中心提供数据</a>

**接口描述**

获取名片数据和商机的一些统计信息

**请求描述**

**GET**  card_and_post



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "card": { // 用户名片数据,可能为空
            "id": 7, // 名片ID
            "user_id": 807720, // 用户ID
            "is_public": 2, // 是否公开 1公开 2不公开
            "card_url": "https://test-imgqn.smm.cn/test/club/user/cardubpDF20191105173608.png",
            "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/nNaGF20190923194241.jpeg",
            "real_name": "张新杰",
            "cellphone": "13127881017",
            "telephone": "099-123456",
            "company_type": "矿产商",
            "company_name": "上海有色网股份有限公司",
            "province_id": 18,
            "city_id": 0,
            "address": "上海浦东新区峨山路91弄20号陆家嘴软件园9号楼9楼",
            "position": "后端工程师",
            "main_product": "铝合金",
            "source_channel": 4,
            "create_time": 1568788590,
            "update_time": 1572946568,
            "province": "上海",
            "city": "",
            "approval_status": 2, // 名片审核状态 1待审核 2通过 3失败
            "reason": "",
            "admin_email": "",
            "industry_list": [ // 名片关联的行业列表
                {
                    "id": 5,
                    "industry_name": "测试003",
                    "status": 2,
                    "disable": 1,
                    "card_num": 2,
                    "sort": 2,
                    "create_admin": "test@smm.cn",
                    "update_admin": "test@smm.cn",
                    "create_time": 1568701331,
                    "update_time": 1571646390
                }
            ],
            "vip_status": 2, //会员状态 0非会员 1过期 2服务中 3关闭
            "vip_type": 1, //会员类型 1月度会员 2年度会员 3体验会员
            "relationship": 0,
            "group_id": 0,
            "group_name": ""
        },
        "published_product_count": 9, // 发布中的商品
        "expired_product_count": 5, // 过期的商品
        "my_post_count": 5, // 我的帖子
        "comment_count": 9, // 我的评论
        "card_req_count": 3 // 待处理的名片请求
    }
}
```
</details>

### <a id="item_sousuo_668602000">搜索</a>



---

#### <a id="search.club_list">API: 搜索圈子列表</a>

**请求描述**

**GET**  search/club_list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
key_word|string|搜索关键词，模糊匹配



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 27,
        "post_count": 207,
        "club_list": [
            {
                "id": 389, // 圈子ID
                "user_id": 1276401, // 圈主用户ID
                "name": "贵金属圈", // 圈子名称
                "introduction": "",// 圈子简介
                "logo": "",
                "h5_background": "",
                "web_background": "",
                "is_recommend": 1, // 是否推荐 0正常 1推荐
                "disabled": 0, // 是否禁用 0正常 1禁用
                "updated_time": 1569296631,
                "created_time": 1555069168,
                "members_amount": 2, // 圈内成员数量
                "post_amount": 1586, // 圈内信息数
                "today_post_amount": 0,// 今日圈内信息数
                "admin_email": "wangayan@smm.cn",
                "is_audit": 0,
                "user_role": "member", // 圈内角色 master：圈主 member：成员
                "user_info": { // 圈主用户中心信息
                    "real_name": "管理员",
                    "user_name": "SMM1544668516YZ",
                    "nickname": "TestAdminNa",
                    "description": "123acddf456",
                    "cellphone": "10000033580",
                    "email": "10000033580@smm.cn",
                    "id": 807584,
                    "company_name": "测试贸易12134",
                    "company_id": 1001572,
                    "company_status": 1,
                    "avatar": "https://test-imgqn.smm.cn/tradecenter/image/iEHxH20190731134712.gif",
                    "company_verify_level": 2,
                    "position": "销售总监",
                    "external_cellphone": "10000033580" // 对外联系方式
                },
                "category_list": [ // 圈子关联分类列表
                	{
                        "id": 3,
                        "name_cn": "铜棒",
                        "level": 2,
                        "parent_id": 2,
                        "sort": 1,
                        "children_ids": "79",
                        "post_num": 19,
                        "type": 0,
                        "status": 1,
                        "is_disabled": 0,
                        "industry_id": 0,
                        "img_url": "",
                        "is_recommend": 1,
                        "create_admin": "test@smm.cn",
                        "create_time": 1571202327,
                        "update_admin": "test@smm.cn",
                        "update_time": 1572331972
                    }	
            	]
            }
        ]
    }
}
```
</details>

---

#### <a id="app.search.club_list">API: 搜索圈子列表</a>

**请求描述**

**GET**  app/search/club_list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
key_word|string|搜索关键词，模糊匹配



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 27,
        "club_list": [
            {
                "id": 389, // 圈子ID
                "user_id": 1276401, // 圈主用户ID
                "name": "贵金属圈", // 圈子名称
                "introduction": "",// 圈子简介
                "logo": "",
                "h5_background": "",
                "web_background": "",
                "is_recommend": 1, // 是否推荐 0正常 1推荐
                "disabled": 0, // 是否禁用 0正常 1禁用
                "updated_time": 1569296631,
                "created_time": 1555069168,
                "members_amount": 2, // 圈内成员数量
                "post_amount": 1586, // 圈内信息数
                "today_post_amount": 0,// 今日圈内信息数
                "admin_email": "wangayan@smm.cn",
                "is_audit": 0,
                "user_role": "member", // 圈内角色 master：圈主 member：成员
                "user_info": { // 圈主用户中心信息
                    "real_name": "管理员",
                    "user_name": "SMM1544668516YZ",
                    "nickname": "TestAdminNa",
                    "description": "123acddf456",
                    "cellphone": "10000033580",
                    "email": "10000033580@smm.cn",
                    "id": 807584,
                    "company_name": "测试贸易12134",
                    "company_id": 1001572,
                    "company_status": 1,
                    "avatar": "https://test-imgqn.smm.cn/tradecenter/image/iEHxH20190731134712.gif",
                    "company_verify_level": 2,
                    "position": "销售总监",
                    "external_cellphone": "10000033580" // 对外联系方式
                },
                "category_list": [ // 圈子关联分类列表
                	{
                        "id": 3,
                        "name_cn": "铜棒",
                        "level": 2,
                        "parent_id": 2,
                        "sort": 1,
                        "children_ids": "79",
                        "post_num": 19,
                        "type": 0,
                        "status": 1,
                        "is_disabled": 0,
                        "industry_id": 0,
                        "img_url": "",
                        "is_recommend": 1,
                        "create_admin": "test@smm.cn",
                        "create_time": 1571202327,
                        "update_admin": "test@smm.cn",
                        "update_time": 1572331972
                    }	
            	],
                "post_list": [ // 最多8条
                    {
			            "id": 213470,
			            "user_id": 807720, // 用户ID
			            "company_id": 1001764, // 企业/店铺ID
			            "title": "撒地方撒",
			            "post_type": 1, // 信息类型 1商品 2帖子
			            "price": 0,
			            "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
			            "province_id": 37,
			            "city_id": 0,
			            "club_id": 0,
			            "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
			            "is_recommend": 0, // 是否推荐 0正常 1推荐
			            "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
			            "updated_time": 1573634453,
			            "created_time": 1573634453,
			            "post_content_rtf": "<p>是打发时</p>\n", // 富文本内容
			            "post_content_txt": "是打发时", // 纯文本内容
			            "cover_pic": "https://test-imgqn.smm.cn/test/b/image/ISKYoNOsUBnZMMJRFxFL20191113044045.png", // 封面
			            "product_pic_set": "https://test-imgqn.smm.cn/test/b/image/ISKYoNOsUBnZMMJRFxFL20191113044045.png", // 图片集合
			            "admin_email": "",
			            "top": 0, // 是否置顶 0否 1是
			            "is_notice": 0, // 是否通知 0否 1是
			            "refresh_time": 0, // 最后一次刷新时间
			            "is_offer": 0, // 是否报价 0否 1是
			            "pic_amount": 1,
			            "is_crawl": 0, // 是否爬虫抓取 0否 1是
			            "unit": "",
			            "area": "",
			            "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
			            "reason": "", // 审核拒绝原因
			            "approval_time": 1573634517, // 审核时间
			            "approver_email": "test@smm.cn",
			            "click_count": 6, // 点击量
			            "sale_number": "", // 可售数量
			            "valid_period": 1, // 有效期（天）
			            "valid_period_time": 1573720917, // 有效期时间戳
			            "category_id": 61, // 所属顶级分类ID
			            "last_category_id": 66, // 所属分类
			            "is_vip": 1, // 发布人是否会员 1是 2否
			            "vip_type": 1, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
			            "location_province": "", // gps 省份
			            "location_city": "", // gps 城市
			            "location_gps": "" // GPS 经纬度
			        }
                ]
            }
        ]
    }
}
```
</details>

---

#### <a id="search.load_all_post">API: 批量更新搜索帖子数据</a>

**接口描述**

更新搜索引擎索引

**请求描述**

**GET**  search/load_all_post



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="search.load_all_club">API: 批量更新搜索圈子数据</a>

**接口描述**

更新搜索引擎索引

**请求描述**

**GET**  search/load_all_club



<details>
<summary>响应描述</summary>

```json

```
</details>

---

#### <a id="search.post_list">API: 搜索帖子列表</a>

**请求描述**

**GET**  search/post_list

**参数描述**

query:

名称|类型|描述
---|---|---
key_word|string|关键词，模糊匹配，为空时返回也为空
page|int|
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 188,
        "club_count": 47,
        "post_list": [
            {
	            "id": 213389,
	            "user_id": 807748, // 用户ID
	            "company_id": 1001572, // 企业/店铺ID
	            "title": "我这个账号是有企Q的哦",
	            "post_type": 1, // 信息类型 1商品 2帖子
	            "price": 0,
	            "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
	            "province_id": 20,
	            "city_id": 144,
	            "club_id": 22,
	            "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
	            "is_recommend": 0, // 是否推荐 0正常 1推荐
	            "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
	            "updated_time": 1571905231,
	            "created_time": 1571905231,
	            "post_content_rtf": "", // 富文本内容
	            "post_content_txt": "", // 纯文本内容
	            "cover_pic": "https://test-imgqn.smm.cn/test/b/image/EYcjagsUSDUxKQvYfNlO20191024042026.jpg", // 封面
	            "product_pic_set": "https://test-imgqn.smm.cn/test/b/image/kgeKsKmfakQBrFSjkLow20191024042026.jpg;https://test-imgqn.smm.cn/test/b/image/PVnORfRFEwGXPbiWlPFm20191024042026.jpg;https://test-imgqn.smm.cn/test/b/image/EYcjagsUSDUxKQvYfNlO20191024042026.jpg", // 图片集合
	            "admin_email": "",
	            "top": 0, // 是否置顶 0否 1是
	            "is_notice": 0, // 是否通知 0否 1是
	            "refresh_time": 0, // 最后一次刷新时间
	            "is_offer": 0, // 是否报价 0否 1是
	            "pic_amount": 3, // 图片总数
	            "is_crawl": 0, // 是否爬虫抓取 0否 1是
	            "unit": "",
	            "area": "",
	            "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
	            "reason": "", // 审核拒绝原因
	            "approval_time": 1571906970, // 审核时间
	            "approver_email": "test@smm.cn",
	            "click_count": 11, // 点击量
	            "sale_number": "222", // 可售数量
	            "valid_period": 100, // 有效期（天）
	            "valid_period_time": 1582182175, // 有效期时间戳
	            "category_id": 2, // 所属顶级分类ID
	            "last_category_id": 8, // 所属分类
	            "is_vip": 1, // 发布人是否会员 1是 2否
	            "vip_type": 2, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
	            "location_province": "", // gps 省份
	            "location_city": "", // gps 城市
	            "location_gps": "", // GPS 经纬度
	            "navbar_name": "铜",
	            "club_name": "电解铜",
	            "province_name": "广西",
	            "city_name": "桂林市",
	            "user_info": { // 发布人名片
	                "id": 64, // 名片ID
	                "user_id": 807748,
	                "is_public": 1,
	                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardcfLqK20191029145002.png",
	                "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/LBVmh20190625135010.jpeg",
	                "real_name": "吴梦娜",
	                "cellphone": "18512197032",
	                "telephone": "18512154782",
	                "company_type": "矿产商",
	                "company_name": "测试贸易12134",
	                "province_id": 18,
	                "city_id": 0,
	                "address": "峨山路",
	                "position": "小职员",
	                "main_product": "铜铝铅",
	                "source_channel": 1,
	                "admin_email": "olduser@smm.cn",
	                "create_time": 1570863392,
	                "update_time": 1573187590
	            },
	            "attribute": [ // 信息属性
	                {
	                    "attribute_id": 42,
	                    "name": "正则",
	                    "attr_type": 2, // 1单选 2文本
	                    "attr_options": "^[A-Za-z0-9]+$", // 单选时为逗号分隔的选项 文本时为正则表达式
	                    "attr_unit": "",
	                    "attr_value": "22"
	                }
	            ],
	            "company_name": "测试贸易12134",
	            "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
	            "vip_company_status_desc": "服务中",
	            "vip_year": 5, // 店铺服务年限
	            "qidian_wpa_url": "http://q.url.cn/ABoDYP?_type=wpa&qidian=true", // 企点URL
	            "category_name": "铜",
	            "last_category_name": "电解铜"
	        }
        ]
    }
}
```
</details>

---

#### <a id="search.posts">API: 搜索帖子列表</a>

**请求描述**

**GET**  search/posts

**参数描述**

query:

名称|类型|描述
---|---|---
key_word|string|搜索关键词，为空时返回结果也为空
page|int|
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 194,
        "club_count": 46,
        "post_list": [
            {
	            "id": 213389,
	            "user_id": 807748, // 用户ID
	            "company_id": 1001572, // 企业/店铺ID
	            "title": "我这个账号是有企Q的哦",
	            "post_type": 1, // 信息类型 1商品 2帖子
	            "price": 0,
	            "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
	            "province_id": 20,
	            "city_id": 144,
	            "club_id": 22,
	            "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
	            "is_recommend": 0, // 是否推荐 0正常 1推荐
	            "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
	            "updated_time": 1571905231,
	            "created_time": 1571905231,
	            "post_content_rtf": "", // 富文本内容
	            "post_content_txt": "", // 纯文本内容
	            "cover_pic": "https://test-imgqn.smm.cn/test/b/image/EYcjagsUSDUxKQvYfNlO20191024042026.jpg", // 封面
	            "product_pic_set": "https://test-imgqn.smm.cn/test/b/image/kgeKsKmfakQBrFSjkLow20191024042026.jpg;https://test-imgqn.smm.cn/test/b/image/PVnORfRFEwGXPbiWlPFm20191024042026.jpg;https://test-imgqn.smm.cn/test/b/image/EYcjagsUSDUxKQvYfNlO20191024042026.jpg", // 图片集合
	            "admin_email": "",
	            "top": 0, // 是否置顶 0否 1是
	            "is_notice": 0, // 是否通知 0否 1是
	            "refresh_time": 0, // 最后一次刷新时间
	            "is_offer": 0, // 是否报价 0否 1是
	            "pic_amount": 3, // 图片总数
	            "is_crawl": 0, // 是否爬虫抓取 0否 1是
	            "unit": "",
	            "area": "",
	            "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
	            "reason": "", // 审核拒绝原因
	            "approval_time": 1571906970, // 审核时间
	            "approver_email": "test@smm.cn",
	            "click_count": 11, // 点击量
	            "sale_number": "222", // 可售数量
	            "valid_period": 100, // 有效期（天）
	            "valid_period_time": 1582182175, // 有效期时间戳
	            "category_id": 2, // 所属顶级分类ID
	            "last_category_id": 8, // 所属分类
	            "is_vip": 1, // 发布人是否会员 1是 2否
	            "vip_type": 2, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
	            "location_province": "", // gps 省份
	            "location_city": "", // gps 城市
	            "location_gps": "", // GPS 经纬度
	            "navbar_name": "铜",
	            "club_name": "电解铜",
	            "province_name": "广西",
	            "city_name": "桂林市",
	            "user_info": { // 发布人名片
	                "id": 64, // 名片ID
	                "user_id": 807748,
	                "is_public": 1,
	                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardcfLqK20191029145002.png",
	                "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/LBVmh20190625135010.jpeg",
	                "real_name": "吴梦娜",
	                "cellphone": "18512197032",
	                "telephone": "18512154782",
	                "company_type": "矿产商",
	                "company_name": "测试贸易12134",
	                "province_id": 18,
	                "city_id": 0,
	                "address": "峨山路",
	                "position": "小职员",
	                "main_product": "铜铝铅",
	                "source_channel": 1,
	                "admin_email": "olduser@smm.cn",
	                "create_time": 1570863392,
	                "update_time": 1573187590
	            },
	            "attribute": [ // 信息属性
	                {
	                    "attribute_id": 42,
	                    "name": "正则",
	                    "attr_type": 2, // 1单选 2文本
	                    "attr_options": "^[A-Za-z0-9]+$", // 单选时为逗号分隔的选项 文本时为正则表达式
	                    "attr_unit": "",
	                    "attr_value": "22"
	                }
	            ],
	            "company_name": "测试贸易12134",
	            "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
	            "vip_company_status_desc": "服务中",
	            "vip_year": 5, // 店铺服务年限
	            "qidian_wpa_url": "http://q.url.cn/ABoDYP?_type=wpa&qidian=true", // 企点URL
	            "category_name": "铜",
	            "last_category_name": "电解铜"
	        }
        ]
    }
}
```
</details>

---

#### <a id="search.post.qidian">API: 企点根据关键词搜索帖子</a>

**接口描述**

查询搜索引擎，最多返回60条数据

**请求描述**

**GET**  search/post/qidian

**参数描述**

query:

名称|类型|描述
---|---|---
key_word|string|搜索关键词，模糊匹配



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "post_list": [
            {
                "post_id": 213190, // 信息ID
                "title": "供应铅锌矿，铅锌矿石，欢迎来电咨询", // 信息标题
                "price": 0,
                "province_id": 19,
                "province_name": "广东",
                "city_id": 137,
                "city_name": "东莞市",
                "user_id": 808198,
                "avatar": "",
                "nickname": "134****9045",
                "company_id": 1001774,
                "company_name": "上海麦拓斯电子商务有限公司",
                "vip_year": 1, // 店铺年限
                "club_id": 95, // 所属圈子ID
                "club_name": "铅锌矿",
                "created_time": 1564390622,
                "updated_time": 1564390622
            }
        ],
        "count": 6
    }
}
```
</details>

---

#### <a id="search.company_list">API: 根据帖子标题搜索帖子重的公司</a>

**接口描述**

走搜索引擎,最多30条；如果搜索引擎查不到，则从数据库找出30条`original_company_name`不为空的帖子

**请求描述**

**GET**  search/company_list

**参数描述**

query:

名称|类型|描述
---|---|---
key_word|string|关键词，模糊匹配



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "company_list": [
            {
                "name": "东莞市致方自动化设备有限责任公司"
            },
            {
                "name": "军发五金制罐厂"
            }
        ]
    }
}
```
</details>

---

#### <a id="search.key_word_list">API: 搜索关键词列表</a>

**请求描述**

**GET**  search/key_word_list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
key_word|string|关键词，模糊匹配



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 2887,
        "key_word_list": [
            {
                "id": 65110,
                "name": "富锌锌粉",
                "updated_time": 1562835563,
                "created_time": 1562835563,
                "admin_email": "liuzhenli@smm.cn",
                "word_type": 2 // 词类型 1:主词 2:相关词
            }
        ]
    }
}
```
</details>

---

#### <a id="search.load_all_key_word">API: 批量更新关键词</a>

**接口描述**

更新搜索引擎索引

**请求描述**

**GET**  search/load_all_key_word

---

#### <a id="">API: 前台例子</a>

**请求描述**

**GET**  

### <a id="item_houtaijiekou_669071000">后台接口</a>

所有后台接口必须传名称为`SMM-ADMIN-TOKEN`的header，值为管理员登录token；

### <a id="item_xingye_669132000">行业</a>



---

#### <a id="admin.industry.save">API: 添加/保存行业</a>

**请求描述**

**POST**  admin/industry/save

**参数描述**

body:

名称|类型|描述
---|---|---
industry_id|int|行业ID ，新增时不填，编辑时必填
industry_name|string|行业名称 必填
sort|int|排序 0～99之间
status|int|状态 `1`显示 `2`隐藏
category_ids|string|关联的分类ID，以英文逗号分割的字符串，如：1,2,3,4



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.industry.list">API: 查询行业列表</a>

**请求描述**

**GET**  admin/industry/list

**参数描述**

query:

名称|类型|描述
---|---|---
industry_id|int|行业ID
industry_name|string|行业名称
page|int|
limit|int|
status|int|状态 `0`全部 `1`显示 `2`隐藏
begin_time|int|行业更新开始时间
end_time|int|行业更新结束时间
disable|int|`0`全部  `1`启用 `2`禁用



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "page": 1,
        "limit": 20,
        "count": 16,
        "industry_list": [
            {
                "id": 2, // 行业ID
                "industry_name": "测试apioi",
                "status": 1, // 1显示 2隐藏
                "disable": 1, // 1启用 2禁用
                "card_num": 1, // 行业关联的名片数
                "sort": 2,
                "create_admin": "test@smm.cn",
                "update_admin": "test@smm.cn",
                "create_time": 1568699500,
                "update_time": 1573803380,
                "category_list": [ // 行业关联的分类
                    {
                        "id": 2, // 分类ID
                        "name_cn": "铜", // 分类名称
                        "level": 1,
                        "parent_id": 0, // 父级分类ID
                        "sort": 1,
                        "children_ids": "3,4,5,6",
                        "post_num": 40, // 关联的信息数
                        "type": 0,
                        "status": 1, // 1显示 2隐藏
                        "is_disabled": 0, // 0启用 1禁用
                        "industry_id": 0,
                        "img_url": "",
                        "is_recommend": 1, // 0正常 1推荐
                        "create_admin": "test@smm.cn",
                        "create_time": 1571202165,
                        "update_admin": "test@smm.cn",
                        "update_time": 1571724168
                    }
                ]
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.industry.disable">API: 禁用或启用行业</a>

**请求描述**

**POST**  admin/industry/disable

**参数描述**

body:

名称|类型|描述
---|---|---
industry_id|int|行业ID
disable|int|行业状态 `1`显示 `2`禁用



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.industry.info.id">API: 获取单个行业信息</a>

**请求描述**

**GET**  admin/industry/info/:id

**参数描述**

path:

名称|类型|描述
---|---|---
id|int|行业ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "id": 2,
        "industry_name": "测试apioi",
        "status": 1,
        "disable": 2,
        "card_num": 1,
        "sort": 2,
        "create_admin": "test@smm.cn",
        "update_admin": "test@smm.cn",
        "create_time": 1568699500,
        "update_time": 1573803380
    }
}
```
</details>

---

#### <a id="admin.industry.migrate">API: 将行业名片迁移至其他行业</a>

**接口描述**

该接口是将指定行业所关联的名片统一更改为关联另一个指定的行业；

**请求描述**

**GET**  admin/industry/migrate

**参数描述**

query:

名称|类型|描述
---|---|---
from_industry_id|int|要迁移的行业id
to_industry_id|int|迁移的目标行业id



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.industry.sync.card_num">API: 手动同步行业关联名片数</a>

**接口描述**

重新统计每个行业下关联的名片数并更新；

**请求描述**

**GET**  admin/industry/sync/card_num

---

#### <a id="admin.industry.batch_order">API: 批量保存行业排序</a>

**请求描述**

**POST**  admin/industry/batch_order

**参数描述**

body:

名称|类型|描述
---|---|---
industry_orders|string|json字符串，如：[{"industry_id":6,"order":1},{"industry_id":5,"order":2},{"industry_id":7,"order":12},{"industry_id":8,"order":4}]



<details>
<summary>响应描述</summary>

```json

```
</details>

### <a id="item_fenleiguanli_669198000">分类管理</a>



---

#### <a id="admin.category.get_category_list">API: 查询分类列表</a>

**请求描述**

**GET**  admin/category/get_category_list

**参数描述**

query:

名称|类型|描述
---|---|---
id|int|分类ID
parent_id|int|父级分类ID
name_cn|string|分类名称，模糊匹配
is_recommend|int|是否推荐：`-1`全部 `0`不推荐 `1`推荐
is_disabled|int|是否禁用：`-1`全部 `0`不禁用 `1`禁用
status|int|是否显示：`0`全部 `1`显示 `2`隐藏
time_type|string|时间区间查询类型：`create` 创建时间 `update`更新时间
begin_time|int|开始时间
end_time|int|结束时间
page|int|
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 107,
        "page": 0,
        "limit": 0,
        "category_list": [
            {
                "id": 1, // 分类ID
                "name_cn": "铝", // 分类名称
                "level": 1, // 分类级别
                "parent_id": 0, // 父级分类ID 0代表顶级分类
                "sort": 2,
                "children_ids": "18,19,20", // 子级分类ID
                "post_num": 1, // 分类下的信息数
                "type": 0,
                "status": 1, // 1显示 2隐藏
                "is_disabled": 0, // 0启用 1禁用
                "industry_id": 0,
                "img_url": "",
                "is_recommend": 1, // 0正常 1推荐分类
                "create_admin": "test@smm.cn",
                "create_time": 1571201643,
                "update_admin": "test@smm.cn",
                "update_time": 1572331589,
                "parent_name": "", // 父级分类名称
                "children_list": [ // 子级分类列表
                    {
                        "category_id": 18,
                        "category_name": "铝原料"
                    },
                    {
                        "category_id": 19,
                        "category_name": "铝加工"
                    }
                ]
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.category.save_category">API: 保存分类</a>

**请求描述**

**POST**  admin/category/save_category

**参数描述**

body:

名称|类型|描述
---|---|---
id|int|分类ID，编辑时必填
parent_id|int|父级分类ID，选填
name_cn|string|分类名称
status|int|显示状态：`1`显示 `2`隐藏
is_disabled|int|禁用状态：`0`正常 `1`禁用
sort|int|排序数字，0～99之间
img_url|string|默认图片，选填



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "category_id": 15 // 创建的分类ID
    }
}
```
</details>

---

#### <a id="admin.category.get_category_info">API: 查询分类详情</a>

**请求描述**

**GET**  admin/category/get_category_info

**参数描述**

query:

名称|类型|描述
---|---|---
id|int|分类ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "id": 1, // 分类ID
        "name_cn": "铝", // 分类名称
        "level": 1, // 分类级别
        "parent_id": 0, // 父级分类ID 0代表顶级分类
        "sort": 2,
        "children_ids": "18,19,20", // 子级分类ID
        "post_num": 1, // 分类下的信息数
        "type": 0,
        "status": 1, // 1显示 2隐藏
        "is_disabled": 0, // 0启用 1禁用
        "industry_id": 0,
        "img_url": "",
        "is_recommend": 1, // 0正常 1推荐分类
        "create_admin": "test@smm.cn",
        "create_time": 1571201643,
        "update_admin": "test@smm.cn",
        "update_time": 1572331589,
        "parent_name": "", // 父级分类名称
        "children_list": [ // 子级分类列表
            {
                "category_id": 18,
                "category_name": "铝原料"
            },
            {
                "category_id": 19,
                "category_name": "铝加工"
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.category.batch_disabled">API: 启用/禁用分类</a>

**接口描述**

当禁用时会将每个分类的所有后代分类一并禁用，启用时为选择那个分类就启用那个分类，后代分类不管

**请求描述**

**POST**  admin/category/batch_disabled

**参数描述**

body:

名称|类型|描述
---|---|---
ids|string|逗号分隔的分类ID
disable|int|禁用状态：`0`启用 `1`禁用



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.category.batch_hide">API: 显示/隐藏分类</a>

**请求描述**

**POST**  admin/category/batch_hide

**参数描述**

body:

名称|类型|描述
---|---|---
ids|string|逗号分隔的分类ID
status|int|禁用状态：`1`显示 `2`隐藏



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.category.batch_recommend">API: 设置获取消推荐分类</a>

**请求描述**

**POST**  admin/category/batch_recommend

**参数描述**

body:

名称|类型|描述
---|---|---
ids|string|逗号分割的分类ID
recommend|int|推荐：`0`不推荐 `1`推荐



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.category.migrate_category">API: 迁移分类</a>

**接口描述**

该接口是将指定分类下发布的信息的所属分类替换为另一个指定的分类

**请求描述**

**GET**  admin/category/migrate_category

**参数描述**

query:

名称|类型|描述
---|---|---
from_category_id|int|被迁移的分类ID
to_category_id|int|迁移的目标分类ID



<details>
<summary>响应描述</summary>

```json

```
</details>

---

#### <a id="admin.category.get_category_attribute_list">API: 查询分类属性列表</a>

**请求描述**

**GET**  admin/category/get_category_attribute_list

**参数描述**

query:

名称|类型|描述
---|---|---
category_id|int|分类ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "attribute_list": [
            {
                "id": 37,
                "name": "12",
                "attr_type": 2, // 1单选 2文本
                "attr_options": "", // 单选时为逗号分割的选项
                "attr_unit": "",
                "sort_number": 0,
                "is_lock": 0 // 1只读，继承父级的属性 0可以修改删除
            },
            {
                "id": 38,
                "name": "2",
                "attr_type": 1,
                "attr_options": "1,2", // 文本时为正则表达式
                "attr_unit": "",
                "sort_number": 0,
                "is_lock": 0
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.category.save_category_attribute">API: 保存分类属性</a>

**接口描述**

只传当前分类自己的属性就可以，父级（`is_lock`=1）的不用传

参数json字段介绍：

名称|类型|描述
---|---|---
category_id|int|分类ID
attributes|array|分类的属性json
name|string|属性名称
attr_type|int|`1`文本 `2`单选
attr_options|string|文本类型时为正则表达式；单选类型时为逗号分割的选项
attr_unit|string|单位
sort_number|int|排序数值

**请求描述**

**POST**  admin/category/save_category_attribute

**参数描述**

特殊参数：

`Content-Type`:`application/json`

```json
{
	"category_id":36,
	"attributes":[
		{
			"name": "名称",
    		"attr_type": 2,
    		"attr_options": "",
    		"attr_unit": "",
    		"sort_number": 0
    	},
    	{
			"name": "型号",
    		"attr_type": 2,
    		"attr_options": "",
    		"attr_unit": "",
    		"sort_number": 0
    	}
	]
}
```

<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.category.get_category_relation_list">API: 查询分类关系列表</a>

**请求描述**

**GET**  admin/category/get_category_relation_list

**参数描述**

query:

名称|类型|描述
---|---|---
category_id|int|分类ID，必填
category_slave_name|string|关联的分类名称，模糊匹配
status|int|状态：`0`全部 `1`启用 `2`禁用
begin_time|int|关联关系开始时间
end_time|int|关联关系结束时间
page|int|
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 1,
        "page": 1,
        "limit": 10,
        "category_relation_list": [
            {
                "id": 184, // 分类关系ID
                "category_id_master": 1, // 分类ID
                "category_master_name": "铝",
                "relation_id": 22, // 关系类型ID
                "relation_name": "测试反向", // 关系类型名称
                "category_id_slave": 2, // 被关联分类ID
                "category_slave_name": "铜",
                "status": 1, // 1启用 2禁用
                "sort": 0,
                "update_admin": "test@smm.cn",
                "update_time": 1573202751
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.category.save_category_relation">API: 保存分类关系</a>

**请求描述**

**POST**  admin/category/save_category_relation

**参数描述**

body:

名称|类型|描述
---|---|---
id|int|分类关系ID，编辑时必填
category_id_master|int|关联的分类ID
relation_id|int|关系类型ID
category_id_slave|int|被关联的分类ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.category.del_category_relation">API: 批量删除分类关系</a>

**请求描述**

**POST**  admin/category/del_category_relation

**参数描述**

body:

名称|类型|描述
---|---|---
ids|string|逗号分隔的分类关系ID，例如：1,2
status|int|状态：`1`启用 `2`删除



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.category.get_category_relation_info">API: 查询分类关系详情</a>

**请求描述**

**GET**  admin/category/get_category_relation_info

**参数描述**

query:

名称|类型|描述
---|---|---
id|int|分类关系ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "id": 1, // 分类关系ID
        "category_id_master": 33, // 关联分类ID
        "category_master_name": "金坷垃",
        "relation_id": 8, // 关系类型ID
        "relation_name": "牛奶",
        "category_id_slave": 37, // 被关联分类ID
        "category_slave_name": "木疙瘩",
        "status": 1, // 1启用 2禁用
        "sort": 0,
        "update_admin": "test@smm.cn",
        "update_time": 1570613183
    }
}
```
</details>

---

#### <a id="admin.category.get_relation_list">API: 查询关系类型列表</a>

**请求描述**

**GET**  admin/category/get_relation_list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 11,
        "page": 1,
        "limit": 10,
        "relation_list": [
            {
                "id": 2, // 关系类型ID
                "name": "下游qw", // 关系类型名称
                "status": 1, // 1启用 2禁用
                "relation_id": 1, // 大于0为双向关系，值代表双向关联的关系类型ID
                "sort": 0,
                "create_admin": "",
                "create_time": 0,
                "update_admin": "",
                "update_time": 1570603374,
                "relation_name": "原料222w" // 双向关系类型的名称
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.category.save_relation">API: 保存关系</a>

**请求描述**

**POST**  admin/category/save_relation

**参数描述**

body:

名称|类型|描述
---|---|---
id|int|关系类型ID，编辑时必填
name|string|关系类型名称
relation_name|string|反向关系类型名称



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.category.del_relation">API: 删除关系类型</a>

**请求描述**

**POST**  admin/category/del_relation

**参数描述**

body:

名称|类型|描述
---|---|---
ids|string|逗号分隔的关系类型ID
status|int|状态：`1`启用 `2`删除



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.category.get_relation_info">API: 查询关系类型详情</a>

**请求描述**

**GET**  admin/category/get_relation_info

**参数描述**

query:

名称|类型|描述
---|---|---
relation_id|int|关系类型ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "id": 2, // 关系类型ID
        "name": "设备",
        "status": 1, // 1启用 2禁用
        "relation_id": 0, // 大于0为双向关系，值代表关联的双向关系类型ID
        "sort": 0,
        "create_admin": "test@smm.cn",
        "create_time": 1571368999,
        "update_admin": "test@smm.cn",
        "update_time": 1571368999,
        "relation_name": ""
    }
}
```
</details>

---

#### <a id="admin.category.batch_order">API: 批量保存分类排序</a>

**请求描述**

**POST**  admin/category/batch_order

**参数描述**

body:

名称|类型|描述
---|---|---
category_orders|string|json字符串，例如：<br/>[{"category_id":2,"order":2},
{"category_id":13,"order":13},
{"category_id":18,"order":18}]



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

### <a id="item_quanziguanli_669491000">圈子管理</a>



---

#### <a id="admin.club.list">API: 查询圈子列表</a>

**请求描述**

**GET**  admin/club/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
name|string|圈子名称，模糊匹配
id|int|圈子ID
disable|int|是否禁用  `-1`全部 `0`正常 `1`禁用
begin_date|int|圈子创建开始时间
end_date|int|圈子创建结束时间



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 475,
        "club_list": [
            {
                "id": 420, // 圈子ID
                "user_id": 808117,
                "name": "鼓风机",
                "introduction": "",
                "logo": "",
                "h5_background": "",
                "web_background": "",
                "is_recommend": 1, // 是否推荐 0正常 1推荐
                "disabled": 0, // 是否禁用 0正常 1禁用
                "updated_time": 1573630862,
                "created_time": 1562205875,
                "members_amount": 6, // 成员数
                "post_amount": 1872, // 信息数
                "today_post_amount": 0, // 今日发布信息数
                "admin_email": "test@smm.cn",
                "is_audit": 0,
                "category_list": [ // 关联的分类列表
                    {
                        "id": 7, // 分类ID
                        "name_cn": "废铜",
                        "level": 3,
                        "parent_id": 6,
                        "sort": 1,
                        "children_ids": "",
                        "post_num": 0,
                        "type": 0,
                        "status": 2,
                        "is_disabled": 0,
                        "industry_id": 0,
                        "img_url": "",
                        "is_recommend": 1,
                        "create_admin": "test@smm.cn",
                        "create_time": 1571205929,
                        "update_admin": "test@smm.cn",
                        "update_time": 1571724168
                    }
                ]
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.club.add_or_edit">API: 添加/编辑圈子</a>

**请求描述**

**POST**  admin/club/add_or_edit

**参数描述**

body:

名称|类型|描述
---|---|---
id|int|圈子ID  编辑时必填
name|string|圈子名称
account|string|圈主账号  `account`和`master_id`二选一
master_id|int|圈主用户ID
category_ids|string|以逗号分割的分类ID，如：1,2,3
introduction|string|圈子简介
logo|string|圈子logo



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.club.enable">API: 启用圈子</a>

**请求描述**

**POST**  admin/club/enable

**参数描述**

body:

名称|类型|描述
---|---|---
id|int|圈子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.club.disable">API: 禁用圈子</a>

**请求描述**

**POST**  admin/club/disable

**参数描述**

body:

名称|类型|描述
---|---|---
id|int|圈子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.club.settle.recommend">API: 设置推荐圈子</a>

**请求描述**

**POST**  admin/club/settle/recommend

**参数描述**

body:

名称|类型|描述
---|---|---
id|int|圈子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.club.cancel.recommend">API: 取消推荐圈子</a>

**请求描述**

**POST**  admin/club/cancel/recommend

**参数描述**

body:

名称|类型|描述
---|---|---
id|int|圈子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.club.members">API: 圈内成员列表</a>

**请求描述**

**GET**  admin/club/members

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
club_id|int|圈子ID
disable|int|圈内成员状态 `-1`全部 `0`正常 `1`禁止加入 



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 2,
        "members": [
            { // 成员名片信息
                "id": 5, // 名片ID
                "user_id": 807328,
                "is_public": 0, // 名片是否公开 1公开 2不公开
                "card_url": "https://test-imgqn.smm.cn/test/admin/company/YIJYO20190918113434.jpeg",
                "avatar": "",
                "real_name": "邱生",
                "cellphone": "18002588022",
                "telephone": "0757-82095526",
                "company_type": "贸易商",
                "company_name": "佛山市凌言网络科技有限公司",
                "province_id": 12,
                "city_id": 0,
                "address": "广东省佛山市禅城区季华六路3号九鼎国际城1区4座1411号",
                "position": "123",
                "main_product": "123",
                "source_channel": 4,
                "admin_email": "test@smm.cn",
                "create_time": 1568704686,
                "update_time": 1568704686,
                "disable": 0, // 成员状态 0正常 1禁止该用户加入此圈
                "join_club_time": 1569316600, // 加圈时间
                "vip_status": 2, // 会员状态 0未开通 1过期 2服务中 3关闭
                "vip_type": 2, // 会员类型 1月度 2年度 3体验 4季度 5半年
                "club_post_num": 2 // 该用户30天内的发帖数
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.club.member.disable">API: 批量禁止或启用圈内成员</a>

**接口描述**

禁止就是踢出成员并禁止再次加入该圈

**请求描述**

**POST**  admin/club/member/disable

**参数描述**

body:

名称|类型|描述
---|---|---
club_id|int|圈子ID
disable|int|`1` 禁止 `0`正常
user_ids|string|以逗号分割的用户ID，如：807720,804478



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.club.users">API: 获取所有加过圈子的用户</a>

**请求描述**

**GET**  admin/club/users

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
user_id|int|用户ID，优先该参数，忽略`company_name`、`nick_name`、`phone`
company_name|string|公司名称
nick_name|string|昵称
phone|string|手机号



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 963,
        "users": [
            {
                "id": 3518,
                "user_id": 808368,
                "created_time": 1568864996,
                "updated_time": 1568864996,
                "clubs": [ // 加入的圈子列表
                    {
                        "id": 119,
                        "name": "铜精矿"
                    }
                ]
            }
            {
                "id": 3509,
                "user_id": 808036,
                "created_time": 1568181592,
                "updated_time": 1568181592,
                "clubs": [
                    {
                        "id": 22,
                        "name": "电解铜"
                    }
                ]
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.club.list_by_member">API: 根据用户获取加入的圈子列表</a>

**请求描述**

**GET**  admin/club/list_by_member

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
role|string|角色：`master`圈主 `member`成员，为空是全部
user_id|int|用户ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 43,
        "page": 1,
        "limit": 10,
        "list": [ // 圈子列表
            {
                "club_id": 128,
                "club_name": "锡粉",
                "master_id": 808117, // 圈主用户ID
                "user_id": 808196,
                "operator_type": 1,
                "operator": "",
                "role": "member", // 用户在该圈子内的角色
                "disable": 0,
                "UpdatedTime": 1564145314,
                "CreatedTime": 1564145314
            },
            {
                "club_id": 345,
                "club_name": "碲锭",
                "master_id": 418905,
                "user_id": 808196,
                "operator_type": 1,
                "operator": "",
                "role": "member",
                "disable": 0,
                "UpdatedTime": 1564143000,
                "CreatedTime": 1564143000
            }
        ]
    }
}
```
</details>

### <a id="item_mingpianguanli_669834000">名片管理</a>



---

#### <a id="admin.usercard.approval.list">API: 获取审核名片列表</a>

**请求描述**

**GET**  admin/usercard/approval/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
approval_status|int|审核状态 `1`待审核 `2`审核通过 `3`审核失败
begin_date|int|开始提交时间
end_date|int|结束提交时间
user_id|int|用户ID
id|int|审核id
real_name|string|真实姓名
cellphone|string|手机号
company_name|string|公司名称，模糊匹配



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 12,
        "page": 1,
        "limit": 10,
        "list": [
            {
                "id": 77, // 审核记录ID
                "user_id": 805780, // 用户ID
                "approval_status": 3, // 审核状态 1待审核 2通过 3拒绝
                "reason": "t", // 审核拒绝原因
                "is_public": 2, // 名片是否公开 1公开 2不公开
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardUmszV20191118135043.png",
                "avatar": "",
                "real_name": "",
                "cellphone": "13162979358",
                "telephone": "",
                "company_type": "",
                "company_name": "",
                "province_id": 0,
                "city_id": 0,
                "address": "",
                "position": "",
                "main_product": "",
                "admin_email": "test@smm.cn",
                "source_channel": 3,
                "share_user_id": 0, // 使用的分享人用户ID，0表示没有
                "industry_ids": "", // 关联的行业ID，逗号分割
                "industry_names": "",
                "create_time": 1574056243,
                "update_time": 1574057083
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.usercard.approval.info">API: 获取单个名片审核记录</a>

**请求描述**

**GET**  admin/usercard/approval/info

**参数描述**

query:

名称|类型|描述
---|---|---
approval_id|int|名片审核记录ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "id": 81, // 审核记录ID
        "user_id": 807720, // 用户ID
        "approval_status": 1, // 审核状态 1待审核 2通过 3拒绝
        "reason": "", // 审核拒绝原因
        "is_public": 1, // 名片是否公开 1公开 2不公开
        "card_url": "https://test-imgqn.smm.cn/test/club/user/cardubpDF20191105173608.png",
        "avatar": "",
        "real_name": "张新杰",
        "cellphone": "13127881017",
        "telephone": "099-123456",
        "company_type": "矿产商",
        "company_name": "上海有色网股份有限公司",
        "province_id": 18,
        "city_id": 0,
        "address": "上海浦东新区峨山路91弄20号陆家嘴软件园9号楼9楼",
        "position": "后端工程师",
        "main_product": "铝合金",
        "admin_email": "",
        "source_channel": 1,
        "share_user_id": 0,
        "industry_ids": "", // 关联的行业ID，以逗号分割
        "industry_names": "",
        "create_time": 1574057608,
        "update_time": 1574057608,
        "province": "",
        "city": "",
        "industry_list": [] // 关联的行业列表
    }
}
```
</details>

---

#### <a id="admin.usercard.batch.approval">API: 批量审核名片</a>

**请求描述**

**POST**  admin/usercard/batch/approval

**参数描述**

body:

名称|类型|描述
---|---|---
approval_ids|string|审核ID 以逗号分割，如：1,22,42
approval_status|int|审核状态 `1`待审核 `2`审核通过 `3`审核失败，只能`2`或`3`
reason|string|审核失败原因，`approval_status`为`3`时必填



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.usercard.approval">API: 审核并编辑名片</a>

**请求描述**

**POST**  admin/usercard/approval

**参数描述**

body:

名称|类型|描述
---|---|---
approval_id|int|审核记录ID
approval_status|int|审核状态 `2`成功 `3`失败
reason|string|审核拒绝原因
is_public|int|是否公开 `1`公开 `2`需要同意
card_url|string|名片图片链接
real_name|string|真实姓名
cellphone|string|手机号
telephone|string|电话号
company_type|string|企业类型 `贸易商`/`矿产商`/`冶炼企业`/`加工企业`/`生产企业`五选一
company_name|string|企业名称
province_id|int|省份id
city_id|int|城市id
address|string|地址·
position|string|职位
industry_ids|string|行业ID，以逗号分割，如：1,15,16
main_product|string|主营产品
source_channel|int|名片来源渠道 `1`pc `2`app `3`wx `4`admin



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.usercard.list">API: 获取名片列表</a>

**请求描述**

**GET**  admin/usercard/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
begin_time|int|名片创建开始时间
end_time|int|名片创建结束时间
id|int|名片ID
user_id|int|用户ID
industry_id|int|行业ID
province_id|int|省份ID
city_id|int|城市ID
real_name|string|真实姓名
cellphone|string|手机号
telephone|string|电话
company_name|string|公司名称，模糊匹配



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 236,
        "page": 1,
        "limit": 10,
        "list": [
            {
                "id": 458, // 名片ID
                "user_id": 805780,
                "is_public": 2,
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardniXik20191118140924.png",
                "avatar": "",
                "real_name": "",
                "cellphone": "13162979358",
                "telephone": "",
                "company_type": "",
                "company_name": "",
                "province_id": 0,
                "city_id": 0,
                "address": "",
                "position": "",
                "main_product": "",
                "source_channel": 3,
                "create_time": 1574057445,
                "update_time": 1574057445,
                "province": "",
                "city": "",
                "approval_status": 2,
                "reason": "",
                "admin_email": "",
                "industry_list": [ // 关联的行业列表
                    {
                        "id": 16,
                        "industry_name": "国际贸易",
                        "status": 1,
                        "disable": 1,
                        "card_num": 21,
                        "sort": 1,
                        "create_admin": "test@smm.cn",
                        "update_admin": "test@smm.cn",
                        "create_time": 1571384075,
                        "update_time": 1571646390
                    }
                ],
                "vip_status": 0,
                "vip_type": 0,
                "relationship": 0,
                "group_id": 0,
                "group_name": ""
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.usercard.info">API: 根据用户ID获取名片</a>

**请求描述**

**GET**  admin/usercard/info

**参数描述**

query:

名称|类型|描述
---|---|---
user_id|int|用户ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "id": 7, // 名片ID
        "user_id": 807720, // 用户ID
        "is_public": 2, // 名片是否公开 1公开 2不公开
        "card_url": "https://test-imgqn.smm.cn/test/club/user/cardubpDF20191105173608.png",
        "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/nNaGF20190923194241.jpeg",
        "real_name": "张新杰",
        "cellphone": "13127881017",
        "telephone": "099-123456",
        "company_type": "矿产商",
        "company_name": "上海有色网股份有限公司",
        "province_id": 18,
        "city_id": 0,
        "address": "上海浦东新区峨山路91弄20号陆家嘴软件园9号楼9楼",
        "position": "后端工程师",
        "main_product": "铝合金",
        "source_channel": 4,
        "create_time": 1568788590,
        "update_time": 1572946568,
        "province": "上海",
        "city": "",
        "approval_status": 2,
        "reason": "",
        "admin_email": "",
        "industry_list": [ // 名片关联的行业列表
            {
                "id": 10,
                "industry_name": "精细化工",
                "status": 1,
                "disable": 1,
                "card_num": 19,
                "sort": 1,
                "create_admin": "test@smm.cn",
                "update_admin": "test@smm.cn",
                "create_time": 1571384041,
                "update_time": 1571646390
            }
        ],
        "vip_status": 2, // 会员状态 1过期 2服务中 3关闭
        "vip_type": 1, // 会员类型 1月度 2年度 3体验 4季度 5半年
        "relationship": 0,
        "group_id": 0,
        "group_name": ""
    }
}
```
</details>

---

#### <a id="admin.usercard.save">API: 添加/编辑名片信息</a>

**请求描述**

**POST**  admin/usercard/save

**参数描述**

body:

名称|类型|描述
---|---|---
account|string|用户账号  和`user_id` 二选一；存在这两个参数则是名片修改，否则添加
user_id|int|名片对应的用户ID 
is_public|int|是否公开 `1`公开 `2`需要同意
card_url|string|名片图片链接
real_name|string|真实姓名
cellphone|string|手机号
telephone|string|电话号
company_type|string|企业类型 `贸易商`/`矿产商`/`冶炼企业`/`加工企业`/`生产企业` 五选一
company_name|string|企业名称
province_id|int|省份id
city_id|int|城市id
address|string|地址
position|string|职位
industry_ids|string|行业ID，以逗号分隔，如：1,2,3
main_product|string|主营产品
source_channel|int|名片来源渠道 `1`pc `2`app `3`wx `4`admin



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.usercard.relationship">API: 获取某个名片的名片夹里的所有名片</a>

**请求描述**

**GET**  admin/usercard/relationship

**参数描述**

query:

名称|类型|描述
---|---|---
card_id|int|名片ID
page|int|
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "relationship_list": [
            {
                "id": 7, // 名片ID
                "user_id": 807720, // 用户ID
                "is_public": 2,
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardubpDF20191105173608.png",
                "avatar": "",
                "real_name": "张新杰",
                "cellphone": "13127881017",
                "telephone": "099-123456",
                "company_type": "矿产商",
                "company_name": "上海有色网股份有限公司",
                "province_id": 18,
                "city_id": 0,
                "address": "上海浦东新区峨山路91弄20号陆家嘴软件园9号楼9楼",
                "position": "后端工程师",
                "main_product": "铝合金",
                "source_channel": 4,
                "admin_email": "",
                "create_time": 1568788590,
                "update_time": 1572946568,
                "province": "上海",
                "city": "",
                "relationship": 2, // 好友关系 1 单向加对方 2互为好友 3待对方确
                "source": 2, // 名片数据来源 1二维码 2商机 3通讯录
                "add_time": 1168633193 // 加为好友的时间戳
            }
        ],
        "count": 1,
        "page": 1,
        "limit": 10
    }
}
```
</details>

### <a id="item_huiyuanguanli_670137000">会员管理</a>



---

#### <a id="admin.vip.list">API: 会员管理列表</a>

**请求描述**

**GET**  admin/vip/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
time_type|string|时间查询类型，`start`：会员开始时间 `end`：会员结束时间 `create`：创建时间 `update`：修改时间
begin_time|int|
end_time|int|
vip_status|int|会员状态 `0`全部 `1`过期 `2`服务中 `3`关闭
company_name|string|名片里的公司名称，模糊匹配
phone|string|手机号



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "vip_user_list": [
            {
                "user_id": 807720,
                "last_refresh": 0,
                "is_recommend": 1,
                "recommend_sort": 1,
                "vip_status": 2, // 会员状态 1过期 2服务中 3关闭
                "vip_type": 1, // 会员类型 1月度 2年度 3体验 4季度 5半年
                "vip_start_date": 1234567890, // 会员开通时间
                "vip_end_date": 1590681600, // 会员结束时间
                "create_time": 0,
                "update_time": 1573803099,
                "admin_email": "test@smm.cn",
                "real_name": "张新杰",
                "cellphone": "13127881017",
                "telephone": "099-123456",
                "user_cellphone": "13127881017", // 用户中心绑定手机号
                "external_cellphone": "13127881017", // 对外联系方式
                "company_name": "上海有色网股份有限公司",
                "province": "上海",
                "city": "",
                "industry_list": [ // 关联的行业列表
                    {
                        "id": 8,
                        "industry_name": "电器001",
                        "status": 1,
                        "disable": 1,
                        "card_num": 3,
                        "sort": 4,
                        "create_admin": "test@smm.cn",
                        "update_admin": "test@smm.cn",
                        "create_time": 1571119885,
                        "update_time": 1571646390
                    }
                ],
                "join_company": true, // 是否加入企业
                "open_shop": true // 是否开通店铺
            }
        ],
        "count": 1,
        "page": 1,
        "limit": 10
    }
}
```
</details>

---

#### <a id="admin.vip.user">API: 根据账号查询用户</a>

**接口描述**

`account`和`user_id`两个参数二选一, 优先用户ID。

**请求描述**

**GET**  admin/vip/user

**参数描述**

query:

名称|类型|描述
---|---|---
account|string|账号 邮箱或手机号
user_id|int|用户ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "user_card_status": 2, // 用户名片状态 0未完善 1待审核 2审核通过 3审核失败 
        "vip_type": 1, // 会员类型 1月度 2年度 3体验 4季度 5半年
        "vip_status": 2, // 会员状态 1过期 2服务中 3关闭
        "vip_start_date": 1234567890,
        "vip_end_date": 1590681600,
        "user_info": { // 用户中心数据
            "real_name": "张新杰",
            "user_name": "SMM1546927067xW",
            "nickname": "toy",
            "description": "",
            "cellphone": "13127881017",
            "email": "",
            "id": 807720,
            "company_name": "上海大宝剑有限公司",
            "company_id": 1001764,
            "company_status": 1,
            "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/nNaGF20190923194241.jpeg",
            "company_verify_level": 2,
            "position": "员工",
            "external_cellphone": "13127881017"
        },
        "user_card_info": { // 用户名片
            "id": 7, // 名片ID
            "user_id": 807720,
            "is_public": 2,
            "card_url": "https://test-imgqn.smm.cn/test/club/user/cardubpDF20191105173608.png",
            "avatar": "",
            "real_name": "张新杰",
            "cellphone": "13127881017",
            "telephone": "099-123456",
            "company_type": "矿产商",
            "company_name": "上海有色网股份有限公司",
            "province_id": 18,
            "city_id": 0,
            "address": "上海浦东新区峨山路91弄20号陆家嘴软件园9号楼9楼",
            "position": "后端工程师",
            "main_product": "铝合金",
            "source_channel": 4,
            "admin_email": "",
            "create_time": 1568788590,
            "update_time": 1572946568
        }
    }
}
```
</details>

---

#### <a id="admin.vip.save">API: 添加/编辑会员</a>

**请求描述**

**POST**  admin/vip/save

**参数描述**

body:

名称|类型|描述
---|---|---
user_id|int|要添加或编辑的会员
vip_status|int|会员状态 `2`开通  `3`关闭
vip_start_date|int|会员开始时间
vip_end_date|int|会员结束时间
vip_type|int|`1`月度 `2`年度



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.vip.openshop">API: 后台开通店铺</a>

**请求描述**

**POST**  admin/vip/openshop

**参数描述**

body:

名称|类型|描述
---|---|---
user_id|int|用户ID
year_base|int|店铺服务年限



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

### <a id="item_dianpuguanli_670211000">店铺管理</a>



---

#### <a id="admin.vipCompany.list">API: 获取企业列表</a>

**请求描述**

**GET**  admin/vipCompany/list

**参数描述**

query:

名称|类型|描述
---|---|---
company_name|string|企业名称，模糊匹配
company_id|int|企业ID
status|int|店铺状态：`0`全部 `1`已过期 `2`服务中 `3`已关闭
time_type|string|时间区间查询类型：<br/>`update` 店铺更新时间 `start` 店铺服务开始时间 `end` 店铺服务结束时间
begin_time|int|
end_time|int|
page|int|
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "company_list": [ // 企业店铺列表
            {
                "id": 26,
                "company_id": 1001764,
                "company_name": "上海大宝剑有限公司",
                "status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
                "status_desc": "服务中",
                "year_base": 6, // 店铺服务年限
                "start_date": 1564329600,
                "end_date": 1682732800,
                "background_pic": "",
                "admin_email": "test@smm.cn",
                "open_person": "",
                "update_time": 1573803099,
                "style_config": "{\"hide_title\":false,\"theme\":\"default\"}",
                "description": "why",
                "style": {
                    "theme": "",
                    "hide_title": false
                },
                "company_district": ""
            }
        ],
        "page": 1,
        "limit": 10,
        "count": 1
    }
}
```
</details>

---

#### <a id="admin.vipCompany.edit">API: 编辑企业店铺信息</a>

**请求描述**

**POST**  admin/vipCompany/edit

**参数描述**

body:

名称|类型|描述
---|---|---
company_id|int|
status|int|店铺状态：`2`开通 `3`关闭
year_base|int|店铺年限
start_date|int|店铺开通时间
end_date|int|店铺结束时间



<details>
<summary>响应描述</summary>

```json
{
    "code": 10150,
    "msg": "服务时间错误",
    "data": null
}
```
</details>

---

#### <a id="admin.vipCompany.pic.list">API: 获取企业图片审核列表</a>

**请求描述**

**GET**  admin/vipCompany/pic/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
company_name|string|企业名称
phone|string|手机号
email|string|邮箱
approval_status|int|图片状态：`0`全部 `1`待审核 `2`审核成功 `3`审核失败
type|int|图片类型：`0`全部 `1`企业背景图 `2`企业简介图
begin_time|int|审核开始时间
end_time|int|审核结束时间



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "company_pic_list": [
            {
                "id": 326, // 审核记录ID
                "name": "", // 图片名称
                "company_id": 1001764, // 企业店铺ID
                "url": "https://test-imgqn.smm.cn/test/questioncenter/verify/image/Zkyce20191030103043.jpeg",
                "type": 2, // 图片类型 1企业背景图 2企业简介图
                "user_id": 807720,
                "approver_email": "",
                "approval_status": 1, // 审核状态 1待审核 2通过 3失败
                "reason": "",
                "create_time": 1573616849,
                "approval_time": 1573617122,
                "email": "",
                "phone": "13127881017",
                "company_name": "上海大宝剑有限公司"
            }
        ],
        "page": 1,
        "limit": 2,
        "count": 0
    }
}
```
</details>

---

#### <a id="admin.vipCompany.batch.pic">API: 批量审核企业图片</a>

**请求描述**

**POST**  admin/vipCompany/batch/pic

**参数描述**

body:

名称|类型|描述
---|---|---
pic_ids|string|逗号分割的待审核图片ID，如：1,2,3
approval_status|int|审核状态：`2`审核通过 `3`审核失败
reason|string|审核原因，审核拒绝时必填



<details>
<summary>响应描述</summary>

```json

```
</details>

---

#### <a id="admin.vipCompany.edit.pic">API: 编辑企业图片</a>

**请求描述**

**POST**  admin/vipCompany/edit/pic

**参数描述**

body:

名称|类型|描述
---|---|---
pic_id|int|图片ID 
pic_url|string|图片链接
pic_type|int|图片类型：`1` 背景图 `2`企业简介图



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.vipCompany.auth.edit">API: 授权店铺编辑权限</a>

**请求描述**

**GET**  admin/vipCompany/auth/edit

**参数描述**

query:

名称|类型|描述
---|---|---
company_id|100156|企业店铺ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "auth_key": "GhblT7txWd" // 授权码 有效期10分钟
    }
}
```
</details>

### <a id="item_fenxiangguanli_670275000">分享管理</a>



---

#### <a id="admin.share.list">API: 分享列表</a>

**请求描述**

**GET**  admin/share/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
user_id|int|被分享人ID
phone|string|被分享人电话
share_user_id|int|分享人ID
share_phone|string|分享人电话
card_status|int|名片激活状态：`1` 激活 `2`未激活
time_type|string|时间查询类型 `create` 开始时间 `update` 更新时间 `reg` 注册时间 `card` 名片完善时间
begin_time|int|名片激活开始时间
end_time|int|名片激活结束时间



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 6,
        "page": 1,
        "limit": 10,
        "share_list": [
            {
                "id": 7, // 分享ID
                "user_id": 800021, // 被分享人用户ID
                "avatar": "",
                "nick_name": "",
                "phone": "",
                "real_name": "",
                "company_name": "",
                "share_user_id": 807720, // 分享人用户ID
                "share_phone": "", // 分享人用户手机号
                "reg_time": 0, // 被分享人注册时间
                "card_time": 1568860483, // 被分享人名片信息完善时间
                "admin_email": "",
                "create_time": 0,
                "update_time": 0
            }
        ]
    }
}
```
</details>

### <a id="item_sousuorizhi_670304000">搜索日志</a>



---

#### <a id="admin.search.log.list">API: 搜索日志</a>

**请求描述**

**GET**  admin/search/log/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
phone|string|搜索用户手机号
user_id|int|搜索用户ID
nickname|string|昵称
keyword|string|关键词，模糊匹配
search_type|string|搜索类型：包括但不仅限于：`商品`、`企业`、`用户`、`信息`
begin_time|int|搜索开始时间
end_time|int|搜索结束时间



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 6983,
        "page": 1,
        "limit": 0,
        "list": [
            {
                "id": 7454,
                "create_time": 1574076940,
                "user_id": 807490,
                "phone": "13761533500",
                "nick_name": "Anna Chen",
                "search_type": "信息",
                "search_content": "声。",
                "result_count": 11
            },
            {
                "id": 7453,
                "create_time": 1574076929,
                "user_id": 807490,
                "phone": "13761533500",
                "nick_name": "Anna Chen",
                "search_type": "信息",
                "search_content": "声",
                "result_count": 11
            }
        ]
    }
}
```
</details>

### <a id="item_duihuanliebiao_670327000">兑换列表</a>



---

#### <a id="admin.exchange.list">API: 查询兑换记录列表</a>

**请求描述**

**GET**  admin/exchange/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|1|
limit|10|
user_id|int|兑换人用户ID
phone|string|兑换人手机号
begin_time|int|兑换开始时间
end_time|int|兑换结束时间



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 1,
        "page": 1,
        "limit": 10,
        "list": [
            {
                "id": 2,
                "user_id": 807720, // 兑换人用户ID
                "phone": "13127881017",
                "product": 1, // 兑换产品ID
                "product_name": "月度商机VIP", // 兑换产品名称
                "use_amount": 5, // 兑换使用的分享份额
                "remain_amount": 0, // 剩余可用的分享份额
                "exchange_time": 1569550326 // 兑换时间
            }
        ]
    }
}
```
</details>

### <a id="item_tieziguanli_670349000">帖子管理</a>



---

#### <a id="admin.post.list">API: 查询帖子列表</a>

**请求描述**

**GET**  admin/post/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
post_source|int|数据来源：`0`全部 `1`用户发布 `2`抓取数据
begin_time|int|帖子更新开始时间
end_time|int|帖子更新结束时间
post_type|int|帖子类型：`0`全部 `1`商品 `2`其他
device_type|int|发布渠道 `0`全部 `1`:web `2`:h5 `3`android `4`ios `5`小程序
publisher_type|int|发布者身份：`0`全部 `1`个人 `2`企业
id|int|帖子ID
nick_name|string|昵称/手机/邮箱/公司名称，四选一
phone|string|手机
company_name|string|公司名称
title|string|帖子标题，模糊匹配
club_name|string|圈子名称，模糊匹配



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 7906,
        "post_list": [
            {
                "id": 213508, 
                "user_id": 804472,
                "company_id": 1001150, // 企业/店铺ID
                "title": "测试111",
                "post_type": 1, // 信息类型 1商品 2帖子
                "price": 666,
                "quantity_unit": 1, // 单位 1：吨 2：千克 3：组 4：只
                "province_id": 17,
                "city_id": 104,
                "club_id": 0,
                "device_type": 4, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 0正常 1推荐
                "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1574133804,
                "created_time": 1574133804,
                "post_content_rtf": "<p>啦啦啦啦啦</p>", // 富文本内容
                "post_content_txt": "啦啦啦啦啦", // 纯文本内容
                "cover_pic": "https://test-imgqn.smm.cn/test/questioncenter/verify/image/RVRHF20191119112323.jpeg", // 封面
                "product_pic_set": "https://test-imgqn.smm.cn/test/questioncenter/verify/image/RVRHF20191119112323.jpeg", // 图片集合
                "admin_email": "",
                "top": 0, // 是否置顶 0否 1是
                "is_notice": 0, // 是否通知 0否 1是
                "refresh_time": 0, // 最后一次刷新时间
                "is_offer": 1, // 是否报价 0否 1是
                "pic_amount": 0, // 图片总数
                "is_crawl": 0, // 是否爬虫抓取 0否 1是
                "unit": "吨",
                "area": "",
                "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
                "reason": "", // 审核拒绝原因
                "approval_time": 1574133818, // 审核时间
                "approver_email": "test@smm.cn",
                "click_count": 8, // 点击量
                "sale_number": "长期供应", // 可售数量
                "valid_period": 1, // 有效期（天）
                "valid_period_time": 1574220218, // 有效期时间戳
                "category_id": 51, // 所属顶级分类ID
                "last_category_id": 54, // 所属分类
                "is_vip": 1, // 发布人是否会员 1是 2否
                "vip_type": 2, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "山东", // gps 省份
                "location_city": "济南市", // gps 城市
                "location_gps": "31.217117009737787,121.52968399980209", // GPS 经纬度
                "club_name": "",
                "category_name": "锡",
                "last_category_name": "锡化工"
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.post.settle.recommend">API: 设置推荐帖子</a>

**请求描述**

**POST**  admin/post/settle/recommend

**参数描述**

body:

名称|类型|描述
---|---|---
id|int|帖子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.post.cancel.recommend">API: 取消推荐帖子</a>

**请求描述**

**POST**  admin/post/cancel/recommend

**参数描述**

body:

名称|类型|描述
---|---|---
id|int|帖子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.post.delete">API: 删除帖子</a>

**请求描述**

**POST**  admin/post/delete

**参数描述**

body:

名称|类型|描述
---|---|---
id|int|要删除的帖子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.post.batch.delete">API: 批量删除帖子</a>

**请求描述**

**POST**  admin/post/batch/delete

**参数描述**

body:

名称|类型|描述
---|---|---
id|string|逗号分割的帖子ID，如：206407,206406



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.post.batch.migrate">API: 批量迁移帖子</a>

**请求描述**

**POST**  admin/post/batch/migrate

**参数描述**

body:

名称|类型|描述
---|---|---
id|string|逗号分割的帖子ID，如：206407,206406
club_id|int|迁移的目标圈子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.post.batch.refresh">API: 批量刷新</a>

**接口描述**

更新信息的修改时间

**请求描述**

**GET**  admin/post/batch/refresh

**参数描述**

query:

名称|类型|描述
---|---|---
id|string|逗号分割的帖子ID，如：206407,206406



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.post.global.refresh">API: 全局刷新</a>

**请求描述**

**GET**  admin/post/global/refresh

---

#### <a id="admin.post.approval.list">API: 获取待审核帖子列表</a>

**请求描述**

**GET**  admin/post/approval/list

**参数描述**

query:

名称|类型|描述
---|---|---
page|int|
limit|int|
approval_status|int|审核状态：`1`待审核 `2`审核通过 `3`审核拒绝
phone|string|用户中心手机号，模糊匹配
email|string|用户中心邮箱，模糊匹配
company_name|string|用户中心企业名称，模糊匹配
title|string|帖子标题，模糊匹配
post_type|int|帖子类型：`0`全部 `1`商品 `2`帖子
begin_time|int|帖子更新开始时间
end_time|int|帖子更新结束时间



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 11,
        "post_list": [
            {
                "id": 213508, 
                "user_id": 804472,
                "company_id": 1001150, // 企业/店铺ID
                "title": "测试111",
                "post_type": 1, // 信息类型 1商品 2帖子
                "price": 666,
                "quantity_unit": 1, // 单位 1：吨 2：千克 3：组 4：只
                "province_id": 17,
                "city_id": 104,
                "club_id": 0,
                "device_type": 4, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
                "is_recommend": 0, // 是否推荐 0正常 1推荐
                "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
                "updated_time": 1574133804,
                "created_time": 1574133804,
                "post_content_rtf": "<p>啦啦啦啦啦</p>", // 富文本内容
                "post_content_txt": "啦啦啦啦啦", // 纯文本内容
                "cover_pic": "https://test-imgqn.smm.cn/test/questioncenter/verify/image/RVRHF20191119112323.jpeg", // 封面
                "product_pic_set": "https://test-imgqn.smm.cn/test/questioncenter/verify/image/RVRHF20191119112323.jpeg", // 图片集合
                "admin_email": "",
                "top": 0, // 是否置顶 0否 1是
                "is_notice": 0, // 是否通知 0否 1是
                "refresh_time": 0, // 最后一次刷新时间
                "is_offer": 1, // 是否报价 0否 1是
                "pic_amount": 0, // 图片总数
                "is_crawl": 0, // 是否爬虫抓取 0否 1是
                "unit": "吨",
                "area": "",
                "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
                "reason": "", // 审核拒绝原因
                "approval_time": 1574133818, // 审核时间
                "approver_email": "test@smm.cn",
                "click_count": 8, // 点击量
                "sale_number": "长期供应", // 可售数量
                "valid_period": 1, // 有效期（天）
                "valid_period_time": 1574220218, // 有效期时间戳
                "category_id": 51, // 所属顶级分类ID
                "last_category_id": 54, // 所属分类
                "is_vip": 1, // 发布人是否会员 1是 2否
                "vip_type": 2, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
                "location_province": "山东", // gps 省份
                "location_city": "济南市", // gps 城市
                "location_gps": "31.217117009737787,121.52968399980209", // GPS 经纬度
                "cellphone": "13127881017",
                "email": "",
                "nickname": "toy",
                "company_name": "上海大宝剑有限公司"
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.post.batch.approval">API: 批量审核帖子</a>

**请求描述**

**POST**  admin/post/batch/approval

**参数描述**

body:

名称|类型|描述
---|---|---
approval_status|int|审核状态：只能为 `2`审核通过 或 `3`审核失败
reason|string|审核拒绝原因，失败必填
post_ids|string|逗号分割的帖子ID，如：1,2,3



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.post.save">API: 编辑帖子并审核通过</a>

**请求描述**

**POST**  admin/post/save

**参数描述**

body:

名称|类型|描述
---|---|---
post_id|int|信息ID
title|string|信息标题
post_type|int|信息类型：`1`商品 `2`帖子
device_type|int|发布渠道 `1`:web `2`:h5 `3`android `4`ios `5`小程序
city_id|int|城市ID
province_id|int|省份ID
product_pic_set|string|帖子图片链接集合，以逗号分割
cover_pic|string|帖子封面链接
price|float|价格
quantity_unit|int|单位：`1`：吨 `2`：千克 `3`：组 `4`：只
is_offer|int|是否报价  `0`议价 `1`是
pic_amount|int|帖子图片数量
sale_number|string|可售数量
valid_period|int| 有效期非VIP会员为`1`，会员可选 `1`、`7`、`30`、`90`



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.post.info.id">API: 查询帖子详情</a>

**请求描述**

**GET**  admin/post/info/:id

**参数描述**

path:

名称|类型|描述
---|---|---
id|int|帖子ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "post_info": {
            "id": 213389,
            "user_id": 807748, // 用户ID
            "company_id": 1001572, // 企业/店铺ID
            "title": "我这个账号是有企Q的哦",
            "post_type": 1, // 信息类型 1商品 2帖子
            "price": 0,
            "quantity_unit": 0, // 单位 1：吨 2：千克 3：组 4：只
            "province_id": 20,
            "city_id": 144,
            "club_id": 22,
            "device_type": 1, // 发布渠道 1:web 2:h5 3android 4ios 5小程序
            "is_recommend": 0, // 是否推荐 0正常 1推荐
            "status": 1, // 1正常 2用户删除 3圈主删除 4后台用户删除
            "updated_time": 1571905231,
            "created_time": 1571905231,
            "post_content_rtf": "", // 富文本内容
            "post_content_txt": "", // 纯文本内容
            "cover_pic": "https://test-imgqn.smm.cn/test/b/image/EYcjagsUSDUxKQvYfNlO20191024042026.jpg", // 封面
            "product_pic_set": "https://test-imgqn.smm.cn/test/b/image/kgeKsKmfakQBrFSjkLow20191024042026.jpg;https://test-imgqn.smm.cn/test/b/image/PVnORfRFEwGXPbiWlPFm20191024042026.jpg;https://test-imgqn.smm.cn/test/b/image/EYcjagsUSDUxKQvYfNlO20191024042026.jpg", // 图片集合
            "admin_email": "",
            "top": 0, // 是否置顶 0否 1是
            "is_notice": 0, // 是否通知 0否 1是
            "refresh_time": 0, // 最后一次刷新时间
            "is_offer": 0, // 是否报价 0否 1是
            "pic_amount": 3, // 图片总数
            "is_crawl": 0, // 是否爬虫抓取 0否 1是
            "unit": "",
            "area": "",
            "approval_status": 2, // 审核状态 1待审核 2审核成功 3拒绝
            "reason": "", // 审核拒绝原因
            "approval_time": 1571906970, // 审核时间
            "approver_email": "test@smm.cn",
            "click_count": 11, // 点击量
            "sale_number": "222", // 可售数量
            "valid_period": 100, // 有效期（天）
            "valid_period_time": 1582182175, // 有效期时间戳
            "category_id": 2, // 所属顶级分类ID
            "last_category_id": 8, // 所属分类
            "is_vip": 1, // 发布人是否会员 1是 2否
            "vip_type": 2, // 发布人会员类型 1月度 2年度 3体验 4季度 5半年
            "location_province": "", // gps 省份
            "location_city": "", // gps 城市
            "location_gps": "", // GPS 经纬度
            "navbar_name": "铜",
            "club_name": "电解铜",
            "province_name": "广西",
            "city_name": "桂林市",
            "user_info": { // 发布人名片
                "id": 64, // 名片ID
                "user_id": 807748,
                "is_public": 1,
                "card_url": "https://test-imgqn.smm.cn/test/club/user/cardcfLqK20191029145002.png",
                "avatar": "https://test-imgqn.smm.cn/test/usercenter/avatar/LBVmh20190625135010.jpeg",
                "real_name": "吴梦娜",
                "cellphone": "18512197032",
                "telephone": "18512154782",
                "company_type": "矿产商",
                "company_name": "测试贸易12134",
                "province_id": 18,
                "city_id": 0,
                "address": "峨山路",
                "position": "小职员",
                "main_product": "铜铝铅",
                "source_channel": 1,
                "admin_email": "olduser@smm.cn",
                "create_time": 1570863392,
                "update_time": 1573187590
            },
            "attribute": [ // 信息属性
                {
                    "attribute_id": 42,
                    "name": "正则",
                    "attr_type": 2, // 1单选 2文本
                    "attr_options": "^[A-Za-z0-9]+$", // 单选时为逗号分隔的选项 文本时为正则表达式
                    "attr_unit": "",
                    "attr_value": "22"
                }
            ],
            "company_name": "测试贸易12134",
            "vip_company_status": 2, // 店铺状态 0为开通 1过期 2服务中 3关闭
            "vip_company_status_desc": "服务中",
            "vip_year": 5, // 店铺服务年限
            "qidian_wpa_url": "http://q.url.cn/ABoDYP?_type=wpa&qidian=true", // 企点URL
            "category_name": "铜",
            "last_category_name": "电解铜"
        }
    }
}
```
</details>

### <a id="item_qita_670735000">其他</a>



---

#### <a id="admin.key_word_list">API: 获取关键词列表</a>

**请求描述**

**GET**  admin/key_word_list

**参数描述**

query:

名称|类型|描述
---|---|---
word_type|int|词类型 `1`:主词 `2`:相关词
name|string|产品名 模糊匹配
id|string|逗号分割的ID，如：1,2,3
begin_time|int|更新开始时间
end_time|int|更新结束时间
page|int|
limit|int|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "count": 61283,
        "key_word_list": [
            {
                "id": 64183,
                "name": "铈钨合金用途",
                "updated_time": 1562292865,
                "created_time": 1562292865,
                "admin_email": "liuzhenli@smm.cn",
                "word_type": 2 // 词性 1主词 2相关词
            }
        ]
    }
}
```
</details>

---

#### <a id="admin.product_words.delete">API: 删除关键词</a>

**请求描述**

**POST**  admin/product_words/delete

**参数描述**

body:

名称|类型|描述
---|---|---
id|string|逗号分隔的ID，如：1,2,3



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.recommend.user.setting">API: 设置商机首页推荐用户榜</a>

**接口描述**

最多设置10个用户

**请求描述**

**POST**  admin/recommend/user/setting

**参数描述**

body:

名称|类型|描述
---|---|---
user_ids|807720,804472|逗号分隔的用户ID，如：807720,804472



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": null
}
```
</details>

---

#### <a id="admin.recommend.user.ids">API: 获取商机首页推荐用户ID</a>

**接口描述**

最多返回10个推荐用户

**请求描述**

**GET**  admin/recommend/user/ids



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "user_ids": [
            807720,
            804472
        ]
    }
}
```
</details>

---

#### <a id="admin.upload.pic">API: 后台上传图片</a>

**请求描述**

**POST**  admin/upload/pic

**参数描述**

body:

名称|类型|描述
---|---|---
file|选择本地文件对象|文件对象
code_type|int|`800`：商机九图<br/>`801`：商机富文本图片<br/>`802`：用户上传企业背景图<br/>`803`：系统默认企业背景图<br/>`804`:   用户名片



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": "https://test-imgqn.smm.cn/test/club/post/rtf_picKhghf20191119174550.jpeg"
}
```
</details>

---

#### <a id="admin.approval.num.count">API: 获取商机各个模块审核数据总数</a>

**请求描述**

**GET**  admin/approval/num/count



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "post_count": 51, // 信息审核
        "card_count": 2, // 名片审核
        "pic_count": 6 // 图片审核
    }
}
```
</details>

### <a id="item_shujuxiufu_670850000">数据修复</a>



---

#### <a id="admin.usercard.init.old">API: 初始化所有老用户的名片</a>

**接口描述**

基本不用，主要是名片功能刚上线时用来生成之前的用户名片

**请求描述**

**GET**  admin/usercard/init/old

---

#### <a id="admin.navbar_label.transfer.category">API: 将导航和标签转换成分类</a>

**接口描述**

基本不用，主要用来将商机2.0上线前的导航和标签转换为分类，同时更新对应的信息至分类

**请求描述**

**GET**  admin/navbar_label/transfer/category

---

#### <a id="admin.generate.user_card_url">API: 生成所有名片图片为空的名片图片</a>

**接口描述**

将线上所有用户名片里的名片图片为空的用户名片生成系统名片图片

**请求描述**

**GET**  admin/generate/user_card_url

---

#### <a id="admin.import.smm_user">API: 导入商机用户名片</a>

**接口描述**

从excel里导入有色网的用户至商机的名片

excel格式（必须为xlsx格式，如果是其他格式，推荐打开后另存为xlsx格式）：

---|用户ID|姓名|手机|电话|企业类型|公司全称|省|市|地址|职位|行业|主营产品|是否公开
---|---|---|---|---|---|---|---|---|---|---|---|---|---
类型|int|string|string|string|string|string|int|int|string|string|string|string|string
描述|有色用户ID|   |   |   |必须以下之一:<br/> `贸易商`、`矿产商`、`冶炼企业`、`加工企业`、`生产企业`|   |商机省份ID|商机城市ID|   |   |商机行业ID，以英文逗号分割，如：1,2,3|   |二选一：`是`或`否`
参考值|807720|张三|13112345678|123456|贸易商|上海有色网信息科技股份有限公司|0|0|上海市浦东新区峨山路91弄20号|工程师|1,2,3|golang、web|否

以上表格代表excel中一行数据

**请求描述**

**POST**  admin/import/smm_user

**参数描述**

body:

名称|参考值|描述
---|---|---
file|选择本地文件对象|excel文件

---

#### <a id="admin">API: 例子</a>

**请求描述**

**GET**  admin

### <a id="item_neiwangjiekou_671436000">内网接口</a>



---

#### <a id="vip.pay_success">API: 购买会员成功回调</a>

**请求描述**

**GET**  vip/pay_success

**参数描述**

query:

名称|类型|描述
---|---|---
user_id|int|用户ID
order_no|string|有色订单号
price_type|int|购买类型：`1`月度 `2`年度 `3`体验 `4`季度 `5`半年



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "begin_time": "2020-03-30 00:00:00", // 购买服务的开始时间
        "end_time": "2020-04-29 00:00:00" // 购买服务的结束时间
    }
}
```
</details>

---

#### <a id="share.reg">API: 用户从分享连接注册回调</a>

**请求描述**

**GET**  share/reg

**参数描述**

query:

名称|类型|描述
---|---|---
user_id|int|使用分享连接的用户
share_user_id|int|分享人用户ID



<details>
<summary>响应描述</summary>

```json
{
    "code": 10150,
    "msg": "已占用分享名额",
    "data": null
}
```
</details>

---

#### <a id="coupon.use">API: 使用优惠券兑换商机会员</a>

**请求描述**

**GET**  coupon/use

**参数描述**

query:

名称|类型|描述
---|---|---
user_id|int|用户ID
price_type|int|兑换的会员类型：`1`月度 `2`年度 `3`体验 `4`季度 `5`半年



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "操作成功",
    "data": {
        "begin_time": "2020-04-29 00:00:00", // 会员服务开始时间
        "end_time": "2020-05-29 00:00:00" // 会员服务结束时间
    }
}
```
</details>

### <a id="item_diaoyongqitafuwujiekou_671604000">调用其他服务接口</a>



---

#### <a id="usercenter.inner.get_paged_company_list">API: [用户中心]查询企业列表/usercenter/inner/get_paged_company_list</a>

**请求描述**

**GET**  usercenter/inner/get_paged_company_list

**参数描述**

query:

名称|参考值|描述
---|---|---
value|1001150,1001246,1001408,1001530,1001572,1001616,1001618,1001625,1001627,1001628,1001629,1001715,1001717,1001719,1001720,1001721,1001722,1001726,1001738,1001748,1001764,1001768,1001774,1001776,1001817,1001840,1001849|
field|company_ids|
page|1|
page_item_count|3|

---

#### <a id="usercenter.inner.get_filter_user_and_company_list">API: [用户中心]获取用户信息/usercenter/inner/get_filter_user_and_company_list</a>

**请求描述**

**GET**  usercenter/inner/get_filter_user_and_company_list

**参数描述**

query:

名称|参考值|描述
---|---|---
field|member_name|user_ids逗号分隔的用户id 
company_name 公司名称
real_name姓名 
nickname昵称 
member_name手机/邮箱/用户名
value|10020180409|    

---

#### <a id="get_flow_view_count">API: 大数据首页今日访客/get_flow_view_count</a>

**请求描述**

**GET**  get_flow_view_count

---

#### <a id="usercenter.inner.get_company_detail">API: [用户中心]获取企业详情</a>

**请求描述**

**GET**  usercenter/inner/get_company_detail

**参数描述**

query:

名称|参考值|描述
---|---|---
company_id|1001572|

---

#### <a id="qidiancenter.get_users">API: 获取企点用户/qidiancenter/get_users?user_ids=804792</a>

**请求描述**

**GET**  qidiancenter/get_users

**参数描述**

query:

名称|参考值|描述
---|---|---
user_ids|804792,804472|

---

#### <a id="inner.cards.list">API: 分页获取通讯录</a>

**接口描述**

http://testplatform.smm.cn:6167


http://127.0.0.1:8009

**请求描述**

**GET**  inner/cards/list

**参数描述**

query:

名称|类型|描述
---|---|---
user_id|720582|
page|1|
limit|10|
keyword|131515|手机号/电话号/姓名



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "成功",
    "data": {
        "list": [
            {
                "id": 3468693971,
                "name": "Apple",
                "cover_img": "",
                "job": "支支吾吾道问我为什么要这么摄影艺术十一五、一样一样是因为自己而努力",
                "company": "在一起就是这样一件事情就是说是呵呵呵呵呵呵呵呵呵嘿日日日日日",
                "profession": "冶金冶炼|五金|采掘不锈钢/铝合金/金属制品",
                "cellphone": "131515",
                "telephone": "244212",
                "group_id": 0,
                "group_name": "未分组",
                "create_time": 1543216878
            }
        ],
        "count": 1,
        "page": 1,
        "limit": 10
    }
}
```
</details>

---

#### <a id="inner.user_share_url">API: 用户通讯录名片</a>

**请求描述**

**GET**  inner/user_share_url

**参数描述**

query:

名称|参考值|描述
---|---|---
user_id|1108148|

---

#### <a id="vcodecenter.inner.v3.send_csy_sms">API: 邀请用户加入有色名片短信vcode_center</a>

**请求描述**

**POST**  vcodecenter/inner/v3/send_csy_sms

**参数描述**

body:

名称|参考值|描述
---|---|---
cellphone|13127881017|
content|张新杰邀请您使用 有色电子名片 点击 https://t.smm.cn/1234324 了解|
app_key|d73adf67f82d5ad81e37e218814aa44e|

---

#### <a id="vcodecenter.inner.v3.check_validate_common">API: 云盾校验</a>

**请求描述**

**GET**  vcodecenter/inner/v3/check_validate_common

**参数描述**

query:

名称|参考值|描述
---|---|---
app_name|club_center|
bind_id|807720|
validate|jsdklfjkl|
captcha_id|61231j2k31230|

---

#### <a id="BCRService.BCR_Crop">API: 名片全能王</a>

**请求描述**

**POST**  BCRService/BCR_Crop

**参数描述**

query:

名称|参考值|描述
---|---|---
PIN|sdafasdfsadf|
user|buoren@smm.cn|
pass|JGNWBDQRGWDWJPSP|
json|0|
lang|15|
size|59109|

body:

名称|参考值|描述
---|---|---
upfile|选择本地文件对象|

---

#### <a id="vcodecenter.inner.v3.get_notify_sms_send_log">API: 查询短信发送记录</a>

**请求描述**

**GET**  vcodecenter/inner/v3/get_notify_sms_send_log

**参数描述**

query:

名称|类型|描述
---|---|---
cellphone|13127881017|
page|1|
limit|2|
code_type|mingpian_msg_notify|



<details>
<summary>响应描述</summary>

```json
{
    "code": 0,
    "msg": "",
    "data": {
        "count": 1,
        "result": [
            {
                "Id": 23544,
                "Ip": "182.254.211.181",
                "Cellphone": "86-13127881017",
                "CodeType": "mingpian_msg_notify",
                "TemplateId": "478848",
                "Status": 1, // 1发送成功 2发送失败
                "Args": "[\"张三在有色商机\",\"：交换电子名片... \",\" t.smm.cn/090SAJL2 \"]",
                "Remark": "",
                "Channel": "ytx",
                "CreateTime": "2019-11-04T10:59:01+08:00"
            }
        ]
    }
}
```
</details>

---

#### <a id="BCRService.BCR_VCF2">API: 名片全能王</a>

**请求描述**

**POST**  BCRService/BCR_VCF2

**参数描述**

query:

名称|参考值|描述
---|---|---
PIN|sdafasdfsadf|
user|buoren@smm.cn|
pass|JGNWBDQRGWDWJPSP|
json|0|
lang|15|
size|59109|

body:

名称|参考值|描述
---|---|---
upfile|选择本地文件对象|

---

#### <a id="inner.comment.count">API: 获取用户评论总数</a>

**请求描述**

**GET**  inner/comment/count

**参数描述**

query:

名称|参考值|描述
---|---|---
topic_type|club-comment|
topic_id||
user_id|807720|
only_comment||

