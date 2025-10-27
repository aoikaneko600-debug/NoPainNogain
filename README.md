<p align="center" style="color:#FF69B4;"></p>

<h1 align="center" style="color:#FF1493; font-size:2.4em; font-weight:800;">効果的なプロテイン摂取ガイド 💖</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Timing-Guide-FF69B4?style=for-the-badge" alt="Timing">
  <img src="https://img.shields.io/badge/Types-Info-FFC0CB?style=for-the-badge" alt="Types">
  <img src="https://img.shields.io/badge/Tips-Quick-FFB6C1?style=for-the-badge" alt="Tips">
</p>

<p>プロテインは効率的なタンパク質補給に便利なサプリメントです。目的や生活に合わせて、タイミングと種類を選びましょう。</p>

<h2 style="color:#FF1493; font-size:1.6em; font-weight:800;">1) 摂取タイミング</h2>
- 運動後30分以内 💪：筋修復が活発なゴールデンタイム。ホエイ推奨。  
- 就寝前（30分〜1時間前）🌙：睡眠中の筋合成をサポート。カゼインが有効。直前は胃に注意。  
- 起床後 ☀️：夜間に消費した分を補給。ホエイが速い。  
- 間食として 🍓：食間の筋分解を抑える目的で有効。

<h2 style="color:#FF1493; font-size:1.6em; font-weight:800;">2) 主な種類と特徴</h2>
- ホエイ（Whey）💨：吸収が速い。運動直後に最適。  
- カゼイン（Casein）⏳：吸収がゆっくり。就寝前や長時間の栄養供給向け。  
- ソイ（Soy）🌱：植物性で腹持ち良し。美容・健康志向やベジの人向け。

<h2 style="color:#FF1493; font-size:1.6em; font-weight:800;">3) メリット・注意点</h2>
- メリット：手軽にたんぱく補給、筋肉の維持・成長をサポート、低脂肪・低カロリー商品が多い。  
- 注意点：満腹感は固形食より弱い、過剰摂取に注意、体質によっては胃腸に合わない場合あり、継続コストがかかる。

<h2 style="color:#FF1493; font-size:1.6em; font-weight:800;">クイックアドバイス</h2>
- 容量はパッケージと目標のたんぱく質量を基準に。食事とのバランスを大切に。  
- 初めてなら少量から試して体調を確認してください。

---

<h2 align="center" style="color:#FF69B4;">🎉 プロテイン摂取ガイド 3択クイズ 🎉</h2>

<div id="quiz-app" style="max-width:500px;margin:0 auto;">
  <script>
    const quiz = [
      {
        question: "運動直後に推奨されるプロテインの種類はどれ？",
        choices: ["ソイプロテイン", "ホエイプロテイン", "カゼインプロテイン"],
        answer: 1 // index of correct choice
      },
      {
        question: "就寝前の摂取に適したプロテインは？",
        choices: ["ホエイプロテイン", "カゼインプロテイン", "ソイプロテイン"],
        answer: 1
      },
      {
        question: "プロテイン摂取時に注意すべきポイントはどれ？",
        choices: [
          "固形食より満腹感が強い",
          "過剰摂取に注意が必要",
          "筋分解を促進する"
        ],
        answer: 1
      }
    ];

    let current = 0;
    let score = 0;

    function renderQuiz() {
      const app = document.getElementById('quiz-app');
      if (current < quiz.length) {
        const q = quiz[current];
        app.innerHTML = `
          <div style="margin-bottom:1em;font-weight:700;">Q${current+1}. ${q.question}</div>
          ${q.choices.map((c,i)=>`
            <button onclick="selectAnswer(${i})"
              style="display:block;width:100%;margin-bottom:8px;padding:8px;font-size:1em;border-radius:5px;border:1px solid #FF69B4;background:#fff;">
              ${c}
            </button>
          `).join('')}
          <div style="margin-top:1em;color:#999;">${current+1} / ${quiz.length}問目</div>
        `;
      } else {
        app.innerHTML = `
          <div style="font-size:1.3em;font-weight:700;color:#FF1493;">結果</div>
          <div style="margin:1em 0;">
            ${quiz.length}問中 <span style="color:#FF69B4;">${score}</span>問正解！<br>
            ${score === quiz.length ? "パーフェクト！💯" : score >= 2 ? "よくできました！👍" : "またチャレンジしてね！"}
          </div>
          <button onclick="restartQuiz()" style="padding:8px 16px;border-radius:5px;border:1px solid #FF69B4;background:#fff;">もう一度挑戦</button>
        `;
      }
    }

    window.selectAnswer = function(index) {
      if (quiz[current].answer === index) score++;
      current++;
      renderQuiz();
    };

    window.restartQuiz = function() {
      current = 0;
      score = 0;
      renderQuiz();
    };

    window.onload = renderQuiz;
  </script>
  <noscript>
    <p>このクイズはJavaScriptを有効にすると遊べます。</p>
  </noscript>
</div>

<p align="center" style="color:#FF69B4;"></p>
