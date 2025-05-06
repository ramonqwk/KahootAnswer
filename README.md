<a href="#"><img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=150&color=8000ff&text=Kahoot%20Answer&fontSize=40&fontAlignY=33&fontColor=ffffff"/></a>

<div align="center">
  <img src="https://i.imgur.com/5frWvoa.png?maxwidth=520&shape=thumb&fidelity=high" width="100px" alt="Alura Logo"/>
</div>

<h2 align="center"><strong>Kahoot Answer</strong></h2>

<p align="center" style="font-size: 16px;">
  O <strong>Kahoot Answer</strong> responde automaticamente os <strong>quizzes</strong> da plataforma <strong>Kahoot</strong>, economizando seu tempo e trabalho.
</p>  
<p align="center"><strong>🔴 Versão 1 – Kahoot: Destaca a Resposta Correta (sem clique, agora com borda e fundo branco)</strong></p>

<p align="center"><strong>Para usar, copie o código abaixo:</strong></p>

<div align="center">

<pre>
<code>
javascript:(async()=>{const id=prompt("Digite o quiz ID:");if(!id)return alert("Quiz ID inválido!");try{const res=await fetch(`https://kahoot.it/rest/kahoots/${id}`,{headers:{"Accept":"application/json"}});if(!res.ok)throw new Error();const data=await res.json(),s=document.createElement("style");s.textContent=`@keyframes pulse{from{border-width:3px}to{border-width:8px}}.highlight{border:3px solid white!important;animation:pulse 1s infinite alternate}`;document.head.appendChild(s);const w=document.createElement("div");w.textContent="By Ramon";w.style.cssText="position:fixed;top:0;right:0;padding:4px 8px;background:rgba(0,0,0,0.5);color:white;font-family:sans-serif;font-size:12px;z-index:9999;";document.body.appendChild(w);let lastQ=-1;const mark=()=>{try{const q=JSON.parse(localStorage.getItem("kahoot-game_session")).questionNumber;if(q!==lastQ){lastQ=q}const a=data.questions[q]?.choices?.findIndex(c=>c.correct),el=document.querySelectorAll('[data-functional-selector^="answer-"]')[a];if(el){el.click();el.classList.add("highlight")}}catch(e){}};new MutationObserver(mark).observe(document.body,{childList:!0,subtree:!0});setInterval(mark,100);document.addEventListener("DOMContentLoaded",mark);}catch(e){alert("Erro ao buscar o Quiz. Verifique o ID.")}})()
</code>
</pre>

</div>

<p align="center">
<sub><i>Clique abaixo para entrar no servidor do Discord ou doar</i></sub>
</p>

<p align="center">
    <a href="https://discord.gg/cZVtWmWsUE"><img width="15%" alt="Discord (CS)" title="Discord (Kahoot Answer)" src="https://i.imgur.com/r0YUgMR.png"/></a>
  &nbsp;
    <a href="https://pixgg.com/Ramon"><img width="15%" alt="Doar" title="Doar" src="https://i.imgur.com/yLUUqaa.png"/></a>
</p>

<p align="center">
  <a href="#"><img src="https://komarev.com/ghpvc/?username=Ramonqwk&style=for-the-badge&label=Views:&color=gray"/></a>
</p>

---

<!-- Créditos -->
<div align="center">
  <img src="https://i.imgur.com/gi0h7c1.jpeg" width="150px" alt="Ramon Profile"/>
  <h3 style="color: #e86a04; animation: pulse 2s infinite;">Criado por Ramon!</h3>
</div>

<a href="#"><img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=150&color=ffffff&section=footer"/></a>
