# 外卖平台主页 - Food Delivery Platform

一个功能完整、设计精美的外卖平台主页系统，支持城市定位、智能搜索、分类导航、商家展示等核心功能。

## ✨ 功能特性

### 核心功能
- **城市定位服务** - 支持全国30个主要城市选择，包括一线、新一线和热门城市
- **智能搜索系统** - 实时搜索建议、热门搜索推荐、历史记录管理
- **多级分类导航** - 8大分类（美食、超市、水果、鲜花、医药、跑腿、下午茶、速食），每行4个，共2行展示
- **商家列表展示** - 商家卡片展示，包含评分、销量、配送信息、优惠活动
- **高级筛选排序** - 支持综合排序、距离、评分、销量等多维度筛选
- **轮播广告系统** - 自动轮播的促销活动展示
- **购物车功能** - 悬浮购物车，实时显示商品数量和总价
- **用户认证** - 登录/注册功能，登录成功后显示欢迎动画和彩带效果

### 视觉特性
- **精美装饰元素** - 渐变背景、装饰图案、悬浮效果
- **响应式设计** - 完美适配桌面端和移动端
- **流畅动画** - 彩带落下、卡片悬浮、按钮交互等丰富动画效果
- **温暖配色** - 橙色主题，营造食欲感和温暖氛围

## 🚀 快速开始

### 方式一：使用独立HTML文件（最简单）

1. 打开 `public/complete-food-delivery.html` 文件
2. 双击在浏览器中打开
3. 无需任何安装或配置，立即可用

### 方式二：Next.js开发环境

#### 安装依赖

\`\`\`bash
# 使用 npm
npm install

# 或使用 yarn
yarn install

# 或使用 pnpm
pnpm install
\`\`\`

#### 启动开发服务器

\`\`\`bash
npm run dev
# 或
yarn dev
# 或
pnpm dev
\`\`\`

访问 [http://localhost:3000](http://localhost:3000) 查看应用

#### 构建生产版本

\`\`\`bash
npm run build
npm start
\`\`\`

## 📦 部署方法

### 方式一：一键部署到Vercel（推荐）

1. 点击v0界面右上角的 **"Publish"** 按钮
2. 自动部署到Vercel，获得在线访问地址
3. 支持自定义域名绑定

### 方式二：通过GitHub部署

1. 点击v0界面右上角的 **GitHub图标**
2. 推送代码到GitHub仓库
3. 在 [vercel.com](https://vercel.com) 导入项目
4. 自动检测Next.js配置并部署

### 方式三：下载本地部署

1. 点击右上角三个点 → "Download ZIP"
2. 解压文件
3. 运行安装和构建命令
4. 部署到任何支持Node.js的服务器

## 📁 项目结构

\`\`\`
├── app/
│   ├── page.tsx              # 主页面
│   ├── layout.tsx            # 全局布局
│   ├── globals.css           # 全局样式和动画
│   ├── merchant/[id]/        # 商家详情页
│   ├── checkout/             # 结算页面
│   └── orders/               # 订单页面
├── components/
│   ├── header.tsx            # 顶部导航栏（城市选择、登录）
│   ├── search-bar.tsx        # 搜索栏（智能建议、热门搜索）
│   ├── category-nav.tsx      # 分类导航（8个分类，2行4列）
│   ├── banner-carousel.tsx   # 轮播广告
│   ├── merchant-list.tsx     # 商家列表
│   ├── merchant-card.tsx     # 商家卡片
│   ├── merchant-filters.tsx  # 筛选器
│   ├── floating-cart.tsx     # 悬浮购物车
│   ├── footer.tsx            # 底部信息
│   ├── welcome-celebration.tsx # 登录欢迎动画
│   └── ui/                   # UI组件库（shadcn/ui）
├── public/
│   ├── index.html            # 独立HTML版本
│   └── complete-food-delivery.html # 完整独立版本
└── README.md                 # 项目文档
\`\`\`

## 🛠 技术栈

### Next.js版本
- **框架**: Next.js 16 (App Router)
- **UI库**: React 19.2
- **样式**: Tailwind CSS v4
- **组件**: shadcn/ui
- **图标**: Lucide React
- **动画**: CSS Animations + Tailwind

### 独立HTML版本
- **纯HTML5 + CSS3 + JavaScript**
- **无依赖**: 可直接在浏览器中运行
- **完整功能**: 包含所有交互和动画效果

## 🎨 设计系统

### 色彩方案
- **主色**: 橙色 (#FF6B35) - 温暖、食欲感
- **辅助色**: 深橙 (#FF8C42)、浅橙 (#FFA07A)
- **中性色**: 灰度系列
- **强调色**: 黄色（评分）、绿色（成功）、红色（优惠）

### 字体
- **标题**: Geist Sans
- **正文**: Geist Sans
- **等宽**: Geist Mono

### 布局
- **响应式网格**: 移动端1列，平板2列，桌面3-4列
- **间距系统**: Tailwind标准间距（4px基准）
- **圆角**: 统一使用8px-16px

## 📱 功能说明

### 城市选择
- 支持30个主要城市
- 分为一线、新一线、热门城市三个分组
- 点击切换当前城市

### 搜索功能
- 实时搜索建议
- 热门搜索词推荐
- 搜索历史记录

### 分类导航
- 8大核心分类
- 每行4个，共2行
- 大图标设计，易于点击

### 商家列表
- 商家卡片展示
- 评分、销量、配送时间
- 优惠活动标签
- 支持筛选和排序

### 登录动画
- 点击登录按钮触发
- 50个彩色彩带从顶部落下
- Welcome卡片弹跳出现
- 持续3.5秒后自动消失

## 🔧 自定义配置

### 修改城市列表
编辑 `components/header.tsx` 中的 `cities` 数组

### 修改分类
编辑 `components/category-nav.tsx` 中的 `categories` 数组

### 修改主题色
编辑 `app/globals.css` 中的 CSS变量

### 添加商家数据
编辑 `components/merchant-list.tsx` 中的 `merchants` 数组

## 📄 许可证

MIT License

## 🤝 贡献

欢迎提交Issue和Pull Request

## 📞 支持

如需帮助，请访问 [vercel.com/help](https://vercel.com/help)

---

**享受你的外卖平台！** 🍔🍕🍜
