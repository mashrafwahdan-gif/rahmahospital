<!DOCTYPE html><html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>مستشفى الرحمة | Rahma Hospital</title>  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family: Arial, sans-serif;
    }

    body{
      background:#f4f7fb;
      color:#222;
      line-height:1.6;
    }

    header{
      background: linear-gradient(135deg,#0f62fe,#42a5f5);
      color:white;
      padding:40px 20px;
      text-align:center;
    }

    header h1{
      font-size:32px;
      margin-bottom:10px;
    }

    nav{
      display:flex;
      justify-content:center;
      gap:20px;
      background:white;
      padding:12px;
      position:sticky;
      top:0;
      box-shadow:0 2px 8px rgba(0,0,0,0.1);
    }

    nav a{
      text-decoration:none;
      color:#0f62fe;
      font-weight:bold;
    }

    section{
      max-width:1000px;
      margin:auto;
      padding:40px 20px;
    }

    .hero{
      background:white;
      padding:40px;
      border-radius:15px;
      text-align:center;
      box-shadow:0 4px 12px rgba(0,0,0,0.08);
    }

    .btn{
      margin-top:15px;
      background:#0f62fe;
      color:white;
      border:none;
      padding:12px 20px;
      border-radius:10px;
      cursor:pointer;
      transition:0.3s;
    }

    .btn:hover{
      background:#0043ce;
    }

    .cards{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
      gap:20px;
      margin-top:20px;
    }

    .card{
      background:white;
      padding:20px;
      border-radius:12px;
      text-align:center;
      box-shadow:0 2px 10px rgba(0,0,0,0.08);
      transition:0.3s;
    }

    .card:hover{
      transform:translateY(-5px);
    }

    form{
      background:white;
      padding:20px;
      border-radius:12px;
      box-shadow:0 2px 10px rgba(0,0,0,0.08);
      display:flex;
      flex-direction:column;
      gap:10px;
    }

    input,select{
      padding:10px;
      border:1px solid #ccc;
      border-radius:8px;
    }

    footer{
      text-align:center;
      padding:20px;
      background:#111;
      color:white;
      margin-top:30px;
    }

    .whatsapp{
      position:fixed;
      bottom:20px;
      left:20px;
      background:#25D366;
      color:white;
      padding:12px 15px;
      border-radius:50px;
      text-decoration:none;
      font-weight:bold;
    }
  </style></head><body><header>
  <h1>مستشفى الرحمة</h1>
  <p>رعاية طبية متكاملة على مدار 24 ساعة</p>
</header><nav>
  <a href="#home">الرئيسية</a>
  <a href="#services">الخدمات</a>
  <a href="#doctors">الأطباء</a>
  <a href="#booking">حجز موعد</a>
  <a href="#contact">تواصل</a>
</nav><section id="home" class="hero">
  <h2>صحتك تهمنا ❤️</h2>
  <p>أفضل رعاية طبية بأحدث الأجهزة وأفضل الأطباء</p>
  <button class="btn" onclick="scrollToBooking()">احجز موعد الآن</button>
</section><section id="services">
  <h2>خدماتنا</h2>
  <div class="cards">
    <div class="card">طوارئ 24 ساعة</div>
    <div class="card">عيادات متخصصة</div>
    <div class="card">تحاليل وأشعة</div>
    <div class="card">رعاية أطفال</div>
  </div>
</section><section id="doctors">
  <h2>أطباؤنا</h2>
  <div class="cards">
    <div class="card">د. أحمد - قلب</div>
    <div class="card">د. منى - أطفال</div>
    <div class="card">د. خالد - جراحة</div>
  </div>
</section><section id="booking">
  <h2>حجز موعد</h2>
  <form onsubmit="book(event)">
    <input type="text" placeholder="الاسم الكامل" required />
    <input type="tel" placeholder="رقم الهاتف" required />
    <select required>
      <option value="">اختر الطبيب</option>
      <option>د. أحمد - قلب</option>
      <option>د. منى - أطفال</option>
      <option>د. خالد - جراحة</option>
    </select>
    <input type="date" required />
    <button class="btn" type="submit">تأكيد الحجز</button>
  </form>
</section><section id="contact">
  <h2>تواصل معنا</h2>
  <p>📍 القاهرة - مصر</p>
  <p>📞 01000000000</p>
  <p>✉ info@rahma.com</p>
</section><footer>
  © 2026 مستشفى الرحمة - جميع الحقوق محفوظة
</footer><a class="whatsapp" href="https://wa.me/201000000000" target="_blank">واتساب</a>

<script>
  function book(e){
    e.preventDefault();
    alert("تم حجز الموعد بنجاح! هنكلمك قريب 💙");
  }

  function scrollToBooking(){
    document.getElementById("booking").scrollIntoView({behavior:"smooth"});
  }
</script></body>
</html>
