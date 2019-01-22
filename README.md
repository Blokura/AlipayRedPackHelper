# 欢迎使用Alipay红包助手带分站版
红包助手是一个帮助用户自动将红包转化为现金的一个小助手。您只需要准备好单笔转账到支付宝接口（企业）以及当面付（可用码支付替代）即可使用本套系统。
本项目支持**开通分站**以及**API**，分站可以自助充值后使用主站内置的单笔转账接口为其订单返款。

- **简洁快速**：从领红包到返款，只需要3步。先领红包，然后助手下单支付，最后等待到账即可。
- **高效快捷**：打开输入金额，直接跳转支付宝付款，无需其他操作。
- **完善后台**：本系统最大的亮点就是分站系统。分站站长有非常完善的后台进行操作，支持 手续费 广告公告 API等设置。
- **API支持**：本系统亦可作为非对外开放的系统，通过调用API可以做成单笔转账接口出租平台。
- **主流对接**：本系统在原本只支持当面付的基础上新增了码支付接口，使分站站长不用再为申请当面付而发愁。
更多乐子等您发觉。

## 搭建平台需求
- 有独立的域名和主机
- 有企业的单笔转账至支付宝接口
- 有企业的即时到账接口
- 当面付接口或码支付接口（如需自行开站）

## 搭建教程

- 1.直接Clone或者Download（这辈子都不会发release的）
- 2.将pay.sql导入数据库
- 3.配置数据库

首先进入config表，修改admin_user为管理员账号，admin_pwd为管理员密码。
然后修改appid为单笔转账至支付宝接口的支付宝APPID，alipayPublicKey为支付宝公钥，saPrivateKey为应用私钥。
payer_show_name修改为返款时显示的付款人名，remark修改为返款备注。
announce为后台公告栏代码，按需修改。

- 4.修改config.php内的数据库连接信息
- 5.访问站点，完成搭建操作
