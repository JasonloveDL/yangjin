---
layout: archive
title: ""
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

<link rel="stylesheet" href="{{ '/assets/css/cv-enhancement.css' | relative_url }}">

<style>
/* 自定义CV样式 */

/* 隐藏Jekyll自动生成的页面标题 */
.page__title,
.archive__item-title,
h1.page__title,
.page-header h1,
.archive h1:first-child,
.archive__item h1,
header h1 {
  display: none !important;
}

/* 隐藏可能的空白标题容器 */
.page__title:empty,
h1:empty {
  display: none !important;
  margin: 0 !important;
  padding: 0 !important;
}

/* 确保内容区域紧凑 */
.archive__item-excerpt p:first-child {
  margin-top: 0;
}

/* 调整页面顶部间距 */
.archive {
  margin-top: 0 !important;
}

.page__content {
  margin-top: 0 !important;
}

.hero-section {
  background: linear-gradient(135deg, #2C3E50 0%, #34495E 100%);
  color: white;
  padding: 3rem 2rem;
  margin: -2rem -2rem 2rem -2rem;
  border-radius: 0 0 15px 15px;
  text-align: center;
}

.achievement-tags {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 1rem;
  margin: 1.5rem 0;
}

.tag {
  background: rgba(255, 255, 255, 0.2);
  color: white;
  padding: 0.5rem 1rem;
  border-radius: 25px;
  font-size: 0.9rem;
  font-weight: bold;
  backdrop-filter: blur(10px);
}

.tag.utd24 {
  background: linear-gradient(45deg, #2C3E50, #34495E);
  box-shadow: 0 3px 10px rgba(44, 62, 80, 0.3);
}

.tag.scholarship {
  background: linear-gradient(45deg, #2C3E50, #34495E);
  box-shadow: 0 3px 10px rgba(44, 62, 80, 0.3);
}

.tag.project {
  background: linear-gradient(45deg, #E67E22, #D35400);
  box-shadow: 0 3px 10px rgba(230, 126, 34, 0.4);
}

.achievements-highlights {
  margin: 2rem 0;
  padding: 2rem;
  background: #f8f9fa;
  border-radius: 15px;
}

.achievement-cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1.5rem;
  margin-top: 1rem;
}

.card {
  background: white;
  padding: 2rem;
  border-radius: 15px;
  text-align: center;
  box-shadow: 0 8px 25px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
}

.card:hover {
  transform: translateY(-5px);
}

.card .number {
  font-size: 2.5rem;
  font-weight: bold;
  color: #2C3E50;
  margin-bottom: 0.5rem;
}

.card .desc {
  color: #7f8c8d;
  line-height: 1.4;
}

/* 论文列表样式 */
.publications-list {
  margin: 2rem 0;
}

.publication-item {
  background: white;
  border-radius: 10px;
  padding: 1.5rem;
  margin: 1rem 0;
  box-shadow: 0 3px 10px rgba(0,0,0,0.08);
  display: flex;
  gap: 1rem;
}

.publication-item.featured {
  background: linear-gradient(135deg, #F8F9FA 0%, #E9ECEF 100%);
  border-left: 4px solid #2C3E50;
}

.pub-number {
  font-weight: bold;
  color: #2C3E50;
  min-width: 25px;
}

.pub-content {
  flex: 1;
}

.pub-text {
  line-height: 1.6;
  margin-bottom: 0.5rem;
  color: #333;
}

.utd-badge {
  background: #2C3E50;
  color: white;
  padding: 0.2rem 0.6rem;
  border-radius: 8px;
  font-size: 0.8rem;
  font-weight: bold;
}

.pub-links {
  display: flex;
  gap: 0.5rem;
}

.pub-links a {
  text-decoration: none;
  font-size: 1.2rem;
  padding: 0.3rem;
  border-radius: 5px;
  transition: transform 0.2s ease;
}

.pub-links a:hover {
  transform: scale(1.1);
}

/* 项目列表样式 */
.projects-list {
  margin: 2rem 0;
}

.project-item {
  background: white;
  border-radius: 10px;
  padding: 1.5rem;
  margin: 1rem 0;
  box-shadow: 0 3px 10px rgba(0,0,0,0.08);
}

.project-item.featured {
  background: linear-gradient(135deg, #F8F9FA 0%, #E9ECEF 100%);
  border-left: 4px solid #2C3E50;
}

.project-content {
  display: flex;
  align-items: center;
}

.project-text {
  line-height: 1.6;
  color: #333;
  flex: 1;
}

.journal-badge {
  display: inline-block;
  background: #F39C12;
  color: white;
  padding: 0.5rem 1rem;
  border-radius: 20px;
  font-size: 0.8rem;
  font-weight: bold;
  margin-bottom: 1rem;
}

.project-card {
  background: white;
  border-radius: 15px;
  padding: 2rem;
  margin: 1rem 0;
  box-shadow: 0 5px 20px rgba(0,0,0,0.1);
}

.project-card.featured {
  border-left: 5px solid #F39C12;
  background: linear-gradient(135deg, #FFF9F0 0%, #FFF5E6 100%);
}

.role-badge {
  background: #27AE60;
  color: white;
  padding: 0.3rem 0.8rem;
  border-radius: 15px;
  font-size: 0.8rem;
  font-weight: bold;
  margin-right: 1rem;
}

.amount {
  background: #E74C3C;
  color: white;
  padding: 0.3rem 0.8rem;
  border-radius: 15px;
  font-size: 0.8rem;
  font-weight: bold;
}

.section-header {
  color: #2C3E50;
  border-bottom: 2px solid #2C3E50;
  padding-bottom: 0.5rem;
  margin-bottom: 2rem;
  font-weight: 600;
}

.education-timeline {
  position: relative;
  padding-left: 2rem;
}

.education-timeline::before {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  width: 2px;
  background: #3498DB;
}

.education-item {
  position: relative;
  background: white;
  border-radius: 10px;
  padding: 1.5rem;
  margin-bottom: 1rem;
  box-shadow: 0 3px 15px rgba(0,0,0,0.1);
}

.education-item::before {
  content: '';
  position: absolute;
  left: -2rem;
  top: 1.5rem;
  width: 12px;
  height: 12px;
  background: #3498DB;
  border-radius: 50%;
  border: 3px solid white;
}

.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
  margin-top: 1rem;
}

.skill-category {
  background: white;
  border-radius: 15px;
  padding: 2rem;
  box-shadow: 0 5px 20px rgba(0,0,0,0.1);
}

.skill-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-top: 1rem;
}

.skill-tags span {
  background: #ECF0F1;
  color: #2C3E50;
  padding: 0.3rem 0.8rem;
  border-radius: 15px;
  font-size: 0.8rem;
}

/* 响应式设计 */
@media (max-width: 768px) {
  .hero-section {
    padding: 2rem 1rem;
    margin: -1rem -1rem 1rem -1rem;
  }
  
  .achievement-tags {
    flex-direction: column;
    align-items: center;
  }
  
  .achievement-cards {
    grid-template-columns: 1fr;
  }
  
  .skills-grid {
    grid-template-columns: 1fr;
  }
  
  /* 确保侧边栏在移动端有足够的高度 */
  .sidebar {
    min-height: auto !important;
  }
}

/* 侧边栏线性响应式设计 */
.author__avatar {
  /* 线性变化：从150px到100px，进一步增大最小尺寸 */
  max-width: clamp(100px, 18vw, 150px) !important;
  transition: all 0.3s ease;
}

.author__name {
  /* 字体线性变化：从1.5rem到1.1rem，增大最小字体 */
  font-size: clamp(1.1rem, 2.8vw, 1.5rem) !important;
  transition: all 0.3s ease;
  line-height: 1.3 !important;
}

.author__urls li {
  /* 联系方式字体线性变化：增大最小字体 */
  font-size: clamp(0.85rem, 2.2vw, 0.9rem) !important;
  transition: all 0.3s ease;
  line-height: 1.4 !important;
}

/* 平板和大屏手机布局 */
@media (max-width: 768px) and (min-width: 481px) {
  .sidebar {
    padding: 2rem 1.5rem !important;
  }
  
  .author__content {
    text-align: center;
  }
  
  .author__avatar {
    margin: 0 auto 1.8rem auto;
    max-width: clamp(130px, 22vw, 170px) !important; /* 进一步增大平板端头像 */
    border-radius: 50%;
  }
  
  .author__name {
    font-size: clamp(1.5rem, 3.5vw, 1.8rem) !important; /* 进一步增大平板端名字字体 */
    margin-bottom: 1.2rem;
    font-weight: 700;
    color: #2C3E50 !important;
  }
  
  .author__urls {
    justify-content: center;
    flex-wrap: wrap;
    gap: 1.2rem;
  }
  
  .author__urls li {
    margin: 0.5rem 0;
    font-size: clamp(1rem, 2.8vw, 1.2rem) !important; /* 进一步增大联系方式字体 */
    color: #34495E !important;
  }
  
  .author__urls li a {
    color: #2C3E50 !important;
    text-decoration: none;
  }
  
  .author__urls li a:hover {
    color: #3498DB !important;
  }
}

/* 很窄屏幕布局：左右排列 */
@media (max-width: 480px) {
  .sidebar {
    padding: 2rem 1.2rem !important; /* 进一步增大内边距 */
  }
  
  .author__avatar {
    margin: 0 !important;
    float: left;
    max-width: clamp(110px, 25vw, 140px) !important; /* 进一步显著增大头像尺寸 */
    border-radius: 50%; /* 确保头像为圆形 */
  }
  
  .author__content {
    margin-left: calc(clamp(110px, 25vw, 140px) + 1.8rem); /* 调整左边距 */
    text-align: left;
    min-height: clamp(140px, 30vw, 180px); /* 进一步增加容器高度 */
    display: flex;
    flex-direction: column;
    justify-content: flex-start; /* 顶部对齐 */
    padding-top: 0.8rem; /* 增加顶部内边距 */
  }
  
  .author__name {
    font-size: clamp(1.3rem, 4.5vw, 1.7rem) !important; /* 进一步增大名字字体 */
    margin-bottom: 0.8rem;
    line-height: 1.1;
    font-weight: 700;
    color: #2C3E50 !important; /* 添加颜色以增强可读性 */
  }
  
  .author__urls-wrapper {
    margin-top: 0.6rem;
    flex: 1;
  }
  
  .author__urls {
    margin: 0;
    padding: 0;
    flex-direction: column;
    gap: 0.6rem; /* 进一步增加行间距 */
  }
  
  .author__urls li {
    margin: 0;
    font-size: clamp(0.9rem, 3.2vw, 1.1rem) !important; /* 进一步增大联系方式字体 */
    line-height: 1.4;
    white-space: nowrap;
    overflow: visible;
    color: #34495E !important; /* 添加颜色 */
  }
  
  .author__urls li a {
    color: #2C3E50 !important; /* 链接颜色 */
    text-decoration: none;
  }
  
  .author__urls li a:hover {
    color: #3498DB !important; /* 悬停颜色 */
  }
  
  /* 清除浮动 */
  .author__urls-wrapper::after {
    content: "";
    display: table;
    clear: both;
  }
}

/* 打印样式 */
@media print {
  .hero-section {
    background: none !important;
    color: black !important;
    border: 2px solid #2C3E50;
  }
  
  .tag {
    background: none !important;
    color: black !important;
    border: 1px solid #2C3E50;
  }
  
  .card, .project-card, .education-item, .skill-category {
    box-shadow: none !important;
    border: 1px solid #ddd;
  }
}
</style>

<!-- Hero区域 -->
<div class="hero-section">
  <h1 style="font-size: 2.5rem; margin-bottom: 0.5rem;">杨晋</h1>
  <h2 style="font-size: 1.3rem; margin-bottom: 1rem; opacity: 0.9;">哈尔滨工业大学博士生（2026年毕业）</h2>
  <div class="achievement-tags">
    <span class="tag utd24">以第一作者身份发表UTD24期刊</span>
    <span class="tag project">国自然青年基础研究项目负责人(30万)</span>
    <span class="tag scholarship">获得24博士国家奖学金</span>
  </div>
  <p style="font-size: 1.1rem; margin-top: 1rem;">
    研究方向：<strong>管理科学与工程 × 人工智能交叉研究</strong>
  </p>
</div>

<!-- 学术研究 -->
<section>
  <h2 class="section-header">论文发表</h2>
  
  <div class="publications-list">
    <!-- UTD24期刊论文突出显示 -->
    <div class="publication-item featured">
      <div class="pub-number">1.</div>
      <div class="pub-content">
        <div class="pub-text"><strong>Jin Yang</strong>, Guangxin Jiang, Yinan Wang, Ying Chen* (2024) An Intelligent End-to-End Neural Architecture Search Framework for Electricity Forecasting Model Development. <em><u>INFORMS Journal on Computing</u></em>, 37(2):480-501. <span class="utd-badge">(UTD24)</span></div>
        <div class="pub-links">
          <a href="{{ '/files/Yang et al_2024_An Intelligent End-to-End Neural Architecture Search Framework for Electricity.pdf' | relative_url }}" target="_blank" title="下载PDF">📄</a>
          <a href="https://doi.org/10.1287/ijoc.2023.0034" target="_blank" title="DOI链接">🔗</a>
        </div>
      </div>
    </div>
    
    <div class="publication-item">
      <div class="pub-number">2.</div>
      <div class="pub-content">
        <div class="pub-text">Xiaojian Wang, Yinan Wang, <strong>Jin Yang</strong>, Ying Chen* (2024) Smartformer: An Intelligent Transformer Compression Framework for Time-Series Modeling. <em><u>IISE Transactions</u></em>, 1-14.</div>
        <div class="pub-links">
          <a href="{{ '/files/Smartformer An intelligent transformer compression framework for time-series modeling.pdf' | relative_url }}" target="_blank" title="下载PDF">📄</a>
          <a href="https://doi.org/10.1080/24725854.2024.2376645" target="_blank" title="DOI链接">🔗</a>
        </div>
      </div>
    </div>
    
    <div class="publication-item">
      <div class="pub-number">3.</div>
      <div class="pub-content">
        <div class="pub-text">Jiancheng Qin, <strong>Jin Yang</strong>, Ying Chen*, Qiang Ye, Hua Li. (2021). Two‐stage short‐term wind power forecasting algorithm using different feature-learning models. <em><u>Fundamental Research</u></em>, 1(4), 472–481.</div>
        <div class="pub-links">
          <a href="{{ '/files/Two-stage-short-term-wind-power-forecasting-algorithm-usin_2021_Fundamental-.pdf' | relative_url }}" target="_blank" title="下载PDF">📄</a>
          <a href="https://doi.org/10.1016/j.fmre.2021.06.010" target="_blank" title="DOI链接">🔗</a>
        </div>
      </div>
    </div>
    
    <div class="publication-item">
      <div class="pub-number">4.</div>
      <div class="pub-content">
        <div class="pub-text">Tao Huo, <strong>Jin Yang</strong>, Chengfei Yue, Xueqin Chen, Xibin Cao (2024) Gradient-based Attitude Planning for Rigid Spacecraft on SO(3). <em><u>Science China-Technological Sciences</u></em>, 68(5): 1520401.</div>
        <div class="pub-links">
          <a href="{{ '/files/s11431-024-2883-1.pdf' | relative_url }}" target="_blank" title="下载PDF">📄</a>
          <a href="https://doi.org/10.1007/s11431-024-2883-1" target="_blank" title="DOI链接">🔗</a>
        </div>
      </div>
    </div>
    
    <div class="publication-item">
      <div class="pub-number">5.</div>
      <div class="pub-content">
        <div class="pub-text">Tao Huo, <strong>Jin Yang</strong>, Yongsheng Luo, Chengfei Yue (2025). Predefined Time Control for Spacecraft with Uncertainty Using Exponential Coordinates. <em><u>23rd IFAC Symposium on Automatic Control in Aerospace</u></em>. (Accepted)</div>
      </div>
    </div>
  </div>
</section>

<!-- 专利 -->
<section style="margin-top: 3rem;">
  <h2 class="section-header">专利</h2>
  
  <div class="publications-list">
    <div class="publication-item">
      <div class="pub-number">1.</div>
      <div class="pub-content">
        <div class="pub-text">岳程斐;霍涛;杨晋;陈雪芹;曹喜滨.一种基于旋转矩阵拓扑结构的姿态路径规划方法、系统、设备和介质[P]. CN115014363A.</div>
      </div>
    </div>
  </div>
</section>

<!-- 工作论文 -->
<section style="margin-top: 3rem;">
  <h2 class="section-header">工作论文</h2>
  
  <div class="publications-list">
    <div class="publication-item">
      <div class="pub-number">1.</div>
      <div class="pub-content">
        <div class="pub-text"><strong>Jin Yang</strong>, Guangxin Jiang. Large Language Model Agents for Time Series Forecasting. Presented at the INFORMS International Conference 2025, Singapore. (Working paper)</div>
      </div>
    </div>
    
    <div class="publication-item">
      <div class="pub-number">2.</div>
      <div class="pub-content">
        <div class="pub-text">Tao Huo, <strong>Jin Yang</strong>, Chengfei Yue, Xueqin Chen, Xibin Cao. Hierarchical multi-terminal attitude planning for rigid-body spacecraft. <em><u>Science China-Information Sciences</u></em>. (Under review)</div>
      </div>
    </div>
    
    <div class="publication-item">
      <div class="pub-number">3.</div>
      <div class="pub-content">
        <div class="pub-text">姜广鑫, 江九运, 郝轶泽, <strong>杨晋</strong>. 人工智能驱动的金融工程研究: 投资组合选择、衍生品定价与风险管理中的进展. <em><u>系统工程理论与实践</u></em>. (Under review)</div>
      </div>
    </div>
    
    <div class="publication-item">
      <div class="pub-number">4.</div>
      <div class="pub-content">
        <div class="pub-text"><strong>Jin Yang</strong>, Guangxin Jiang. Gradient-Informed Neural Networks: Enhancing Deep Learning with Direct Stochastic Gradient Estimators. (Working paper)</div>
      </div>
    </div>
  </div>
</section>

<!-- 科研项目 -->
<section style="margin-top: 3rem;">
  <h2 class="section-header">科研项目</h2>
  
  <div class="projects-list">
    <!-- 主持项目突出 -->
    <div class="project-item featured">
      <div class="project-content">
        <div class="project-text">国家自然科学基金青年学生基础研究项目（博士研究生）, 724B2012, 基于智能化深度学习的复杂随机系统预测方法, 2025/01-2026/12, 30万, 在研, <strong>主持</strong></div>
      </div>
    </div>
    
    <div class="project-item featured">
      <div class="project-content">
        <div class="project-text">哈尔滨工业大学点子基金（青年学生类）, HIT.DZJJ.2024029, 基于先验知识的智能化深度学习预测方法及应用, 2024/08-2025/08, 3万, 在研, <strong>主持</strong></div>
      </div>
    </div>
    
    <div class="project-item">
      <div class="project-content">
        <div class="project-text">国家自然科学基金重大项目，72293562，复杂供应链网络风险传播机理和韧性评估, 2023/01-2027/12，225万，在研，骨干成员</div>
      </div>
    </div>
    
    <div class="project-item">
      <div class="project-content">
        <div class="project-text">中能公司风功率预测人工智能深度学习算法及软件采购，2019/06-2020/06，30万，骨干成员</div>
      </div>
    </div>
    
    <div class="project-item">
      <div class="project-content">
        <div class="project-text">人工智能技术在电力企业管理决策中的应用，2021/06-2021/12，50万，骨干成员</div>
      </div>
    </div>
    
    <div class="project-item">
      <div class="project-content">
        <div class="project-text">中央军委科技委智创项目, 201-CXCY-***-**-**-**, 复杂随机系统**********理论, 2021/01-2023/12，100万，结题，成员</div>
      </div>
    </div>
  </div>
</section>

<!-- 教育背景 -->
<section style="margin-top: 3rem;">
  <h2 class="section-header">教育背景</h2>
  <div class="education-timeline">
    <div class="education-item">
      <div style="font-size: 1.2rem; font-weight: bold; color: #2C3E50; margin-bottom: 0.5rem;">管理科学与工程 博士在读</div>
      <div style="color: #3498DB; font-weight: bold; margin-bottom: 0.5rem;">哈尔滨工业大学 经济与管理学院</div>
      <div style="color: #7f8c8d; font-size: 0.9rem; margin-bottom: 0.5rem;">2021.09 - 至今（预计2026年毕业）</div>
    </div>
    <div class="education-item">
      <div style="font-size: 1.2rem; font-weight: bold; color: #2C3E50; margin-bottom: 0.5rem;">计算机科学与技术 学士</div>
      <div style="color: #3498DB; font-weight: bold; margin-bottom: 0.5rem;">哈尔滨工业大学 计算机科学与技术学院</div>
      <div style="color: #7f8c8d; font-size: 0.9rem; margin-bottom: 0.5rem;">2017.09 - 2021.06</div>
    </div>
  </div>
</section>


<!-- 获奖荣誉 -->
<section style="margin-top: 3rem;">
  <h2 class="section-header">获奖荣誉</h2>
  
  <div class="publications-list">
    <!-- 2024博士国家奖学金特别突出 -->
    <div class="publication-item featured" style="background: linear-gradient(135deg, #F8F9FA 0%, #E9ECEF 100%); border-left: 4px solid #2C3E50; padding: 2rem;">
      <div class="pub-content">
        <div class="pub-text" style="font-size: 1.1rem; font-weight: bold; color: #2C3E50;">2024年度博士生国家奖学金</div>
      </div>
    </div>
    
    <div class="publication-item">
      <div class="pub-content">
        <div class="pub-text">2023年度第十二届黄梯云奖励基金 二等奖</div>
      </div>
    </div>
    
    <div class="publication-item">
      <div class="pub-content">
        <div class="pub-text">2023年度第七届全国兵器推演大赛智能空中博弈算法挑战赛 三等奖</div>
      </div>
    </div>
    
    <div class="publication-item">
      <div class="pub-content">
        <div class="pub-text">2020年度第十三届全国大学生软件创新大赛 三等奖</div>
      </div>
    </div>
    
    <div class="publication-item">
      <div class="pub-content">
        <div class="pub-text">2018年度国家励志奖学金</div>
      </div>
    </div>
  </div>
</section>

<!-- 学术活动 -->
<section style="margin-top: 3rem;">
  <h2 class="section-header">学术活动与服务</h2>
  
  <div style="background: white; padding: 2rem; border-radius: 15px; box-shadow: 0 5px 20px rgba(0,0,0,0.1);">
    <h3 style="color: #2C3E50; margin-bottom: 1.5rem;">会议报告与参与</h3>
    <ul style="line-height: 2; color: #555;">
      <li><strong>The 2025 INFORMS International Conference</strong> - 会议报告 (2025.07)</li>
      <li><strong>The 2024 Workshop on AI-empowered Systems Simulation (WASS 2024)</strong> - 会议报告 (2024.11)</li>
      <li><strong>第六届体系工程学术会议</strong> - 会议报告 (2024.08)</li>
      <li><strong>第十九届服务系统与服务管理国际会议 ICSSSM2024</strong> - 会议报告 (2024.08)</li>
      <li><strong>第十四届华人学者管理科学与工程国际年会CSAMSE 2022</strong> - Session Chair/会议报告 (2022.07)</li>
    </ul>
  </div>
</section>

<!-- 求职意向 -->
<section style="margin-top: 3rem;">
  <h2 class="section-header">求职意向</h2>
  <div style="background: linear-gradient(135deg, #E8F6F3 0%, #D5EDDF 100%); padding: 2rem; border-radius: 15px; border-left: 5px solid #27AE60;">
    <p style="font-size: 1.1rem; line-height: 1.8; color: #2C3E50; margin-bottom: 1.5rem;">
      期望在高等院校从事教学科研工作，主要从事<strong>管理科学与工程</strong>、<strong>人工智能</strong>等相关领域的研究。
    </p>
  </div>
</section>

<!-- PDF下载按钮 -->
<div style="text-align: center; margin: 3rem 0;">
  <div style="text-align: center; display: flex; gap: 1rem; justify-content: center;">
    <a href="{{ '/files/2025杨晋.pdf' | relative_url }}" download="2025杨晋_简历.pdf" style="background: linear-gradient(45deg, #2C3E50, #34495E); color: white; border: none; padding: 1rem 2rem; border-radius: 10px; font-size: 1.1rem; font-weight: bold; cursor: pointer; box-shadow: 0 3px 10px rgba(44, 62, 80, 0.3); transition: transform 0.3s ease; text-decoration: none; display: inline-block;" onmouseover="this.style.transform='translateY(-2px)'" onmouseout="this.style.transform='translateY(0)'">
      下载PDF简历
    </a>
  </div>
</div>

---

<div style="text-align: center; color: #7f8c8d; font-size: 0.9rem; margin-top: 2rem; padding-top: 2rem; border-top: 1px solid #ECF0F1;">
  <p><strong>杨晋</strong> | 哈尔滨工业大学博士生 | 管理科学与工程、人工智能交叉研究 | 更新于2025年7月</p>
</div>