# Texttospeech
小马配音 文字转语音 声音 配音神器 商业产品官方API http://peiyin.xiaomawenku.com/api.html <br/>
自行试听，远超过国内的百度，腾讯，华为云，各种云开源的产品。自行对比，无需解释。<br/>
作者为：百度的资深架构师 马开东 开发<br/>
5秒立刻mp3 wav文件，  52种语音 试听:http://peiyin.xiaomawenku.com/shiting.html 供您选择<br/>
各类抖音 快手 客服 销售 文学 阅读 小说 方言 中英文场景支持 7*24小时自动服务。<br/>
本站已服务500万用户，3亿次配音，值得信赖！<br/> 小马配音高质量低价格才是王道 该工具由 公司企业信息：北京小马未来科技有限公司 开发 对外提供API 合作微信 makaidongzi



1.首先 免费注册用户<br/>
2.开通SVIP会员并充值金额 加入SVIP会员特惠<br/>
3.小马配音调用API接口：<br/>
HTTP协议 POST请求：URL：http://peiyin.xiaomawenku.com/PeiYin/xiaomapeiyin_api_to_peiyin<br/>
参数：<br/>
xiaomapeiyin_text: 配音内容<br/>
caiyanglv: 采样率 8=8000K； 16=16000K<br/>
geshi: 格式后缀 1=pcm; 2=wav; 3=mp3; 4=alaw;<br/>
renming_id: 主播id 2到52<br/>
pitchRate: 音调 -500 到 500<br/>
speechRate: 语速 -500 到 500<br/>
volume: 音量 0 到 100<br/>
bgurl: 背景音乐 http://xxx.mp3<br/>
xiaomapeiyin_svip_user_id:注册并开通svip的id<br/>
xiaomapeiyin_svip_token:客服给你的秘钥<br/>
返回json：<br/>
已经合成的线上地址url 使用http下载即可。<br/>
调用成功：<br/>
{"data":{"xiaomapeiyin_result_url":"http://peiyin.xiaomawenku.com/xiaomapeiyin_down/202007.html?isDown=1&filename=小马配音合成文件.mp3"},"msg":"小马配音，调用成功":1}<br/>
调用失败：<br/>
{"data":{},"msg":"小马配音，调用失败,原因参数：xiaomapeiyin_svip_token或xiaomapeiyin_svip_user_id不对","status":400}<br/>
