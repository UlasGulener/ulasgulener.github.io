<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ulas Gulener | Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-50 text-gray-900 font-sans">

    <header class="p-6 flex justify-between items-center bg-white shadow-sm sticky top-0 z-50">
        <h1 class="text-xl font-bold tracking-tight">UG.PORTFOLIO</h1>
        <div class="space-x-4">
            <button onclick="changeLang('tr')" class="hover:text-blue-600 font-medium">TR</button>
            <span class="text-gray-300">|</span>
            <button onclick="changeLang('en')" class="hover:text-blue-600 font-medium">EN</button>
        </div>
    </header>

    <section class="max-w-4xl mx-auto py-20 px-6 text-center">
        <h2 id="hero-title" class="text-4xl md:text-5xl font-extrabold mb-4 text-gray-800">
            Data Analyst & Excel Automation Specialist
        </h2>
        <p id="hero-sub" class="text-lg text-gray-600 mb-8">
            Error-free data management and professional reporting solutions.
        </p>
        <a href="#contact" class="bg-blue-600 text-white px-8 py-3 rounded-lg font-semibold hover:bg-blue-700 transition">Contact Me</a>
    </section>

    <section class="bg-white py-16 border-y border-gray-100">
        <div class="max-w-4xl mx-auto px-6 grid md:grid-cols-2 gap-8">
            <div class="p-6 border border-gray-100 rounded-xl hover:shadow-md transition">
                <h3 class="text-xl font-bold mb-2">Excel & VBA</h3>
                <p id="skill-1" class="text-gray-600">Complex automation, custom macros, and advanced data modeling.</p>
            </div>
            <div class="p-6 border border-gray-100 rounded-xl hover:shadow-md transition">
                <h3 class="text-xl font-bold mb-2">Quality Analytics</h3>
                <p id="skill-2" class="text-gray-600">Reporting for automotive & manufacturing sectors with 0-PPM precision.</p>
            </div>
        </div>
    </section>

    <footer id="contact" class="py-20 text-center bg-gray-900 text-white">
        <h2 class="text-2xl font-bold mb-6">Let's Connect</h2>
        <div class="flex justify-center space-x-6">
            <a href="https://fiverr.com/ulasgulener" class="hover:text-blue-400">Fiverr</a>
            <a href="https://linkedin.com/in/ulasgulener" class="hover:text-blue-400">LinkedIn</a>
            <a href="mailto:ulasglnrl@gmail.com" class="hover:text-blue-400">E-mail</a>
        </div>
    </footer>

    <script>
        const content = {
            tr: {
                heroTitle: "Veri Analisti ve Excel Otomasyon Uzmanı",
                heroSub: "Hatasız veri yönetimi ve profesyonel raporlama çözümleri.",
                skill1: "Karmaşık otomasyonlar, özel makrolar ve ileri düzey veri modelleme.",
                skill2: "Otomotiv ve imalat sektörü için 'Sıfır Hata' disipliniyle raporlama."
            },
            en: {
                heroTitle: "Data Analyst & Excel Automation Specialist",
                heroSub: "Error-free data management and professional reporting solutions.",
                skill1: "Complex automation, custom macros, and advanced data modeling.",
                skill2: "Reporting for automotive & manufacturing sectors with 0-PPM precision."
            }
        };

        function changeLang(lang) {
            document.getElementById('hero-title').innerText = content[lang].heroTitle;
            document.getElementById('hero-sub').innerText = content[lang].heroSub;
            document.getElementById('skill-1').innerText = content[lang].skill1;
            document.getElementById('skill-2').innerText = content[lang].skill2;
        }
    </script>
</body>
</html>
