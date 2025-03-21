<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="张泾平的个人主页，化学领域从业者，热爱创新与探索。">
  <meta name="keywords" content="张泾平, 化学, 分析检测, 个人主页">
  <meta name="author" content="张泾平">
  <title>张泾平 OlderPing 的个人主页</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
  <style>
    /* 全局样式 */
    body {
      font-family: 'Roboto', Arial, sans-serif;
      margin: 0;
      padding: 20px;
      background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://source.unsplash.com/featured/1920x1080/?nature,water');
      background-size: cover;
      background-position: center;
      color: #fff;
      overflow: hidden;
      position: relative;
      animation: backgroundZoom 20s infinite alternate;
    }

    @keyframes backgroundZoom {
      0% { background-size: 100% auto; }
      100% { background-size: 120% auto; }
    }

    /* 动态粒子背景 */
    #particles-js {
      position: absolute;
      width: 100%;
      height: 100%;
      top: 0;
      left: 0;
      z-index: 1;
    }

    /* 内容区域样式 */
    .content {
      background-color: rgba(255, 255, 255, 0.1);
      max-width: 800px;
      margin: 0 auto;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
      backdrop-filter: blur(10px);
      position: relative;
      z-index: 2;
      animation: fadeIn 1s ease-in-out;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .content:hover {
      transform: translateY(-10px);
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.4);
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    /* 头部样式 */
    .header {
      text-align: center;
      border-bottom: 2px solid rgba(255, 255, 255, 0.1);
      padding-bottom: 20px;
      margin-bottom: 30px;
    }

    .profile-pic {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      border: 4px solid #2E7D32;
      margin-bottom: 20px;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      box-shadow: 0 0 20px rgba(46, 125, 50, 0.5);
    }

    .profile-pic:hover {
      transform: scale(1.1);
      box-shadow: 0 0 30px rgba(46, 125, 50, 0.8);
    }

    .header h1 {
      font-size: 2.5rem;
      margin: 0;
      color: #2E7D32;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
      background: linear-gradient(45deg, #2E7D32, #1B5E20);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .header p {
      font-size: 1.1rem;
      color: rgba(255, 255, 255, 0.8);
    }

    /* 部分样式 */
    .section {
      margin: 40px 0;
    }

    .section h2 {
      font-size: 1.8rem;
      color: #2E7D32;
      border-bottom: 2px solid rgba(255, 255, 255, 0.1);
      padding-bottom: 10px;
      margin-bottom: 20px;
      text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.2);
    }

    .section ul {
      list-style-type: disc;
      padding-left: 20px;
    }

    .section ul li {
      margin: 10px 0;
      font-size: 1rem;
      color: rgba(255, 255, 255, 0.9);
    }

    /* 按钮样式 */
    .button {
      display: inline-block;
      padding: 10px 20px;
      background-color: #2E7D32;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      margin: 5px;
      transition: background-color 0.3s ease, transform 0.2s ease, box-shadow 0.3s ease;
      position: relative;
      overflow: hidden;
    }

    .button::after {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      width: 300%;
      height: 300%;
      background: radial-gradient(circle, rgba(255, 255, 255, 0.4), rgba(255, 255, 255, 0));
      transform: translate(-50%, -50%) scale(0);
      transition: transform 0.5s ease;
    }

    .button:hover {
      background-color: #1B5E20;
      transform: scale(1.05);
      box-shadow: 0 0 20px rgba(46, 125, 50, 0.6);
    }

    .button:active {
      transform: scale(0.95);
    }

    .button:hover::after {
      transform: translate(-50%, -50%) scale(1);
    }

    /* 页脚样式 */
    .footer {
      text-align: center;
      margin-top: 40px;
      padding: 20px;
      border-top: 1px solid rgba(255, 255, 255, 0.1);
      color: rgba(255, 255, 255, 0.7);
    }

    /* 响应式设计 */
    @media (max-width: 600px) {
      body {
        padding: 10px;
      }
      .content {
        padding: 20px;
      }
      .header h1 {
        font-size: 1.8rem;
      }
      .header p {
        font-size: 1rem;
      }
      .section h2 {
        font-size: 1.4rem;
      }
      .section ul li {
        font-size: 0.9rem;
      }
    }
  </style>
</head>
<body>
  <!-- 动态粒子背景 -->
  <div id="particles-js"></div>

  <div class="content">
    <div class="header">
      <img src="https://your-image-url.com/your-profile-pic.jpg" alt="张泾平的头像" class="profile-pic">
      <h1>张泾平</h1>
      <p>比较热情 · 相当的不专业 · 十分注重但自身并不怎么创新</p>
    </div>

    <div class="section">
      <h2>📌 关于我</h2>
      <p>这里写你的个人简介，比如：</p>
      <ul>
        <li>从事化学领域/分析检测方向</li>
        <li>暂无工作经验/学习经历较少</li>
        <li>曾经是个靓仔</li>
      </ul>
    </div>

    <div class="section">
      <h2>🎓 教育背景</h2>
      <p>安康学院 · 应用化学 · 2019-2023</p>
    </div>

    <div class="section">
      <h2>📞 你想联系我吗</h2>
      <ul>
        <li>邮箱：<a href="mailto:2672900270@qq.com" class="button"><i class="fas fa-envelope"></i> 发送邮件</a></li>
        <li>微信：ZJP_Polaris</li>
        <li>电话：<a href="tel:15829537810" class="button"><i class="fas fa-phone"></i> 拨打电话</a></li>
        <li>GitHub：<a href="https://github.com/ZJP-Polaris" class="button"><i class="fab fa-github"></i> 访问 GitHub</a></li>
      </ul>
    </div>

    <div class="footer">
      <p>© 2023 张泾平. 保留所有权利。</p>
      <p>
        <a href="https://linkedin.com/in/你的用户名" class="button">LinkedIn</a>
        <a href="https://twitter.com/你的用户名" class="button">Twitter</a>
      </p>
    </div>
  </div>

  <!-- 动态粒子库 -->
  <script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
  <script>
    // 初始化粒子背景
    particlesJS('particles-js', {
      particles: {
        number: { value: 80, density: { enable: true, value_area: 800 } },
        color: { value: '#2E7D32' },
        shape: { type: 'circle' },
        opacity: { value: 0.5, random: true },
        size: { value: 3, random: true },
        line_linked: { enable: true, distance: 150, color: '#2E7D32', opacity: 0.4, width: 1 },
        move: { enable: true, speed: 3, direction: 'none', random: true, straight: false, out_mode: 'out' }
      },
      interactivity: {
        detect_on: 'canvas',
        events: { onhover: { enable: true, mode: 'repulse' }, onclick: { enable: true, mode: 'push' } }
      },
      retina_detect: true
    });
  </script>
</body>
</html>
