> Any-Proxy可以帮助你完美地反向代理浏览任意网站  
> 免去复杂的程序，不到10KB文件即可兼容性极好地高速代理访问任意网站  
  
> 最新版本将退出指令改成了~q 这将在输入时更加便捷  
> 需配置伪静态，nginx伪静态规则如下：  
> if ( !-e $request_filename) {  
>     rewrite ^/(.*)$ /index.php?$1 last;  
>     break;  
> }  
  
> index.php 外链、外链图片、外链静态文件等请求不通过Any-Proxy，地址栏不会显示目标域名  
> index_all.php 区别为传统版，地址栏会显示目标域名，性能不及前者  
> index_all.php 所有外链、外链图片、外链静态文件等请求都通过Any-Proxy
  
> 支持POST、Cookie，https/http均可使用  
> 支持伪造IP，$anyip值为1发送服务器IP头，值为2则发送随机IP，值为3发送客户端IP  
> 已解决中文乱码问题，自动转换  
  
> 在当前链接末尾输入 ~q 可以退出当前页面回到首页  
> 在域名后面加上链接地址即可访问：  
> https://turl.chat/http://+需访问的链接 （必须添加http(s)://）  
  
> 如 ：https://turl.chat/http://ip38.com/  
  
> 测试站点：https://turl.chat/ 请求量超过50次将会无法访问  
  
  
![Image](https://p.pstatp.com/origin/1382700019aa3271d8dbf)  
![Image](https://p.pstatp.com/origin/1381300028eead6fe7615)  

> 基于：https://github.com/koala0529/reverse-proxy-php 修改  
> 请勿用于非法用途，否则后果自负。
