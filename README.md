<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>崔静雯 · 作品集</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #f0f2f5;  /* 柔和背景色 */
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", sans-serif;
        }

        /* 自定义头部 – 美观且不干扰PDF */
        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 2rem 1rem;
            text-align: center;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        }
        .hero h1 {
            font-size: 2.2rem;
            letter-spacing: -0.5px;
            margin-bottom: 0.5rem;
            font-weight: 600;
        }
        .hero p {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        /* 关键：PDF容器占满剩余空间，无任何内外边距 */
        .pdf-container {
            width: 100%;
            height: calc(100vh - 140px);  /* 减去头部高度，留出滚动空间 */
            background: #fff;
            margin: 0;
            padding: 0;
            overflow: hidden;
        }

        /* iframe 完全撑满容器，不留一丝空白 */
        .pdf-container iframe {
            display: block;
            width: 100%;
            height: 100%;
            border: none;
            margin: 0;
            padding: 0;
        }

        /* 小屏手机适配：头部稍微缩小，保证PDF可视区足够 */
        @media (max-width: 600px) {
            .hero { padding: 1.2rem 0.8rem; }
            .hero h1 { font-size: 1.6rem; }
            .pdf-container { height: calc(100vh - 110px); }
        }
    </style>
</head>
<body>

<div class="hero">
    <h1>📁 崔静雯的作品集</h1>
    <p>感谢查看我的作品集 (*^▽^*)  —  建议电脑端全屏浏览</p>
</div>

<div class="pdf-container">
    <!-- 关键修复：添加 #view=FitW 让PDF宽度自适应，同时隐藏多余工具栏 -->
    <iframe src="UXportfolio.pdf#toolbar=0&navpanes=0&scrollbar=1&view=FitW&zoom=page-width"></iframe>
</div>

</body>
</html>
