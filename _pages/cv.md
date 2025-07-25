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

/* 桌面端优化设计 */
@media (min-width: 1024px) {
  .sidebar {
    margin: 0 !important;
    border-radius: 0 15px 15px 0 !important;
    padding: 2.5rem !important;
    display: flex !important;
    flex-direction: column !important;
    align-items: center !important;
  }
  
  .author__avatar {
    margin: 0 auto 1.2rem auto !important; /* 减少底部间距 */
    width: clamp(160px, 18vw, 200px) !important;
  }
  
  .author__content {
    text-align: center !important;
    margin: 0 !important; /* 移除margin */
  }
  
  .author__name {
    font-size: 1.8rem !important;
    margin: 0 !important; /* 移除所有margin */
    text-align: center !important;
    padding: 0 !important;
  }
  
  .author__urls {
    gap: 1rem !important;
    flex-direction: column !important;
    align-items: center !important;
  }
  
  .author__urls li {
    font-size: 1rem !important;
    text-align: center !important;
    min-width: 200px !important;
    padding: 0.8rem 1.2rem !important;
    border-radius: 25px !important;
  }
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
}

/* 修复侧边栏在所有设备上的显示问题 */
.sidebar .author__urls {
  display: block !important;
  position: relative !important;
  margin: 1rem 0 0 0 !important;
  padding: 0 !important;
  border: none !important;
  background: transparent !important;
  box-shadow: none !important;
  z-index: auto !important;
}

.sidebar .author__urls:before,
.sidebar .author__urls:after {
  display: none !important;
}

/* 美化侧边栏整体设计 */
.sidebar {
  background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%) !important;
  border-radius: 15px !important;
  box-shadow: 0 8px 32px rgba(0,0,0,0.1) !important;
  overflow: visible !important; /* 改为visible以避免裁剪 */
  padding: 2rem 1.5rem !important;
}

/* 重新设计作者档案的布局结构 */
.sidebar .author__profile,
.sidebar > div:first-child {
  display: flex !important;
  flex-direction: column !important;
  align-items: center !important;
  text-align: center !important;
  gap: 0.8rem !important; /* 减少整体间距 */
}

/* 确保所有屏幕尺寸下的居中布局 */
.sidebar .author__avatar,
.sidebar .author__content,
.sidebar .author__urls-wrapper {
  text-align: center !important;
  align-self: center !important;
}

.author__avatar img {
  border: 4px solid white !important;
  box-shadow: 0 4px 15px rgba(0,0,0,0.2) !important;
  transition: transform 0.3s ease !important;
}

.author__avatar img:hover {
  transform: scale(1.05) !important;
}

.author__name {
  color: #2C3E50 !important;
  font-weight: 700 !important;
  text-shadow: 0 1px 3px rgba(0,0,0,0.1) !important;
}

.author__urls li {
  background: rgba(255,255,255,0.8) !important;
  margin-bottom: 0.5rem !important;
  padding: 0.8rem 1rem !important;
  border-radius: 25px !important;
  transition: all 0.3s ease !important;
  border: 1px solid rgba(44, 62, 80, 0.1) !important;
}

.author__urls li:hover {
  background: rgba(255,255,255,1) !important;
  transform: translateY(-2px) !important;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15) !important;
}

.author__urls li i {
  color: #3498DB !important;
  margin-right: 0.8rem !important;
  font-size: 1.1rem !important;
}

.author__urls li a {
  color: #2C3E50 !important;
  text-decoration: none !important;
  font-weight: 500 !important;
}

.author__urls li a:hover {
  color: #3498DB !important;
}

/* 彻底重写头像样式，覆盖原始限制 */
.author__avatar {
  /* 完全覆盖原始样式 */
  display: block !important;
  width: auto !important;
  height: auto !important;
  max-width: none !important;
  /* 线性变化：从200px到120px，大幅增大尺寸 */
  width: clamp(120px, 25vw, 200px) !important;
  transition: all 0.3s ease;
  margin: 0 auto !important;
  text-align: center !important;
}

.author__avatar img {
  /* 确保图片填满容器 */
  width: 100% !important;
  height: auto !important;
  max-width: none !important;
  border-radius: 50% !important;
}

.author__name {
  /* 字体线性变化：从1.5rem到1.1rem，增大最小字体 */
  font-size: clamp(1.1rem, 2.8vw, 1.5rem) !important;
  transition: all 0.3s ease;
  line-height: 1.2 !important;
  margin: 0 !important; /* 移除默认margin */
  padding: 0 !important; /* 移除默认padding */
}

.author__urls li {
  font-size: clamp(0.85rem, 2.2vw, 0.9rem) !important;
  transition: all 0.3s ease;
  line-height: 1.4 !important;
  white-space: normal !important;
}

/* 平板端优化设计 */
@media (max-width: 768px) and (min-width: 481px) {
  .sidebar {
    margin: 1rem !important;
    padding: 2.5rem 2rem !important;
    background: linear-gradient(135deg, #ffffff 0%, #f8f9fa 100%) !important;
  }
  
  .author__content {
    text-align: center !important;
  }
  
  .author__avatar {
    margin: 0 auto 1rem auto !important; /* 减少底部间距 */
    max-width: clamp(140px, 24vw, 180px) !important;
    display: block !important;
  }
  
  .author__name {
    font-size: clamp(1.6rem, 4vw, 2rem) !important;
    margin: 0 !important; /* 移除所有margin */
    text-align: center !important;
    padding: 0 !important;
  }
  
  .author__urls-wrapper {
    text-align: center !important;
  }
  
  .author__urls {
    justify-content: center !important;
    flex-wrap: wrap !important;
    gap: 1rem !important;
    align-items: center !important;
  }
  
  .author__urls li {
    font-size: clamp(1.05rem, 3vw, 1.25rem) !important;
    margin: 0.5rem !important;
    min-width: 240px !important;
    text-align: center !important;
    padding: 1rem 1.5rem !important;
    border-radius: 25px !important;
    background: rgba(255,255,255,0.9) !important;
    box-shadow: 0 2px 8px rgba(0,0,0,0.08) !important;
  }
}

/* 手机端优化设计 */
@media (max-width: 480px) {
  .sidebar {
    margin: 1rem !important;
    padding: 3rem 2rem !important; /* 增加padding为头像留出更多空间 */
    background: linear-gradient(135deg, #ffffff 0%, #f8f9fa 100%) !important;
    min-height: auto !important;
    overflow: visible !important;
  }
  
  .author__avatar {
    /* 手机端头像进一步放大 */
    width: clamp(180px, 40vw, 220px) !important;
    margin: 0 auto 1rem auto !important; /* 减少底部间距 */
    float: none !important;
    display: block !important;
    text-align: center !important;
    position: relative !important;
  }
  
  .author__avatar img {
    width: 100% !important;
    height: auto !important;
    border: 5px solid white !important;
    box-shadow: 0 6px 20px rgba(0,0,0,0.25) !important;
  }
  
  .author__content {
    margin-left: 0 !important;
    text-align: center !important;
    min-height: auto !important;
    display: block !important;
    padding-top: 0 !important;
  }
  
  .author__name {
    font-size: clamp(1.4rem, 5vw, 1.8rem) !important;
    margin: 0 !important; /* 移除所有margin */
    line-height: 1.2 !important;
    text-align: center !important;
    padding: 0 !important; /* 移除padding */
  }
  
  .author__urls-wrapper {
    margin-top: 0 !important;
    text-align: center !important;
  }
  
  .author__urls {
    margin: 0 !important;
    padding: 0 !important;
    flex-direction: column !important;
    gap: 0.8rem !important;
    align-items: center !important;
  }
  
  .author__urls li {
    font-size: clamp(1.0rem, 3.8vw, 1.2rem) !important;
    line-height: 1.5 !important;
    white-space: nowrap !important;
    text-align: center !important;
    max-width: 90% !important;
    padding: 1rem 1.5rem !important;
    margin: 0.8rem 0 !important;
    border-radius: 30px !important;
    background: rgba(255,255,255,0.95) !important;
    box-shadow: 0 3px 12px rgba(0,0,0,0.1) !important;
  }
  
  .author__urls li i {
    color: #3498DB !important;
    margin-right: 1rem !important;
    font-size: 1.2rem !important;
  }
  
  /* 清除浮动 */
  .author__urls-wrapper::after {
    display: none !important;
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

<script>
// 复制手机号码功能
function copyPhoneNumber(phoneNumber) {
  // 使用现代浏览器的clipboard API
  if (navigator.clipboard && window.isSecureContext) {
    navigator.clipboard.writeText(phoneNumber).then(function() {
      showCopyMessage('手机号码已复制到剪贴板：' + phoneNumber);
    }).catch(function(err) {
      console.error('复制失败：', err);
      fallbackCopyTextToClipboard(phoneNumber);
    });
  } else {
    // 降级方案
    fallbackCopyTextToClipboard(phoneNumber);
  }
}

// 降级复制方案
function fallbackCopyTextToClipboard(text) {
  var textArea = document.createElement("textarea");
  textArea.value = text;
  
  // 避免滚动到底部
  textArea.style.position = "fixed";
  textArea.style.top = "0";
  textArea.style.left = "0";
  textArea.style.width = "2em";
  textArea.style.height = "2em";
  textArea.style.padding = "0";
  textArea.style.border = "none";
  textArea.style.outline = "none";
  textArea.style.boxShadow = "none";
  textArea.style.background = "transparent";
  
  document.body.appendChild(textArea);
  textArea.focus();
  textArea.select();
  
  try {
    var successful = document.execCommand('copy');
    if (successful) {
      showCopyMessage('手机号码已复制到剪贴板：' + text);
    } else {
      showCopyMessage('复制失败，请手动复制：' + text);
    }
  } catch (err) {
    console.error('降级复制也失败了：', err);
    showCopyMessage('复制失败，请手动复制：' + text);
  }
  
  document.body.removeChild(textArea);
}

// 显示复制成功消息
function showCopyMessage(message) {
  // 创建提示框
  var messageDiv = document.createElement('div');
  messageDiv.textContent = message;
  messageDiv.style.cssText = `
    position: fixed;
    top: 20px;
    left: 50%;
    transform: translateX(-50%);
    background: #2C3E50;
    color: white;
    padding: 12px 20px;
    border-radius: 25px;
    font-size: 0.9rem;
    z-index: 10000;
    box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    animation: fadeInOut 3s ease-in-out;
  `;
  
  // 添加动画样式
  if (!document.getElementById('copy-message-style')) {
    var style = document.createElement('style');
    style.id = 'copy-message-style';
    style.textContent = `
      @keyframes fadeInOut {
        0% { opacity: 0; transform: translateX(-50%) translateY(-10px); }
        15% { opacity: 1; transform: translateX(-50%) translateY(0); }
        85% { opacity: 1; transform: translateX(-50%) translateY(0); }
        100% { opacity: 0; transform: translateX(-50%) translateY(-10px); }
      }
    `;
    document.head.appendChild(style);
  }
  
  document.body.appendChild(messageDiv);
  
  // 3秒后移除提示框
  setTimeout(function() {
    if (messageDiv.parentNode) {
      messageDiv.parentNode.removeChild(messageDiv);
    }
  }, 3000);
}
</script>

<div style="text-align: center; color: #7f8c8d; font-size: 0.9rem; margin-top: 2rem; padding-top: 2rem; border-top: 1px solid #ECF0F1;">
  <p><strong>杨晋</strong> | 哈尔滨工业大学博士生 | 管理科学与工程、人工智能交叉研究 | 更新于2025年7月</p>
</div>