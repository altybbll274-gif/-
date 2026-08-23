<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> مدرسة الأمير بشير الشريف الثانوية بنات</title>
    <meta name="description" content="مدرسة الأمير بشير الشريف الثانوية بنات - مؤسسة تعليمية رائدة تهدف إلى تمكين الطالبات وتطوير قدراتهن الأكاديمية والشخصية.">
    
    <!-- يمكنك إضافة Font Awesome للأيقونات -->
    <!-- <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"> -->
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #FFFFFF;
            color: #1F2937;
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Header & Navigation */
        header {
            background: linear-gradient(135deg, #1F2937 0%, #374151 100%);
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 20px rgba(0,0,0,0.2);
            transition: all 0.3s ease;
        }

        header.scrolled {
            padding: 0.5rem 0;
            background: rgba(31, 41, 55, 0.95);
            backdrop-filter: blur(10px);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 1rem;
            text-decoration: none;
            color: white;
        }

        .logo img {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid #3B82F6;
            transition: transform 0.3s ease;
        }

        .logo:hover img {
            transform: rotate(360deg);
        }

        .logo-text {
            font-size: 1.2rem;
            font-weight: bold;
            color: white;
            line-height: 1.4;
        }

        .logo-text span {
            color: #3B82F6;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            font-size: 1rem;
            position: relative;
            padding: 0.5rem 0;
            transition: color 0.3s ease;
        }

        nav ul li a::after {
            content: '';
            position: absolute;
            bottom: 0;
            right: 0;
            width: 0;
            height: 2px;
            background: #3B82F6;
            transition: width 0.3s ease;
        }

        nav ul li a:hover {
            color: #3B82F6;
        }

        nav ul li a:hover::after {
            width: 100%;
        }

        .hamburger {
            display: none;
            cursor: pointer;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
        }

        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, rgba(31, 41, 55, 0.9), rgba(59, 130, 246, 0.7)), url('https://placehold.co/1920x1080/1F2937/FFFFFF?text=مدرسة+الأمير+بشير+الشريف') no-repeat center center/cover;
            background-color: #1F2937;
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 80px;
        }

        .hero-content {
            max-width: 800px;
            animation: fadeInUp 1s ease;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
            line-height: 1.3;
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            opacity: 0.95;
        }

        .hero-buttons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 0.8rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }

        .btn-primary {
            background: #3B82F6;
            color: white;
            box-shadow: 0 4px 15px rgba(59, 130, 246, 0.4);
        }

        .btn-primary:hover {
            background: #2563EB;
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(59, 130, 246, 0.6);
        }

        .btn-outline {
            background: transparent;
            color: white;
            border: 2px solid white;
        }

        .btn-outline:hover {
            background: white;
            color: #1F2937;
            transform: translateY(-3px);
        }

        /* Sections */
        .section {
            padding: 5rem 2rem;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: #1F2937;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background: #3B82F6;
            margin: 1rem auto;
            border-radius: 2px;
        }

        .section-subtitle {
            text-align: center;
            color: #6B7280;
            margin-bottom: 3rem;
            font-size: 1.1rem;
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            max-width: 1200px;
            margin: 0 auto;
            align-items: center;
        }

        .about-image {
            position: relative;
            overflow: hidden;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }

        .about-image img {
            width: 100%;
            height: 400px;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .about-image:hover img {
            transform: scale(1.05);
        }

        .about-content h3 {
            font-size: 2rem;
            color: #1F2937;
            margin-bottom: 1.5rem;
        }

        .about-content p {
            color: #4B5563;
            margin-bottom: 1.5rem;
            font-size: 1.1rem;
        }

        .features-list {
            list-style: none;
            margin-top: 2rem;
        }

        .features-list li {
            padding: 0.5rem 0;
            display: flex;
            align-items: center;
            gap: 1rem;
            color: #4B5563;
        }

        .features-list li::before {
            content: '✓';
            color: #3B82F6;
            font-weight: bold;
            font-size: 1.2rem;
        }

        /* Programs */
        .programs {
            background: linear-gradient(135deg, #F3F4F6 0%, #E5E7EB 100%);
        }

        .programs-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .program-card {
            background: white;
            border-radius: 20px;
            padding: 2rem;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            border: 2px solid transparent;
        }

        .program-card:hover {
            transform: translateY(-10px);
            border-color: #3B82F6;
            box-shadow: 0 20px 40px rgba(59, 130, 246, 0.2);
        }

        .program-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
            color: #3B82F6;
        }

        .program-card h3 {
            font-size: 1.5rem;
            color: #1F2937;
            margin-bottom: 1rem;
        }

        .program-card p {
            color: #6B7280;
            margin-bottom: 1.5rem;
        }

        .program-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
            margin-bottom: 1rem;
        }

        /* Statistics */
        .stats {
            background: linear-gradient(135deg, #1F2937, #374151);
            color: white;
            padding: 4rem 2rem;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
            text-align: center;
        }

        .stat-item {
            padding: 1.5rem;
        }

        .stat-number {
            font-size: 3rem;
            font-weight: bold;
            color: #3B82F6;
            margin-bottom: 0.5rem;
        }

        .stat-label {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        /* Gallery */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 15px;
            cursor: pointer;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        .gallery-item img {
            width: 100%;
            height: 300px;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .gallery-item:hover img {
            transform: scale(1.1);
        }

        .gallery-overlay {
            position: absolute;
            bottom: 0;
            right: 0;
            left: 0;
            background: linear-gradient(transparent, rgba(31, 41, 55, 0.9));
            color: white;
            padding: 1.5rem;
            transform: translateY(100%);
            transition: transform 0.3s ease;
        }

        .gallery-item:hover .gallery-overlay {
            transform: translateY(0);
        }

        /* Contact */
        .contact {
            background: linear-gradient(135deg, #F3F4F6 0%, #E5E7EB 100%);
        }

        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .contact-info {
            padding: 2rem;
            background: white;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }

        .contact-info h3 {
            margin-bottom: 2rem;
            color: #1F2937;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1.5rem;
            padding: 1rem;
            background: #F9FAFB;
            border-radius: 10px;
            transition: all 0.3s ease;
        }

        .contact-item:hover {
            background: #E5E7EB;
            transform: translateX(-5px);
        }

        .contact-icon {
            font-size: 1.5rem;
            color: #3B82F6;
        }

        .contact-form {
            padding: 2rem;
            background: white;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }

        .contact-form h3 {
            margin-bottom: 2rem;
            color: #1F2937;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            color: #1F2937;
            font-weight: 500;
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 0.8rem;
            border: 2px solid #E5E7EB;
            border-radius: 10px;
            font-size: 1rem;
            transition: all 0.3s ease;
            background: #F9FAFB;
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: #3B82F6;
            box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.1);
        }

        /* Footer */
        footer {
            background: #1F2937;
            color: white;
            padding: 3rem 2rem 1rem;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-section h3 {
            margin-bottom: 1rem;
            color: #3B82F6;
        }

        .footer-section p {
            color: #9CA3AF;
            line-height: 1.8;
        }

        .footer-section a {
            color: #9CA3AF;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-section a:hover {
            color: #3B82F6;
        }

        .footer-bottom {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid #374151;
            color: #9CA3AF;
        }

        .copyright {
            font-size: 0.9rem;
        }

        .copyright strong {
            color: #3B82F6;
        }

        /* Animations */
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .fade-in {
            animation: fadeIn 1s ease;
        }

        /* Success Message */
        .success-message {
            display: none;
            text-align: center;
            padding: 2rem;
            background: #F0FDF4;
            border: 2px solid #22C55E;
            border-radius: 10px;
            margin-top: 1rem;
        }

        .success-message.show {
            display: block;
            animation: fadeIn 0.5s ease;
        }

        .success-message h3 {
            color: #22C55E;
            margin-bottom: 0.5rem;
        }

        .success-message p {
            color: #166534;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-container { padding: 0 1rem; }
            .hamburger { display: block; }
            nav ul {
                display: none;
                position: absolute;
                top: 100%;
                right: 0;
                left: 0;
                background: #1F2937;
                flex-direction: column;
                padding: 1rem;
                gap: 0.5rem;
                box-shadow: 0 10px 20px rgba(0,0,0,0.3);
            }
            nav ul.show { display: flex; animation: fadeIn 0.3s ease; }
            nav ul li a { display: block; padding: 1rem; }
            .hero h1 { font-size: 2rem; }
            .hero p { font-size: 1rem; }
            .about-grid, .contact-grid { grid-template-columns: 1fr; gap: 2rem; }
            .section { padding: 3rem 1rem; }
            .section-title { font-size: 1.8rem; }
            .stats-grid { grid-template-columns: repeat(2, 1fr); }
            .programs-grid, .gallery-grid { grid-template-columns: 1fr; }
        }

        @media (max-width: 480px) {
            .hero-buttons { flex-direction: column; width: 100%; }
            .btn { width: 100%; text-align: center; }
            .stats-grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

    <header id="header">
        <div class="nav-container">
            <a href="#home" class="logo">
                <img src="https://placehold.co/60/60/1F2937/FFFFFF?text=م" alt="شعار المدرسة">
                <div class="logo-text">
                    مدرسة الأمير بشير الشريف<br>
                    <span>الثانوية بنات</span>
                </div>
            </a>
            <button class="hamburger" onclick="toggleMenu()">☰</button>
            <nav>
                <ul id="nav-menu">
                    <li><a href="#home" onclick="closeMenu()">الرئيسية</a></li>
                    <li><a href="#about" onclick="closeMenu()">عن المدرسة</a></li>
                    <li><a href="#programs" onclick="closeMenu()">البرامج</a></li>
                    <li><a href="#gallery" onclick="closeMenu()">المعرض</a></li>
                    <li><a href="#contact" onclick="closeMenu()">اتصل بنا</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section class="hero" id="home">
        <div class="hero-content">
            <h1>مدرسة الأمير بشير الشريف الثانوية بنات</h1>
            <p>مؤسسة تعليمية رائدة تهدف إلى تمكين الطالبات وتطوير قدراتهن الأكاديمية والشخصية في بيئة تعليمية متميزة</p>
            <div class="hero-buttons">
                <a href="#about" class="btn btn-primary">اكتشف المزيد</a>
                <a href="#contact" class="btn btn-outline">تواصل معنا</a>
            </div>
        </div>
    </section>

    <section class="section" id="about">
        <h2 class="section-title">عن مدرستنا</h2>
        <p class="section-subtitle">نلتزم بتقديم تعليم عالي الجودة لجميع الطالبات</p>
        <div class="about-grid">
            <div class="about-image">
                <img src="https://placehold.co/600x400/1F2937/FFFFFF?text=صورة+المدرسة" alt="عن المدرسة">
            </div>
            <div class="about-content">
                <h3>رسالتنا ورؤيتنا</h3>
                <p>تسعى مدرسة الأمير بشير الشريف الثانوية بنات إلى توفير بيئة تعليمية محفزة تساعد الطالبات على تحقيق أهدافهن الأكاديمية والشخصية. نحن نؤمن بأن كل طالبة لديها القدرة على النجاح والتميز.</p>
                <p>نوفر برامج تعليمية متطورة ومرافق حديثة وفريق تدريسي مؤهل لضمان أفضل تجربة تعليمية ممكنة.</p>
                <ul class="features-list">
                    <li>منهج تعليمي متطور ومعتمد</li>
                    <li>فريق تدريسي مؤهل وذو خبرة</li>
                    <li>مرافق حديثة ومجهزة بأحدث التقنيات</li>
                    <li>أنشطة لا منهجية متنوعة ومبتكرة</li>
                    <li>بيئة تعليمية آمنة وداعمة</li>
                    <li>متابعة فردية لكل طالبة</li>
                </ul>
            </div>
        </div>
    </section>

    <section class="section programs" id="programs">
        <h2 class="section-title">برامجنا التعليمية</h2>
        <p class="section-subtitle">برامج متنوعة تناسب احتياجات جميع الطالبات</p>
        <div class="programs-grid">
            <div class="program-card">
                <div class="program-icon">📚</div>
                <img src="https://placehold.co/600x400/1F2937/FFFFFF?text=المنهج+الأكاديمي" alt="المنهج الأكاديمي">
                <h3>المنهج الأكاديمي</h3>
                <p>منهج شامل ومتطور يغطي جميع المواد الأساسية وفق أعلى المعايير التعليمية</p>
                <a href="#contact" class="btn btn-primary">اعرف المزيد</a>
            </div>
            <div class="program-card">
                <div class="program-icon">🎨</div>
                <img src="https://placehold.co/600x400/1F2937/FFFFFF?text=الأنشطة+اللامنهجية" alt="الأنشطة اللامنهجية">
                <h3>الأنشطة اللامنهجية</h3>
                <p>مجموعة واسعة من الأنشطة الرياضية والفنية والثقافية لتطوير المهارات</p>
                <a href="#contact" class="btn btn-primary">اعرف المزيد</a>
            </div>
            <div class="program-card">
                <div class="program-icon">💻</div>
                <img src="https://placehold.co/600x400/1F2937/FFFFFF?text=التقنية+والمعلوماتية" alt="التقنية والمعلوماتية">
                <h3>التقنية والمعلوماتية</h3>
                <p>برامج تقنية متقدمة لإعداد الطالبات لمستقبل رقمي مشرق</p>
                <a href="#contact" class="btn btn-primary">اعرف المزيد</a>
            </div>
        </div>
    </section>

    <section class="stats">
        <div class="stats-grid">
            <div class="stat-item">
                <div class="stat-number" data-target="500">0</div>
                <div class="stat-label">طالبة</div>
            </div>
            <div class="stat-item">
                <div class="stat-number" data-target="50">0</div>
                <div class="stat-label">معلمة</div>
            </div>
            <div class="stat-item">
                <div class="stat-number" data-target="98">0</div>
                <div class="stat-label">نسبة النجاح %</div>
            </div>
            <div class="stat-item">
                <div class="stat-number" data-target="15">0</div>
                <div class="stat-label">عاماً من التميز</div>
            </div>
        </div>
    </section>

    <section class="section" id="gallery">
        <h2 class="section-title">معرض الصور</h2>
        <p class="section-subtitle">لقطات من حياتنا المدرسية وأنشطتنا</p>
        <div class="gallery-grid">
            <div class="gallery-item">
                <img src="https://placehold.co/800x600/1F2937/FFFFFF?text=الحرم+المدرسي" alt="الحرم المدرسي">
                <div class="gallery-overlay"><h3>الحرم المدرسي</h3><p>مرافق حديثة ومجهزة</p></div>
            </div>
            <div class="gallery-item">
                <img src="https://placehold.co/800x600/1F2937/FFFFFF?text=الفصول+الدراسية" alt="الفصول الدراسية">
                <div class="gallery-overlay"><h3>الفصول الدراسية</h3><p>بيئة تعليمية محفزة</p></div>
            </div>
            <div class="gallery-item">
                <img src="https://placehold.co/800x600/1F2937/FFFFFF?text=المكتبة" alt="المكتبة">
                <div class="gallery-overlay"><h3>المكتبة</h3><p>مصادر تعليمية متنوعة</p></div>
            </div>
            <div class="gallery-item">
                <img src="https://placehold.co/800x600/1F2937/FFFFFF?text=المختبرات" alt="المختبرات">
                <div class="gallery-overlay"><h3>المختبرات العلمية</h3><p>تجارب علمية عملية</p></div>
            </div>
            <div class="gallery-item">
                <img src="https://placehold.co/800x600/1F2937/FFFFFF?text=الملعب+الرياضي" alt="الملعب الرياضي">
                <div class="gallery-overlay"><h3>الملعب الرياضي</h3><p>أنشطة رياضية متنوعة</p></div>
            </div>
            <div class="gallery-item">
                <img src="https://placehold.co/800x600/1F2937/FFFFFF?text=الأنشطة+الطلابية" alt="الأنشطة الطلابية">
                <div class="gallery-overlay"><h3>الأنشطة الطلابية</h3><p>فعاليات ومناسبات مدرسية</p></div>
            </div>
        </div>
    </section>

    <section class="section contact" id="contact">
        <h2 class="section-title">تواصل معنا</h2>
        <p class="section-subtitle">نحن هنا للإجابة على جميع استفساراتكم</p>
        <div class="contact-grid">
            <div class="contact-info">
                <h3>معلومات التواصل</h3>
                <div class="contact-item"><span class="contact-icon">📍</span><div><h4>العنوان</h4><p>الخرطوم - السودان</p></div></div>
                <div class="contact-item"><span class="contact-icon">📞</span><div><h4>الهاتف</h4><p>249+ XX XXX XXXX</p></div></div>
                <div class="contact-item"><span class="contact-icon">✉️</span><div><h4>البريد الإلكتروني</h4><p>info@school.edu.sd</p></div></div>
                <div class="contact-item"><span class="contact-icon">🕐</span><div><h4>ساعات العمل</h4><p>الأحد - الخميس: 7:00 ص - 3:00 م</p></div></div>
            </div>
            <div class="contact-form">
                <h3>أرسل لنا رسالة</h3>
                <form id="contactForm">
                    <div class="form-group">
                        <label for="name">الاسم الكامل</label>
                        <input type="text" id="name" name="name" required placeholder="أدخل اسمك الكامل">
                    </div>
                    <div class="form-group">
                        <label for="email">البريد الإلكتروني</label>
                        <input type="email" id="email" name="email" required placeholder="example@email.com">
                    </div>
                    <div class="form-group">
                        <label for="phone">رقم الهاتف</label>
                        <input type="tel" id="phone" name="phone" placeholder="أدخل رقم هاتفك">
                    </div>
                    <div class="form-group">
                        <label for="subject">الموضوع</label>
                        <select id="subject" name="subject" required>
                            <option value="">اختر الموضوع</option>
                            <option value="admission">الالتحاق والتسجيل</option>
                            <option value="programs">البرامج التعليمية</option>
                            <option value="activities">الأنشطة المدرسية</option>
                            <option value="other">استفسار عام</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="message">الرسالة</label>
                        <textarea id="message" name="message" rows="5" required placeholder="اكتب رسالتك هنا..."></textarea>
                    </div>
                    <button type="submit" class="btn btn-primary" style="width: 100%;">إرسال الرسالة</button>
                </form>
                <div class="success-message" id="successMessage">
                    <h3>✓ تم استلام رسالتك</h3>
                    <p>شكراً لتواصلك معنا. سنقوم بالرد عليك في أقرب وقت ممكن.</p>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="footer-content">
            <div class="footer-section">
                <h3>عن المدرسة</h3>
                <p>مدرسة الأمير بشير الشريف الثانوية بنات - مؤسسة تعليمية رائدة تهدف إلى تمكين الطالبات وتطوير قدراتهن الأكاديمية والشخصية.</p>
            </div>
            <div class="footer-section">
                <h3>روابط سريعة</h3>
                <p><a href="#home">الرئيسية</a></p>
                <p><a href="#about">عن المدرسة</a></p>
                <p><a href="#programs">البرامج</a></p>
                <p><a href="#gallery">المعرض</a></p>
                <p><a href="#contact">اتصل بنا</a></p>
            </div>
            <div class="footer-section">
                <h3>تواصل معنا</h3>
                <p>📍 الخرطوم - السودان</p>
                <p>📞 249+ XX XXX XXXX</p>
                <p>✉️ info@school.edu.sd</p>
            </div>
        </div>
        <div class="footer-bottom">
            <p class="copyright">جميع الحقوق محفوظة © <strong>مدرسة الأمير بشير الشريف الثانوية بنات</strong> 2026</p>
        </div>
    </footer>

    <script>
        // 1. القائمة المتنقلة للهواتف
        function toggleMenu() {
            const menu = document.getElementById('nav-menu');
            menu.classList.toggle('show');
        }
        function closeMenu() {
            const menu = document.getElementById('nav-menu');
            if (menu.classList.contains('show')) {
                menu.classList.remove('show');
            }
        }

        // 2. تأثير الشريط عند التمرير
        const header = document.getElementById('header');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });

        // 3. العدادات الإحصائية المتحركة
        const counters = document.querySelectorAll('.stat-number');
        const speed = 200;

        const animateCounters = () => {
            counters.forEach(counter => {
                const target = +counter.getAttribute('data-target');
                const count = +counter.innerText;
                const increment = target / speed;
                if (count < target) {
                    counter.innerText = Math.ceil(count + increment);
                    setTimeout(animateCounters, 10);
                } else {
                    counter.innerText = target;
                }
            });
        };

        // تشغيل العدادات عند الوصول للقسم
        const statsSection = document.querySelector('.stats');
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    animateCounters();
                    observer.unobserve(statsSection);
                }
            });
        }, { threshold: 0.5 });
        observer.observe(statsSection);

        // 4. التحقق من النموذج وإرساله
        const form = document.getElementById('contactForm');
        const successMessage = document.getElementById('successMessage');

        form.addEventListener('submit', function(e) {
            e.preventDefault();
            
            // التحقق من صحة البيانات
            const name = document.getElementById('name').value.trim();
            const email = document.getElementById('email').value.trim();
            const subject = document.getElementById('subject').value;
            const message = document.getElementById('message').value.trim();

            if (!name || !email || !subject || !message) {
                alert('يرجى ملء جميع الحقول المطلوبة');
                return;
            }

            // محاكاة الإرسال الناجح
            form.reset();
            successMessage.classList.add('show');
            
            // يإخفاء رسالة النجاح بعد 5 ثوانٍ
            setTimeout(() => {
                successMessage.classList.remove('show');
            }, 5000);
        });

        // 5. تمرير سلس عند النقر على روابط التنقل
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                window.scrollTo({
                    top: targetElement.offsetTop - 80,
                    behavior: 'smooth'
                });
            });
        });
    </script>

</body>
</html>
