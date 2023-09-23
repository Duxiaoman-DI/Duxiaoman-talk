# Duxiaoman-talk

## 我们是谁？
度小满数据智能应用部隶属公司技术团队，由度小满数据智能应用部总经理、技术委员会执行主席杨青带领，布局智能获客、风险经营模型、数据生态、人工智能建设等方向，持续加强创新技术研发，以创新科技为金融发展助力。团队由来自海内外顶尖院校的专家成员共同组建，拥有数十项技术专利，多次斩获国际大奖，相关论文被CIKM、CVPR、ACM MM等国际顶会收录，在对内赋能公司业务基础上持续对外输出技术影响力。    

## 知识沉淀   
团队深耕计算机视觉、自然语言处理、图算法、自动化人工智能等算法研究，通过自研创新算法，形成AI产品与技术能力，应用于公司营销、经营、风控、反欺诈全流程业务场景：一方面，在基于百度生态内数据生成的信用评分卡效果不断提升，帮助金融机构极大拓展了信贷业务的服务半径；另一方面，技术中台的建设、以及对「因果推断」等前沿技术的探索进一步实现了对客户的精细化运营，在提升效率的同时，大大降低了运营成本。     
以下是我们再AI算法、平台、风控与因果推断等领域的公开演讲材料：   

**平台实践**   
* [图平台在金融风控中的应用实践 (2023全国知识图谱与语义计算大会)](#ccksgraph)
* [度小满金融超大规模图平台实践](#graphplat)
* [度小满自动机器学习平台实践](#automl)

**AI类**    
* [AI防欺诈不应只是单点突破，要有“全链条”屏障](#deepfake)
* [图机器学习引领征信解读进入5.0时代](#graph5)
* [大模型让AI诈骗成精了，10分钟骗走430w](#ai_llm)
* [金融场景下人脸识别的安全应用实践](#face)
* [OCR技术在小微场景中的应用](#ocr_xw)
* [图机器学习在度小满征信建模中的应用](#graph_zx)
* [AI在度小满征信解读中的应用](#aizx)
  

**信贷风控**    
* 金融数智化转型面临的挑战是数据治理
* 大数据风控模型实践
* [数据科学与金融风控模型](#riskm1)
* [图机器学习在度小满风控中的应用](#graphrisk)
* 大数据在征信上的实践
* [以贷养贷不会被发现？大错特错，时序网络助力风控升级](#rnn)

**因果推断**   
* [因果推断在度小满金融场景的应用探索](#causal1)
* [基于反事实因果推断的金融额度模型](#amountlimit)

## 平台实践  
### <span id='ccksgraph'>图平台在金融风控中的应用实践(2023全国知识图谱与语义计算大会)</span> 
**全文**  [图平台在金融风控中的应用实践](https://ccks.gz.bcebos.com/2023/CCKS%E8%AE%BA%E5%9D%9B%E2%80%94%E2%80%94%E6%9D%A8%E9%9D%92%2020230827.pdf)    
**简介**  在金融行业应用中目前图平台主要面临三大挑战：海量关联数据的高效存储、过高的图建模门槛、难以满足用户个性化建模与分析需求。    
为应对这些挑战，度小满推出了大规模分布式图计算平台。该平台以度小满海量数据(603138)位底层架构，搭建了度小满自研的图数据库、分布式推理框架、表示学习平台等基础设施，结合图神经网络、大规模无监督表示学习等技术，同时集成全流程自动建模、智能可视化图分析等功能，能够在智能获客、智能反欺诈、智能风控、智能审核等应用场景中赋能。   
目前，度小满自研的图数据库已经支持百亿节点、千亿边的数据规模，多条查询能达到毫秒级，在图计算能力上，包括了15类的图分析算法，分析效率也提升了10倍以上。   
<img src="https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E5%9B%BE%E5%B9%B3%E5%8F%B0-%E5%8F%AF%E6%89%A9%E5%B1%95%E9%AB%98%E6%80%A7%E8%83%BD%E5%9B%BE%E6%95%B0%E6%8D%AE%E5%BA%93.PNG" width=550 height=300 />
<br/>

### <span id='graphplat'>度小满金融超大规模图平台实践</span>   
**全文**  [度小满金融超大规模图平台实践](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E5%BA%A6%E5%B0%8F%E6%BB%A1%E9%87%91%E8%9E%8D%E8%B6%85%E5%A4%A7%E8%A7%84%E6%A8%A1%E5%9B%BE%E5%B9%B3%E5%8F%B0%E5%AE%9E%E8%B7%B5.md)    
**简介**  金融风控场景数据间有天然的关联。关联信息可以加强模型风险区分能力。复杂数据场景及海量数据规模给关联信息的管理、建模和模型部署都带来了巨大的挑战。本文将介绍度小满内部构建的超大规模图平台的一些经验与思考，并重点讲解在实践中碰到的问题与解决方式。主要内容包括：① 图数据治理；② 图模型训练；③ 图在线部署；④ 总结思考。
<img src="https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E5%9B%BE%E5%B9%B3%E5%8F%B0eros%E7%BB%93%E6%9E%84%E5%9B%BE.png" width=550 height=300 border=10 />
<br/>

### <span id='automl'>度小满自动机器学习平台实践</span>   
**全文**  [度小满自动机器学习平台实践](https://www.51cto.com/article/746831.html)    
**简介**  随着 AI 技术的发展，不同业务涉及的 AI 技术越来越多样，同时 AI 模型参数量逐年爆发式增长，如何克服 AI 算法落地面临的开发成本高、对人工依赖强、算法不稳定及落地周期长等问题，成为困扰人工智能从业者的难题。而“自动机器学习平台”是解决 AI 落地压力的关键方法。本文将分享度小满在搭建自动机器学习平台 ATLAS 的实践经验。    
<img src="https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E8%87%AA%E5%8A%A8%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E5%B9%B3%E5%8F%B0%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E4%BC%98%E5%8C%96.png" width=550 height=300/>
<br/>

## AI类   
### <span id='deepfake'>AI防欺诈不应只是单点突破</span> ，要有“全链条”屏障 
**全文**   [人工智能在金融领域的最新应用与探索方向](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/AI%E9%98%B2%E6%AC%BA%E8%AF%88%E4%B8%8D%E5%BA%94%E5%8F%AA%E6%98%AF%E5%8D%95%E7%82%B9%E7%AA%81%E7%A0%B4%20%EF%BC%8C%E8%A6%81%E6%9C%89%E2%80%9C%E5%85%A8%E9%93%BE%E6%9D%A1%E2%80%9D%E5%B1%8F%E9%9A%9C.pdf)      
**简介**   技术是一把双刃剑，人工智能在如火如荼发展过程中，利用AI技术造假、伪造等事件也是屡见不鲜。就在前不久，国内某大型银行的人脸识别环节被诈骗分子攻破，诈骗团伙利用注入绕过、深度伪造等技术冒名顶替银行卡持有者本人，从其银行卡中盗取数十余万元。    
那么面对如此现状，又该如何破解？7月20日，在“北大光华-度小满金融科技前沿技术研讨会”上，度小满技术委员会执行主席杨青介绍了前沿AI技术在金融领域的具体应用。    
杨青认为，金融领域要做到AI防深伪，不仅仅是识别人脸的真假这么简单。在AI科技与金融不断深入融合的当下，获客、风控等日常环节均在朝着智能化方向变化。因此，金融领域的AI防深伪，不应当只是针对DeepFake这种技术的单点突破，而是要守住整个链条、每个节点的安全，建立“全链条”屏障。    
随着人脸认证的普及应用，不法分子通过DeepFake这样的技术来伪造人脸的诈骗也日益增多。“眼见未必为实”，这类虚假视频肉眼往往无法识别，怎么防范这类新型风险？度小满的防深伪技术，运用了千万级样本；从中提取了多域视觉特征：包含傅立叶频谱特征、小波特征、和RGB空域特征等等，利用多特征融合共同辅助鉴伪。目前度小满防深伪技术已经可以覆盖各种深伪形式，比如静态人像图片活化和AI换脸等，千分之一误报率下召回为90%以上。    
反欺诈是金融风控审核的第一步，目的是排除“坏人”，对于通过这一步的“好人”，如何判断他的信用，决定给多少授信额度呢？度小满利用NLP自然语言处理技术对征信报告进行分析和识别，再通过自监督预训练模型，从而达到从文本中识别用户风险的目的。 ![pic1](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/ai_upgrade.PNG)   
<br/>

### <span id='graph5'>图机器学习引领征信解读</span>进入5.0时代 
**全文**   [图机器学习引领征信解读进入5.0时代](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E5%9B%BE%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E5%BC%95%E9%A2%86%E5%BE%81%E4%BF%A1%E8%A7%A3%E8%AF%BB%E8%BF%9B%E5%85%A55.1%E6%97%B6%E4%BB%A3%E2%80%94%E2%80%94AI%E6%8A%80%E6%9C%AF%E5%9C%A8%E6%99%BA%E8%83%BD%E9%87%91%E8%9E%8D%E4%B8%AD%E7%9A%84%E5%BA%94%E7%94%A8.pdf)      
**简介**   2022年3月26日，由华夏时报社主办的“数据智能重塑实体：2022智能数据论坛”在线上举办。论坛集结了数据智能相关领域的专家学者，深入探讨当前行业发展的新趋势。度小满技术委员会执行主席、数据智能部总经理杨青受邀出席论坛，并发表 “AI技术在智能金融中的应用”的主题演讲。     
杨青表示，目前智能金融面临三大核心业务：如何提升获客效率、风险识别能力以及老客经营能力。“数据+AI”则是打开这三道大门的“钥匙”，也是大数据时代智能金融企业必备的能力。他重点介绍了度小满利用AI构建的OCR（光学字符识别技术）产品矩阵，以及利用图机器学习挖掘征信报告的经验。     
他指出，解读征信报告数据，从技术角度来看，历经了从1.0专家经验时代到4.0深度学习时代的跨越，如今来到了5.0利用图机器学习挖掘信息时代。   
<br/>

### <span id='ai_llm'>大模型让AI诈骗成精了，10分钟骗走430w</span>
**全文**   [大模型让AI诈骗成精10分钟骗走430w](https://www.qbitai.com/2023/05/55771.html)      
**简介**   随着AGIC技术大爆发，普通人接触到各种先进生成工具变得不费吹灰之力，制作出越发难以识别的高质量deepfake视频越来越容易，我们想要一眼识破这些造假内容就更加困难。     
实际上，应对deepfake其实早已有比较成熟的技术方法和方案。    
<img src="https://www.qbitai.com/wp-content/uploads/replace/7bbbf78222a47f0e18c0cc693608487a.jpeg" width=550 height=300 />

<br/>

### <span id='face'>金融场景下人脸识别的安全应用实践</span>
**全文**   [金融场景下人脸识别的安全应用实践](https://www.geekpark.net/news/311643)      
**简介**   1月16日，由中国信息通信研究院云计算与大数据研究所（以下简称“中国信通院云大所”）、可信人脸应用守护计划、中国通信标准化协会TC602联合主办的“护脸计划2022年度成果发布会”在云端召开。度小满的“谛观生物认证系统”通过了本次最新评测。    
<img src="https://imgslim.geekpark.net/uploads/image/file/4c/89/4c89bef27e513552027ca6f0d1a70c15.png" width=250 height=400 />

<br/>


### <span id='ocr_xw'>OCR技术在小微场景中的应用</span>
**全文**   [度小满金融OCR技术在小微场景中的应用](https://www.modb.pro/db/232796)      
**简介**   相比大中型企业，小微企业具有很明显的特点，资产规模小、抵押物不足、抗风险能力弱等。由于其自身的特点和经营发展的需要，小微企业具有“短、小、频、急”的借贷需求。   
然而，由于信息不对称，融资难、融资贵，是众多小微企业面临的一大难题，融资的周期长，尤其是“首贷难”，更是“难上加难”，这些仍然制约着小微企业的发展。    
我们借助OCR技术，构建了全流程的小微OCR产品，重点包括了身份证、驾驶证、行驶证、营业执照、保单等，涉及到小微企业的多个方面。除此以外，我们还设计了OCR模型闭环生产的全流程，包含需求、数据、训练、发布、监控。    
<img src="https://oss-emcsprod-public.modb.pro/wechatSpider/modb_20220106_6d1bfab2-6ee0-11ec-9a0c-fa163eb4f6be.png" width=550 height=300 />
<br/>

### <span id='graph_zx'>图机器学习在度小满征信建模中的应用</span>  
**全文**   [图机器学习在度小满征信建模中的应用](https://www.modb.pro/doc/72121)      
**简介**   度小满将深度学习、图计算、多模态识别等技术应用于风控，从文本、行为、多媒体等数据中提取风险变量，取得了显著的突破。本文将重点介绍利用图机器学习对强金融数据——征信报告的挖掘。在对征信报告的利用方面，历史上和如今各机构主要使用评分卡模型，该模型一般基于专家经验加工几个或者几十个特征，最后处理成一个加和模型。除了简单模型，复杂模型主要有两个思路：一是加工提取更多特征，利用更复杂的比如树模型；二是基于原始数据，做非结构化特征来构建端到端的模型。这三个方向度小满都有尝试。   
![pic1](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/2%E5%9B%BE%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E5%9C%A8duxioaman%E5%BE%81%E4%BF%A1%E6%8A%A5%E5%91%8A%E7%9A%84%E5%BB%BA%E6%A8%A1.PNG)   
<br/>

### <span id='aizx'>AI在度小满征信解读中的应用</span> 
**全文**  [AI在度小满征信解读中的应用](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/AI%E5%9C%A8%E5%BA%A6%E5%B0%8F%E6%BB%A1%E5%BE%81%E4%BF%A1%E8%A7%A3%E8%AF%BB%E4%B8%AD%E7%9A%84%E5%BA%94%E7%94%A8.md)    
**简介**  报告的主题是AI技术在征信解读中的应用，主要介绍我们针对金融征信数据以及面向信贷领域模型在技术上的优化实践。本文侧重于介绍度小满在基于征信报告开发端到端模型时的模型架构、经验、难点。    
![pic2](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/pretrain2.PNG)   
<br/>

## 信贷风控   
### <span id='rnn'>以贷养贷不会被发现？大错特错，时序网络助力风控升级</span> 
**全文**  [度小满风控创新式探索](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E4%BB%A5%E8%B4%B7%E5%85%BB%E8%B4%B7%E4%B8%8D%E4%BC%9A%E8%A2%AB%E5%8F%91%E7%8E%B0%EF%BC%9F%E5%A4%A7%E9%94%99%E7%89%B9%E9%94%99%EF%BC%8C%E6%97%B6%E5%BA%8F%E7%BD%91%E7%BB%9C%E5%8A%A9%E5%8A%9B%E9%A3%8E%E6%8E%A7%E5%8D%87%E7%BA%A7.md)   
**简介**  随着大数据与人工智能的引入，金融风控领域出现了很多探索与创新，针对海量非结构化数据的研究和挖掘，更是层出不穷。   
在信贷领域内，征信报告是一种非常常见的非结构化数据，过去主要通过专家经验从中加工出风险相关特征。然而，在我们的案例中可以看到，传统特征加工方式无法捕捉到用户以贷养贷的风险，而时序网络可以非常细致地观察到用户的时间变化趋势，能够更好地发现这种潜在的风险行为。这就说明，对包含大量文本、非结构化的数据，传统挖掘方式面临巨大挑战；我们将详细介绍度小满对征信这类非结构化数据的创新式探索。   
![pic3](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E5%BE%81%E4%BF%A1%E6%8A%A5%E5%91%8A%E8%A7%A3%E8%AF%BB%E6%8A%80%E6%9C%AF%E5%8F%91%E5%B1%95%E8%B6%8B%E5%8A%BF2.PNG)   
<br/>   

### <span id='riskm1'>数据科学与金融风控模型</span> 
**全文**  [数据科学与金融风控模型](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E6%95%B0%E6%8D%AE%E7%A7%91%E5%AD%A6%E4%B8%8E%E9%87%91%E8%9E%8D%E9%A3%8E%E6%8E%A7%E6%A8%A1%E5%9E%8B.md)     
**简介**  众所周知，信息时代下的数据就是能源，就是生产力。但是面对海量、纷繁的数据，特别是在金融领域，如何充分地利用数据是核心问题。本次分享主要想和大家一起探讨下，在金融风控场景下，如何通过数据对齐模型和业务目标，哪些数据、方法可以应用于风控模型，通过哪些指标可以正确地评估模型效果，以及最终如何用数据科学解释模型结果。本报告围绕下面四点展开：科学定义数据、科学应用数据、科学评估数据、科学解释数据。   
<br/>   


### <span id='graphrisk'>图机器学习在度小满风控中的应用</span> 
**全文**  [图机器学习在度小满风控中的应用](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E5%9B%BE%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E5%9C%A8%E5%BA%A6%E5%B0%8F%E6%BB%A1%E9%A3%8E%E6%8E%A7%E4%B8%AD%E7%9A%84%E5%BA%94%E7%94%A8.md)    
**简介**  图机器学习是当前热门方向，各大金融科技公司都开始着手对图技术进行研究与应用。度小满使用图数据库去存储数据，并利用图分析算法来甄别团伙欺诈行为，极大程度提高了数据存储和挖掘能力，同时为金融风控业务提供实时有效的风险信息。本报告主要通过应用方法和案例解读，为大家在图机器学习落地产品化方面提供参考，并展示了度小满超大规模图平台Eros的框架和在度小满的应用。    
![graph_risk](https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E5%9B%BE%E5%9C%A8%E9%87%91%E8%9E%8D%E9%A2%86%E5%9F%9F%E7%9A%84%E5%BA%94%E7%94%A8%E6%BC%94%E8%BF%9B2.PNG)    
<br/>


## 因果推断   
### <span id='causal1'>因果推断在度小满金融场景的应用探索</span> 
**全文**  [因果推断在度小满金融场景的应用探索](https://mp.weixin.qq.com/s/jZbSTKSC0G1VC6qz0VaVfA)    
**简介**  因果推断类问题，是以因果输出作为基础，解决带有约束条件的全局最优化问题。具体到度小满所在信贷场景，我们团队主要聚焦在两类问题上：    
- 一是通过因果推断做 Offer 优化。Offer 会影响到用户风险的变化，在 Offer 优化场景下，我们希望在控制风险的前提下，给用户配置不同的额度和定价，从而达到盈利最优。
- 二是存在一些运营的手段，在控制成本的情况下，给用户配置不同的运营手段，从而达到 ROI 最大化。
<img src="https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E5%9B%A0%E6%9E%9C%E6%8E%A8%E6%96%AD%E5%9C%A8%E5%BA%A6%E5%B0%8F%E6%BB%A1%E7%9A%84%E5%BA%94%E7%94%A8-%E8%A7%82%E6%B5%8B%E6%B5%81%E9%87%8F%E5%BB%BA%E6%A8%A1.PNG" width=550 height=300 />
<br/>

### <span id='amountlimit'>基于反事实因果推断的金融额度模型</span> 
**全文**  [基于反事实因果推断的金融额度模型](https://www.modb.pro/doc/94287)    
**简介**   基于关联的机器学习已经在金融科技领域有着广泛而成熟的应用。在用户申请额度之前，平台会通过其历史征信记录，来初步识别用户的潜在需求和违约风险(逾期率)。平台授予用户的额度会进一步影响用户的逾期率。通常认为，授信额度与逾期率呈现正相关关系。但历史数据往往呈现出辛普森悖论，即高额度优质用户的逾期率显著低于一般用户。传统机器学习无法解决额度与风险的悖论关系，必须借助因果推断做反事实估计。本报告将主要向大家介绍，团队从0到1地在大规模观测样本上，利用因果表示学习搭建额度模型框架，并且取得了突破性的业务收益。。
<img src="https://github.com/Duxiaoman-DI/Duxiaoman-talk/blob/main/%E5%8F%8D%E4%BA%8B%E5%AE%9E%E9%A2%9D%E5%BA%A6%E6%A8%A1%E5%9E%8B.png" width=550 height=300 />
<br/>

