<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <!-- 针对手机端适配，禁止缩放 -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <!-- 让它在 iPhone 上像原生 App 一样全屏显示 -->
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
  <title>26成都教招刷题</title>
  <style>
    /* 界面样式 */
    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
      background-color: #f5f7fa;
      margin: 0;
      padding: 20px;
      color: #333;
    }
    .header {
      text-align: center;
      font-size: 18px;
      font-weight: bold;
      margin-bottom: 20px;
      color: #409eff;
    }
    .card {
      background: #fff;
      border-radius: 12px;
      padding: 20px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.05);
      margin-bottom: 20px;
    }
    .question {
      font-size: 18px;
      line-height: 1.5;
      margin-bottom: 20px;
    }
    .option {
      display: block;
      width: 100%;
      padding: 15px;
      margin-bottom: 12px;
      border: 1px solid #dcdfe6;
      border-radius: 8px;
      background: #fff;
      font-size: 16px;
      text-align: left;
      box-sizing: border-box;
      transition: all 0.2s;
    }
    .option:active { background: #f0f2f5; }
    /* 正确和错误的颜色 */
    .correct { background-color: #f0f9eb !important; border-color: #67c23a !important; color: #67c23a; }
    .wrong { background-color: #fef0f0 !important; border-color: #f56c6c !important; color: #f56c6c; }
    
    .analysis-box {
      display: none; /* 默认隐藏，答题后显示 */
      margin-top: 20px;
      padding: 15px;
      background: #ecf5ff;
      border-radius: 8px;
      color: #409eff;
      line-height: 1.5;
    }
    .next-btn {
      display: none; /* 默认隐藏 */
      width: 100%;
      padding: 15px;
      background: #409eff;
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 18px;
      margin-top: 20px;
    }
  </style>
</head>
<body>

  <div class="header">
    <span id="progress">1 / 3</span> 题
  </div>

  <div class="card">
    <div class="question" id="questionText">题目加载中...</div>
    <div id="optionsContainer">
      <!-- 选项会通过 JS 生成到这里 -->
    </div>
    <div class="analysis-box" id="analysisBox"></div>
  </div>

  <button class="next-btn" id="nextBtn" onclick="nextQuestion()">下一题</button>

  <!-- 引入第一步写的题库文件 -->
  <script src="questions.js"></script>
  
  <script>
    let currentIndex = 0; // 当前做到第几题

    const questionText = document.getElementById('questionText');
    const optionsContainer = document.getElementById('optionsContainer');
    const analysisBox = document.getElementById('analysisBox');
    const nextBtn = document.getElementById('nextBtn');
    const progressText = document.getElementById('progress');

    // 渲染题目
    function loadQuestion() {
      const q = questionBank[currentIndex];
      progressText.innerText = `${currentIndex + 1} / ${questionBank.length}`;
      questionText.innerText = q.question;
      
      // 清空旧选项和解析
      optionsContainer.innerHTML = '';
      analysisBox.style.display = 'none';
      nextBtn.style.display = 'none';

      // 生成新选项
      q.options.forEach((opt, index) => {
        const btn = document.createElement('button');
        btn.className = 'option';
        btn.innerText = opt;
        btn.onclick = () => checkAnswer(index, btn);
        optionsContainer.appendChild(btn);
      });
    }

    // 检查答案
    function checkAnswer(selectedIndex, clickedBtn) {
      const q = questionBank[currentIndex];
      const allBtns = optionsContainer.querySelectorAll('.option');
      
      // 禁用所有按钮，防止重复点击
      allBtns.forEach(btn => btn.onclick = null);

      if (selectedIndex === q.answer) {
        clickedBtn.classList.add('correct');
      } else {
        clickedBtn.classList.add('wrong');
        // 如果选错了，把正确的标绿提示出来
        allBtns[q.answer].classList.add('correct');
      }

      // 显示解析和下一题按钮
      analysisBox.innerText = q.analysis;
      analysisBox.style.display = 'block';
      
      // 如果不是最后一题，显示下一题按钮；否则显示完成
      if (currentIndex < questionBank.length - 1) {
        nextBtn.innerText = '下一题';
        nextBtn.style.display = 'block';
      } else {
        nextBtn.innerText = '重新开始';
        nextBtn.style.display = 'block';
      }
    }

    // 点击下一题
    function nextQuestion() {
      if (currentIndex < questionBank.length - 1) {
        currentIndex++;
        loadQuestion();
      } else {
        // 刷完一遍，重新开始
        currentIndex = 0;
        loadQuestion();
        window.scrollTo(0, 0); // 滚回顶部
      }
    }

    // 页面加载完毕后立即执行
    window.onload = loadQuestion;
  </script>
</body>
</html>
