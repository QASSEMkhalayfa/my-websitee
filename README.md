ميح
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مجموعة الأحاديث</title>
    <style>
        body {
            font-family: 'Tajawal', Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 20px;
            color: #333;
            transition: background-color 0.3s, color 0.3s;
        }

        header {
            background-color: #4CAF50; /* لون أخضر */
            color: white;
            padding: 20px;
            text-align: center;
            border-radius: 10px;
            margin-bottom: 20px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            transition: background-color 0.3s;
            animation: fadeIn 0.5s ease-in-out;
        }

        nav {
            margin-bottom: 20px;
            display: flex;
            justify-content: center;
            gap: 15px;
        }

        nav a {
            padding: 10px 15px;
            text-decoration: none;
            color: white;
            background-color: #4CAF50; /* لون أخضر */
            border-radius: 5px;
            transition: background-color 0.3s, transform 0.3s;
            animation: slideIn 0.5s ease-in-out;
        }

        nav a:hover {
            background-color: #45a049; /* لون أخضر أغمق */
            transform: scale(1.05);
        }

        .section {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
            padding: 20px;
            transition: transform 0.3s;
            opacity: 0;
            animation: fadeIn 0.5s forwards;
        }

        .section:hover {
            transform: translateY(-5px);
        }

        h2 {
            color: #4CAF50; /* لون أخضر */
            margin-bottom: 10px;
        }

        footer {
            text-align: center;
            margin-top: 20px;
            font-size: 14px;
            color: #777;
        }

        .dark-mode {
            background-color: #1e1e2f; /* لون داكن */
            color: #fff;
        }

        .dark-mode header {
            background-color: #333; /* لون داكن */
        }

        .dark-mode nav a {
            background-color: #333; /* لون داكن */
            color: white;
        }

        .dark-mode nav a:hover {
            background-color: #45a049; /* لون أخضر أغمق */
        }

        .dark-mode .section {
            background-color: #2d2d44; /* لون داكن */
            color: #fff;
        }

        .dark-mode footer {
            color: #bbb;
        }

        .dark-mode-toggle {
            position: fixed;
            bottom: 20px;
            left: 20px; /* تغيير إلى الجهة اليسرى */
            padding: 10px 15px;
            background-color: #4CAF50; /* لون أخضر */
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .dark-mode-toggle:hover {
            background-color: #45a049; /* لون أخضر أغمق */
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes slideIn {
            from { transform: translateY(-20px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        .info {
            display: none;
            background-color: #e7f3fe; /* لون أزرق فاتح */
            border-left: 6px solid #2196F3; /* لون أزرق */
            padding: 10px;
            margin-top: 10px;
            border-radius: 5px;
        }

        .toggle-info {
            cursor: pointer;
            color: #4CAF50; /* لون أخضر */
            font-weight: bold;
            display: block;
            margin-top: 10px;
        }

        .toggle-info.up::after {
            content: ' ▲'; /* سهم لأعلى */
        }

        .toggle-info.down::after {
            content: ' ▼'; /* سهم لأسفل */
        }

        .additional-note {
            margin-top: 20px;
            background-color: #fff3cd; /* لون أصفر فاتح */
            border: 1px solid #ffeeba; /* لون أصفر */
            padding: 15px;
            border-radius: 5px;
            font-weight: bold;
            text-align: center;
        }

        .button {
            display: inline-block;
            padding: 10px 15px;
            margin: 5px;
            text-decoration: none;
            color: white;
            background: linear-gradient(90deg, #007bff, #0056b3); /* تدرج لوني أزرق */
            border-radius: 5px;
            transition: background 0.3s, transform 0.3s;
        }

        .button:hover {
            background: linear-gradient(90deg, #0056b3, #007bff); /* تدرج لوني عند التمرير */
            transform: scale(1.05);
        }

        @media (max-width: 600px) {
            nav {
                flex-direction: column;
                align-items: center;
            }

            nav a {
                width: 100%;
                text-align: center;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>الأحاديث النبوية الشريفة</h1>
    <p>الكتب الستة و التي هي الاساس و كتاب الامام احمد و الموطا للامام مالك</p>
</header>

<nav>
    <a href="#bukhari">صحيح البخاري</a>
    <a href="#muslim">صحيح مسلم</a>
    <a href="#abu-dawood">سنن أبي داود</a>
    <a href="#tirmidhi">جامع الترمذي</a>
    <a href="#nasaai">سنن النسائي</a>
    <a href="#ibn-majah">سنن ابن ماجه</a>
    <a href="#malik">موطأ مالك</a>
    <a href="#ahmad">مسند أحمد</a>
</nav>

<!-- قسم الكتب الستة -->
<h2>الكتب الستة</h2>
<div class="section" id="bukhari">
    <h2>صحيح البخاري</h2>
    <p>يمكنك الاطلاع على الأحاديث من صحيح البخاري من خلال الرابط التالي:</p>
    <a href="books/bukhari.pdf" target="_blank" class="button">عرض صحيح البخاري</a>
    <a href="books/bukhari.pdf" download class="button">تحميل صحيح البخاري</a>
    <span class="toggle-info down">معلومات الكتاب</span>
    <div class="info">
        <p>صحيح البخاري: أصح كتاب حديث عند أهل السنة، جمعه الإمام البخاري بدقة شديدة، ويضم <strong>2,600 حديث بدون تكرار</strong>.</p>
    </div>
</div>

<div class="section" id="muslim">
    <h2>صحيح مسلم</h2>
    <p>يمكنك الاطلاع على الأحاديث من صحيح مسلم من خلال الرابط التالي:</p>
    <a href="books/muslim.pdf" target="_blank" class="button">عرض صحيح مسلم</a>
    <a href="books/muslim.pdf" download class="button">تحميل صحيح مسلم</a>
    <span class="toggle-info down">معلومات الكتاب</span>
    <div class="info">
        <p>صحيح مسلم: ثاني أصح كتب الحديث، جمعه الإمام مسلم ورتّبه بدقة موضوعية، ويضم <strong>3,033 حديثًا بدون تكرار</strong>.</p>
    </div>
</div>

<div class="section" id="abu-dawood">
    <h2>سنن أبي داود</h2>
    <p>يمكنك الاطلاع على الأحاديث من سنن أبي داود من خلال الرابط التالي:</p>
    <a href="books/abu-dawood.pdf" target="_blank" class="button">عرض سنن أبي داود</a>
    <a href="books/abu-dawood.pdf" download class="button">تحميل سنن أبي داود</a>
    <span class="toggle-info down">معلومات الكتاب</span>
    <div class="info">
        <p>سنن أبي داود: كتاب فقهي يحتوي على <strong>5,274 حديثًا</strong>، جمعه الإمام أبو داود، ويضم أحاديث صحيحة وحسنة وضعيفة مع بيان درجتها غالبًا.</p>
    </div>
</div>

<div class="section" id="tirmidhi">
    <h2>جامع الترمذي</h2>
    <p>يمكنك الاطلاع على الأحاديث من جامع الترمذي من خلال الرابط التالي:</p>
    <a href="books/tirmidhi.pdf" target="_blank" class="button">عرض جامع الترمذي</a>
    <a href="books/tirmidhi.pdf" download class="button">تحميل جامع الترمذي</a>
    <span class="toggle-info down">معلومات الكتاب</span>
    <div class="info">
        <p>سنن الترمذي: يتميز بتقسيم الأحاديث إلى صحيحة وحسنة وضعيفة، ويضم <strong>4,000 حديث</strong> مع شروح للفقهاء وآراء الصحابة.</p>
    </div>
</div>

<div class="section" id="nasaai">
    <h2>سنن النسائي</h2>
    <p>يمكنك الاطلاع على الأحاديث من سنن النسائي من خلال الرابط التالي:</p>
    <a href="books/nasaai.pdf" target="_blank" class="button">عرض سنن النسائي</a>
    <a href="books/nasaai.pdf" download class="button">تحميل سنن النسائي</a>
    <span class="toggle-info down">معلومات الكتاب</span>
    <div class="info">
        <p>سنن النسائي: من أدق كتب السنن في الصحة بعد البخاري ومسلم، يركز على الأحاديث الفقهية، ويحتوي على <strong>5,000 حديث</strong>.</p>
    </div>
</div>

<div class="section" id="ibn-majah">
    <h2>سنن ابن ماجه</h2>
    <p>يمكنك الاطلاع على الأحاديث من سنن ابن ماجه من خلال الرابط التالي:</p>
    <a href="books/ibn-majah.pdf" target="_blank" class="button">عرض سنن ابن ماجه</a>
    <a href="books/ibn-majah.pdf" download class="button">تحميل سنن ابن ماجه</a>
    <span class="toggle-info down">معلومات الكتاب</span>
    <div class="info">
        <p>سنن ابن ماجه: يضم <strong>4,341 حديثًا</strong>، منها أحاديث زائدة عن الكتب الخمسة الأخرى، لكنه يحتوي على عدد أكبر من الأحاديث الضعيفة.</p>
    </div>
</div>

<!-- قسم الموطأ وكتاب أحمد -->
<h2>كتب أخرى</h2>
<div class="section" id="malik">
    <h2>موطأ مالك</h2>
    <p>يمكنك الاطلاع على الأحاديث من موطأ مالك من خلال الرابط التالي:</p>
    <a href="books/malik.pdf" target="_blank" class="button">عرض موطأ مالك</a>
    <a href="books/malik.pdf" download class="button">تحميل موطأ مالك</a>
    <span class="toggle-info down">معلومات الكتاب</span>
    <div class="info">
        <p>موطأ مالك: من أقدم كتب الحديث، يضم <strong>1,720 حديثًا</strong> بين مرفوع وموقوف، ويمزج بين الحديث والفقه المالكي.</p>
    </div>
</div>

<div class="section" id="ahmad">
    <h2>مسند أحمد</h2>
    <p>يمكنك الاطلاع على الأحاديث من مسند أحمد من خلال الرابط التالي:</p>
    <a href="books/ahmad.pdf" target="_blank" class="button">عرض مسند أحمد</a>
    <a href="books/ahmad.pdf" download class="button">تحميل مسند أحمد</a>
    <span class="toggle-info down">معلومات الكتاب</span>
    <div class="info">
        <p>مسند أحمد: جمعه <strong>الإمام أحمد بن حنبل</strong> ويضم حوالي <strong>40,000 حديث</strong>، منها <strong>10,000 مكررة</strong>، مرتب على أسماء الصحابة وليس الأبواب الفقهية، ويشمل أحاديث صحيحة وضعيفة لكنه مرجع واسع وشامل في الحديث.</p>
    </div>
</div>

 <div class="additional-note">
    <p>ملاحظة: اتفق العلماء على أهمية هذه الكتب، ولكنها ليست بمثابة الكتب الستة في الصحة والموثوقية.</p>
</div>

<footer>
    <h4>آلُِلُِهـم صلُِ وُسلُِم عٍلُِى سيدِنآ محٍمدِ💙</p4>
</footer>

<button class="dark-mode-toggle" id="darkModeToggle">🌙</button>

<script>
    const darkModeToggle = document.getElementById('darkModeToggle');
    const toggleInfoElements = document.querySelectorAll('.toggle-info');
    let isDarkMode = false;

    darkModeToggle.addEventListener('click', () => {
        isDarkMode = !isDarkMode;
        document.body.classList.toggle('dark-mode', isDarkMode);
        darkModeToggle.textContent = isDarkMode ? '☀️' : '🌙';
    });

    toggleInfoElements.forEach((toggle) => {
        toggle.addEventListener('click', () => {
            const info = toggle.parentElement.querySelector('.info');
            info.style.display = info.style.display === 'block' ? 'none' : 'block';
            toggle.classList.toggle('up', info.style.display === 'block');
            toggle.classList.toggle('down', info.style.display === 'none');
        });
    });
</script>

</body>
</html> 
