<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cinema KR.MR - الصفحة الرئيسية</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700;900&display=swap');
        
        body {
            font-family: 'Tajawal', sans-serif;
            background-color: #0a0a0a;
            color: white;
        }
        
        .gradient-text {
            background: linear-gradient(45deg, #e50914, #b81d24);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .btn-red {
            background: linear-gradient(45deg, #e50914, #b81d24);
            transition: all 0.3s ease;
        }
        
        .btn-red:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(229, 9, 20, 0.3);
        }
        
        .genre-card {
            transition: all 0.3s ease;
        }
        
        .genre-card:hover {
            transform: scale(1.05);
        }
        
        .footer-link {
            transition: all 0.2s ease;
        }
        
        .footer-link:hover {
            color: #e50914;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col">
    <!-- Header -->
    <header class="bg-black py-4 px-6 shadow-lg sticky top-0 z-50">
        <div class="container mx-auto flex justify-between items-center">
            <div class="flex items-center space-x-2 space-x-reverse">
                <i class="fas fa-film text-red-600 text-2xl"></i>
                <h1 class="text-3xl font-bold gradient-text">Cinema KR.MR</h1>
            </div>
            <button class="md:hidden text-white focus:outline-none" id="menu-toggle">
                <i class="fas fa-bars text-2xl"></i>
            </button>
            <nav class="hidden md:flex space-x-8 space-x-reverse">
                <a href="#home" class="text-white hover:text-red-500 transition">الرئيسية</a>
                <a href="#movies" class="text-white hover:text-red-500 transition">الأفلام</a>
                <a href="#forum" class="text-white hover:text-red-500 transition">المنتدى</a>
                <a href="#support" class="text-white hover:text-red-500 transition">الدعم</a>
            </nav>
        </div>
    </header>

    <!-- Mobile Menu -->
    <div class="md:hidden hidden bg-black py-4 px-6 shadow-lg" id="mobile-menu">
        <div class="flex flex-col space-y-4">
            <a href="#home" class="text-white hover:text-red-500 transition">الرئيسية</a>
            <a href="#movies" class="text-white hover:text-red-500 transition">الأفلام</a>
            <a href="#forum" class="text-white hover:text-red-500 transition">المنتدى</a>
            <a href="#support" class="text-white hover:text-red-500 transition">الدعم</a>
        </div>
    </div>

    <!-- Hero Section -->
    <section id="home" class="flex-grow flex items-center justify-center bg-cover bg-center" style="background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://images.unsplash.com/photo-1489599849927-2ee91cede3ba?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');">
        <div class="container mx-auto px-6 py-16 text-center">
            <h1 class="text-4xl md:text-6xl font-bold mb-6 gradient-text">Cinema KR.MR</h1>
            <p class="text-xl md:text-2xl mb-12 text-gray-300">وجهتك الأولى لأفضل الأفلام والمسلسلات العربية والعالمية</p>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 max-w-4xl mx-auto">
                <!-- Download Movies Button -->
                <div class="bg-black bg-opacity-70 rounded-lg p-6 border border-gray-800">
                    <i class="fas fa-download text-red-600 text-4xl mb-4"></i>
                    <h3 class="text-xl font-bold mb-3">تحميل الأفلام</h3>
                    <p class="text-gray-300 mb-4">تصفح وتحميل أحدث الأفلام بجودة عالية</p>
                    <a href="#movies" class="btn-red text-white py-2 px-6 rounded-full inline-block font-medium">استكشف</a>
                </div>
                
                <!-- Movie Genres Button -->
                <div class="bg-black bg-opacity-70 rounded-lg p-6 border border-gray-800">
                    <i class="fas fa-film text-red-600 text-4xl mb-4"></i>
                    <h3 class="text-xl font-bold mb-3">أنواع الأفلام</h3>
                    <p class="text-gray-300 mb-4">تصفح الأفلام حسب النوع الذي تفضله</p>
                    <a href="#genres" class="btn-red text-white py-2 px-6 rounded-full inline-block font-medium">استكشف</a>
                </div>
                
                <!-- Forum Button -->
                <div class="bg-black bg-opacity-70 rounded-lg p-6 border border-gray-800">
                    <i class="fas fa-users text-red-600 text-4xl mb-4"></i>
                    <h3 class="text-xl font-bold mb-3">المنتدى</h3>
                    <p class="text-gray-300 mb-4">انضم إلى مجتمعنا وناقش أفلامك المفضلة</p>
                    <a href="#forum" class="btn-red text-white py-2 px-6 rounded-full inline-block font-medium">انضم الآن</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Movies Section -->
    <section id="movies" class="py-16 bg-gray-900">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold mb-12 text-center gradient-text">تحميل الأفلام</h2>
            
            <!-- Search Bar -->
            <div class="max-w-2xl mx-auto mb-12">
                <div class="relative">
                    <input type="text" placeholder="ابحث عن فيلم..." class="w-full bg-gray-800 text-white py-3 px-6 rounded-full focus:outline-none focus:ring-2 focus:ring-red-600">
                    <button class="absolute left-3 top-1/2 transform -translate-y-1/2 text-gray-400">
                        <i class="fas fa-search"></i>
                    </button>
                </div>
            </div>
            
            <!-- Filters -->
            <div class="flex flex-wrap justify-center gap-4 mb-12">
                <button class="bg-red-600 text-white py-2 px-6 rounded-full">الكل</button>
                <button class="bg-gray-800 text-white py-2 px-6 rounded-full hover:bg-gray-700">أكشن</button>
                <button class="bg-gray-800 text-white py-2 px-6 rounded-full hover:bg-gray-700">دراما</button>
                <button class="bg-gray-800 text-white py-2 px-6 rounded-full hover:bg-gray-700">كوميديا</button>
                <button class="bg-gray-800 text-white py-2 px-6 rounded-full hover:bg-gray-700">رعب</button>
                <button class="bg-gray-800 text-white py-2 px-6 rounded-full hover:bg-gray-700">خيال علمي</button>
                <button class="bg-gray-800 text-white py-2 px-6 rounded-full hover:bg-gray-700">رومانسي</button>
            </div>
            
            <!-- Movies Grid -->
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-6">
                <!-- Movie Card 1 -->
                <div class="bg-gray-800 rounded-lg overflow-hidden shadow-lg transition transform hover:-translate-y-2">
                    <img src="https://via.placeholder.com/300x450" alt="Movie Poster" class="w-full h-64 object-cover">
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-1">اسم الفيلم</h3>
                        <div class="flex justify-between items-center text-sm text-gray-400 mb-2">
                            <span>2023</span>
                            <span>8.5/10</span>
                        </div>
                        <div class="flex space-x-2 space-x-reverse">
                            <span class="bg-gray-700 text-xs px-2 py-1 rounded">أكشن</span>
                            <span class="bg-gray-700 text-xs px-2 py-1 rounded">مغامرة</span>
                        </div>
                        <button class="btn-red w-full mt-3 py-2 rounded">تحميل</button>
                    </div>
                </div>
                
                <!-- Movie Card 2 -->
                <div class="bg-gray-800 rounded-lg overflow-hidden shadow-lg transition transform hover:-translate-y-2">
                    <img src="https://via.placeholder.com/300x450" alt="Movie Poster" class="w-full h-64 object-cover">
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-1">اسم الفيلم</h3>
                        <div class="flex justify-between items-center text-sm text-gray-400 mb-2">
                            <span>2023</span>
                            <span>9.0/10</span>
                        </div>
                        <div class="flex space-x-2 space-x-reverse">
                            <span class="bg-gray-700 text-xs px-2 py-1 rounded">دراما</span>
                            <span class="bg-gray-700 text-xs px-2 py-1 rounded">رومانسي</span>
                        </div>
                        <button class="btn-red w-full mt-3 py-2 rounded">تحميل</button>
                    </div>
                </div>
                
                <!-- Movie Card 3 -->
                <div class="bg-gray-800 rounded-lg overflow-hidden shadow-lg transition transform hover:-translate-y-2">
                    <img src="https://via.placeholder.com/300x450" alt="Movie Poster" class="w-full h-64 object-cover">
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-1">اسم الفيلم</h3>
                        <div class="flex justify-between items-center text-sm text-gray-400 mb-2">
                            <span>2023</span>
                            <span>7.8/10</span>
                        </div>
                        <div class="flex space-x-2 space-x-reverse">
                            <span class="bg-gray-700 text-xs px-2 py-1 rounded">كوميديا</span>
                        </div>
                        <button class="btn-red w-full mt-3 py-2 rounded">تحميل</button>
                    </div>
                </div>
                
                <!-- Movie Card 4 -->
                <div class="bg-gray-800 rounded-lg overflow-hidden shadow-lg transition transform hover:-translate-y-2">
                    <img src="https://via.placeholder.com/300x450" alt="Movie Poster" class="w-full h-64 object-cover">
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-1">اسم الفيلم</h3>
                        <div class="flex justify-between items-center text-sm text-gray-400 mb-2">
                            <span>2023</span>
                            <span>8.2/10</span>
                        </div>
                        <div class="flex space-x-2 space-x-reverse">
                            <span class="bg-gray-700 text-xs px-2 py-1 rounded">خيال علمي</span>
                            <span class="bg-gray-700 text-xs px-2 py-1 rounded">أكشن</span>
                        </div>
                        <button class="btn-red w-full mt-3 py-2 rounded">تحميل</button>
                    </div>
                </div>
                
                <!-- Movie Card 5 -->
                <div class="bg-gray-800 rounded-lg overflow-hidden shadow-lg transition transform hover:-translate-y-2">
                    <img src="https://via.placeholder.com/300x450" alt="Movie Poster" class="w-full h-64 object-cover">
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-1">اسم الفيلم</h3>
                        <div class="flex justify-between items-center text-sm text-gray-400 mb-2">
                            <span>2023</span>
                            <span>7.5/10</span>
                        </div>
                        <div class="flex space-x-2 space-x-reverse">
                            <span class="bg-gray-700 text-xs px-2 py-1 rounded">رعب</span>
                            <span class="bg-gray-700 text-xs px-2 py-1 rounded">غموض</span>
                        </div>
                        <button class="btn-red w-full mt-3 py-2 rounded">تحميل</button>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <button class="btn-red text-white py-3 px-8 rounded-full font-medium">عرض المزيد</button>
            </div>
        </div>
    </section>

    <!-- Genres Section -->
    <section id="genres" class="py-16 bg-black">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold mb-12 text-center gradient-text">تصفح حسب النوع</h2>
            
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-6">
                <!-- Action -->
                <div class="genre-card bg-gray-900 rounded-lg overflow-hidden shadow-lg text-center p-8">
                    <i class="fas fa-explosion text-red-600 text-4xl mb-4"></i>
                    <h3 class="font-bold text-xl mb-2">أكشن</h3>
                    <p class="text-gray-400 text-sm">120 فيلم</p>
                </div>
                
                <!-- Drama -->
                <div class="genre-card bg-gray-900 rounded-lg overflow-hidden shadow-lg text-center p-8">
                    <i class="fas fa-theater-masks text-red-600 text-4xl mb-4"></i>
                    <h3 class="font-bold text-xl mb-2">دراما</h3>
                    <p class="text-gray-400 text-sm">95 فيلم</p>
                </div>
                
                <!-- Comedy -->
                <div class="genre-card bg-gray-900 rounded-lg overflow-hidden shadow-lg text-center p-8">
                    <i class="fas fa-laugh-squint text-red-600 text-4xl mb-4"></i>
                    <h3 class="font-bold text-xl mb-2">كوميديا</h3>
                    <p class="text-gray-400 text-sm">75 فيلم</p>
                </div>
                
                <!-- Horror -->
                <div class="genre-card bg-gray-900 rounded-lg overflow-hidden shadow-lg text-center p-8">
                    <i class="fas fa-ghost text-red-600 text-4xl mb-4"></i>
                    <h3 class="font-bold text-xl mb-2">رعب</h3>
                    <p class="text-gray-400 text-sm">60 فيلم</p>
                </div>
                
                <!-- Sci-Fi -->
                <div class="genre-card bg-gray-900 rounded-lg overflow-hidden shadow-lg text-center p-8">
                    <i class="fas fa-rocket text-red-600 text-4xl mb-4"></i>
                    <h3 class="font-bold text-xl mb-2">خيال علمي</h3>
                    <p class="text-gray-400 text-sm">45 فيلم</p>
                </div>
                
                <!-- Romance -->
                <div class="genre-card bg-gray-900 rounded-lg overflow-hidden shadow-lg text-center p-8">
                    <i class="fas fa-heart text-red-600 text-4xl mb-4"></i>
                    <h3 class="font-bold text-xl mb-2">رومانسي</h3>
                    <p class="text-gray-400 text-sm">80 فيلم</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Codes Section -->
    <section class="py-16 bg-gray-900">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold mb-12 text-center gradient-text">أكواد العروض الخاصة</h2>
            
            <div class="max-w-3xl mx-auto bg-gray-800 rounded-lg p-8 shadow-lg">
                <div class="flex flex-col md:flex-row items-center justify-between mb-8">
                    <div>
                        <h3 class="font-bold text-xl mb-2">كود خصم 20%</h3>
                        <p class="text-gray-400">صالح حتى 30 ديسمبر 2023</p>
                    </div>
                    <div class="bg-black text-red-500 font-mono text-xl px-6 py-3 rounded mt-4 md:mt-0">KRMR20</div>
                </div>
                
                <div class="flex flex-col md:flex-row items-center justify-between mb-8">
                    <div>
                        <h3 class="font-bold text-xl mb-2">كود خصم 15%</h3>
                        <p class="text-gray-400">صالح حتى 15 يناير 2024</p>
                    </div>
                    <div class="bg-black text-red-500 font-mono text-xl px-6 py-3 rounded mt-4 md:mt-0">CINEMA15</div>
                </div>
                
                <div class="flex flex-col md:flex-row items-center justify-between">
                    <div>
                        <h3 class="font-bold text-xl mb-2">كود خصم 10%</h3>
                        <p class="text-gray-400">صالح حتى نهاية العام</p>
                    </div>
                    <div class="bg-black text-red-500 font-mono text-xl px-6 py-3 rounded mt-4 md:mt-0">MOVIE10</div>
                </div>
                
                <div class="mt-12 text-center">
                    <button class="btn-red text-white py-3 px-8 rounded-full font-medium">المزيد من الأكواد</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Forum Section -->
    <section id="forum" class="py-16 bg-black">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold mb-12 text-center gradient-text">منتدى السينما</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Forum Card 1 -->
                <div class="bg-gray-900 rounded-lg overflow-hidden shadow-lg">
                    <div class="p-6">
                        <div class="flex items-center mb-4">
                            <div class="bg-red-600 w-12 h-12 rounded-full flex items-center justify-center text-white font-bold">AK</div>
                            <div class="mr-3">
                                <h4 class="font-bold">أحمد خالد</h4>
                                <p class="text-gray-400 text-sm">منذ ساعتين</p>
                            </div>
                        </div>
                        <h3 class="font-bold text-xl mb-3">أفضل أفلام الأكشن لهذا العام</h3>
                        <p class="text-gray-300 mb-4">ما هي أفضل أفلام الأكشن التي شاهدتموها هذا العام؟ أنا شخصياً أعجبت كثيراً بفيلم John Wick 4...</p>
                        <div class="flex justify-between items-center">
                            <div class="flex space-x-2 space-x-reverse">
                                <span class="text-gray-400"><i class="fas fa-comment"></i> 24</span>
                                <span class="text-gray-400"><i class="fas fa-heart"></i> 56</span>
                            </div>
                            <a href="#" class="text-red-500 hover:text-red-400">اقرأ المزيد</a>
                        </div>
                    </div>
                </div>
                
                <!-- Forum Card 2 -->
                <div class="bg-gray-900 rounded-lg overflow-hidden shadow-lg">
                    <div class="p-6">
                        <div class="flex items-center mb-4">
                            <div class="bg-blue-600 w-12 h-12 rounded-full flex items-center justify-center text-white font-bold">SM</div>
                            <div class="mr-3">
                                <h4 class="font-bold">سارة محمد</h4>
                                <p class="text-gray-400 text-sm">منذ يوم</p>
                            </div>
                        </div>
                        <h3 class="font-bold text-xl mb-3">توصيات لأفلام رومانسية</h3>
                        <p class="text-gray-300 mb-4">أبحث عن أفلام رومانسية جيدة، هل من توصيات؟ أفضل تلك التي تحتوي على قصة واقعية...</p>
                        <div class="flex justify-between items-center">
                            <div class="flex space-x-2 space-x-reverse">
                                <span class="text-gray-400"><i class="fas fa-comment"></i> 18</span>
                                <span class="text-gray-400"><i class="fas fa-heart"></i> 32</span>
                            </div>
                            <a href="#" class="text-red-500 hover:text-red-400">اقرأ المزيد</a>
                        </div>
                    </div>
                </div>
                
                <!-- Forum Card 3 -->
                <div class="bg-gray-900 rounded-lg overflow-hidden shadow-lg">
                    <div class="p-6">
                        <div class="flex items-center mb-4">
                            <div class="bg-green-600 w-12 h-12 rounded-full flex items-center justify-center text-white font-bold">YA</div>
                            <div class="mr-3">
                                <h4 class="font-bold">يوسف أحمد</h4>
                                <p class="text-gray-400 text-sm">منذ 3 أيام</p>
                            </div>
                        </div>
                        <h3 class="font-bold text-xl mb-3">أفلام الخيال العلمي المقبلة</h3>
                        <p class="text-gray-300 mb-4">ما هي أفلام الخيال العلمي التي تنتظرونها في العام القادم؟ أنا متحمس جداً لفيلم Dune الجزء الثاني...</p>
                        <div class="flex justify-between items-center">
                            <div class="flex space-x-2 space-x-reverse">
                                <span class="text-gray-400"><i class="fas fa-comment"></i> 42</span>
                                <span class="text-gray-400"><i class="fas fa-heart"></i> 78</span>
                            </div>
                            <a href="#" class="text-red-500 hover:text-red-400">اقرأ المزيد</a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <button class="btn-red text-white py-3 px-8 rounded-full font-medium">عرض المزيد من المناقشات</button>
            </div>
        </div>
    </section>

    <!-- Support Section -->
    <section id="support" class="py-16 bg-gray-900">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold mb-12 text-center gradient-text">الدعم الفني</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-12 max-w-4xl mx-auto">
                <!-- Contact Form -->
                <div class="bg-gray-800 rounded-lg p-8 shadow-lg">
                    <h3 class="font-bold text-xl mb-6">تواصل معنا</h3>
                    <form>
                        <div class="mb-4">
                            <label for="name" class="block text-gray-300 mb-2">الاسم</label>
                            <input type="text" id="name" class="w-full bg-gray-700 text-white py-2 px-4 rounded focus:outline-none focus:ring-2 focus:ring-red-600">
                        </div>
                        <div class="mb-4">
                            <label for="email" class="block text-gray-300 mb-2">البريد الإلكتروني</label>
                            <input type="email" id="email" class="w-full bg-gray-700 text-white py-2 px-4 rounded focus:outline-none focus:ring-2 focus:ring-red-600">
                        </div>
                        <div class="mb-4">
                            <label for="subject" class="block text-gray-300 mb-2">الموضوع</label>
                            <select id="subject" class="w-full bg-gray-700 text-white py-2 px-4 rounded focus:outline-none focus:ring-2 focus:ring-red-600">
                                <option>استفسار عام</option>
                                <option>مشكلة تقنية</option>
                                <option>اقتراح</option>
                                <option>شكوى</option>
                            </select>
                        </div>
                        <div class="mb-4">
                            <label for="message" class="block text-gray-300 mb-2">الرسالة</label>
                            <textarea id="message" rows="4" class="w-full bg-gray-700 text-white py-2 px-4 rounded focus:outline-none focus:ring-2 focus:ring-red-600"></textarea>
                        </div>
                        <button type="submit" class="btn-red w-full py-3 rounded font-medium">إرسال</button>
                    </form>
                </div>
                
                <!-- Contact Info -->
                <div class="bg-gray-800 rounded-lg p-8 shadow-lg">
                    <h3 class="font-bold text-xl mb-6">معلومات التواصل</h3>
                    
                    <div class="flex items-start mb-6">
                        <i class="fas fa-envelope text-red-600 text-xl mt-1 ml-3"></i>
                        <div>
                            <h4 class="font-bold">البريد الإلكتروني</h4>
                            <p class="text-gray-300">support@cinemakrmr.com</p>
                        </div>
                    </div>
                    
                    <div class="flex items-start mb-6">
                        <i class="fas fa-phone-alt text-red-600 text-xl mt-1 ml-3"></i>
                        <div>
                            <h4 class="font-bold">الهاتف</h4>
                            <p class="text-gray-300">+966 12 345 6789</p>
                        </div>
                    </div>
                    
                    <div class="flex items-start mb-6">
                        <i class="fas fa-clock text-red-600 text-xl mt-1 ml-3"></i>
                        <div>
                            <h4 class="font-bold">ساعات العمل</h4>
                            <p class="text-gray-300">من الأحد إلى الخميس</p>
                            <p class="text-gray-300">9 صباحاً - 5 مساءً</p>
                        </div>
                    </div>
                    
                    <div class="flex items-start">
                        <i class="fas fa-question-circle text-red-600 text-xl mt-1 ml-3"></i>
                        <div>
                            <h4 class="font-bold">الأسئلة الشائعة</h4>
                            <a href="#" class="text-red-500 hover:text-red-400 block">كيفية تحميل الأفلام؟</a>
                            <a href="#" class="text-red-500 hover:text-red-400 block">مشاكل في التشغيل</a>
                            <a href="#" class="text-red-500 hover:text-red-400 block">استرداد المال</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Privacy Policy Section -->
    <section class="py-16 bg-black">
        <div class="container mx-auto px-6 max-w-4xl">
            <h2 class="text-3xl font-bold mb-12 text-center gradient-text">سياسة الخصوصية</h2>
            
            <div class="bg-gray-900 rounded-lg p-8 shadow-lg">
                <div class="mb-8">
                    <h3 class="font-bold text-xl mb-4 text-red-500">1. المعلومات التي نجمعها</h3>
                    <p class="text-gray-300">نقوم بجمع المعلومات التي تقدمها لنا عند التسجيل في موقعنا، مثل اسمك وعنوان بريدك الإلكتروني. كما قد نجمع معلومات حول كيفية استخدامك لموقعنا.</p>
                </div>
                
                <div class="mb-8">
                    <h3 class="font-bold text-xl mb-4 text-red-500">2. كيفية استخدام المعلومات</h3>
                    <p class="text-gray-300">نستخدم المعلومات التي نجمعها لتقديم خدماتنا وتحسينها، وللاتصال بك فيما يتعلق بحسابك، ولإرسال التحديثات والعروض الخاصة.</p>
                </div>
                
                <div class="mb-8">
                    <h3 class="font-bold text-xl mb-4 text-red-500">3. مشاركة المعلومات</h3>
                    <p class="text-gray-300">لا نبيع أو نؤجر معلوماتك الشخصية لأطراف ثالثة. قد نشارك معلومات مجمعة وغير شخصية لأغراض إحصائية أو تحليلية.</p>
                </div>
                
                <div class="mb-8">
                    <h3 class="font-bold text-xl mb-4 text-red-500">4. حماية المعلومات</h3>
                    <p class="text-gray-300">نحن نستخدم إجراءات أمنية معقولة لحماية معلوماتك الشخصية من الوصول غير المصرح به أو الكشف أو التغيير أو التدمير.</p>
                </div>
                
                <div>
                    <h3 class="font-bold text-xl mb-4 text-red-500">5. التغييرات على السياسة</h3>
                    <p class="text-gray-300">قد نقوم بتحديث سياسة الخصوصية هذه من وقت لآخر. سننشر أي تغييرات على هذه الصفحة ونخطر المستخدمين إذا كانت التغييرات كبيرة.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black py-12 border-t border-gray-800">
        <div class="container mx-auto px-6">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-12">
                <!-- About -->
                <div>
                    <div class="flex items-center space-x-2 space-x-reverse mb-4">
                        <i class="fas fa-film text-red-600 text-xl"></i>
                        <h3 class="text-xl font-bold gradient-text">Cinema KR.MR</h3>
                    </div>
                    <p class="text-gray-400 mb-4">وجهتك الأولى لأفضل الأفلام والمسلسلات العربية والعالمية بجودة عالية.</p>
                    <div class="flex space-x-4 space-x-reverse">
                        <a href="#" class="text-gray-400 hover:text-red-500"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="text-gray-400 hover:text-red-500"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="text-gray-400 hover:text-red-500"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="text-gray-400 hover:text-red-500"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                
                <!-- Quick Links -->
                <div>
                    <h3 class="text-lg font-bold mb-4">روابط سريعة</h3>
                    <ul class="space-y-2">
                        <li><a href="#home" class="footer-link text-gray-400">الرئيسية</a></li>
                        <li><a href="#movies" class="footer-link text-gray-400">الأفلام</a></li>
                        <li><a href="#genres" class="footer-link text-gray-400">أنواع الأفلام</a></li>
                        <li><a href="#forum" class="footer-link text-gray-400">المنتدى</a></li>
                        <li><a href="#support" class="footer-link text-gray-400">الدعم الفني</a></li>
                    </ul>
                </div>
                
                <!-- Categories -->
                <div>
                    <h3 class="text-lg font-bold mb-4">الأقسام</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="footer-link text-gray-400">أفلام جديدة</a></li>
                        <li><a href="#" class="footer-link text-gray-400">أفلام شائعة</a></li>
                        <li><a href="#" class="footer-link text-gray-400">أفلام تقييم عالي</a></li>
                        <li><a href="#" class="footer-link text-gray-400">مسلسلات</a></li>
                        <li><a href="#" class="footer-link text-gray-400">أفلام عربية</a></li>
                    </ul>
                </div>
                
                <!-- Newsletter -->
                <div>
                    <h3 class="text-lg font-bold mb-4">النشرة البريدية</h3>
                    <p class="text-gray-400 mb-4">اشترك في نشرتنا البريدية لتصلك آخر التحديثات والعروض.</p>
                    <div class="flex">
                        <input type="email" placeholder="بريدك الإلكتروني" class="bg-gray-800 text-white py-2 px-4 rounded-r focus:outline-none w-full">
                        <button class="btn-red text-white py-2 px-4 rounded-l"><i class="fas fa-paper-plane"></i></button>
                    </div>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-500 text-sm mb-4 md:mb-0">© 2023 Cinema KR.MR. جميع الحقوق محفوظة.</p>
                <div class="flex space-x-6 space-x-reverse">
                    <a href="#" class="footer-link text-gray-500 text-sm">شروط الاستخدام</a>
                    <a href="#" class="footer-link text-gray-500 text-sm">سياسة الخصوصية</a>
                    <a href="#" class="footer-link text-gray-500 text-sm">ملفات تعريف الارتباط</a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        document.getElementById('menu-toggle').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    const mobileMenu = document.getElementById('mobile-menu');
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                }
            });
        });
    </script>
</body>
</html>
