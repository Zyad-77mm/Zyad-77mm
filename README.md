<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="موقع رياضي شامل يحتوي على أخبار، نتائج مباشرة، مقاطع فيديو، ونصائح لياقة بدنية">
    <meta name="keywords" content="رياضة, كرة قدم, كرة سلة, لياقة, أخبار رياضية, فيديو رياضي">
    <title>موقع الرياضة الشامل</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- رأس الصفحة (Header) -->
    <header>
        <div class="logo">
            <h1><a href="#">موقع الرياضة الشامل</a></h1>
        </div>
        <nav>
            <ul>
                <li><a href="#home">الصفحة الرئيسية</a></li>
                <li><a href="#news">أخبار الرياضة</a></li>
                <li><a href="#videos">مقاطع الفيديو</a></li>
                <li><a href="#fitness">نصائح لياقة</a></li>
                <li><a href="#live-scores">النتائج المباشرة</a></li>
                <li><a href="#forum">المنتدى</a></li>
                <li><a href="#contact">اتصل بنا</a></li>
            </ul>
        </nav>
    </header>

    <!-- الصفحة الرئيسية (Home Page) -->
    <main>
        <section id="home">
            <h2>أحدث الأخبار الرياضية</h2>
            <article class="news-article">
                <h3>فوز ريال مدريد على برشلونة في الكلاسيكو</h3>
                <p>في مباراة حافلة بالإثارة، تمكن فريق ريال مدريد من الفوز على برشلونة بنتيجة 3-1...</p>
                <a href="#">اقرأ المزيد</a>
            </article>
            <!-- يمكن إضافة المزيد من المقالات -->
        </section>

        <!-- قسم مقاطع الفيديو (Sports Videos) -->
        <section id="videos">
            <h2>أفضل مقاطع الفيديو الرياضية</h2>
            <div class="video-gallery">
                <div class="video">
                    <iframe width="300" height="200" src="https://www.youtube.com/embed/XXXXXXXX" frameborder="0" allowfullscreen></iframe>
                    <p>أفضل أهداف الموسم</p>
                </div>
                <!-- المزيد من مقاطع الفيديو -->
            </div>
        </section>

        <!-- قسم النصائح لياقة بدنية (Fitness Tips) -->
        <section id="fitness">
            <h2>نصائح لياقة بدنية</h2>
            <ul>
                <li>تمارين القوة لبناء العضلات</li>
                <li>تمارين القلب لحرق الدهون</li>
                <li>نصائح حول التغذية الرياضية</li>
            </ul>
        </section>

        <!-- قسم النتائج المباشرة (Live Scores) -->
        <section id="live-scores">
            <h2>النتائج المباشرة</h2>
            <div class="live-score">
                <p><strong>الدوري الإنجليزي:</strong> مانشستر يونايتد 2-1 مانشستر سيتي</p>
                <p><strong>الدوري الإسباني:</strong> ريال مدريد 3-1 برشلونة</p>
                <!-- المزيد من النتائج -->
            </div>
        </section>

        <!-- قسم المنتدى الرياضي (Sports Forum) -->
        <section id="forum">
            <h2>المنتدى الرياضي</h2>
            <p>ناقش آخر الأحداث الرياضية مع الأعضاء الآخرين في المنتدى الرياضي. <a href="#">انضم إلى المنتدى الآن</a></p>
        </section>
    </main>

    <!-- التذييل (Footer) -->
    <footer>
        <p>&copy; 2024 موقع الرياضة الشامل. جميع الحقوق محفوظة.</p>
        <p><a href="#contact">اتصل بنا</a></p>
    </footer>

</body>
</html>
/* الأساسيات */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

/* تصميم الهيدر */
header {
    background-color: #333;
    color: white;
    padding: 15px;
    text-align: center;
}

header .logo h1 a {
    color: white;
    text-decoration: none;
    font-size: 2rem;
}

/* تصميم القوائم */
nav ul {
    list-style: none;
    padding: 0;
    display: flex;
    justify-content: center;
    margin-top: 15px;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 1.2rem;
}

nav ul li a:hover {
    text-decoration: underline;
}

/* تصميم الصفحة الرئيسية */
main {
    padding: 20px;
    background-color: #f4f4f4;
}

h2 {
    font-size: 2rem;
    color: #333;
}

.news-article {
    margin-bottom: 20px;
}

.news-article h3 {
    font-size: 1.8rem;
    color: #444;
}

a {
    text-decoration: none;
    color: #007BFF;
}

a:hover {
    text-decoration: underline;
}

/* تصميم قسم الفيديوهات */
.video-gallery {
    display: flex;
    gap: 20px;
}

.video iframe {
    width: 100%;
    max-width: 300px;
    height: 200px;
}

/* تصميم النتائج المباشرة */
.live-score p {
    font-size: 1.2rem;
    margin-bottom: 10px;
}

/* التصميم المتجاوب */
@media (max-width: 768px) {
    header .logo h1 {
        font-size: 1.5rem;
    }

    nav ul {
        flex-direction: column;
        margin-top: 10px;
    }

    nav ul li {
        margin: 5px 0;
    }

    .video-gallery {
        flex-direction: column;
    }

    .video iframe {
        max-width: 100%;
    }
}
<button id="loadMoreNews">عرض المزيد من الأخبار</button>
<div id="newsSection"></div>

<script>
document.getElementById('loadMoreNews').addEventListener('click', function() {
    let newsSection = document.getElementById('newsSection');
    newsSection.innerHTML += "<p>تم إضافة المزيد من الأخبار...</p>";  // يمكن تحميل الأخبار من API هنا
});
</script>
