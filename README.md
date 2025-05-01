# 网站导航 - 实用工具与AI游戏集合

## 项目概述
这是一个集成了多种实用工具和AI游戏的网站导航页面，提供简洁美观的界面和丰富的功能集合。

## 主要特性

### 🎨 现代化UI设计
- 响应式布局，适配各种设备
- 深色/浅色主题切换（自动跟随系统偏好）
- 卡片式布局，动画效果流畅
- 美观的渐变色标题栏

### 🔍 智能搜索功能
- 实时搜索过滤网站
- 支持标题、描述和关键词搜索
- 无结果提示

### 🛠️ 实用工具集合
1. **UUID生成器** - 快速生成随机UUID
2. **随机数生成器** - 自定义范围随机数生成
3. **Python在线运行器** - 浏览器中运行Python代码
4. **赞助支持** - 支持网站发展

### 🎮 AI游戏娱乐
1. **AI猜人物游戏** - 与AI互动猜人物
2. **AI井字棋对战** - 挑战人工智能
3. **人机验证挑战** - Steam风格验证游戏

### 📢 公告系统
- 每日首次访问显示公告
- 可手动查看公告
- 美观的弹窗设计

## 技术实现

### 前端技术
- 纯HTML/CSS/JavaScript实现
- CSS变量实现主题切换
- Flexbox和Grid布局
- 动画和过渡效果增强用户体验

### 特色功能代码
```javascript
// 主题切换
themeToggle.addEventListener('click', () => {
    const currentTheme = document.documentElement.getAttribute('data-theme');
    const newTheme = currentTheme === 'dark' ? 'light' : 'dark';
    document.documentElement.setAttribute('data-theme', newTheme);
    localStorage.setItem('theme', newTheme);
    icon.classList.toggle('fa-moon');
    icon.classList.toggle('fa-sun');
});

// 智能搜索
document.getElementById('searchInput').addEventListener('input', function(e) {
    const searchTerm = e.target.value.toLowerCase();
    const cards = document.querySelectorAll('.link-card');
    // ...搜索逻辑
});
