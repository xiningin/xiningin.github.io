---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<!-- 
{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %} -->

<span class='anchor' id='about-me'></span>

I am currently pursuing a master's degree in the [HCP Laboratory](https://www.sysu-hcp.net/home/) <img src='images/hcp.jpg' style='width: 1.2em;'> at Sun Yat-sen University in Guangzhou, ​​under the supervision of [​​Professor Liang Lin (林倞)](http://www.linliang.net/)​​, cooperating with [Associate Professor Pengxu Wei (魏朋旭)](https://pengxuwei.github.io/).

I graduated from Software Engineering College, [Northeast University](http://www.neu.edu.cn/)(东北大学软件学院) with a bachelor's degree. 

During my undergraduate studies, I served as a research intern in [Associate Professor Shi Feng (冯时)](https://neu-datamining.github.io/cse/fengshi/)'s [NEU Data Mining group](https://neu-datamining.github.io/), where I conducted research on **Image-Text Multimodal Sentiment Analysis**. 

Following my undergraduate studies, I joined [DISC Lab](http://www.fudan-disc.com/) <img src='images/disc.jpg' style='width: 1.2em;'> led by [Associate Professor Zhongyu Wei (魏忠钰)](http://www.fudan-disc.com/people/zywei) at Fudan University as a long-term research intern, focusing on the systematic evaluation and interpretability analysis of **Large Vision-Language Models** (e.g., LLaVA).

I won the National Scholarship (国家奖学金), the First Prize Scholarship of the College (院级优秀学生一等奖), the First Prize of the [Yonyou Network Technology Scholarship](https://neunews.neu.edu.cn/info/1005/191311.htm) (用友奖学金一等奖), etc.

My research interest includes **Video/Image Generation** and **Large Vision Language Model**. 

<!-- # 🔥 News
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  -->

# 🏛️ Publications 
<span class='anchor' id='publications'></span>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICCV 2025</div><img src='images\convdiff.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Can We Achieve Efficient Diffusion without Self-Attention Distilling Self-Attention into Convolutions](https://arxiv.org/pdf/2504.21292)

ZiYi Dong, <u>Chengxing Zhou</u>, Weijian Deng, Pengxu Wei, Xiangyang Ji, Liang Lin

<!-- `TLDR` We analyze self-attention scores in SDXL/PixArt/Flux, identifying low-frequency bias and high-frequency local signals.  These are replaced with pooling layers and multi-scale CNNs via distillation, maintaining quality while reducing computation and accelerating generation. -->
`TLDR` We propose **$\Delta$-ConvBlocks**, a novel module for image generation models (e.g., SDXL, PixArt) based on **multi-scale CNNs and adaptive pooling**, which distills the self-attention mechanism. Compared to linear-attention modules (also with $O(n)$ complexity), our design **reduces computational cost by 5.42×** while **maintaining comparable generation quality**.  
</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACL 2025</div><img src='images/VisionRegion.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Activating Distributed Visual Region within LLMs for Efficient and Effective Vision-Language Training and Inference](https://arxiv.org/pdf/2412.12785)

Siyuan Wang, Dianyi Wang, <u>Chengxing Zhou</u>(共一), Zejun Li, Zhihao Fan, Xuanjing Huang, Zhongyu Wei

<!-- `TLDR` This study offers an effective and efficient strategy for LVLM training and inference by activating a layer-wise visual region within LLMs, which proves consistently effective across different models. -->
`TLDR` We propose an efficient training strategy for large vision-language models, where only **25% of sparsely and uniformly distributed layer-wise parameters** (the "visual cortex" of the large language model) in the backbone LLM are fine-tuned. **This approach reduces training time by 23% while retaining nearly 99% of visual performance and slightly improving pure text processing capability.**
</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACMMM 2024</div><img src='images/ReFormEval.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[REFORM-EVAL: Evaluating Large Vision Language Models via Unified Re-Formulation of Task-Oriented Benckmarks](https://dl.acm.org/doi/abs/10.1145/3664647.3681529)

Zejun Li, Ye Wang, Mengfei Du, Qingwen Liu, Binhao Wu, Jiwen Zhang, <u>Chengxing Zhou</u> Zhihao Fan, Jie Fu, Jingjing Chen, Zhongyu Wei, Xuanjing Huang

`TLDR` This work proposes to re-formulate existing benchmarks into unified LVLM-compatible formats, and presents the ReForm-Eval benchmark, **an open-sourced benchmark and evaluation framework** offering substantial data for **evaluating various capabilities of LVLMs**.

</div>
</div>

# 📝 Projects
<span class='anchor' id='projects'></span>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <img src='images\MultiScaleIR.png' alt="sym" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

  **底层视觉下游任务通用大模型 Denoise Anything**


  `TLDR` We propose a **unified diffusion-based framework** for low-level vision tasks, where image denoising, over/under-exposure correction, and related problems are uniformly modeled as **degenerated noise removal**. Our approach **outperforms existing all-in-one methods** on standard metrics (PSNR, SSIM, LPIPS) and even **surpasses task-specific state-of-the-art models** in certain applications (e.g., dehazing, desnowing).  


  <!-- Zejun Li, Ye Wang, Mengfei Du, Qingwen Liu, Binhao Wu, Jiwen Zhang, <u>Chengxing Zhou</u> Zhihao Fan, Jie Fu, Jingjing Chen, Zhongyu Wei, Xuanjing Huang -->

  <!-- `TLDR` This work proposes to re-formulate existing benchmarks into unified LVLM-compatible formats, and presents the ReForm-Eval benchmark, an open-sourced benchmark and evaluation framework offering substantial data for evaluating various capabilities of LVLMs. -->

  </div>
</div>


# 🎖 Honors and Awards
<span class='anchor' id='honors-and-awards'></span>
- *2023.03* **National Gold Medal** 
'Challenge Cup' National College Student Business Plan Competition ([第十三届“挑战杯”中国大学生创业计划竞赛](https://www.tiaozhanbei.net/)).
- *2022.08* **National Second Prize** 
WeChat Mini Program & Mini Game Development Competition, a national-tier segment of the China Collegiate Computing Contest ([2022年中国高校计算机大赛微信小程序、小游戏应用开发赛](https://developers.weixin.qq.com/community/competition/intro)).
- *2022.10* **Provincial First Prize** 
with subsequent nomination for National First Prize evaluation China Undergraduate Mathematical Contest in Modeling (MCM, [2022年高教社杯全国大学生数学建模竞赛](https://www.mcm.edu.cn/)).
- *2022.09* **Provincial Gold Medal**
China College Students' Internet+ Innovation and Entrepreneurship Competition ([“建行杯”辽宁省第八届“互联网+”大学生创新创业大赛](https://cy.ncss.cn/))

# 🎓 Educations
<span class='anchor' id='educations'></span>
- *2024.09 - now*, I am currently pursuing a Master of Science degree in Computer Science at Sun Yat-sen University (中山大学计算机学院) <img src='images/sysucs.jpg' style='width: 2.4em;'>, where I conduct research in the Human Cyber Physical Intelligence Integration Lab ([HCP Lab](https://www.sysu-hcp.net/home/)).
- *2020.09 - 2024.06*, I earned my Bachelor's degree in Software Engineering College at Northeastern University (东北大学软件学院) <img src='images/neuse.jpg' style='width: 2.8em;'> before being admitted through recommendation exemption to Sun Yat-sen University's Computer Science College.

# 💬 ​More About Me
<span class='anchor' id='more-about-me'></span>
🤖 I'm deeply passionate about cutting-edge AI technologies and committed to developing solid, practical, and interesting work that creates real-world impact. 🔬 My research interests span across multiple domains of artificial intelligence, with particular enthusiasm for implementable solutions.

Beyond my professional pursuits, I maintain diverse hobbies including ✈️ traveling, 🏃 running, 🎮 PC gaming, and 🎲 board games - all of which continuously inspire my technical work with fresh perspectives.

😆 I'm always open to meaningful discussions about technology or casual hangouts. 📬 Feel free to reach out via email or connect on WeChat (xxxiiinnggg) - whether you'd like to 💡 exchange ideas about AI or 🎉 organize a game night!
