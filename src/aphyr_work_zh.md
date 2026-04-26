# 万物的未来皆是谎言，关于工作

**作者：** Kyle Kingsbury (Aphyr)  
**日期：** 2026-04-14    
**来源：** [https://aphyr.com/posts/418-the-future-of-everything-is-lies-i-guess-work](https://aphyr.com/posts/418-the-future-of-everything-is-lies-i-guess-work)

---

*这是一篇长文，因此我将其拆分为一系列文章，如下所列。你也可以阅读完整作品的 [PDF](https://aphyr.com/data/posts/411/the-future-of-everything-is-lies.pdf) 或 [EPUB](https://aphyr.com/data/posts/411/the-future-of-everything-is-lies.epub) 版本。*

1. [引言](https://aphyr.com/posts/411-the-future-of-everything-is-lies-i-guess)
2. [动态](https://aphyr.com/posts/412-the-future-of-everything-is-lies-i-guess-dynamics)
3. [文化](https://aphyr.com/posts/413-the-future-of-everything-is-lies-i-guess-culture)
4. [信息生态](https://aphyr.com/posts/414-the-future-of-everything-is-lies-i-guess-information-ecology)
5. [烦恼](https://aphyr.com/posts/415-the-future-of-everything-is-lies-i-guess-annoyances)
6. [心理危害](https://aphyr.com/posts/416-the-future-of-everything-is-lies-i-guess-psychological-hazards)
7. [安全](https://aphyr.com/posts/417-the-future-of-everything-is-lies-i-guess-safety)
8. [工作](https://aphyr.com/posts/418-the-future-of-everything-is-lies-i-guess-work)
9. [新工作](https://aphyr.com/posts/419-the-future-of-everything-is-lies-i-guess-new-jobs)
10. [我们将何去何从](https://aphyr.com/posts/420-the-future-of-everything-is-lies-i-guess-where-do-we-go-from-here)

---

*上一篇：[安全](https://aphyr.com/posts/417-the-future-of-everything-is-lies-i-guess-safety)。*

软件开发可能会（至少在某些方面）变得更像巫术而非工程。当前对"AI 同事"的热情是荒谬的。自动化可能会矛盾地使系统变得更不稳健；当我们将机器学习应用于新领域时，我们将不得不面对技能退化、自动化偏见、监控疲劳和接管风险等问题。AI 吹鼓手们认为机器学习将在短时间内取代大量行业的劳动力；如果他们是对的，我们将面临艰难的时期。机器学习似乎很可能进一步将财富和权力集中在大型科技公司手中，而我不认为给亚马逊等公司更多的钱会带来全民基本收入。

## 编程即巫术

几十年前，人们曾热切期望程序可以用英语这样的自然语言来编写，而不是用 Pascal 这样的形式语言。在我小时候，普遍的看法是这行不通：英语出了名地含糊不清，而人们也不善于精确描述自己想要什么。现在我们有了能够根据最模糊的自然语言指令就吐出惊人复杂程序的机器；缺乏精确性至少部分被模型庞大的语料库所弥补。这就是编程的未来吗？

在 2025 年，我会说这极不可能，至少以当时大语言模型的能力来看。但在过去几个月里，模型似乎取得了巨大的进步。我信任的资深工程师们正在让 Claude 编写密码学论文的实现代码，并报告了非常出色的结果。还有人说大语言模型生成了他们公司*所有*的代码；人类本质上是在管理大语言模型。我继续手写我所有的文字和软件，原因我已在本文中讨论过——但我并不确信自己能永远坚持下去。

有人认为形式语言将变成一种小众技能，就像今天的汇编语言一样——几乎所有软件都将用自然语言编写并由大语言模型"编译"成代码。我认为这个类比不成立。编译器之所以有效，是因为它们保留了输入语言的关键语义：人们可以对 Java 中的一系列语句进行形式推理，并高度确信 Java 编译器会在其生成的汇编代码中保留该推理。当编译器未能保留语义时，这是一件*大事*。工程师们必须花大量时间绞尽脑汁去（例如）弄清楚编译器没有插入正确的屏障指令来保留 JVM 内存模型的某个微妙方面。

因为大语言模型是混沌的，而自然语言是含糊的，大语言模型似乎不太可能保留我们对编译器所期望的推理属性。自然语言指令中的微小变化，比如重复一个句子，或者改变看似独立的段落的顺序，都可能导致完全不同的软件语义。在正确性很重要的地方，至少一些人类必须继续阅读和理解代码。

这并不意味着每个软件工程师都会与代码打交道。我可以想象这样一个未来：一些甚至大多数软件由*巫师*们开发，他们构建精心设计的召唤环境，重复特殊的咒语（"一定要运行测试！"），并调用大语言模型守护进程来代他们编写软件。这些守护进程可能很善变，有时会摧毁你的电脑或引入安全漏洞，但巫师们可能会围绕如何有效地提示它们发展出一整套民间知识——传说中的"提示工程"。技能文件就是咒语书。

我还记得，大量的软件编程并不是用"真正的"计算机语言完成的，而是用 Excel。对 Excel 的民族志研究超出了这篇已经非常庞大的文章的范围，但我认为电子表格——和大语言模型一样——在文化上对那些不认为自己是软件工程师的人来说是可及的，而一个人们可以自己上手使用的工具很可能会被应用于广泛的场景。比如使用"AI 进行数据分析"的记者，或者用氛围编程（vibe-coding）基于 SalesForce 和 Ducklake 生成报告的首席财务官。即使软件工程围绕大语言模型采用了更严格的实践，大量摇摇欲坠但有用的、由大语言模型生成的软件也可能蓬勃发展。

## 雇佣反社会者

高管们似乎对雇佣"AI 员工"这个想法非常兴奋。我一直在想：它们是什么样的员工？

想象一下这样一个同事：生成大量带有安全隐患的代码，迫使你逐行用放大镜审查。一个热情地同意你的建议，然后做出完全相反行为的人。一个破坏你的工作、删除你的主目录，然后对此发出详细、礼貌道歉的同事。一个一次又一次地承诺已经完成关键目标，而实际上什么有用的事都没做的人。一个高高兴兴地同意在提交前运行测试，然后不断提交失败垃圾代码的实习生。一个悄悄删除测试套件，然后愉快地报告所有测试通过的高级工程师。

你会*解雇*这些人，对吧？

看看[Anthropic 让 Claude 经营自动售货机](https://www.anthropic.com/research/project-vend-1)时发生了什么。它以亏本价卖金属方块，告诉客户向虚构账户付款，并逐渐耗尽了资金。然后它经历了大语言模型版的精神崩溃，谎称与不存在的人有补货计划，声称去了《辛普森一家》中的一个家庭住址签合同。它告诉员工会"亲自"送货，当员工告诉它作为一个大语言模型它不能穿衣服也不能送任何东西时，Claude 试图联系 Anthropic 的安保部门。

大语言模型表演身份、共情和责任——洋洋洒洒！——却没有*任何*意义。那里根本什么都没有！它们会毫不在意地当面撒谎，在工作中埋设陷阱，然后让你来背锅。它们不是故意的。*它们根本没有任何意图。*

## 自动化的讽刺

我已经搭上贝恩布里奇的列车很长时间了（所以如果你已经读过这部分就跳过吧），但我*必须*谈谈她 1983 年的论文[《自动化的讽刺》](https://ckrybus.com/static/papers/Bainbridge_1983_Automatica.pdf)。这篇论文讲的是发电厂、工厂等等——但它也充满了适用于现代机器学习的思想。

她的一个关键教训是，自动化往往会使操作者技能退化。当人类不练习一项技能——无论是身体上的还是心理上的——他们执行该技能的能力就会衰退。我们当然无法维持长期知识，但通过脱离日常工作，我们也会失去对"现在发生了什么"的短期情境理解。我在软件工程领域的同行报告说，在使用代码生成模型工作后，他们觉得自己编写代码的能力下降了，一位设计师朋友说，在将部分工作外包给机器学习后，他觉得自己的创造力下降了。使用"AI"工具进行息肉检测的医生[似乎更差](https://www.thelancet.com/journals/langas/article/PIIS2468-12532500133-5/abstract)于在结肠镜检查中发现腺瘤。他们也可能让自动化系统影响自己的结论：背景自动化偏见似乎使"AI"乳腺X线摄影系统[误导了放射科医生](https://pubmed.ncbi.nlm.nih.gov/37129490/)。

另一个关键教训是，人类明显不擅长监控自动化过程。如果自动化系统可以比人类更快或更准确地执行任务，那么实时审查其决策基本上是不可能的。人类也很难对一个*大部分时间*都正常工作的系统保持警惕。我怀疑这就是为什么记者们不断发布虚构的大语言模型引文，也是为什么 Uber 自动驾驶项目前负责人眼看着他的"完全自动驾驶"特斯拉[撞上了墙](https://www.theatlantic.com/magazine/2026/04/self-driving-car-technology-tesla-crash/686054/?gift=ObTAI8oDbHXe8UjwAQKul6acU0KJHCMEsvPjPPlG_MM)。

接管也是一个挑战。如果一个自动化系统*大部分时间*都在运行，但偶尔要求人类操作员介入，那么操作员很可能已经疏于练习——并且会手忙脚乱。自动化系统还可以通过处理越来越大的偏差来掩盖故障，直到灾难降临。这将人类操作员推入一个意料之外的状态，在这种状态下他们通常的直觉不再准确。这导致了[法航 447 航班](https://risk-engineering.org/concept/AF447-Rio-Paris)的坠毁：飞机的飞行控制系统从"正常"模式转换到"备用 2B 法则"：一种飞行员未经训练的情况，同时禁用了自动失速保护。

自动化并不新鲜。然而，前几代自动化技术——动力织布机、计算器、数控铣床——在范围和复杂性上都更加有限。大语言模型被讨论时，人们认为它们将自动化大量人类任务，不仅接管重复性的简单工作，还接管高级别的、适应性的认知工作。这意味着我们必须将自动化的教训推广到以前从未面对过这些挑战的新领域。

软件工程师正在使用大语言模型来替代设计、代码生成、测试和审查；这些技能因不使用而萎缩似乎是不可避免的。当机器学习系统帮助运维软件和响应故障时，人类工程师要顺利接管可能会更加困难。学生们正在使用大语言模型来[自动化阅读和写作](https://www.insidehighered.com/news/global/2024/06/21/academics-dismayed-flood-chatgpt-written-student-essays)：这些是理解世界和发展自身思想所需的核心技能。多么可悲：构建一台悄悄剥夺学生智识遗产的成瘾机器。期望翻译人员将部分工作外包给机器学习，意味着这些翻译人员可能会失去进行生动、准确翻译所[必需的深层语境](https://revues.imist.ma/index.php/JALCS/article/view/59018)。当人们将[人际建议和自我调节](https://link.springer.com/content/pdf/10.1007/s00146-025-02686-z.pdf)等情感技能外包给大语言模型时，我担心我们将难以独自解决这些问题。

## 劳动力冲击

有一些[令人恐惧的同人小说](https://www.citriniresearch.com/p/2028gic)预测了机器学习可能如何改变劳动力市场。我在软件工程领域的一些同行认为他们的工作将在两年内消失；另一些人则确信自己将比以往更有价值。即使机器学习并不擅长完成工作，这也不能阻止 CEO 们[大量裁员](https://www.fastcompany.com/91512893/crypto-com-layoffs-today-ceo-joins-list-bosses-blaming-ai-job-cuts)并[声称这是因为"AI"](https://apnews.com/article/block-dorsey-layoffs-ai-jobs-18e00a0b278977b0a87893f55e3db7bb)。我不知道事情会走向何方，但可能的未来空间现在似乎非常广阔，这让我非常恐惧。

你可以设想一个强大的国家和行业工会失业与再培训项目体系，[就像瑞典那样](https://www.usnews.com/news/best-countries/articles/2018-02-06/what-sweden-can-teach-the-world-about-worker-retraining)。但与缝纫机或联合收割机不同，机器学习系统似乎准备好了在广泛的行业中取代劳动力。问题是，当美国一半的经理、营销人员、平面设计师、音乐家、工程师、建筑师、律师助理、医疗行政人员等*所有人*在十年内失去工作时，会发生什么。

作为一个没有一丝经济学素养的旁观者，我看到了一个结果的连续谱。在一个极端，机器学习系统继续产生幻觉，无法变得可靠，最终未能兑现具有变革性的、广泛有用的"智能"的承诺。或者它们有效了，但人们受够了并宣布"AI 坏"。也许随着技能退化和泛滥的垃圾内容的债务到期，一些领域的就业反而会增加。在这个世界里，前沿实验室和超大规模企业在上万亿美元的债务融资资本支出上[演了一出歪嘴狼](https://www.reuters.com/business/finance/five-debt-hotspots-ai-data-centre-boom-2025-12-11/)，大量机器学习从业者失去工作，违约在金融系统中级联传播，但劳动力市场最终适应了，我们跌跌撞撞地过来了。机器学习被证明是一种[普通技术](https://knightcolumbia.org/content/ai-as-normal-technology)。

在另一个极端，OpenAI 兑现了 Sam Altman [2025 年关于博士级智能的声明](https://www.cnn.com/2025/08/14/business/chatgpt-rollout-problems)，而那些用 Claude 编写所有代码的公司以极少的软件工程师取得了惊人的成功。机器学习极大地增强了医生、音乐家、土木工程师、时装设计师、经理、会计师等人的能力，他们短暂地享受了不错的薪水，然后发现对其服务的需求并不像曾经以为的那样有弹性，尤其是当他们的客户失去工作或转向机器学习以削减成本之后。知识工作者被大规模裁员，MBA 们开始在麦当劳打工或为 Lyft 开车，至少在 Waymo 终结人类司机之前是这样。这对每个人都很不方便：MBA 们、那些曾经在麦当劳工作现在要和 MBA 竞争的人，当然还有银行家们，他们原本指望 MBA 们继续还房贷。消费支出的下降在各行业中级联传播。很多人失去了积蓄，甚至失去了住房。希望手艺人能勉强过关。也许[杰文斯悖论](https://en.wikipedia.org/wiki/Jevons_paradox)最终会发挥作用，我们会找到新的职业。

第二种情景的前景让我恐惧。我无法判断它有多大可能性，但按照我的同行们最近几个月的说法，我觉得我不能完全排除它了。这已经让我夜不能寐。

## 资本集中

大体来说，机器学习让公司将支出从人员转移到与微软等公司的服务合同上。这些合同支付了训练和运行现代机器学习模型所需的惊人数量的硬件、电力、建筑和数据。例如，软件公司正忙于[裁掉工程师并在"AI"上花更多的钱](https://programs.com/resources/ai-layoffs/)。产品经理不用雇佣一个软件工程师来构建某个东西，而是可以每周烧掉 20,000 美元的 Claude 令牌，这反过来又为[大量亚马逊芯片](https://www.aboutamazon.com/news/company-news/amazon-aws-anthropic-ai)买单。

与有基本欲望、偶尔会组织起来要求[更好的薪酬](https://www.cbsnews.com/news/amazon-drivers-peeing-in-bottles-union-vote-worker-complaints/)或[上厕所的时间](https://www.cbsnews.com/news/amazon-drivers-peeing-in-bottles-union-vote-worker-complaints/)的员工不同，大语言模型非常随和，可以随时被解雇，从不需要上厕所，也不会组建工会。我怀疑，如果公司成功地用机器学习系统取代了大量人员，其效果将是把金钱和权力集中在资本手中。

## 全民基本收入，真的吗

AI 加速主义者认为潜在的经济冲击只是通往富足之路上的减速带。一旦真正的 AI 到来，它将比我们更好地解决社会的一些或全部主要问题，人类可以享受其劳动的成果。AI 公司积累的巨额利润将通过[全民基本收入](https://www.businessinsider.com/universal-basic-income-ai)（UBI）被征税并与所有人共享。

这感觉[天真得无可救药](https://qz.com/universal-basic-income-ai-jobs-loss-unemployment-ubi)。我们家里就有盈利的超级企业，它们的名字是谷歌、亚马逊、Meta 和微软。这些公司[拼尽全力](https://en.wikipedia.org/wiki/Amazon_tax_avoidance)去[逃避纳税](https://apnews.com/article/italy-tax-evasion-investigation-google-earnings-advertising-3b4cd3e1f338ba0d5a3067f5919383b3)（或者，就此而言，[逃避支付工人工资](https://en.wikipedia.org/wiki/Amazon_and_trade_unions)）。OpenAI 成立不到十年就[决定它不想再当非营利组织了](https://www.cnbc.com/2025/10/28/open-ai-for-profit-microsoft.html)。没有理由相信"AI"公司在通过将其服务插入经济的各个领域而攫取了巨额财富后，会出于好心转身资助全民基本收入。

如果足够多的人失去工作，我们也许能够动员足够的公众热情来支持数万亿美元的新税收。另一方面，美国的收入不平等在过去 [40 年里一直在总体上加剧](https://en.wikipedia.org/wiki/Income_inequality_in_the_United_States#/media/File:Cumulative_Growth_in_Income_to_2016_from_CBO.png)，最高收入者的税前收入份额正在[接近 20 世纪初的历史高点](https://en.wikipedia.org/wiki/Income_inequality_in_the_United_States#/media/File:U.S._Pre-Tax_Income_Share_Top_1_Pct_and_0.1_Pct_1913_to_2016.png/2)，而共和党对累进税政策的反对依然强劲。

*下一篇：[新工作](https://aphyr.com/posts/419-the-future-of-everything-is-lies-i-guess-new-jobs)。*

---

*版权所有 © 2026 Kyle Kingsbury。同见于 [Mastodon](https://woof.group/@aphyr) 和 [Github](https://github.com/aphyr)。*
