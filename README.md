# WeChatImpl
微信接口笔记
# 微信卡包接口
1.获取ticket  
https://api.weixin.qq.com/cgi-bin/ticket/getticket?access_token=access_token&type=wx_card

2.获取授权url(这个url用来领取卡券)  
https://api.weixin.qq.com/card/invoice/getauthurl?access_token=access_token  
```
{
    "redirect_url": "",
    "timestamp": "1509507223930",
    "source": "web",
    "ticket": "9KwiourQPRN3vx3Nn1c_iWH7TTPW0y09oFFHqz3q9QtTbgCVIzE_UxJ_fisKXptI1JFumAmmKpwzSThq-24R3Q",
    "s_pappid": "d3hjYWNiN2Q0YTBjMTIzNGY0X6UbIfgPk9I_Pc2verrrz-Rss-6fN2-sFjll59Jdo3XD",
    "money": "55500",
    "type": 2,
    "order_id": "20171101104029344764"
}
```
3.回调上传内容到微信，返回mediaId
4.发送发票到卡包
