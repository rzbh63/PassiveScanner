## 中文
这是一个基于Mitmproxy和Arachni的被动式扫描器。
* arachni
* celery
* mitmproxy

![基本流程图.png](https://github.com/jjf012/PassiveScanner/raw/master/images/process.png)

其中为了能够让`celery`运行在windows上面，我选择的版本是3.1.25。
redis作为celery的broker并且设置了密码。
通过`celery -A scan worker --loglevel=info`启动worker。
`proxy.py`的默认端口是8080。

![mysql.png](https://github.com/jjf012/PassiveScanner/raw/master/images/mysql.png)

**更新**

使用[PreparedStatement](https://github.com/ring04h/fpymysql/commit/fd2084b8601a670cb4ca75d78da46a6ec433cf4b)

参考链接
* [基于Arachni构建黑盒扫描平台](http://bobao.360.cn/learning/detail/3533.html)
* [wyproxy](https://github.com/ring04h/wyproxy)
* [Arachni](https://github.com/Arachni/arachni/wiki/REST-API)
* [arachni-python-client](https://github.com/yukito/arachni-python-client)

## English
This is a passive scanner based on Mitmproxy and Arachni.
* Arachni
* Celery
* Mitmproxy

Which in order to be able to `celery` run on windows, I chose the version is 3.1.25.
Redis as celery broker and set the password.
Start worker with `celery -A scan worker - loglevel = info`.
The default port for `proxy.py` is 8080.

**update**

use Mysql [PreparedStatement](https://github.com/ring04h/fpymysql/commit/fd2084b8601a670cb4ca75d78da46a6ec433cf4b)

Reference link
* [Based on Arachni build black box scanning platform](http://bobao.360.cn/learning/detail/3533.html)
* [Wyproxy](https://github.com/ring04h/wyproxy)
* [Arachni](https://github.com/Arachni/arachni/wiki/REST-API)
* [arachni-python-client](https://github.com/yukito/arachni-python-client)