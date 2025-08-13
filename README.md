<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>صفحتك الترحيبية</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {font-family: 'Cairo', sans-serif; position: relative; transition: background 0.3s, color 0.3s;}
    .fade-in {opacity: 0; transform: translateY(20px); transition: opacity 1s ease, transform 1s ease;}
    .fade-in.show {opacity: 1; transform: translateY(0);}
    #particles-js {position: fixed; width: 100%; height: 100%; top: 0; left: 0; z-index: -1;}
    .dark-mode {background-color: #1a202c; color: #e2e8f0;}
    .dark-mode header, .dark-mode footer, .dark-mode section.bg-white, .dark-mode section.bg-gray-50, .dark-mode form.bg-white {background-color: #2d3748; color: #e2e8f0;}
    .hover-effect:hover {transform: scale(1.08) rotate(1deg); box-shadow: 0 8px 25px rgba(0,0,0,0.2);}
  </style>
  <script src="https://cdn.jsdelivr.net/npm/particles.js"></script>
</head>
<body class="bg-gray-100">
  <!-- Background Animation -->
  <div id="particles-js"></div>

  <!-- Dark Mode Toggle -->
  <button id="darkToggle" class="fixed top-4 left-4 z-50 bg-indigo-600 text-white px-4 py-2 rounded-full shadow hover:bg-indigo-700 transition">🌙</button>

  <!-- Header -->
  <header class="flex justify-between items-center px-8 py-4 bg-white shadow-md sticky top-0 z-40">
    <h1 class="text-2xl font-bold text-indigo-600">شركتي</h1>
    <nav class="space-x-6 hidden md:flex">
      <a href="#features" class="text-gray-600 hover:text-indigo-600 transition">المميزات</a>
      <a href="#services" class="text-gray-600 hover:text-indigo-600 transition">الخدمات</a>
      <a href="#about" class="text-gray-600 hover:text-indigo-600 transition">من نحن</a>
      <a href="#contact" class="text-gray-600 hover:text-indigo-600 transition">تواصل</a>
    </nav>
    <a href="#cta" class="bg-indigo-600 text-white px-4 py-2 rounded-lg hover:bg-indigo-700 transition">جرّب الآن</a>
  </header>

  <!-- Hero Section -->
  <section class="text-center py-20 bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500 text-white relative">
    <h2 class="text-4xl md:text-6xl font-bold mb-6 animate-bounce">مرحباً بك في المستقبل</h2>
    <p class="text-lg md:text-2xl mb-8">حلول مبتكرة لتطوير أعمالك وجذب عملائك</p>
    <a href="#cta" class="bg-white text-indigo-600 px-6 py-3 rounded-full font-bold text-lg hover:bg-gray-100 transition hover-effect">ابدأ الآن</a>
  </section>

  <!-- Features -->
  <section id="features" class="py-16 px-8 grid md:grid-cols-3 gap-8 text-center">
    <div class="bg-white p-6 rounded-2xl shadow hover-effect transition fade-in">
      <h3 class="text-xl font-bold mb-4 text-indigo-600">تصميم عصري</h3>
      <p class="text-gray-600">واجهات جذابة بأحدث معايير التصميم</p>
    </div>
    <div class="bg-white p-6 rounded-2xl shadow hover-effect transition fade-in">
      <h3 class="text-xl font-bold mb-4 text-indigo-600">سرعة الأداء</h3>
      <p class="text-gray-600">أداء فائق وتجربة مستخدم مثالية</p>
    </div>
    <div class="bg-white p-6 rounded-2xl shadow hover-effect transition fade-in">
      <h3 class="text-xl font-bold mb-4 text-indigo-600">دعم مستمر</h3>
      <p class="text-gray-600">خدمة عملاء ودعم تقني على مدار الساعة</p>
    </div>
  </section>

  <!-- Services Section -->
  <section id="services" class="py-16 px-8 bg-gray-50">
    <h2 class="text-3xl font-bold text-center mb-10">خدماتنا</h2>
    <div class="grid md:grid-cols-3 gap-8 text-center">
      <div class="bg-white p-6 rounded-xl shadow hover-effect transition fade-in">
        <h3 class="text-lg font-bold mb-3 text-indigo-600">تصميم مواقع</h3>
        <p class="text-gray-600">تصميم مواقع احترافية عصرية بأحدث التقنيات</p>
      </div>
      <div class="bg-white p-6 rounded-xl shadow hover-effect transition fade-in">
        <h3 class="text-lg font-bold mb-3 text-indigo-600">التسويق الرقمي</h3>
        <p class="text-gray-600">حملات تسويقية مدروسة لزيادة عملائك</p>
      </div>
      <div class="bg-white p-6 rounded-xl shadow hover-effect transition fade-in">
        <h3 class="text-lg font-bold mb-3 text-indigo-600">تحليل البيانات</h3>
        <p class="text-gray-600">تقارير دقيقة لتحسين أداء أعمالك</p>
      </div>
    </div>
  </section>

  <!-- Call to Action -->
  <section id="cta" class="text-center py-16 bg-indigo-600 text-white">
    <h2 class="text-3xl font-bold mb-4">ابدأ رحلتك معنا الآن</h2>
    <p class="mb-6 text-lg">انضم إلى مئات العملاء السعداء وحقق أهدافك بسرعة</p>
    <form class="max-w-md mx-auto flex gap-2">
      <input type="email" placeholder="أدخل بريدك الإلكتروني" class="w-full p-3 rounded-lg text-gray-700 focus:outline-none">
      <button type="submit" class="bg-pink-500 hover:bg-pink-600 px-6 py-3 rounded-lg font-bold hover-effect">اشترك</button>
    </form>
  </section>

  <!-- Contact Form & Social Media -->
  <section id="contact" class="py-16 px-8 bg-gray-100">
    <h2 class="text-3xl font-bold text-center mb-6">تواصل معنا</h2>
    <form class="max-w-lg mx-auto bg-white p-6 rounded-xl shadow space-y-4">
      <input type="text" placeholder="الاسم" class="w-full p-3 border rounded-lg focus:outline-none">
      <input type="email" placeholder="البريد الإلكتروني" class="w-full p-3 border rounded-lg focus:outline-none">
      <textarea placeholder="رسالتك" class="w-full p-3 border rounded-lg focus:outline-none" rows="4"></textarea>
      <button type="submit" class="bg-indigo-600 text-white px-6 py-3 rounded-lg hover:bg-indigo-700 transition w-full hover-effect">إرسال</button>
    </form>
    <div class="flex justify-center mt-6 space-x-4 text-indigo-600 text-2xl">
      <a href="#" class="hover:text-pink-500"><i class="fab fa-facebook"></i></a>
      <a href="#" class="hover:text-pink-500"><i class="fab fa-twitter"></i></a>
      <a href="#" class="hover:text-pink-500"><i class="fab fa-instagram"></i></a>
    </div>
  </section>

  <!-- Footer -->
  <footer class="text-center py-6 bg-gray-200 text-gray-700">
    <p>© 2025 جميع الحقوق محفوظة - شركتي</p>
  </footer>

  <script>
    const fadeElements = document.querySelectorAll('.fade-in');
    window.addEventListener('scroll', () => {
      fadeElements.forEach(el => {
        const rect = el.getBoundingClientRect();
        if(rect.top < window.innerHeight - 100) {
          el.classList.add('show');
        }
      });
    });

    particlesJS('particles-js', {
      particles: {
        number: { value: 80, density: { enable: true, value_area: 800 } },
        color: { value: '#ffffff' },
        shape: { type: 'circle' },
        opacity: { value: 0.5 },
        size: { value: 3 },
        line_linked: { enable: true, color: '#ffffff', opacity: 0.4 },
        move: { enable: true, speed: 3 }
      }
    });

    const darkToggle = document.getElementById('darkToggle');
    darkToggle.addEventListener('click', () => {
      document.body.classList.toggle('dark-mode');
      darkToggle.textContent = document.body.classList.contains('dark-mode') ? '☀️' : '🌙';
    });
  </script>
  <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
</body>
</html>
