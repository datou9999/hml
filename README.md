
<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="DATOU CLOUD 专注企业通信系统、语音网关、即时通讯、WebRTC及海外云基础设施部署与技术服务。">
<title>DATOU CLOUD | 企业通信与云计算技术服务</title>
<style>
:root {
  --bg:#07111f;
  --panel:#101f33;
  --panel2:#0c192b;
  --blue:#42a5ff;
  --cyan:#35e0dc;
  --white:#f3f7ff;
  --muted:#a4b3c8;
  --border:rgba(255,255,255,.1);
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{
  font-family:Arial,"Microsoft YaHei",sans-serif;
  background:var(--bg);
  color:var(--white);
  line-height:1.7;
}
a{text-decoration:none;color:inherit}
.container{width:min(1160px,90%);margin:auto}
header{
  position:sticky;top:0;z-index:10;
  background:rgba(7,17,31,.92);
  backdrop-filter:blur(14px);
  border-bottom:1px solid var(--border);
}
.nav{
  min-height:72px;display:flex;
  justify-content:space-between;align-items:center;
  gap:20px;
}
.logo{font-size:23px;font-weight:900;letter-spacing:1px}
.logo span{color:var(--cyan)}
nav{display:flex;gap:25px;align-items:center}
nav a{font-size:14px;color:var(--muted)}
nav a:hover{color:var(--cyan)}
.menu-btn{display:none;background:none;border:0;color:white;font-size:25px}
.hero{
  padding:110px 0 100px;
  background:
  radial-gradient(ellipse at 80% 20%,rgba(27,123,255,.24),transparent 42%),
  radial-gradient(ellipse at 15% 80%,rgba(22,212,201,.12),transparent 35%);
}
.tag{
  display:inline-block;padding:6px 14px;
  border:1px solid rgba(53,224,220,.35);
  border-radius:30px;color:var(--cyan);
  font-size:13px;margin-bottom:24px;
}
.hero h1{font-size:clamp(36px,6vw,66px);line-height:1.2;max-width:850px}
.hero h1 span{
  background:linear-gradient(90deg,var(--blue),var(--cyan));
  -webkit-background-clip:text;color:transparent;
}
.hero p{color:var(--muted);font-size:17px;max-width:680px;margin:24px 0 32px}
.btn{
  display:inline-block;padding:12px 25px;
  border-radius:7px;background:linear-gradient(90deg,#268cff,#25c9d0);
  color:#041321;font-weight:bold;
}
.btn-outline{
  display:inline-block;padding:11px 24px;border:1px solid var(--border);
  border-radius:7px;margin-left:10px;color:white;
}
section{padding:85px 0}
.section-title{text-align:center;margin-bottom:48px}
.section-title h2{font-size:34px;margin-bottom:10px}
.section-title p{color:var(--muted)}
.services{
  display:grid;grid-template-columns:repeat(3,1fr);gap:20px;
}
.service{
  background:linear-gradient(145deg,var(--panel),var(--panel2));
  border:1px solid var(--border);border-radius:13px;
  padding:27px;transition:.25s;
}
.service:hover{transform:translateY(-5px);border-color:var(--blue)}
.service .icon{font-size:30px;margin-bottom:14px}
.service h3{font-size:19px;margin-bottom:10px}
.service p{font-size:14px;color:var(--muted)}
.service ul{margin:15px 0 0 18px;color:var(--muted);font-size:13px}
.service li{margin:5px 0}
.about{background:#0a1728}
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:50px;align-items:center}
.about h2{font-size:34px;margin-bottom:18px}
.about p{color:var(--muted);margin-bottom:14px}
.features{display:grid;grid-template-columns:1fr 1fr;gap:14px}
.feature{
  background:var(--panel);padding:19px;border:1px solid var(--border);
  border-radius:10px;
}
.feature strong{display:block;color:var(--cyan);font-size:18px}
.feature span{font-size:13px;color:var(--muted)}
.process{
  display:grid;grid-template-columns:repeat(4,1fr);gap:18px;
}
.step{padding:24px;background:var(--panel);border-radius:10px;border:1px solid var(--border)}
.step b{font-size:28px;color:var(--cyan)}
.step h3{margin:10px 0}
.step p{font-size:14px;color:var(--muted)}
.contact{
  background:linear-gradient(120deg,#102b49,#0b2433);
  border-top:1px solid var(--border);
  border-bottom:1px solid var(--border);
  text-align:center;
}
.contact h2{font-size:34px;margin-bottom:12px}
.contact p{color:var(--muted);margin-bottom:25px}
footer{padding:28px 0;color:var(--muted);font-size:13px}
.footer-row{display:flex;justify-content:space-between;gap:20px;flex-wrap:wrap}
@media(max-width:850px){
  .services{grid-template-columns:repeat(2,1fr)}
  .about-grid{grid-template-columns:1fr}
  .process{grid-template-columns:repeat(2,1fr)}
}
@media(max-width:600px){
  .nav{min-height:65px}
  .menu-btn{display:block}
  nav{
    display:none;position:absolute;top:65px;left:0;width:100%;
    background:#0a1728;padding:20px;
    flex-direction:column;align-items:flex-start;
    border-bottom:1px solid var(--border);
  }
  nav.open{display:flex}
  .hero{padding:75px 0}
  .services,.process{grid-template-columns:1fr}
  .features{grid-template-columns:1fr 1fr}
  section{padding:65px 0}
  .btn-outline{margin:12px 0 0}
}
</style>
</head>
<body>

<header>
  <div class="container nav">
    <a class="logo" href="#">DATOU <span>CLOUD</span></a>
    <button class="menu-btn" onclick="toggleMenu()" aria-label="打开菜单">☰</button>
    <nav id="nav">
      <a href="#home" onclick="closeMenu()">首页</a>
      <a href="#services" onclick="closeMenu()">服务项目</a>
      <a href="#about" onclick="closeMenu()">关于我们</a>
      <a href="#process" onclick="closeMenu()">服务流程</a>
      <a href="#contact" onclick="closeMenu()">联系我们</a>
    </nav>
  </div>
</header>

<main>
<section class="hero" id="home">
  <div class="container">
    <div class="tag">ENTERPRISE COMMUNICATION · CLOUD TECHNOLOGY</div>
    <h1>连接企业通信<br><span>构建数字化基础设施</span></h1>
    <p>
      DATOU CLOUD 专注企业通信系统、语音设备调试、即时通讯平台、
      WebRTC 技术集成及海外云基础设施部署。
      为企业提供从系统搭建到后期维护的一站式技术服务。
    </p>
    <a class="btn" href="#services">了解服务项目</a>
    <a class="btn-outline" href="#contact">联系技术团队</a>
  </div>
</section>

<section id="services">
  <div class="container">
    <div class="section-title">
      <h2>我们的服务</h2>
      <p>面向企业的通信系统与云计算技术解决方案</p>
    </div>

    <div class="services">

      <article class="service">
        <div class="icon">☎️</div>
        <h3>3CX 授权与系统部署</h3>
        <p>企业 IP PBX 通信系统搭建、授权配置及技术维护。</p>
        <ul>
          <li>3CX 系统安装与迁移</li>
          <li>分机、话机及呼叫路由配置</li>
          <li>SIP Trunk 对接调试</li>
          <li>系统维护与故障排查</li>
        </ul>
      </article>

      <article class="service">
        <div class="icon">🖥️</div>
        <h3>OKCC 系统部署</h3>
        <p>为企业提供呼叫中心系统环境搭建与技术支持。</p>
        <ul>
          <li>OKCC 环境部署</li>
          <li>坐席及队列配置</li>
          <li>呼叫流程调试</li>
          <li>系统运行维护</li>
        </ul>
      </article>

      <article class="service">
        <div class="icon">🌐</div>
        <h3>SIP 线路技术调试</h3>
        <p>协助企业对接已有的 SIP 服务商及通信线路。</p>
        <ul>
          <li>SIP 注册与认证排查</li>
          <li>呼入呼出路由配置</li>
          <li>号码格式与外显调试</li>
          <li>信令及 RTP 媒体排查</li>
        </ul>
      </article>

      <article class="service">
        <div class="icon">🔌</div>
        <h3>语音网关与 PBX 设备</h3>
        <p>实体语音设备、数字中继及模拟线路接入调试。</p>
        <ul>
          <li>E1 / PRI 数字中继</li>
          <li>FXO / FXS 网关配置</li>
          <li>语音网关与 PBX 对接</li>
          <li>设备信令及线路故障排查</li>
        </ul>
      </article>

      <article class="service">
        <div class="icon">💬</div>
        <h3>即时聊天系统</h3>
        <p>为企业搭建内部沟通及客户在线交流平台。</p>
        <ul>
          <li>即时聊天平台部署</li>
          <li>用户及权限管理</li>
          <li>消息服务配置</li>
          <li>企业系统集成</li>
        </ul>
      </article>

      <article class="service">
        <div class="icon">🎥</div>
        <h3>即时语音与视频通话</h3>
        <p>企业实时音视频通信系统搭建及集成。</p>
        <ul>
          <li>语音通话系统</li>
          <li>视频会议功能</li>
          <li>实时音视频服务部署</li>
          <li>网络及媒体质量调试</li>
        </ul>
      </article>

      <article class="service">
        <div class="icon">⚡</div>
        <h3>WebRTC 嵌入式通话</h3>
        <p>将浏览器语音通话能力集成到企业网站及业务平台。</p>
        <ul>
          <li>网页点击通话方案</li>
          <li>浏览器软电话集成</li>
          <li>WebRTC 与 PBX 对接</li>
          <li>WSS / ICE / RTP 配置</li>
        </ul>
      </article>

      <article class="service">
        <div class="icon">☁️</div>
        <h3>海外云服务器与公网 IP</h3>
        <p>协助企业规划和配置海外云计算基础设施。</p>
        <ul>
          <li>海外 VPS / 云服务器部署</li>
          <li>公网 IPv4 配置协助</li>
          <li>服务器环境安装</li>
          <li>网络及访问优化</li>
        </ul>
      </article>

      <article class="service">
        <div class="icon">🛠️</div>
        <h3>系统运维与技术支持</h3>
        <p>提供 Linux 服务器及企业 IT 系统维护服务。</p>
        <ul>
          <li>Linux 系统管理</li>
          <li>Docker / Nginx 部署</li>
          <li>数据库及系统迁移</li>
          <li>安全加固与故障排查</li>
        </ul>
      </article>

    </div>
  </div>
</section>

<section class="about" id="about">
  <div class="container about-grid">
    <div>
      <div class="tag">ABOUT DATOU CLOUD</div>
      <h2>专注技术，让企业通信更简单</h2>
      <p>
        DATOU CLOUD 是一家面向企业客户的通信系统与云计算技术服务品牌。
        我们围绕企业通信、呼叫中心、实时音视频及云基础设施，
        提供系统部署、设备调试、技术集成与持续运维服务。
      </p>
      <p>
        从前期技术方案规划，到系统安装、线路对接、功能调试，
        再到后期维护，我们致力于帮助企业建立稳定、可靠、
        易于管理的技术环境。
      </p>
    </div>
    <div class="features">
      <div class="feature">
        <strong>系统部署</strong>
        <span>从安装到上线</span>
      </div>
      <div class="feature">
        <strong>设备调试</strong>
        <span>通信设备与线路集成</span>
      </div>
      <div class="feature">
        <strong>技术集成</strong>
        <span>平台与业务系统对接</span>
      </div>
      <div class="feature">
        <strong>持续运维</strong>
        <span>故障排查与技术支持</span>
      </div>
    </div>
  </div>
</section>

<section id="process">
  <div class="container">
    <div class="section-title">
      <h2>服务流程</h2>
      <p>清晰、高效、专业的技术服务流程</p>
    </div>
    <div class="process">
      <div class="step">
        <b>01</b>
        <h3>需求沟通</h3>
        <p>了解企业业务场景、现有设备及技术需求。</p>
      </div>
      <div class="step">
        <b>02</b>
        <h3>方案规划</h3>
        <p>根据实际需求制定系统部署及技术实施方案。</p>
      </div>
      <div class="step">
        <b>03</b>
        <h3>部署调试</h3>
        <p>完成服务器、系统、设备及相关接口配置。</p>
      </div>
      <div class="step">
        <b>04</b>
        <h3>维护支持</h3>
        <p>提供后续技术支持、运行维护与问题排查。</p>
      </div>
    </div>
  </div>
</section>

<section class="contact" id="contact">
  <div class="container">
    <div class="tag">CONTACT US</div>
    <h2>开启您的企业技术项目</h2>
    <p>无论是通信系统部署、设备调试，还是云服务器配置，欢迎联系我们。</p>
    <!-- 将下面的邮箱替换为你的真实业务邮箱 -->
    <a class="btn" href="mailto:YOUR_EMAIL@example.com">联系技术团队</a>
  </div>
</section>
</main>

<footer>
  <div class="container footer-row">
    <div>
      <strong>DATOU <span style="color:#35e0dc">CLOUD</span></strong>
      <p>Enterprise Communication & Cloud Technology</p>
    </div>
    <div>© <span id="year"></span> DATOU CLOUD. All Rights Reserved.</div>
  </div>
</footer>

<script>
function toggleMenu(){
  document.getElementById('nav').classList.toggle('open');
}
function closeMenu(){
  document.getElementById('nav').classList.remove('open');
}
document.getElementById('year').textContent = new Date().getFullYear();
</script>

</body>
</html>
