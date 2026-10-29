[index.html](https://github.com/user-attachments/files/34154566/index.html)
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Patisserie Vanilla - باتيسري فانيلا</title>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --pink-main: #E8A5B8;
            --pink-dark: #C7738B;
            --pink-light: #FFF0F4;
            --pink-soft: #F8E5EC;
            --text-color: #332228;
            --text-muted: #7A5C65;
            --white: #FFFFFF;
            --shadow: 0 10px 30px rgba(199, 115, 139, 0.15);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Tajawal', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--pink-light);
            color: var(--text-color);
        }

        /* Navbar */
        header {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 2px solid var(--pink-soft);
            box-shadow: 0 4px 15px rgba(0,0,0,0.03);
        }

        .navbar {
            max-width: 1200px;
            margin: 0 auto;
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
            text-decoration: none;
        }

        .logo-icon {
            width: 45px;
            height: 45px;
            background: linear-gradient(135deg, var(--pink-main), var(--pink-dark));
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            color: var(--white);
            font-size: 1.2rem;
        }

        .logo-text h1 {
            font-size: 1.3rem;
            color: var(--pink-dark);
            font-weight: 800;
        }

        .logo-text span {
            font-size: 0.75rem;
            color: var(--text-muted);
        }

        .nav-links {
            display: flex;
            gap: 20px;
            list-style: none;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-color);
            font-weight: 600;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: var(--pink-dark);
        }

        .btn-header {
            background-color: var(--pink-dark);
            color: var(--white);
            padding: 8px 20px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: 700;
            font-size: 0.9rem;
            transition: 0.3s;
        }

        .btn-header:hover {
            background-color: var(--pink-main);
        }

        /* Hero */
        .hero {
            max-width: 1200px;
            margin: 0 auto;
            padding: 60px 20px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .hero-badge {
            background-color: var(--pink-soft);
            color: var(--pink-dark);
            padding: 6px 16px;
            border-radius: 20px;
            font-weight: 700;
            font-size: 0.9rem;
            display: inline-block;
            margin-bottom: 15px;
        }

        .hero h2 {
            font-size: 2.6rem;
            line-height: 1.2;
            margin-bottom: 15px;
        }

        .hero h2 span {
            color: var(--pink-dark);
        }

        .hero p {
            color: var(--text-muted);
            font-size: 1.1rem;
            margin-bottom: 25px;
        }

        .hero-btns {
            display: flex;
            gap: 15px;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--pink-dark), var(--pink-main));
            color: var(--white);
            padding: 12px 25px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 700;
            box-shadow: var(--shadow);
        }

        .btn-insta {
            background-color: var(--white);
            color: var(--pink-dark);
            border: 2px solid var(--pink-soft);
            padding: 12px 25px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 700;
        }

        .hero-img {
            width: 100%;
            border-radius: 30px;
            box-shadow: var(--shadow);
            object-fit: cover;
            height: 380px;
        }

        /* Specialty Croissant Section */
        .specialty {
            background-color: var(--white);
            padding: 60px 20px;
            border-top: 2px solid var(--pink-soft);
            border-bottom: 2px solid var(--pink-soft);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
        }

        .section-title h3 {
            font-size: 2.2rem;
            color: var(--text-color);
        }

        .section-title p {
            color: var(--text-muted);
        }

        .croissant-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .croissant-card {
            background: var(--pink-light);
            border-radius: 25px;
            overflow: hidden;
            box-shadow: var(--shadow);
            border: 1px solid var(--pink-soft);
        }

        .croissant-card img {
            width: 100%;
            height: 230px;
            object-fit: cover;
        }

        .croissant-info {
            padding: 20px;
            text-align: center;
        }

        .croissant-info h4 {
            font-size: 1.4rem;
            color: var(--pink-dark);
            margin-bottom: 8px;
        }

        /* Catalog Section */
        .catalog {
            padding: 80px 20px;
        }

        .catalog-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .catalog-card {
            background-color: var(--white);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.03);
            border: 1px solid var(--pink-soft);
            transition: 0.3s;
        }

        .catalog-card:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow);
        }

        .catalog-card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }

        .catalog-card-body {
            padding: 15px;
            text-align: center;
        }

        .catalog-card-body h5 {
            font-size: 1.1rem;
            color: var(--text-color);
            margin-bottom: 5px;
        }

        .catalog-card-body p {
            color: var(--text-muted);
            font-size: 0.85rem;
        }

        /* Map & Info */
        .info-section {
            background-color: var(--white);
            padding: 60px 20px;
            border-top: 2px solid var(--pink-soft);
        }

        .info-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .info-box h4 {
            font-size: 1.8rem;
            color: var(--pink-dark);
            margin-bottom: 15px;
        }

        .info-item {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 15px;
            font-size: 1.1rem;
        }

        .info-item i {
            color: var(--pink-dark);
            font-size: 1.3rem;
        }

        .map-btn {
            display: inline-block;
            margin-top: 15px;
            background-color: var(--pink-dark);
            color: var(--white);
            padding: 12px 25px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: 700;
        }

        /* Footer */
        footer {
            background-color: var(--text-color);
            color: var(--white);
            text-align: center;
            padding: 30px 20px;
        }

        footer p {
            color: var(--pink-soft);
            font-size: 0.9rem;
        }

        @media (max-width: 768px) {
            .hero, .info-grid {
                grid-template-columns: 1fr;
                text-align: center;
            }
            .hero-btns {
                justify-content: center;
            }
            .nav-links {
                display: none;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="navbar">
            <a href="#" class="logo">
                <div class="logo-icon"><i class="fa-solid fa-bread-slice"></i></div>
                <div class="logo-text">
                    <h1>Patisserie Vanilla</h1>
                    <span>باتيسري فانيلا</span>
                </div>
            </a>
            <ul class="nav-links">
                <li><a href="#hero">الرئيسية</a></li>
                <li><a href="#croissant">الكرواسون المميز</a></li>
                <li><a href="#catalog">قائمة الأصناف</a></li>
                <li><a href="#location">الموقع والتواصل</a></li>
            </ul>
            <a href="https://www.instagram.com/patisserie__vanill" target="_blank" class="btn-header">
                <i class="fa-brands fa-instagram"></i> انستغرام
            </a>
        </div>
    </header>

    <section class="hero" id="hero">
        <div>
            <span class="hero-badge">🥐 تخصص الكرواسون والحلويات الفاخرة</span>
            <h2>عالم من القرمشة <span>والطعم الفرنسي الأصيل</span></h2>
            <p>نعد لكم يومياً أشهى أنواع الكرواسون المحشو بعناية بأيدي كادر فني مهارته عالية، إلى جانب تشكيلة فاخرة من الكيك والحلويات.</p>
            <div class="hero-btns">
                <a href="#catalog" class="btn-primary">استعرض الأصناف</a>
                <a href="https://www.instagram.com/patisserie__vanill" target="_blank" class="btn-insta">تابعنا على الانستغرام</a>
            </div>
        </div>
        <img src="https://images.unsplash.com/photo-1555507036-ab1f4038808a?auto=format&fit=crop&w=800&q=80" alt="Patisserie Vanilla Hero" class="hero-img">
    </section>

    <!-- Croissant Specialty Section -->
    <section class="specialty" id="croissant">
        <div class="container">
            <div class="section-title">
                <h3>تخصصنا في الكرواسون</h3>
                <p>نصنع لكم النوعين الأحب إلى قلوبكم بطبقات هشّة وزبدة غنية بأيدي خبراء ماهرين</p>
            </div>
            <div class="croissant-grid">
                <div class="croissant-card">
                    <img src="https://images.unsplash.com/photo-1530610476181-d83430b64dcd?auto=format&fit=crop&w=600&q=80" alt="كرواسون جبنة">
                    <div class="croissant-info">
                        <h4>كرواسون الجبنة</h4>
                        <p>عجينة مورقة طازجة محشوة بأجود أنواع الأجبان الغنية.</p>
                    </div>
                </div>
                <div class="croissant-card">
                    <img src="https://images.unsplash.com/photo-1608198093002-ad4e005484ec?auto=format&fit=crop&w=600&q=80" alt="كرواسون شوكولاتة">
                    <div class="croissant-info">
                        <h4>كرواسون الشوكولاتة</h4>
                        <p>محشو بالشوكولاتة اللذيذة المذابة ومخبوز يومياً.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- General Catalog -->
    <section class="catalog" id="catalog">
        <div class="container">
            <div class="section-title">
                <h3>قائمة أصناف باتيسري فانيلا</h3>
                <p>تصفح تشكيلتنا المتنوعة من الحلويات والمخبوزات</p>
            </div>
            <div class="catalog-grid">
                <div class="catalog-card">
                    <img src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?auto=format&fit=crop&w=500&q=80" alt="قوالب الكيك والجاتو">
                    <div class="catalog-card-body">
                        <h5>قوالب الكيك والجاتو</h5>
                        <p>تصاميم فاخرة لمختلف المناسبات</p>
                    </div>
                </div>
                <div class="catalog-card">
                    <img src="https://images.unsplash.com/photo-1551024709-8f23befc6f87?auto=format&fit=crop&w=500&q=80" alt="قطع الكيك والتشيز كيك">
                    <div class="catalog-card-body">
                        <h5>قطع الكيك والتشيز كيك</h5>
                        <p>نكهات غنية ومتنوعة يومياً</p>
                    </div>
                </div>
                <div class="catalog-card">
                    <img src="https://images.unsplash.com/photo-1527515862127-a4fc05baf7a5?auto=format&fit=crop&w=500&q=80" alt="الحلا العربي والمعمول">
                    <div class="catalog-card-body">
                        <h5>الحلا العربي ومعمول التمر</h5>
                        <p>طعم أصيل بالسمن البلدي والفاخر</p>
                    </div>
                </div>
                <div class="catalog-card">
                    <img src="https://images.unsplash.com/photo-1551106652-a5bcf4b29ab6?auto=format&fit=crop&w=500&q=80" alt="الدونات">
                    <div class="catalog-card-body">
                        <h5>الدونات الهشة</h5>
                        <p>بتغطيات الشوكولاتة والكراميل المتنوعة</p>
                    </div>
                </div>
                <div class="catalog-card">
                    <img src="https://images.unsplash.com/photo-1509440159596-0249088772ff?auto=format&fit=crop&w=500&q=80" alt="التوست والمخبوزات">
                    <div class="catalog-card-body">
                        <h5>خبز التوست والمخبوزات</h5>
                        <p>طازجة يومياً لإفطارك المميز</p>
                    </div>
                </div>
                <div class="catalog-card">
                    <img src="https://images.unsplash.com/photo-1558961363-fa8fdf82db35?auto=format&fit=crop&w=500&q=80" alt="السابليه والكوكيز">
                    <div class="catalog-card-body">
                        <h5>السابليه والكوكيز</h5>
                        <p>تشكيلة هشة تذوب في الفم</p>
                    </div>
                </div>
                <div class="catalog-card">
                    <img src="https://images.unsplash.com/photo-1590080875515-8a3a8dc5735e?auto=format&fit=crop&w=500&q=80" alt="البرازق والغريبة">
                    <div class="catalog-card-body">
                        <h5>البرازق والغريبة</h5>
                        <p>نواشف فاخرة ومقرمشة بالفستق والسمسم</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Location and Contact -->
    <section class="info-section" id="location">
        <div class="container info-grid">
            <div class="info-box">
                <h4>زورونا في موقع المحل</h4>
                <div class="info-item">
                    <i class="fa-solid fa-location-dot"></i>
                    <span>منبج، سوريا (GWGV+6XM, Unnamed Road)</span>
                </div>
                <div class="info-item">
                    <i class="fa-brands fa-instagram"></i>
                    <span>@patisserie__vanill</span>
                </div>
                <a href="https://maps.google.com/?q=GWGV%2B6XM,+Unnamed+Road,+Manbij,+Syria" target="_blank" class="map-btn">
                    <i class="fa-solid fa-map-location-dot"></i> افتح الموقع في Google Maps
                </a>
            </div>
            <div>
                <img src="https://images.unsplash.com/photo-1509440159596-0249088772ff?auto=format&fit=crop&w=800&q=80" style="width:100%; border-radius: 20px;" alt="موقع محل فانيلا">
            </div>
        </div>
    </section>

    <footer>
        <p>جميع الحقوق محفوظة &copy; Patisserie Vanilla - باتيسري فانيلا 2026</p>
    </footer>

</body>
</html>
