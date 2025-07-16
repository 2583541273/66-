<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>66素材库 - 沙雕动画素材天堂</title>
    <style>
        :root {
            --primary: #FF6B6B;
            --secondary: #4ECDC4;
            --dark: #292F36;
            --light: #F7FFF7;
            --accent: #FFE66D;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', 'Microsoft YaHei', sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 1rem 0;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 2rem;
            font-weight: 700;
            text-decoration: none;
            color: white;
            display: flex;
            align-items: center;
        }
        
        .logo img {
            height: 50px;
            margin-right: 10px;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 1.5rem;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            padding: 0.5rem 1rem;
            border-radius: 20px;
        }
        
        nav ul li a:hover {
            background-color: rgba(255,255,255,0.2);
        }
        
        .hero {
            height: 60vh;
            background: url('https://source.unsplash.com/random/1600x900/?cartoon,funny') center/cover no-repeat;
            display: flex;
            align-items: center;
            position: relative;
        }
        
        .hero::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(to right, rgba(0,0,0,0.7), rgba(0,0,0,0.3));
        }
        
        .hero-content {
            position: relative;
            z-index: 1;
            color: white;
            max-width: 600px;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--accent);
            color: var(--dark);
            padding: 0.8rem 1.5rem;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }
        
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        .section-title {
            text-align: center;
            margin: 3rem 0;
            font-size: 2.5rem;
            color: var(--dark);
            position: relative;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: linear-gradient(to right, var(--primary), var(--secondary));
            border-radius: 2px;
        }
        
        .categories {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 4rem;
        }
        
        .category-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }
        
        .category-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.2);
        }
        
        .category-img {
            height: 200px;
            overflow: hidden;
        }
        
        .category-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .category-card:hover .category-img img {
            transform: scale(1.1);
        }
        
        .category-info {
            padding: 1.5rem;
        }
        
        .category-info h3 {
            margin-bottom: 0.5rem;
            color: var(--dark);
        }
        
        .category-info p {
            color: #666;
            margin-bottom: 1rem;
        }
        
        .category-info .btn {
            padding: 0.5rem 1rem;
            font-size: 0.9rem;
        }
        
        footer {
            background-color: var(--dark);
            color: white;
            padding: 3rem 0;
            margin-top: 3rem;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
        }
        
        .footer-column h3 {
            margin-bottom: 1.5rem;
            font-size: 1.2rem;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-column h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 2px;
            background: linear-gradient(to right, var(--primary), var(--secondary));
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 0.8rem;
        }
        
        .footer-column ul li a {
            color: #ccc;
            text-decoration: none;
            transition: all 0.3s ease;
        }
        
        .footer-column ul li a:hover {
            color: white;
            padding-left: 5px;
        }
        
        .social-links {
            display: flex;
            gap: 1rem;
        }
        
        .social-links a {
            display: inline-block;
            width: 40px;
            height: 40px;
            background-color: rgba(255,255,255,0.1);
            border-radius: 50%;
            text-align: center;
            line-height: 40px;
            color: white;
            transition: all 0.3s ease;
        }
        
        .social-links a:hover {
            background-color: var(--primary);
            transform: translateY(-3px);
        }
        
        .copyright {
            text-align: center;
            margin-top: 2rem;
            padding-top: 2rem;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: #aaa;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 1rem;
                justify-content: center;
            }
            
            nav ul li {
                margin: 0 0.5rem;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .section-title {
                font-size: 2rem;
            }
        }
        
        @media (max-width: 480px) {
            .logo {
                font-size: 1.5rem;
            }
            
            .logo img {
                height: 40px;
            }
            
            nav ul li a {
                font-size: 0.9rem;
                padding: 0.3rem 0.6rem;
            }
            
            .hero {
                height: 50vh;
            }
            
            .categories {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <a href="#" class="logo">
                    <img src="https://via.placeholder.com/50" alt="66素材库">
                    66素材库
                </a>
                <nav>
                    <ul>
                        <li><a href="#">首页</a></li>
                        <li><a href="#">素材分类</a></li>
                        <li><a href="#">热门推荐</a></li>
                        <li><a href="#">上传素材</a></li>
                        <li><a href="#">关于我们</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
    
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>发现创意无限的可能</h1>
                <p>海量沙雕动画素材免费下载，让你的创作更加轻松有趣</p>
                <a href="#" class="btn">立即探索</a>
            </div>
        </div>
    </section>
    
    <section class="container">
        <h2 class="section-title">热门素材分类</h2>
        
        <div class="categories">
            <div class="category-card">
                <div class="category-img">
                    <img src="https://source.unsplash.com/random/400x300/?cartoon,character" alt="角色素材">
                </div>
                <div class="category-info">
                    <h3>搞笑角色</h3>
                    <p>各种沙雕动画角色素材，包含多种表情和动作</p>
                    <a href="#" class="btn">查看全部</a>
                </div>
            </div>
            
            <div class="category-card">
                <div class="category-img">
                    <img src="https://source.unsplash.com/random/400x300/?background,scene" alt="场景素材">
                </div>
                <div class="category-info">
                    <h3>动画场景</h3>
                    <p>丰富的背景场景素材，适用于各种动画制作</p>
                    <a href="#" class="btn">查看全部</a>
                </div>
            </div>
            
            <div class="category-card">
                <div class="category-img">
                    <img src="https://source.unsplash.com/random/400x300/?sound,music" alt="音效素材">
                </div>
                <div class="category-info">
                    <h3>搞笑音效</h3>
                    <p>各类搞笑音效合集，让你的动画更有趣</p>
                    <a href="#" class="btn">查看全部</a>
                </div>
            </div>
            
            <div class="category-card">
                <div class="category-img">
                    <img src="https://source.unsplash.com/random/400x300/?prop,object" alt="道具素材">
                </div>
                <div class="category-info">
                    <h3>动画道具</h3>
                    <p>各种动画中常用的道具和物品素材</p>
                    <a href="#" class="btn">查看全部</a>
                </div>
            </div>
        </div>
    </section>
    
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>关于我们</h3>
                    <p>66素材库致力于为创作者提供高质量的沙雕动画素材，让创作变得更加简单有趣。</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-weibo"></i></a>
                        <a href="#"><i class="fab fa-qq"></i></a>
                        <a href="#"><i class="fab fa-weixin"></i></a>
                        <a href="#"><i class="fab fa-bilibili"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>快速链接</h3>
                    <ul>
                        <li><a href="#">首页</a></li>
                        <li><a href="#">素材分类</a></li>
                        <li><a href="#">热门推荐</a></li>
                        <li><a href="#">上传素材</a></li>
                        <li><a href="#">用户协议</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>帮助中心</h3>
                    <ul>
                        <li><a href="#">常见问题</a></li>
                        <li><a href="#">素材上传指南</a></li>
                        <li><a href="#">版权说明</a></li>
                        <li><a href="#">联系我们</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>联系方式</h3>
                    <ul>
                        <li>邮箱：contact@66sucai.com</li>
                        <li>QQ：123456789</li>
                        <li>微信：66sucai</li>
                        <li>地址：北京市朝阳区创意园区</li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2025 66素材库 版权所有 | 京ICP备12345678号</p>
            </div>
        </div>
    </footer>
    
    <!-- Font Awesome for icons -->
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
</body>
</html>
