|         |            |
| ------------- |:-------------:|
| 更新日期     | 2019年12月26日 |
| 产品名称      |  普通话一点通   |
| 文档状态 | 基本完成      |
| 设计者       | 江泽锋 |
| 开发者       | 江泽锋 |
| QA | 江泽锋  |


### 第一部分

#### 一、加值宣言 

- 讯飞语音识别API的价值：
> 可以将用户自定义阅读评测的内容记录下来，解决用户会读但不会写或不会拼音的情况，如“日”，并且生成试卷评测内容。
- 百度手写文字识别API的价值：
> 可以将用户自定义阅读评测的内容记录下来，解决用户会写不会读的情况，并且生成试卷评测内容。
- 百度文本纠错API的价值：
> 可以将用户语音识别后生成的试卷评测内容进行进一步处理，减少语音识别的文本错误，增加自定义试卷内容的准确性。
- 讯飞语音评测API的价值：
> 可以根据用户输入的普通话录音或音频自动对发音水平进行评价、发音错误、缺陷定位和问题分析。帮助用户提高普通话发音准确度以及普通话等级考试成绩。

#### 二、用户需求
- 考取教师资格的前提是要获取相应的普通话等级证书，此类用户需要一个软件，帮助他们准确的掌握普通话等级考试高分的发音标准，提高备考效率。
- 事业单位人员应聘需要相关的普通话等级证书，此类用户需要一个软件，帮助他们准确的掌握普通话等级考试高分的发音标准，提高考试分数。
- 想要学好普通话的用户需要一个软件来纠正他们的发音，帮助他们达到标准的发音水平。

#### 三、核心价值 
最小可行性产品：
- 提供国家级评测标准给用户，帮助用户提升普通话口语能力及普通话证书考试成绩。

#### 四、用户痛点
|序号|用户痛点|
|------|---|
|1|普通话等级测试机测前三题是系统自动评分，系统是即时评分，考生语音结束，后台便会有前三题成绩，但是平时练习并没有机会接触到这类评测系统和机器，无法拿捏机器的评分标准，并进行针对性改善发音，提高成绩|
|2|普通话和用户方言在语音上的差异导致用户常常拿捏不准，没有一个准确的记忆。|
|3|身边的语言环境复杂，无法根据身边的人得出准确读音，尽管已经通过普通话等级测试亦无法每次准确根据评定标准发音，无法为用户提供参考标准|
|4|网上无法找到同步国家普通话等级考试标准的评测学习软件|

#### 五、产品简介
- 该产品提供语音识别输入为用户提供录入自定义试卷内容的方式。
- 该产品可以为对用户的发音标准按照国家级标准进行评价，对发音错误、缺陷等进行定位和问题分析。
- 该产品可以为用户提供历年普通话等级考试真题训练评测，有助于提高用户普通话等级考试分数。
- 该产品可以提供国家发布的六十篇等级考试篇章的标准mp3录音，以及每个考试涉及字的标准录音。

#### 六、人工智能概率性
- 目前对于中文，讯飞语音识别成功率达98%，百度98%，搜狗97%。
- 目前讯飞语音评测应用于国家普通话等级考试、英语四六级考试中，得到国家认可。
> 错误现象的解决方法：
- 当语音识别内容出现偏差时，提供修改功能，用户可以手动修改无法识别或者识别错误的地方，并且进行记录，减少同类情况。
- 当文本纠错产生误判时，用户可以再次修改。
- 当手写识别字体产生错误时，用户可以再次修改。
#### 七、需求列表与人工智能API加值
|优先级|用户需求|功能实现|api加值
| ---------- | --------- |----------- |------
| 重要 |用户需要一个帮助他们准确的掌握普通话等级考试高分的发音标准，提高备考效率及分数 |讯飞语音评测API | 通过智能语音技术自动对发音水平进行评价、发音错误、缺陷定位和问题分析
| 次重要 |用户需要可以以语音转为文字的方式记录下来，提高记录效率，同时解决用户会读但不会写或不会拼音的情况，如“日”|讯飞语音识别API| 提高试卷自定义试卷内容速度
| 一般重要|将用户语音识别后生成的试卷评测内容进行进一步处理，减少语音识别的文本错误，增加自定义试卷内容的准确性。 |百度文本纠错API| 用户可以手动纠错，重要性一般
| 一般重要|将用户自定义阅读评测的内容记录下来，解决用户会写不会读的情况|讯飞手写字体识别API| 用户可以使用手写输入法输入替代

#### 八、人工智能API加值
- 语音识别API的加值：
> 可以将用户自定义阅读评测的内容记录下来，解决用户会读但不会写或不会拼音的情况，如“日”
- 手写字体识别API的加值：
> 可以将用户自定义阅读评测的内容记录下来，解决用户会写不会读的情况，并且生成试卷评测内容。
- 文本纠错API的加值：
> 减少语音识别的文本错误，提高自定义试卷内容的准确性。
- 语音评测API的加值：
> 根据用户输入的普通话录音或音频自动对发音水平进行评价、发音错误、缺陷定位和问题分析。帮助用户提高普通话发音准确度以及普通话等级考试成绩。

### 第二部分：原型

#### 产品架构图
- ![avatar](<https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/img/axure1.png>)

#### 核心交互及功能介绍
- ![avatar](<https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/img/axure2.png>)

#### 原型文档

- [原型交互文档](http://nfunm036.gitee.io/api-final-axure)
- [原型文档下载](https://gitee.com/NFUNM036/api-final-axure)
- 口头操作说明：课上已说明。
2-3分钟，留下「的确这是个可行丶可用的人工智能加值产品」的印象。

### 第三部分：产品使用关键AI或机器学习之API的输出入展示

#### API使用水平
> 输入输出皆在代码中有所展现
- 语音识别API [详细代码示例](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/%E8%AE%AF%E9%A3%9E%E8%AF%AD%E9%9F%B3%E8%AF%86%E5%88%AB.ipynb)
- 文本纠错API [详细代码示例](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/WBJC_BAIDU.ipynb)
- 语音评测API [详细代码示例](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/API_XF_PC.ipynb)
- 手写字体识别API [详细代码示例](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/%E7%99%BE%E5%BA%A6%E6%89%8B%E5%86%99%E5%AD%97%E4%BD%93%E8%AF%86%E5%88%AB.ipynb)

#### API使用比较分析


#### 手写字体识别API比较

- 百度ai开放平台和讯飞开放平台提供手写字体识别服务搜索引擎排名较为靠前，为此进行比较。

|对比平台|百度|讯飞|
|---|---|---|
|代码比较|[百度手写字体识别api详细代码示例](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/%E7%99%BE%E5%BA%A6%E6%89%8B%E5%86%99%E5%AD%97%E4%BD%93%E8%AF%86%E5%88%AB.ipynb)|[讯飞手写字体识别api详细代码](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/%E8%AE%AF%E9%A3%9E%E6%89%8B%E5%86%99%E5%AD%97%E4%BD%93%E8%AF%86%E5%88%AB.ipynb)|
|使用效果|中文字体识别效果很好，字体格式完全正确；对于英文的字体识别断句分词糟糕，无法使用，|识别准确，但是默认输出为文字编码，并非中文字体，相比百度手写字体识别，英语文字的识别准确度非常高，单词分段等清晰无误，全文仅有一处错误|
|成熟度|[2019-12-17推出最新版的api文档](https://ai.baidu.com/ai-doc/OCR/hk3h7y2qq)，调用方法和过程简单，官方文档有在github给定参考代码|[有详细的api调用文档及说明，可以直接下载使用](https://www.xfyun.cn/doc/words/wordRecg/API.html)|
|性价比|每日 50 次免费调用量，开通按量后付费。调用失败不计费。预付费套餐10万次只需要740元[百度ai开放平台手写字api产品价格](https://ai.baidu.com/ai-doc/OCR/Ek3h7xvq7)|免费次数为90天10万服务量，付费则为1万服务量350/年，10万服务量3200/年；100万服务量30000元/年[讯飞开放平台手写字体识别api产品价格](https://www.xfyun.cn/services/wordRecg)|
|服务评估|有api文档且有[示例代码](https://github.com/Baidu-AIP/QuickStart/tree/master/OCR)，调整参数以及接口链接即可使用，应用场景和参数完整，便于使用，且输出结果易处理|[具有详细的调用API说明文档](https://www.xfyun.cn/doc/words/wordRecg/API.html)及[api调用代码](https://www.xfyun.cn/doc/words/wordRecg/API.html#%E8%B0%83%E7%94%A8%E7%A4%BA%E4%BE%8B)|

- 总结：通过对比调取百度ai开放平台和讯飞开放平台提供的手写字识别api，对比输出结果，综合上述内容，最终选定使用百度开发平台提供的手写字体API服务。
> 讯飞使用文档有错误示范，其中对于语言参数的设置有误，讯飞提供en（英文），cn|en（中文或中英混合）两种参数设置，如果设置en,识别英文的确很不错，全文仅有一处错误，但是当需要识别中文时，按照文档我需要把语言参数设置为‘cn|en’，这时候返回的结果则是一堆中文编码而不是文字。如若想要返回结果为中文，只能默认语言参数为en(英文)，文档存在误导成分。然后在日后的测试中，无论如何设置返回的都是中文编码。
#### 语音识别API比较

|对比平台|百度|讯飞|
|---|---|---|
|代码比较|[百度语音识别API详细代码示例](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/%E7%99%BE%E5%BA%A6%E8%AF%AD%E9%9F%B3%E8%AF%86%E5%88%AB.ipynb)|[讯飞语音识别API详细代码](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/%E8%AE%AF%E9%A3%9E%E8%AF%AD%E9%9F%B3%E8%AF%86%E5%88%AB.ipynb)|
|使用效果|百度语音识别无论是‘输入法模型’还是‘搜索模型输出’两种方式结果都不准确，无法使用。|识别准确，连感叹语气都识别出来了。|
|成熟度|[2019-12-19推出最新版的api文档](https://ai.baidu.com/ai-doc/SPEECH/Vk38lxily)，调用方法和过程简单，官方文档有在github给定[参考代码](https://github.com/Baidu-AIP/speech-demo)|有详细的[api调用文档及说明](https://www.xfyun.cn/doc/asr/lfasr/API.html)，可以直接下载使用[示例代码](https://www.xfyun.cn/doc/asr/lfasr/API.html#%E8%B0%83%E7%94%A8%E7%A4%BA%E4%BE%8B)|
|性价比|12000元/1QPS/一年，无限制调用量[百度ai开放平台语音识别API产品价格](https://ai.baidu.com/ai-doc/SPEECH/Jk38lxn2j)|按音频时长计费，四个套餐，198/20小时/一年，1180/200小时/一年，2700/500小时/一年，4900/1000小时/一年[讯飞开放平台手写字体识别api产品价格](https://www.xfyun.cn/services/lfasr?ch=bdtg&renqun_youhua=478960)|
|服务评估|有api文档且有[示例代码](https://github.com/Baidu-AIP/speech-demo)，调整参数以及接口链接即可使用，但是输出结果不准确，无法使用|[具有详细的调用API说明文档](https://www.xfyun.cn/doc/asr/lfasr/API.html#%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E)及[api调用代码](https://www.xfyun.cn/doc/asr/lfasr/API.html#%E8%B0%83%E7%94%A8%E7%A4%BA%E4%BE%8B)|

- 总结：通过对比调取百度ai开放平台和讯飞开放平台提供的语音识别api，对比输出结果，使用量大百度性价比高，但讯飞输出结果准确，综合上述内容，最终选定使用讯飞开发平台提供的语音识别API服务。


#### API使用后风险报告

使用后风险报告：在PRD文件中是否有说明且提供连结证据，所使用的API类别的现在及未来发展性，如API市场竞争程度丶输入输出限制丶定价丶及可替代的程序库（改用自己开发的代码及数据库而不用API）等等
##### 手写字体识别API
- 自行进行代码测试比较，百度api和讯飞api利用同一图片进行比较，百度api中文识别率更高，但仍存在一些误差，可能会对用户体验造成影响，但增设了文本纠错功能，且app可对错误识别的文字进行更正。

对比项 | 百度 | 讯飞 | 总结
---|---|---|---
API市场竞争程度 | google搜索排行为第二 | google搜索排行第十五 | 百度搜索引擎排名较前，且直接显示百度AI首页，讯飞亦是显示首页
输入输出限制 | 支持中英文手写字体及数字识别，英文输入效果不理想，中文很好 | 支持中英文自动识别，中文输出为中文编码，不利于处理 | 由于APP的定位，API是服务于中文识别的，百度在中文字体上的优势更大
定价 | [百度ai开放平台手写字api产品价格](https://ai.baidu.com/ai-doc/OCR/9k3h7xuv6)|[讯飞开放平台手写字api产品价格](https://www.xfyun.cn/services/wordRecg)| 从免费额度来看，百度提供每日50次免费调用量，讯飞提供90天10w次调用的免费调用量。但是百度可进行按套餐付费与按量付费两种方式，讯飞仅支持套餐。

- 总结：短期测试英文识别来讲可使用讯飞的免费额度，以及如果是处理中文则只能用百度，如若是大规模使用则百度性价比更高，更为划算。

##### 语音识别API
- 自行进行代码测试比较，百度api和讯飞api利用同一段语音进行比较，讯飞api中文识别率更高，但个别情况有误差，可能会对用户体验造成影响，但增设了文本纠错功能，且app可对错误识别的文字进行更正。

对比项 | 百度 | 讯飞 | 总结
---|---|---|---
API市场竞争程度 | google搜索排行为第二 | google搜索排行第十五 | 百度搜索引擎排名较前，且直接显示百度AI首页，讯飞则是显示语音SDK下载页面。
输入输出限制 | 支持粤语、四川话方言、英文识别，中文输出效果不理想 | 支持中、广东话、河南话、四川话等方言，英、日语、俄语、西班牙语、法语、韩语、泰语、德语、越南语、阿拉伯语、保加利亚语识别，普通话输出准确，语气上扬准确识别为感叹号。 | 由于API准确性的考量，API是服务于中文识别的，讯飞在语音识别上的优势更大。
定价 | [百度ai开放平台语音识别api产品价格](https://ai.baidu.com/ai-doc/SPEECH/Jk38lxn2j)|[讯飞开放平台语音识别api产品价格](https://www.xfyun.cn/services/voicedictation)| 从免费额度来看，百度提供每日50次免费调用量，讯飞提供90天10w次调用的免费调用量。但是百度可进行按套餐付费与按量付费两种方式，讯飞仅支持套餐。

- 总结：短期测试英文识别来讲可使用讯飞的免费额度，以及如果是处理中文则只能用百度，如若是大规模使用则百度性价比更高，更为划算。

#### API加分项
> 用到的的api有文本纠错API、手写字识别API、语音识别API、语音评测API
- [文本纠错代码示例](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/WBJC_BAIDU.ipynb)
- [手写识别代码示例](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/%E7%99%BE%E5%BA%A6%E6%89%8B%E5%86%99%E5%AD%97%E4%BD%93%E8%AF%86%E5%88%AB.ipynb)
- [语音识别代码示例](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/%E8%AE%AF%E9%A3%9E%E8%AF%AD%E9%9F%B3%E8%AF%86%E5%88%AB.ipynb)
- [语音评测代码示例](https://github.com/jzf-timer/git-github.com-jzf-timer-API_Final/blob/master/code/API_XF_PC.ipynb)