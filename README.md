<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Minamoto no Tora - 12.9</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family: Arial, Helvetica, sans-serif;
}

html{
  scroll-behavior:smooth;
}

body{
  background:#f1f5f9;
  color:#0f172a;
  line-height:1.6;
}

/* ===== BANNER ===== */
header{
  position: relative;
  text-align: center;
  padding: 60px 20px;
  color: white;
  overflow: hidden;
}

/* lớp nền ảnh */
header::before{
  content: "";
  position: absolute;
  inset: 0;
  background: url("https://i.ibb.co/TMtFcdHv/image.png") center/cover no-repeat;
  filter: blur(2px);
  transform: scale(1.1); 
  z-index: -1;
}


header h1{
  font-size:32px;
  margin-bottom:10px;
}

header p{
  font-size:18px;
  opacity:0.9;
}

nav{
  margin-top:25px;
}

nav a{
  display:inline-block;
  color:white;
  text-decoration:none;
  padding:10px 20px;
  margin:5px;
  border-radius:30px;
  transition:0.3s;
  background:rgba(255,255,255,0.15);
}

nav a:hover{
  background:white;
  color:#7c3aed;
}

/* ===== SECTION ===== */
section{
  padding:60px 20px;
  max-width:1100px;
  margin:auto;
}

.card{
  background:white;
  padding:30px;
  border-radius:18px;
  margin-bottom:30px;
  box-shadow:0 10px 25px rgba(0,0,0,0.08);
  transition:0.3s;
}

.card:hover{
  transform:translateY(-5px);
}

h2{
  color:#7c3aed;
  margin-bottom:20px;
}

/* ===== ACTIVITIES ===== */
.activities{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
  gap:20px;
  margin-bottom:25px;
}

.activity-btn{
  background:linear-gradient(135deg,#6366f1,#a855f7);
  border:none;
  padding:18px;
  border-radius:15px;
  color:white;
  font-size:17px;
  cursor:pointer;
  transition:0.3s;
}

.activity-btn:hover{
  transform:scale(1.07);
}

.activity-content{
  display:none;
  animation:fade 0.5s ease-in-out;
}

@keyframes fade{
  from{opacity:0; transform:translateY(20px);}
  to{opacity:1; transform:translateY(0);}
}

/* ===== GALLERY ===== */
.gallery{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
  gap:20px;
  margin-top:20px;
}

.gallery img{
  width:100%;
  height:220px;
  object-fit:cover;
  border-radius:15px;
  transition:0.3s;
}

.gallery img:hover{
  transform:scale(1.05);
}

/* ===== FOOTER ===== */
footer{
  text-align:center;
  padding:40px;
  background:#e0e7ff;
  margin-top:40px;
}
</style>
</head>

<body>

<header id="home">
  <h1>CLB Minamoto no Tora 源の虎</h1>
  <p>12.9 – Trường THPT Huỳnh Văn Nghệ</p>
  <p>"Thanh xuân là hành trình, không phải đích đến."</p>

  <nav>
    <a href="#home">Trang Chủ</a>
    <a href="#activities">Hoạt Động</a>
    <a href="#contact">Liên Hệ</a>
  </nav>
</header>

<section>
  <div class="card">
    <h2>📌 Thông Tin Chuyến Đi</h2>
    <p><b>Lớp:</b> 12.9</p>
    <p><b>Câu lạc bộ:</b> Minamoto no Tora</p>
    <p><b>Trường:</b> THPT Huỳnh Văn Nghệ</p>
    <p><b>Thời gian:</b> 23 – 25 / 01 / 2026</p>
  </div>
</section>

<section id="activities">
<h2>🔥 Hoạt Động Nổi Bật</h2>
<div class="activities">
  <button class="activity-btn" onclick="showContent('dalat')">Đà Lạt</button>
  <button class="activity-btn" onclick="showContent('vannghe')">Văn Nghệ</button>
  <button class="activity-btn" onclick="showContent('team')">Team Building</button>
</div>

<div id="dalat" class="activity-content card">
  <h3>🌲 Tham Quan Đà Lạt</h3>
  <p>Khám phá thành phố mộng mơ với những khoảnh khắc đáng nhớ.</p>
  <div class="gallery">
    <img src="https://i.ibb.co/4R8Bddpw/image.png" alt="Đà Lạt 1">
    <img src="https://i.ibb.co/rRZmXmx2/image.png" alt="Đà Lạt 2">
    <img src="https://i.ibb.co/Zp6F7nr1/image.png" alt="Đà Lạt 3">
    <img src="https://i.ibb.co/pB7pCz1J/image.png" alt="Đà Lạt 3">
  </div>
</div>

<div id="vannghe" class="activity-content card">
  <h3>🎤 Văn Nghệ</h3>
  <p>Những tiết mục đặc sắc và đầy cảm xúc.</p>
  <div class="gallery">
    <img src="https://i.ibb.co/5WZC2Dh5/image.png" alt="Văn nghệ 1">
    <img src="https://i.ibb.co/607tq6xL/image.png" alt="Văn nghệ 2">
    <img src="https://i.ibb.co/NQbGFjc/image.png" alt="Văn nghệ 3">
    <img src="https://i.ibb.co/vvRqr5vH/image.png" alt="Văn nghệ 3">
  </div>
</div>

<div id="team" class="activity-content card">
  <h3>🏕️ Team Building</h3>
  <p>Trò chơi vận động giúp tăng tinh thần đoàn kết.</p>
  <div class="gallery">
    <img src="https://i.ibb.co/HL1HFVf9/image.png" alt="Team 1">
    <img src="https://i.ibb.co/Cp9N2rGP/image.png" alt="Team 2">
  
  </div>
</div>

</section>

<section id="contact">
  <div class="card">
    <h2>📞 Liên Hệ</h2>
    <p><b>Lại Thị Thuý Hà</b> – STT: 10 – Lớp 12.9</p>
    <p><b>Lê Thị Phương Nhi</b> – STT: 27 – Lớp 12.9</p>
    <p><b>Đỗ Thành Nhân </b> – STT: 26 – Lớp 12.9</p>
    <p><b>Nguyễn Duy Mạnh</b> – STT: 20 – Lớp 12.9</p>
    <p>Email: thpthuynhvannghe@gmail.com</p>
  </div>
</section>

<footer>
  <h3>CLB Minamoto no Tora 源の虎 12.9</h3>
  <p>Trường THPT Huỳnh Văn Nghệ</p>
  <p>© 2026 - Kỷ yếu Đà Lạt</p>
</footer>

<script>
function showContent(id){
  document.querySelectorAll('.activity-content').forEach(el=>{
    el.style.display='none';
  });
  const box = document.getElementById(id);
  box.style.display='block';
  box.scrollIntoView({behavior:'smooth', block:'start'});
}
</script>

</body>
</html>
