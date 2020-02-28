# Nature Medicine：单细胞RNA-seq筛选免疫检查点阻滞剂持续响应的血液标志物

免疫检查点阻滞剂（immune checkpoint blockades，ICBs）在黑色素瘤治疗上取得了重大进展，已应用于临床的ICBs包括抗CTLA-4 单抗、抗PD-1及其配体PD-L1单抗等。部分患者在疾病缓解的一段时间后出现耐药，甚至绝大多数患者初治就对ICB不敏感。因此，揭示患者对ICB的应答敏感性/耐药机制及其重要。药物应答或耐药问题仍是临床上待解决的难题，那么单细胞测序是如何帮助解决此类问题的？

2020年2月10日发表于Nature Medicine杂志的文章**应用强大的单细胞RNAseq技术揭示了CD8+T细胞可以作为转移性黑色素瘤患者对免疫检查点抑制剂治疗药物持续应答的血液标志物**。

![image](https://github.com/HIT-ImmunologyLab/single-cell-reference/raw/master/images/zhoufx/file_name.png)

## 背景
通常免疫检查点阻滞剂（ICB）的敏感性是由肿瘤属性决定的，即可以根据肿瘤负载、淋巴细胞浸润等肿瘤特征获知ICB治疗的敏感性、推测肿瘤免疫治疗相关的敏感性标志物。已有文献通过大规模的外周血免疫亚群细胞转录组数据分析，发现一些保守的预后标志物也与机体ICB药物应答反应相关。因此，与表征肿瘤特征无关的基因对ICB治疗后患者应答机制的调控值得探讨。目前免疫治疗过程中对外周血标志物的有效性评价是缺乏的。

CD8+ T细胞在黑色素瘤的免疫响应中起着关键作用，因此作者着重探讨患者CD8+ T在ICB治疗过程中的响应机制。

文章脉络：

1.外周血与组织样本RNA-seq分析差异基因和关键通路；

2.TCR RNA-seq分析T细胞免疫应答状态；

3.流式细胞术及单细胞测序识别起关键调节作用的CD8+T细胞类型；

4.单细胞测序深入探讨可能影响患者持续免疫应答的分子机制。


## 1.外周血RNA-seq发现了什么？
患者治疗后与治疗前比较：通过比较黑色素瘤患者治疗后21天与治疗前（day 0）CD8+ T的转录组表达数据。抗PD-1、抗CTLA-4联合治疗（cICB）与单独抗PD-1（sICB）患者差异基因存在部分交集，能够引起相似的功能效应（图1a-c）。

cICB治疗与 sICB治疗比较：对接受2种方案治疗的患者观察发现，大多数的差异基因会在患者接受sICB治疗的第4个疗程中消失，而cICB联合治疗的患者仍有稳定的差异基因表达。提示从转录组水平看，cICB治疗效果可能更加稳定。接着GSAE分析差异基因（cICB组vs. sICB组）参与的信号通路，推测cICB治疗可能会增强细胞增殖、抑制炎症发生（图1f）。

![image](https://github.com/HIT-ImmunologyLab/single-cell-reference/raw/master/images/zhoufx/figure1.webp)

图中ipiNivo是分别针对PD-1、CTLA4的两种免疫治疗药物；pembro指针对PD-1的免疫治疗药物

## 2.组织样本转录组分析：识别患者长期响应的相关信号通路 

将治疗6个月设定为关键的时间节点，根据患者接受ICB治疗6个月时有无响应分为响应组与进展组。

CD8+T细胞RNA-seq数据分析结果显示：患者长期响应的机制与TCR信号通路、G2/M转换正相关；与MAPKK、Toll样受体信号通路负相关（图2a、b）。

![image](https://github.com/HIT-ImmunologyLab/single-cell-reference/raw/master/images/zhoufx/figure2.webp)

## 3. TCR（T细胞受体） RNA-seq分析：
由于TRAV-、TRBV-分别编码TCR α链和β链，通过qPCR及富集分析发现：6个月时仍维持响应的患者组织CD8+T细胞TRAV-、TRBV-高表达，TRA、TRB基因与患者预后相关（图3c、d）。患者能否响应及能否长期响应与ICB治疗后21天TCR克隆数有关（图3f、h）

![image](https://github.com/HIT-ImmunologyLab/single-cell-reference/raw/master/images/zhoufx/figure3.webp)

![image](https://github.com/HIT-ImmunologyLab/single-cell-reference/raw/master/images/zhoufx/figure4.webp)

## 4.探讨TCR large克隆数对转移性黑色素瘤患者治疗、预后的重要性：

作者将TCR每链中占总克隆数>0.5%的克隆称作“large”，可理解为TCR富集程度高的克隆。

Large克隆数可以反映转移性黑色素瘤患者对ICB治疗的应答程度，并且是一个重要的预后指标(图4a、d)。

![image](https://github.com/HIT-ImmunologyLab/single-cell-reference/raw/master/images/zhoufx/figure5.webp)

## 5. TCR large克隆青睐于哪种T细胞？
首先，作者想到了最常用的流式方法根据细胞表面分子标记进行鉴定，采集ICB治疗患者PBMC样本，分析结果表明：CD8+效应性记忆T细胞数与large克隆数高度相关（图5f），而与CD4+T细胞无明显相关性。证实机体IBC药物应答过程中CD8+T细胞的特异性。

![image](https://github.com/HIT-ImmunologyLab/single-cell-reference/raw/master/images/zhoufx/figure6.webp)

## 单细胞测序发现了什么？
单细胞测序可以对样本进行单个细胞的转录组分析，根据转录组特征识别已知或未知的细胞亚群，在鉴别ICB应答反应中发挥作用的T细胞类型时展现出巨大潜力。

ICB治疗患者的血液样本经PBMC分离后做单细胞转录组分析，得到4个细胞亚群，其中cluster 4有效应性记忆T细胞的特征，并与cluster 1 中一少部分细胞共同构成large克隆TCR的T细胞（图6a、b、e）。large细胞群与其余细胞亚群相比，large克隆TCR的T细胞有独特的细胞毒性表达谱（图6f、g）。这些细胞毒性分子的差异表达可能是黑色素瘤患者ICB药物应答过程中的关键机制。

![image](https://github.com/HIT-ImmunologyLab/single-cell-reference/raw/master/images/zhoufx/figure8.webp)

## 总结
转移性黑色素瘤患者的转录组数据分析与TCR分析、单细胞测序技术相结合，巧妙地证实效应性记忆T细胞在ICB治疗过程中，黑色素瘤患者持续响应的重要作用。可能通过增加大克隆数量、消耗小克隆数量的方式，或过表达效应性记忆T细胞、细胞毒性T细胞特征性基因CCL4、GNLY和NKG7等方式，影响TCR的信号传递过程。外周血CD8+ T细胞可作为转移性黑色素瘤免疫检查点抑制剂持续响应的血液标志物，将为未来临床更加精准的用药提供很好的指导。

## Reference
1. Peripheral CD8+ T cell characteristics associated with durable responses to immune checkpoint blockade in patients with metastatic melanoma （https://doi.org/10.1038/s41591-019-0734-6）
2. 分析帖子： https://mp.weixin.qq.com/s/z11G7s-ZaLeVIkLz_IrOqw
3. 源码： https://bitbucket.org/Fairfaxlab/identification-of-peripheral-cd8-t-cell-subsets-associated/src/master/