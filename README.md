# 页面制作
按照以下需求完成页面制作，制作完成后将项目压缩为zip发送至邮箱 chao.zhang@hibobi.com

## 需求说明
**1.顶通模块**
内容文案固定为包邮门槛信息

**2.banner模块**
根据数据展示banner图

**3.类目推荐**
横滑展示第二页，配置要求不少于8个，第二页不足8个上下展示，右方可以空白；
此模块必配标题，模块标题为图片

**4.一行一个广告位-1**
此模块可以连续展示多个图片，模块标题为图片；
**5.Flashsale商品**

此模块标题固定，倒计时由数据提供，商品列表可横滑。商品模块包含商品图片，商品标签（商品折扣），商品价格，商品售卖进度条
**6.商品集合**

此模块由标题，资源位，商品集合组成；模块标题为图片资源位为图片，商品集合可横滑；商品模块包含商品图片,商品标签（商品折扣），商品价格；
**7.商品推荐**

此模块由标题，商品组成，模块标题传图；商品模块从左到又展示，为卡片模式，商品模块包含商品图片，商品标签（商品折扣），商品价格

## 设计稿
![SketchCoverdf37d207699283b2c635735734dba87247a74d3f598e9df40078746c7bbf113e](https://user-images.githubusercontent.com/38548417/121689607-60851780-caf7-11eb-943c-8680f5206d15.png)

## 设计稿模块说明
![0](https://user-images.githubusercontent.com/38548417/121689942-d2f5f780-caf7-11eb-8dcc-d4e59f437cc8.png)

## mock数据  
``` json
字段说明： 
type: 2-> banner；3:->类目推荐;4:->一行一个广告位-1;5->Flashsale商品;6->商品集合;7->商品推荐
title: { // 标题对象
  title: ''， // 图片title
  url: '' // 图片链接
}
"content":[ // 资源位数据
  {
     "title":"", // 图片title
     "url":"", // 图片链接
     "link":"" // 跳转链接
   }
]
 "goods":[
    {
      "id":84,
      "good_en_title":"",
      "name":"",
      "img":"", // 图片地址
      "img_type":1, // 图片类型
      "origin_price":0, // 原售价
      "price":0, // 现售价
      "stock":836,  // 
      "percentage":28, // 进度条
      "discount":"50%", // 折扣力度
      "good_label":"",
      "label":1, // 标签类型
      "new_label":0, // 大于0展示折扣标签
      "left_num":0,
      "is_activity":0,
      "is_single_activity":0
    }
]


{

        "activities": [
            {
                "type":2,
                "title":{
                    "title":"Comprar Por Categoría",
                    "url":"https://images.hibobi.com/product/000051/home_cards/1622547939668cYp7ZzM4ErHiDMpsEmh.png"
},
                "content":[
                    {
                        "title":"Hasta -70%",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319365366XxYHwzTSKQJHc4J7fmS.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2781-relate.html"
                    }
                ]
               
            },
            {
                "type":3,
                "title":{
                    "title":"Shop by Categories",
                    "url":"https://images.hibobi.com/product/000051/home_cards/1623322325259TFsQhawreyi4ZYc8iZd.png"
             
                },
              
                "content":[
                    {
                        "title":"Jumpsuits",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319466736f8QzE8MEzffyCPNErNJ.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2722-relate.html"
                    },
                    {
                        "title":"Sets",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319475521ddXr2dzdrBeheJhFYKa.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2684-relate.html"
                    },
                    {
                        "title":"Dresses",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319484388NksWcBcimHEzXSbRSAx.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2685-relate.html"
                    },
                    {
                        "title":"Pajamas",
                        "url":"https://images.hibobi.com/product/000051/home_cards/16233194892564EiDeKQpt7xGMMFweF2.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2688-relate.html"
                    },
                    {
                        "title":"Accessories",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319493874DAiZXDebHnXt4tdGsAy.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2706-relate.html"
                    },
                    {
                        "title":"Mumz",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319498080HeMPcKcCi2tY4bQSnZN.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2723-relate.html"
                    },
                    {
                        "title":"Shoes",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319503378hWKdAYpTJ3eHtiGscJA.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2707-relate.html"
                    },
                    {
                        "title":"Baby Supplies",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319507832DrMHcJwkFcsfWrkDPNX.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2724-relate.html"
                    },
                    {
                        "title":"Floral",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319586126i36aJtHYF4PEnKKWx4s.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-1443-relate.html"
                    },
                    {
                        "title":"Letters",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319595115HBH3hWDZXZYzD6A3328.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-1446-relate.html"
                    },
                    {
                        "title":"Stripe",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319599685ztkzQMpwNeJpfEsS4ap.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2744-relate.html"
                    },
                    {
                        "title":"Polka Dot",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319605422yiJSfmG2WW2aR7snfpD.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-1448-relate.html"
                    },
                    {
                        "title":"Animal",
                        "url":"https://images.hibobi.com/product/000051/home_cards/16233196122672rGJsS4NQsRxm4Y3a85.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-1444-relate.html"
                    },
                    {
                        "title":"Plaid",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319620528BNhA7jDZ8dBGEPBAzi2.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-1447-relate.html"
                    },
                    {
                        "title":"Cartoon",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319625692BGYzc7X47S8tdQYWPC3.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2745-relate.html"
                    },
                    {
                        "title":"Camouflage",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319629726sSsrs5bdWF5MEm36tpB.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-1445-relate.html"
                    }
                ],
                "more":{

                }
            },
            {
                "type":4,
                "title":{
                    "title":"Venta de Hibobi",
                    "url":"https://images.hibobi.com/product/000051/home_cards/16233223425762tezT7wcsK27X5aJbJd.png"
           
                },
               
                "content":[
                    {
                        "title":"Verano Afrutado",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319672025wNcn4CcdGCyBwkHrJC2.png",
                        "link":"https://m.hibobi.com/activity/activity_title?activity_id=789"
                    },
                    {
                        "title":"Romántico todo el verano",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319676444F3XKa72F6tjGeHQRczb.png",
                        "link":"https://m.hibobi.com/activity/activity_title?activity_id=788"
                    },
                    {
                        "title":"Great Sale",
                        "url":"https://images.hibobi.com/product/000051/home_cards/16233324514317Pr3YzzXKBGJ4EMJYsi.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2642-relate.html"
                    }
                ]
               
            },
            {
                "type":5,
                "title":{
                
                    "countdown":70734,
                    "link":"https://m.hibobi.com/activity/dailylimited"
                },
                "goods":[
                    {
                        "id":84,
                        "good_en_title":"3-piece Floral Printed Jumpsuit with Headband & Hat for Baby Girl",
                        "name":"3-piece Floral Printed Jumpsuit with Headband & Hat for Baby Girl",
                        "img":"https://images.hibobi.com/products/000032000063/e88d8c62-b44d-4ce5-ad7a-9cd18f556e27.JPG",
                        "img_type":1,
                        "origin_price":235.4,
                        "price":117.7,
                        "stock":836,
                        "percentage":28,
                        "discount":"50%",
                        "good_label":"",
                        "label":1,
                        "new_label":5,
                        "left_num":48,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":192392,
                        "good_en_title":"Toddler Girl Letter Print T-shirt & Suspender Shorts",
                        "name":"Toddler Girl Letter Print T-shirt & Suspender Shorts",
                        "img":"https://images.hibobi.com/supply/products/000291001456/5a4f8580-f4c9-03d1-3ee8-18cd03c8da53.jpeg",
                        "img_type":1,
                        "origin_price":306.24,
                        "price":238.87,
                        "stock":772,
                        "percentage":0,
                        "discount":"22%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":20,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":177398,
                        "good_en_title":"Cotton Animal Socks for Children's",
                        "name":"Cotton Animal Socks for Children's",
                        "img":"https://images.hibobi.com/supply/products/000182000423/348b32fd-4d77-810c-9378-ed933a7c3a07.jpeg",
                        "img_type":1,
                        "origin_price":207.02,
                        "price":31.05,
                        "stock":38,
                        "percentage":0,
                        "discount":"85%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":10,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":180170,
                        "good_en_title":"Baby Boy Cute Pattern Pajamas Sets",
                        "name":"Baby Boy Cute Pattern Pajamas Sets",
                        "img":"https://images.hibobi.com/supply/products/000709002685/62ae735e-43f6-7fbf-4171-f5eaf077ea76.jpeg",
                        "img_type":1,
                        "origin_price":256.08,
                        "price":128.04,
                        "stock":1427,
                        "percentage":0,
                        "discount":"50%",
                        "good_label":"",
                        "label":1,
                        "new_label":5,
                        "left_num":30,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":182282,
                        "good_en_title":"Toddler Girl Small Buds Print Dress & Straw Hat",
                        "name":"Toddler Girl Small Buds Print Dress & Straw Hat",
                        "img":"https://images.hibobi.com/supply/products/000673000125/d966bb55-5a75-6526-347c-b801a625b70a.jpeg",
                        "img_type":1,
                        "origin_price":267.96,
                        "price":209.01,
                        "stock":4258,
                        "percentage":0,
                        "discount":"22%",
                        "good_label":"https://images.hibobi.com/product/000177/promotions/1623227165618e5a3xCJhfkJzssN8ztc.png",
                        "label":1,
                        "new_label":4,
                        "left_num":50,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{
                            "id":788,
                            "activity_type":"discount",
                            "role":"BUY 2 GET 20% OFF",
                            "en_role":"BUY 2 GET 20% OFF",
                            "role_new":[
                                " Buy 2 Get 20% Off "
                            ],
                            "en_role_new":[
                                " Buy 2 Get 20% Off "
                            ],
                            "title":" Buy 2 Get 20% Off ",
                            "start_at":"2021-06-10 09:00:00",
                            "end_at":"2021-06-17 08:59:59",
                            "is_website":0
                        }
                    },
                    {
                        "id":193107,
                        "good_en_title":"Children Bow Decor Metal Frame Sunglasses",
                        "name":"Children Bow Decor Metal Frame Sunglasses",
                        "img":"https://images.hibobi.com/supply/products/000182000577/94f31d67-1241-aa34-9fca-598a6568797d.jpeg",
                        "img_type":1,
                        "origin_price":227.7,
                        "price":79.7,
                        "stock":389,
                        "percentage":0,
                        "discount":"65%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":20,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":192454,
                        "good_en_title":"Baby Cartoon Animal Pattern Jumpsuit",
                        "name":"Baby Cartoon Animal Pattern Jumpsuit",
                        "img":"https://images.hibobi.com/supply/products/000205000981/854eafcf-5631-7674-863b-2a82bfa43e8f.jpeg",
                        "img_type":1,
                        "origin_price":276.32,
                        "price":221.06,
                        "stock":959,
                        "percentage":0,
                        "discount":"20%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":20,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":185341,
                        "good_en_title":"Toddler Boy Cartoon Pattern T-Shirt & Shorts",
                        "name":"Toddler Boy Cartoon Pattern T-Shirt & Shorts",
                        "img":"https://images.hibobi.com/supply/products/000709003103/797a4f4e-3093-d717-a7a7-7c13ed202618.jpeg",
                        "img_type":1,
                        "origin_price":236.5,
                        "price":118.25,
                        "stock":11,
                        "percentage":0,
                        "discount":"50%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":11,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":169192,
                        "good_en_title":"Plaid Dress for Girl",
                        "name":"Plaid Dress for Girl",
                        "img":"https://images.hibobi.com/supply/products/000414000252/e1fd9525-32aa-0135-225f-2b0f84aba478.jpeg",
                        "img_type":1,
                        "origin_price":390.28,
                        "price":214.65,
                        "stock":5,
                        "percentage":0,
                        "discount":"45%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":5,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":193043,
                        "good_en_title":"Baby Girl Ruffle Sleeve Leopard Print Bodysuit & Bow Decor Shorts & Headband",
                        "name":"Baby Girl Ruffle Sleeve Leopard Print Bodysuit & Bow Decor Shorts & Headband",
                        "img":"https://images.hibobi.com/supply/products/000198000538/a05f0661-41c3-a4e3-7458-c770ca9e5169.jpeg",
                        "img_type":1,
                        "origin_price":258.72,
                        "price":232.85,
                        "stock":173,
                        "percentage":0,
                        "discount":"10%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":20,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":143942,
                        "good_en_title":"2 Pieces Basketball Tank & Shorts for Toddler Boy",
                        "name":"2 Pieces Basketball Tank & Shorts for Toddler Boy",
                        "img":"https://images.hibobi.com/supply/products/000385000050/2967682d-e2f4-de35-4c29-5c0641e224d7.jpeg",
                        "img_type":1,
                        "origin_price":260.26,
                        "price":143.14,
                        "stock":14938,
                        "percentage":28,
                        "discount":"45%",
                        "good_label":"",
                        "label":1,
                        "new_label":5,
                        "left_num":48,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":166118,
                        "good_en_title":"2-piece Wings Pattern Hoodie & Pants for Boy",
                        "name":"2-piece Wings Pattern Hoodie & Pants for Boy",
                        "img":"https://images.hibobi.com/supply/products/000365000705/b0ed3bf8-88e0-decb-8e34-3f32dbb7afa9.jpeg",
                        "img_type":1,
                        "origin_price":496.76,
                        "price":372.57,
                        "stock":11,
                        "percentage":0,
                        "discount":"25%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":10,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":178421,
                        "good_en_title":"3-piece Bodysuit for Baby Girl",
                        "name":"3-piece Bodysuit for Baby Girl",
                        "img":"https://images.hibobi.com/products/000077/1e109907-5e4e-4a43-981d-3e54a7ed8063.jpg",
                        "img_type":1,
                        "origin_price":254.32,
                        "price":127.16,
                        "stock":7,
                        "percentage":0,
                        "discount":"50%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":7,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":193029,
                        "good_en_title":"Toddler Girl Cartoon Figure Pattern Letter Print T-shirt & Leopard Pants",
                        "name":"Toddler Girl Cartoon Figure Pattern Letter Print T-shirt & Leopard Pants",
                        "img":"https://images.hibobi.com/supply/products/000198000535/6525a251-3d12-3369-b55a-7959548a7413.jpeg",
                        "img_type":1,
                        "origin_price":297.66,
                        "price":238.13,
                        "stock":471,
                        "percentage":0,
                        "discount":"20%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":20,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":192561,
                        "good_en_title":"Girl Polka Dot Layered Cami Top & Pants",
                        "name":"Girl Polka Dot Layered Cami Top & Pants",
                        "img":"https://images.hibobi.com/supply/products/000704000077/77036c51-2768-ffb1-a9ad-b5a313976fc8.jpeg",
                        "img_type":1,
                        "origin_price":372.68,
                        "price":298.14,
                        "stock":286,
                        "percentage":0,
                        "discount":"20%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":20,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":152185,
                        "good_en_title":"Bow Decor Toddler Shoes for Baby Girl",
                        "name":"Bow Decor Toddler Shoes for Baby Girl",
                        "img":"https://images.hibobi.com/supply/products/000392000284/a9a1c7c9-c5b2-f53d-ec58-f9a358645bf7.jpeg",
                        "img_type":1,
                        "origin_price":254.32,
                        "price":76.3,
                        "stock":7,
                        "percentage":0,
                        "discount":"70%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":7,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":179752,
                        "good_en_title":"Toddler Boy Big Pocket Sweatshirt & Pants",
                        "name":"Toddler Boy Big Pocket Sweatshirt & Pants",
                        "img":"https://images.hibobi.com/products/000068/36aa6650-fc84-46e1-a640-e2031359921d.JPG",
                        "img_type":1,
                        "origin_price":423.06,
                        "price":169.22,
                        "stock":6,
                        "percentage":51,
                        "discount":"60%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":6,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":182122,
                        "good_en_title":"Girl Tendon Off-shoulder Skirt",
                        "name":"Girl Tendon Off-shoulder Skirt",
                        "img":"https://images.hibobi.com/supply/products/000411000203/dddf3ba6-1c52-02f4-30d8-6ddb0d5cf521.jpeg",
                        "img_type":1,
                        "origin_price":396.66,
                        "price":337.16,
                        "stock":2357,
                        "percentage":0,
                        "discount":"15%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":50,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":169409,
                        "good_en_title":"Dinosaur Pattern Jumpsuit for Baby Boy",
                        "name":"Dinosaur Pattern Jumpsuit for Baby Boy",
                        "img":"https://images.hibobi.com/supply/products/000360002642/5bab28df-fdd4-c87c-aad9-76a6a42d4db6.jpeg",
                        "img_type":1,
                        "origin_price":283.36,
                        "price":99.18,
                        "stock":14,
                        "percentage":0,
                        "discount":"65%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":14,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":171775,
                        "good_en_title":"Floral Printed Dress for Toddler Girl",
                        "name":"Floral Printed Dress for Toddler Girl",
                        "img":"https://images.hibobi.com/supply/products/000360002387/7cb4ed65-786c-9e1c-f941-cf0055915538.jpeg",
                        "img_type":1,
                        "origin_price":342.98,
                        "price":137.19,
                        "stock":7,
                        "percentage":0,
                        "discount":"60%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":7,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":176581,
                        "good_en_title":"Letter Pattern Long Sleeve T-shirt for Boy",
                        "name":"Letter Pattern Long Sleeve T-shirt for Boy",
                        "img":"https://images.hibobi.com/supply/products/000041000471/db3b7dd4-7133-96a6-3f68-77e3bfdc1cdb.jpeg",
                        "img_type":1,
                        "origin_price":283.36,
                        "price":240.86,
                        "stock":10,
                        "percentage":0,
                        "discount":"15%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":10,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":182366,
                        "good_en_title":"Solid Short-sleeve Nursing Top",
                        "name":"Solid Short-sleeve Nursing Top",
                        "img":"https://images.hibobi.com/supply/products/000693000033/a14fc46c-dec8-2602-89e1-ccfc391b0651.jpeg",
                        "img_type":1,
                        "origin_price":319.44,
                        "price":127.78,
                        "stock":13,
                        "percentage":0,
                        "discount":"60%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":13,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":179421,
                        "good_en_title":"Toddler Boy Sneakers",
                        "name":"Toddler Boy Sneakers",
                        "img":"https://images.hibobi.com/supply/products/000402000282/81392189-e1c9-f824-e764-ddb2ebb0416e.jpeg",
                        "img_type":1,
                        "origin_price":408.98,
                        "price":204.49,
                        "stock":13,
                        "percentage":0,
                        "discount":"50%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":13,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":188325,
                        "good_en_title":"Baby Girl Ribbed Skirt",
                        "name":"Baby Girl Ribbed Skirt",
                        "img":"https://images.hibobi.com/supply/products/000479000594/0348a678-45ba-e1cc-5db6-9eaf15cc7f39.jpeg",
                        "img_type":1,
                        "origin_price":189.86,
                        "price":151.89,
                        "stock":3115,
                        "percentage":0,
                        "discount":"20%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":30,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":183517,
                        "good_en_title":"Toddler Girl Flying Sleeve Rainbow Striped Dress",
                        "name":"Toddler Girl Flying Sleeve Rainbow Striped Dress",
                        "img":"https://images.hibobi.com/supply/products/000481000439/b12fa8ee-16ae-3b4c-53f8-605785826f12.jpeg",
                        "img_type":1,
                        "origin_price":208.12,
                        "price":124.87,
                        "stock":12,
                        "percentage":0,
                        "discount":"40%",
                        "good_label":"",
                        "label":1,
                        "new_label":4,
                        "left_num":12,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    }
                ],
                "content":[

                ]
            },
            {
                "type":9,
                "title":{
                    "title":"Estilo de Hibobi",
                    "url":"https://images.hibobi.com/product/000051/home_cards/1623322370624Jk2dTathbwThtpjZPEm.png",
                    "link":""
                },
                "goods":[
                    {
                        "id":110379,
                        "good_en_title":"Baby's Fruit Print Long Sleeve Romper With Headband",
                        "name":"Baby's Fruit Print Long Sleeve Romper With Headband",
                        "img":"https://images.hibobi.com/supply/products/000222000034/97e807f1-f59b-1d26-0f80-5eb3a863e370.jpeg",
                        "img_type":"",
                        "origin_price":725.78,
                        "price":423.06,
                        "stock":5539,
                        "percentage":0,
                        "discount":"42%",
                        "good_label":"",
                        "label":0,
                        "new_label":0,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":0,
                        "promotion":{

                        }
                    },
                    {
                        "id":138740,
                        "good_en_title":"2-piece Lace Lapel Collar & Dungarees for Baby Girl",
                        "name":"2-piece Lace Lapel Collar & Dungarees for Baby Girl",
                        "img":"https://images.hibobi.com/supply/products/000226000229/b28b1cec-c209-01d6-df90-cb4d571c81ff.jpeg",
                        "img_type":"",
                        "origin_price":505.78,
                        "price":263.34,
                        "stock":4188,
                        "percentage":0,
                        "discount":"48%",
                        "good_label":"",
                        "label":0,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":0,
                        "promotion":{

                        }
                    },
                    {
                        "id":145759,
                        "good_en_title":"2-piece Bow Decor Striped Bodysuit & Headband for Baby Girl",
                        "name":"2-piece Bow Decor Striped Bodysuit & Headband for Baby Girl",
                        "img":"https://images.hibobi.com/supply/products/000213000445/ac5b6eb2-0f06-79ac-d75a-1d151e69b138.jpeg",
                        "img_type":"",
                        "origin_price":0,
                        "price":295.68,
                        "stock":1432,
                        "percentage":0,
                        "discount":0,
                        "good_label":"https://images.hibobi.com/product/000130/promotions/162328918332962EQZkwbwAyshr7WJK8.png",
                        "label":0,
                        "new_label":0,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":0,
                        "promotion":{
                            "id":789,
                            "activity_type":"discount",
                            "role":"BUY 3 GET 25% OFF",
                            "en_role":"BUY 3 GET 25% OFF",
                            "role_new":[
                                " Buy 3 Get 25% Off "
                            ],
                            "en_role_new":[
                                " Buy 3 Get 25% Off "
                            ],
                            "title":" Buy 3 Get 25% Off ",
                            "start_at":"2021-06-10 09:00:00",
                            "end_at":"2021-06-17 08:59:59",
                            "is_website":0
                        }
                    },
                    {
                        "id":156666,
                        "good_en_title":"Solid Ruffle Jumpsuit for Baby Girl",
                        "name":"Solid Ruffle Jumpsuit for Baby Girl",
                        "img":"https://images.hibobi.com/supply/products/000396000479/da8b2b11-a1ea-27ad-2b72-51dc90bf950f.jpeg",
                        "img_type":"",
                        "origin_price":0,
                        "price":221.1,
                        "stock":2796,
                        "percentage":0,
                        "discount":0,
                        "good_label":"",
                        "label":0,
                        "new_label":0,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":0,
                        "promotion":{

                        }
                    },
                    {
                        "id":175960,
                        "good_en_title":"3-piece Ruffle Romper & Headband & Pants for Baby Girl",
                        "name":"3-piece Ruffle Romper & Headband & Pants for Baby Girl",
                        "img":"https://images.hibobi.com/supply/products/000519000075/facad0f2-9abd-5d9b-8f2e-2b4fded5132c.jpeg",
                        "img_type":"",
                        "origin_price":0,
                        "price":337.04,
                        "stock":44264,
                        "percentage":0,
                        "discount":0,
                        "good_label":"",
                        "label":0,
                        "new_label":0,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":0,
                        "promotion":{

                        }
                    },
                    {
                        "id":179371,
                        "good_en_title":"3-piece Romper & Headband & Shorts for Baby Girl",
                        "name":"3-piece Romper & Headband & Shorts for Baby Girl",
                        "img":"https://images.hibobi.com/supply/products/000198000438/5571df44-326f-be6a-5d58-651f901d7471.jpeg",
                        "img_type":"",
                        "origin_price":0,
                        "price":210.54,
                        "stock":1063,
                        "percentage":0,
                        "discount":0,
                        "good_label":"",
                        "label":0,
                        "new_label":0,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":0,
                        "promotion":{

                        }
                    },
                    {
                        "id":184690,
                        "good_en_title":"Baby Girl Daisy Print Bodysuit & Headband",
                        "name":"Baby Girl Daisy Print Bodysuit & Headband",
                        "img":"https://images.hibobi.com/supply/products/000416000048/c030f113-a88b-d847-69b9-4fd63e23494f.jpeg",
                        "img_type":"",
                        "origin_price":0,
                        "price":214.28,
                        "stock":2509,
                        "percentage":0,
                        "discount":0,
                        "good_label":"",
                        "label":0,
                        "new_label":0,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":0,
                        "promotion":{

                        }
                    },
                    {
                        "id":185918,
                        "good_en_title":"Baby Girl Floral Pattern Sling Swimsuit & Swimming Trunks",
                        "name":"Baby Girl Floral Pattern Sling Swimsuit & Swimming Trunks",
                        "img":"https://images.hibobi.com/supply/products/000452000505/838031e8-573b-d33c-250e-3aa29029a27d.jpeg",
                        "img_type":"",
                        "origin_price":283.8,
                        "price":184.47,
                        "stock":116,
                        "percentage":0,
                        "discount":"35%",
                        "good_label":"",
                        "label":2,
                        "new_label":2,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":186320,
                        "good_en_title":"Baby Girl Mermaid Bodysuit & Headband",
                        "name":"Baby Girl Mermaid Bodysuit & Headband",
                        "img":"https://images.hibobi.com/supply/products/000202000274/e9c9e539-08b5-3dc5-cfca-a0c001baf4c7.jpeg",
                        "img_type":"",
                        "origin_price":271.7,
                        "price":217.36,
                        "stock":17812,
                        "percentage":0,
                        "discount":"20%",
                        "good_label":"",
                        "label":2,
                        "new_label":2,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":186821,
                        "good_en_title":"Baby Girl Leopard Print T-shirt & Pants & Bowknot Headband",
                        "name":"Baby Girl Leopard Print T-shirt & Pants & Bowknot Headband",
                        "img":"https://images.hibobi.com/supply/products/000209000038/b33327d7-04d0-02f6-77e8-4bea94dce73a.jpeg",
                        "img_type":"",
                        "origin_price":0,
                        "price":254.32,
                        "stock":99914,
                        "percentage":0,
                        "discount":0,
                        "good_label":"",
                        "label":0,
                        "new_label":0,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":0,
                        "promotion":{

                        }
                    }
                ],
                "content":[
                    {
                        "title":"",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319758225TDTBTCPWcPAPYYTn4FA.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2807-relate.html"
                    }
                ],
                "more":{
                    "title":"",
                    "url":"",
                    "link":"https://m.hibobi.com/categories/Sport-Cate-2807-relate.html"
                }
            },
            {
                "type":9,
                "title":{
                    "title":"Estilo de Hibobi",
                    "url":"https://images.hibobi.com/product/000051/home_cards/1623322381829ttfWarZ2MAPJ2QNmEEs.png",
                    "link":""
                },
                "goods":[
                    {
                        "id":119364,
                        "good_en_title":"2-piece Color Contrast Pullover & Pants for Toddler Boy",
                        "name":"2-piece Color Contrast Pullover & Pants for Toddler Boy",
                        "img":"https://images.hibobi.com/supply/products/000186000021/a3b3d53a-c579-15f2-98b4-8bf3c874275a.jpeg",
                        "img_type":"",
                        "origin_price":348.92,
                        "price":279.14,
                        "stock":6952,
                        "percentage":0,
                        "discount":"20%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":124199,
                        "good_en_title":"3-piece Floral Printed Hooded Coat & Sweatshirts & Pants for Toddler Boy",
                        "name":"3-piece Floral Printed Hooded Coat & Sweatshirts & Pants for Toddler Boy",
                        "img":"https://images.hibobi.com/products/000087/720c197b-1778-4cad-a5ec-b09397979447.jpeg",
                        "img_type":"",
                        "origin_price":419.98,
                        "price":365.38,
                        "stock":806,
                        "percentage":0,
                        "discount":"13%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":129127,
                        "good_en_title":"2-piece Solid Pocket Design Pullover & Pants for Toddler Boy",
                        "name":"2-piece Solid Pocket Design Pullover & Pants for Toddler Boy",
                        "img":"https://images.hibobi.com/supply/products/000291000231/d277b3ff-54ae-13d2-414b-18ff9c32c38f.jpeg",
                        "img_type":"",
                        "origin_price":342.98,
                        "price":291.53,
                        "stock":1361,
                        "percentage":0,
                        "discount":"15%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":142631,
                        "good_en_title":"2-piece Solid Denim Shirt & Pants for Toddler Boy（No Shoes）",
                        "name":"2-piece Solid Denim Shirt & Pants for Toddler Boy（No Shoes）",
                        "img":"https://images.hibobi.com/supply/products/000360001268/31ce8f73-aaeb-3b05-67f7-1926505692f5.jpeg",
                        "img_type":"",
                        "origin_price":366.74,
                        "price":311.73,
                        "stock":6701,
                        "percentage":0,
                        "discount":"15%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":159197,
                        "good_en_title":"2-piece Fashion Smile  Print  Pullover and Jeans",
                        "name":"2-piece Fashion Smile  Print  Pullover and Jeans",
                        "img":"https://images.hibobi.com/supply/products/000360003392/9daeecce-2b5c-297a-80d2-2d182a270b10.jpeg",
                        "img_type":"",
                        "origin_price":331.1,
                        "price":264.88,
                        "stock":19424,
                        "percentage":0,
                        "discount":"20%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":159205,
                        "good_en_title":"2-piece Fashion Sport Dinosaur Print Color-block Suits",
                        "name":"2-piece Fashion Sport Dinosaur Print Color-block Suits",
                        "img":"https://images.hibobi.com/supply/products/000360003397/7f60cc3d-586b-d309-2f30-8b1e16f076a6.jpeg",
                        "img_type":"",
                        "origin_price":337.04,
                        "price":286.48,
                        "stock":13816,
                        "percentage":0,
                        "discount":"15%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":160139,
                        "good_en_title":"2-piece Camouflage Sweatshirts & Pants for Toddler Boy",
                        "name":"2-piece Camouflage Sweatshirts & Pants for Toddler Boy",
                        "img":"https://images.hibobi.com/products/000087/1c75b898-2686-43cf-8946-e143448d2716.jpeg",
                        "img_type":"",
                        "origin_price":354.86,
                        "price":283.89,
                        "stock":850,
                        "percentage":0,
                        "discount":"20%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":161869,
                        "good_en_title":"2-piece Cartoon Design Sweatshirts & Pants for Toddler Boy",
                        "name":"2-piece Cartoon Design Sweatshirts & Pants for Toddler Boy",
                        "img":"https://images.hibobi.com/supply/products/000291001199/8388536c-1e08-0e4f-e255-5581b01a1e14.jpeg",
                        "img_type":"",
                        "origin_price":342.98,
                        "price":274.38,
                        "stock":448,
                        "percentage":0,
                        "discount":"20%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":172649,
                        "good_en_title":"2-piece Cartoon Design Sweatshirts & Pants for Toddler Boy",
                        "name":"2-piece Cartoon Design Sweatshirts & Pants for Toddler Boy",
                        "img":"https://images.hibobi.com/supply/products/000387000248/db7c14ea-5939-0ba1-cd03-ffd51b9d127d.jpeg",
                        "img_type":"",
                        "origin_price":257.18,
                        "price":192.89,
                        "stock":90,
                        "percentage":0,
                        "discount":"25%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":179198,
                        "good_en_title":"2-piece Coat & Pants for Toddler Boy",
                        "name":"2-piece Coat & Pants for Toddler Boy",
                        "img":"https://images.hibobi.com/supply/products/000041000516/9308aafd-b924-e7bd-3cd8-6baa6e6ac1a8.jpeg",
                        "img_type":"",
                        "origin_price":295.68,
                        "price":236.54,
                        "stock":9842,
                        "percentage":0,
                        "discount":"20%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    }
                ],
                "content":[
                    {
                        "title":"",
                        "url":"https://images.hibobi.com/product/000051/home_cards/1623319819924BTsbQWAJkjNzGXKyfim.png",
                        "link":"https://m.hibobi.com/categories/Sport-Cate-2782-relate.html"
                    }
                ],
                "more":{
                    "title":"",
                    "url":"",
                    "link":"https://m.hibobi.com/categories/Sport-Cate-2782-relate.html"
                }
            },
            {
                "type":10,
                "title":{
                    "title":"All 40% off",
                    "url":"https:\/\/images.hibobi.com\/product\/000214\/home_cards\/16228817943618PQCNfZ88sCbrdnBZCQ.jpg",
                    "link":"https:\/\/m.hibobi.com\/categories\/Sport-Cate-2645-relate.html"
                },
                "goods":[
                    {
                        "id":184920,
                        "good_en_title":"Toddler Boy 2pcs Monkey Striped T-shirt & Shorts",
                        "name":"Toddler Boy 2pcs Monkey Striped T-shirt & Shorts",
                        "img":"https:\/\/images.hibobi.com\/products\/000089\/72561c40-4dc7-4358-a8ec-cb120e69829c.JPG",
                        "img_type":"",
                        "origin_price":28.31,
                        "price":16.99,
                        "stock":444,
                        "percentage":0,
                        "discount":"40%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":185994,
                        "good_en_title":"Toddler Boy 2pcs Rocket Pattern T-shirt & Shorts",
                        "name":"Toddler Boy 2pcs Rocket Pattern T-shirt & Shorts",
                        "img":"https:\/\/images.hibobi.com\/supply\/products\/000717000013\/df084abe-36d8-abcf-0613-2efe2d86a750.jpeg",
                        "img_type":"",
                        "origin_price":24.49,
                        "price":14.69,
                        "stock":564,
                        "percentage":0,
                        "discount":"40%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":186026,
                        "good_en_title":"Toddler Boy 2pcs Best Football T-shirt & Shorts",
                        "name":"Toddler Boy 2pcs Best Football T-shirt & Shorts",
                        "img":"https:\/\/images.hibobi.com\/products\/000089\/917d2d81-9c5a-474b-b594-8c55a5c0ed1f.jpg",
                        "img_type":"",
                        "origin_price":24.53,
                        "price":14.72,
                        "stock":344,
                        "percentage":0,
                        "discount":"40%",
                        "good_label":"",
                        "label":2,
                        "new_label":2,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":189272,
                        "good_en_title":"Toddler Boy Elephant Pattern T-shirt & Striped Shorts",
                        "name":"Toddler Boy Elephant Pattern T-shirt & Striped Shorts",
                        "img":"https:\/\/images.hibobi.com\/supply\/products\/000717000022\/fc5d3bde-6a8e-bbf6-a477-43d5dc04ef2f.jpeg",
                        "img_type":"",
                        "origin_price":31.05,
                        "price":18.63,
                        "stock":768,
                        "percentage":0,
                        "discount":"40%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":189278,
                        "good_en_title":"Toddler Boy Shark Pattern Suit",
                        "name":"Toddler Boy Shark Pattern Suit",
                        "img":"https:\/\/images.hibobi.com\/supply\/products\/000717000023\/a3061fe0-4e8f-4111-d0c1-64d4b4db4201.jpeg",
                        "img_type":"",
                        "origin_price":28.65,
                        "price":17.19,
                        "stock":809,
                        "percentage":0,
                        "discount":"40%",
                        "good_label":"",
                        "label":2,
                        "new_label":2,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    },
                    {
                        "id":190606,
                        "good_en_title":"Baby Solid Color Sleeveless Ribbed Bodysuit",
                        "name":"Baby Solid Color Sleeveless Ribbed Bodysuit",
                        "img":"https:\/\/images.hibobi.com\/supply\/products\/000479000631\/72c26029-7fa3-9e02-21ad-d5170e4e2bfa.jpeg",
                        "img_type":"",
                        "origin_price":19.16,
                        "price":11.5,
                        "stock":2552,
                        "percentage":0,
                        "discount":"40%",
                        "good_label":"",
                        "label":2,
                        "new_label":5,
                        "left_num":0,
                        "is_activity":0,
                        "is_single_activity":1,
                        "promotion":{

                        }
                    }
                ]
            
            }
          
        ]

}

```
