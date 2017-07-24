# wxpay_php_v3
微信官方PHP V3,修改了几处原版API的错误:
##1
WxPayConfig文件中配置，加上
```
const NOTIFY_URL = "<notify_url_here>";(默认注释)
```

##2
WxpayAPI_php_v3\lib\WxPay.Notify.php的第79行。
这里把括号里面的$return_code参数删除掉。

##3
WxPay.Notify.php文件
在文件头加上require_once "WxPay.Api.php";

