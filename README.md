# kimi17-bot.github.io
<!DOCTYPE html>
<html lang="ko">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GRP Korea Inc. | 선도적인 해양 솔루션</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet"
        href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Noto+Sans+KR:wght@400;500;700&display=swap">
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        body {
            font-family: 'Noto Sans KR', 'Inter', sans-serif;
        }

        .section-title {
            font-size: 2.25rem;
            /* 36px */
            font-weight: 700;
            margin-bottom: 1rem;
            text-align: center;
        }

        .section-subtitle {
            font-size: 1.125rem;
            /* 18px */
            color: #6b7280;
            text-align: center;
            max-width: 800px;
            margin: 0 auto 3rem auto;
        }

        .timeline-item::before {
            content: '';
            position: absolute;
            left: -31px;
            top: 5px;
            width: 20px;
            height: 20px;
            border-radius: 50%;
            background-color: #3b82f6;
            border: 4px solid #f3f4f6;
        }

        .fade-in {
            animation: fadeIn 1s ease-in-out;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>

<body class="bg-gray-50 text-gray-800">

    <!-- Header -->
    <header id="header" class="bg-white shadow-md sticky top-0 z-50 transition-all duration-300">
        <div class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold text-blue-600">GRP KOREA</a>
            <nav class="hidden md:flex space-x-8 items-center">
                <a href="#about" class="text-gray-600 hover:text-blue-600 transition">회사소개</a>
                <a href="#gallery" class="text-gray-600 hover:text-blue-600 transition">갤러리</a>
                <a href="#history" class="text-gray-600 hover:text-blue-600 transition">연혁</a>
                <a href="#technology" class="text-gray-600 hover:text-blue-600 transition">핵심기술</a>
                <a href="#research-development" class="text-gray-600 hover:text-blue-600 transition">연구개발</a>
                <a href="#products" class="text-gray-600 hover:text-blue-600 transition">제품소개</a>
                <a href="#performance" class="text-gray-600 hover:text-blue-600 transition">납품실적</a>
                <a href="#contact"
                    class="bg-blue-600 text-white px-4 py-2 rounded-md hover:bg-blue-700 transition">문의하기</a>
            </nav>
            <button id="mobile-menu-button" class="md:hidden">
                <i data-lucide="menu"></i>
            </button>
        </div>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden px-6 pb-4">
            <a href="#about" class="block py-2 text-gray-600 hover:text-blue-600">회사소개</a>
            <a href="#gallery" class="block py-2 text-gray-600 hover:text-blue-600">갤러리</a>
            <a href="#history" class="block py-2 text-gray-600 hover:text-blue-600">연혁</a>
            <a href="#technology" class="block py-2 text-gray-600 hover:text-blue-600">핵심기술</a>
            <a href="#research-development" class="block py-2 text-gray-600 hover:text-blue-600">연구개발</a>
            <a href="#products" class="block py-2 text-gray-600 hover:text-blue-600">제품소개</a>
            <a href="#performance" class="block py-2 text-gray-600 hover:text-blue-600">납품실적</a>
            <a href="#contact"
                class="block mt-2 bg-blue-600 text-white text-center px-4 py-2 rounded-md hover:bg-blue-700">문의하기</a>
        </div>
    </header>

    <!-- Hero Section with Video Background -->
    <section id="hero" class="relative h-screen flex items-center justify-center text-center text-white overflow-hidden">
        <!-- Video Background -->
        <video id="hero-video" autoplay loop muted playsinline class="absolute top-0 left-0 w-full h-full object-cover z-0">
            <!-- The video source is now pointing to the GitHub URL -->
            <source src="https://github.com/kimi17-bot/GRPKorea/blob/main/grpkorea_hero.mp4?raw=true" type="video/mp4">
            Your browser does not support the video tag.
        </video>
        <!-- Overlay to ensure text readability -->
        <div class="absolute top-0 left-0 w-full h-full bg-black bg-opacity-60 z-10"></div>
        
        <!-- Content -->
        <div class="relative z-20 container mx-auto px-6">
            <h1 class="text-4xl md:text-6xl font-bold mb-4 leading-tight fade-in">최고의 기술력으로 해양의 미래를 선도합니다</h1>
            <p class="text-lg md:text-xl max-w-3xl mx-auto mb-8 fade-in" style="animation-delay: 0.2s;">GRP Korea는 1992년부터 축적된
                기술과 노하우를 바탕으로 고속단정(R.I.B.), 복합소재 패널 등 최고의 해양 관련 제품을 생산합니다.</p>
            <a href="#products"
                class="bg-white text-blue-600 font-bold py-3 px-8 rounded-full hover:bg-gray-200 transition duration-300 ease-in-out transform hover:scale-105 fade-in"
                style="animation-delay: 0.4s;">제품 살펴보기</a>
        </div>
        
        <!-- Sound Toggle Button -->
        <button id="sound-toggle-button" class="absolute bottom-8 right-8 z-20 bg-white/20 backdrop-blur-sm p-3 rounded-full text-white hover:bg-white/30 transition">
            <i id="sound-off-icon" data-lucide="volume-x"></i>
            <i id="sound-on-icon" data-lucide="volume-2" class="hidden"></i>
        </button>
    </section>

    <main>
        <!-- About Us Section -->
        <section id="about" class="py-20 bg-white">
            <div class="container mx-auto px-6">
                <h2 class="section-title">회사소개</h2>
                <p class="section-subtitle">대한민국 최고의 기술과 소재로 품질과 서비스의 우수성을 자랑하며, 카누 국산화를 시작으로 해양 관련 제품 생산에 앞장서고 있습니다.
                </p>
                <div class="grid md:grid-cols-2 gap-12 items-center">
                    <div>
                        <img src="https://github.com/kimi17-bot/GRPKorea/blob/main/factory.jpg?raw=true" alt="GRP Korea 공장 이미지" class="rounded-lg shadow-xl">
                    </div>
                    <div class="space-y-6">
                        <div class="bg-gray-100 p-6 rounded-lg">
                            <h3 class="text-xl font-bold mb-2 text-blue-600">GRP Korea Inc.</h3>
                            <p class="text-gray-600">1992년 설립 이래, 저희는 카누 국산화라는 목표를 가지고 시작하여 현재는 고속단정, 복합소재 패널 등 다양한 해양
                                관련 제품을 생산하는 전문 기업으로 성장했습니다. 최고의 기술력과 품질로 고객 만족을 실현하겠습니다.</p>
                        </div>
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 text-sm">
                            <div class="bg-gray-100 p-4 rounded-lg flex items-start space-x-3">
                                <i data-lucide="building-2" class="text-blue-500 mt-1"></i>
                                <div><strong class="font-semibold">회사명:</strong> (주)지알피코리아</div>
                            </div>
                            <div class="bg-gray-100 p-4 rounded-lg flex items-start space-x-3">
                                <i data-lucide="user" class="text-blue-500 mt-1"></i>
                                <div><strong class="font-semibold">대표이사:</strong> 황규상</div>
                            </div>
                            <div class="bg-gray-100 p-4 rounded-lg flex items-start space-x-3">
                                <i data-lucide="calendar" class="text-blue-500 mt-1"></i>
                                <div><strong class="font-semibold">설립일:</strong> 1992년 3월 1일</div>
                            </div>
                            <div class="bg-gray-100 p-4 rounded-lg flex items-start space-x-3">
                                <i data-lucide="package" class="text-blue-500 mt-1"></i>
                                <div><strong class="font-semibold">주요제품:</strong> R.I.B., 폼펜더, FRP 패널, 부표 등</div>
                            </div>
                        </div>
                        <div class="bg-gray-100 p-4 rounded-lg flex items-start space-x-3">
                            <i data-lucide="map-pin" class="text-blue-500 mt-1 flex-shrink-0"></i>
                            <div><strong class="font-semibold">본사:</strong> 충청남도 천안시 동남구 풍세면 미죽로 152</div>
                        </div>
                        <div class="bg-gray-100 p-4 rounded-lg flex items-start space-x-3">
                            <i data-lucide="map-pin" class="text-blue-500 mt-1 flex-shrink-0"></i>
                            <div><strong class="font-semibold">제2공장:</strong> 경상북도 포항시 남구 동해면 석리 105</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Gallery Section -->
        <section id="gallery" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title">갤러리</h2>
                <p class="section-subtitle">GRP Korea의 활동 및 제품 사진들입니다.</p>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Gallery Image Box -->
                    <div class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://placehold.co/400x300/e2e8f0/334155?text=Image+Placeholder" alt="Gallery Image 1" class="w-full h-64 object-cover">
                    </div>
                    <!-- Gallery Image Box -->
                    <div class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://placehold.co/400x300/e2e8f0/334155?text=Image+Placeholder" alt="Gallery Image 2" class="w-full h-64 object-cover">
                    </div>
                    <!-- Gallery Image Box -->
                    <div class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://placehold.co/400x300/e2e8f0/334155?text=Image+Placeholder" alt="Gallery Image 3" class="w-full h-64 object-cover">
                    </div>
                     <!-- Gallery Image Box -->
                    <div class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://placehold.co/400x300/e2e8f0/334155?text=Image+Placeholder" alt="Gallery Image 4" class="w-full h-64 object-cover">
                    </div>
                    <!-- Gallery Image Box -->
                    <div class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://placehold.co/400x300/e2e8f0/334155?text=Image+Placeholder" alt="Gallery Image 5" class="w-full h-64 object-cover">
                    </div>
                    <!-- Gallery Image Box -->
                    <div class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://placehold.co/400x300/e2e8f0/334155?text=Image+Placeholder" alt="Gallery Image 6" class="w-full h-64 object-cover">
                    </div>
                </div>
            </div>
        </section>

        <!-- History Section -->
        <section id="history" class="py-20 bg-white">
            <div class="container mx-auto px-6">
                <h2 class="section-title">회사 연혁</h2>
                <p class="section-subtitle">혁신과 도전으로 걸어온 GRP Korea의 발자취입니다.</p>
                <div class="relative max-w-2xl mx-auto border-l-2 border-gray-200 pl-8">
                    <div class="timeline-item mb-12">
                        <h3 class="text-lg font-semibold text-blue-600">1992</h3>
                        <p class="text-gray-600">그린스포츠 설립</p>
                    </div>
                    <div class="timeline-item mb-12">
                        <h3 class="text-lg font-semibold text-blue-600">1996</h3>
                        <p class="text-gray-600">선수용 카누 국산화 성공</p>
                    </div>
                    <div class="timeline-item mb-12">
                        <h3 class="text-lg font-semibold text-blue-600">2005</h3>
                        <p class="text-gray-600">국내 최초 10m급 R.I.B. 진공성형 공법 개발 성공</p>
                    </div>
                    <div class="timeline-item mb-12">
                        <h3 class="text-lg font-semibold text-blue-600">2006</h3>
                        <p class="text-gray-600">GRP Korea로 상호 변경</p>
                        <p class="mt-1 text-gray-600">국내 최초 폼 충전식 펜더 제작</p>
                    </div>
                    <div class="timeline-item mb-12">
                        <h3 class="text-lg font-semibold text-blue-600">2011</h3>
                        <p class="text-gray-600">충격 흡수형 경량 부표 개발 및 해양경찰청 R.I.B 납품</p>
                    </div>
                     <div class="timeline-item mb-12">
                        <h3 class="text-lg font-semibold text-blue-600">2013</h3>
                        <p class="text-gray-600">해양경찰청 R.I.B 납품</p>
                    </div>
                     <div class="timeline-item mb-12">
                        <h3 class="text-lg font-semibold text-blue-600">2014</h3>
                        <p class="text-gray-600">해양경찰청 R.I.B 납품</p>
                    </div>
                     <div class="timeline-item mb-12">
                        <h3 class="text-lg font-semibold text-blue-600">2015</h3>
                        <p class="text-gray-600">대한민국 해병대 R.I.B 납품</p>
                    </div>
                    <div class="timeline-item mb-12">
                        <h3 class="text-lg font-semibold text-blue-600">2016</h3>
                        <p class="text-gray-600">포항 제2공장 가동</p>
                        <p class="mt-1 text-gray-600">서해어업관리단 및 해양경찰청 R.I.B 납품</p>
                    </div>
                    <div class="timeline-item mb-12">
                        <h3 class="text-lg font-semibold text-blue-600">2020</h3>
                        <p class="text-gray-600">인도네시아 SAMUDERA 조선소와 협력</p>
                        <p class="mt-1 text-gray-600">대만 CSBC 조선소와 협력 계약 체결</p>
                    </div>
                    <div class="timeline-item">
                        <h3 class="text-lg font-semibold text-blue-600">2024</h3>
                        <p class="text-gray-600">대만 JONGSHYN 조선소와 첫 계약</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Technology Section -->
        <section id="technology" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title">핵심 기술</h2>
                <p class="section-subtitle">GRP Korea의 경쟁력은 독보적인 기술력에서 나옵니다.</p>
                <div class="grid md:grid-cols-2 gap-10">
                    <div class="bg-gray-50 p-8 rounded-lg shadow-md">
                        <div class="flex items-center mb-4">
                            <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                <i data-lucide="wind"></i>
                            </div>
                            <h3 class="text-2xl font-bold">진공 성형 공법 (Vacuum Infusion)</h3>
                        </div>
                        <p class="mb-4 text-gray-600">최상의 강도와 경량화를 동시에 실현하는 첨단 공법입니다.</p>
                        <ul class="space-y-2 text-gray-700">
                            <li class="flex items-center">
                                <i data-lucide="check-circle" class="text-green-500 mr-2"></i>높은 섬유-수지 비율 (최대 70%)로 강도 및
                                강성 향상</li>
                            <li class="flex items-center">
                                <i data-lucide="check-circle" class="text-green-500 mr-2"></i>기포 최소화로 일관된 품질 유지</li>
                            <li class="flex items-center">
                                <i data-lucide="check-circle" class="text-green-500 mr-2"></i>VOC 발생이 없는 친환경 공정</li>
                            <li class="flex items-center">
                                <i data-lucide="check-circle" class="text-green-500 mr-2"></i>복잡한 형상 및 코어 작업에 효율적</li>
                        </ul>
                    </div>
                    <div class="bg-gray-50 p-8 rounded-lg shadow-md">
                        <div class="flex items-center mb-4">
                            <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                <i data-lucide="shield"></i>
                            </div>
                            <h3 class="text-2xl font-bold">폼 충전식 펜더 (Foam Filled Fender)</h3>
                        </div>
                        <p class="mb-4 text-gray-600">내구성과 충격 흡수력이 뛰어난 차세대 펜더 기술입니다.</p>
                        <ul class="space-y-2 text-gray-700">
                            <li class="flex items-center">
                                <i data-lucide="check-circle" class="text-green-500 mr-2"></i>높은 에너지 흡수율 (공기식 펜더 대비 최대
                                40% 우수)</li>
                            <li class="flex items-center">
                                <i data-lucide="check-circle" class="text-green-500 mr-2"></i>펑크 시에도 가라앉지 않는 안전성</li>
                            <li class="flex items-center">
                                <i data-lucide="check-circle" class="text-green-500 mr-2"></i>유지보수가 거의 필요 없는 편리성</li>
                            <li class="flex items-center">
                                <i data-lucide="check-circle" class="text-green-500 mr-2"></i>내구성, 탄성, 내해수성, 내UV성이 뛰어난
                                폴리우레아 코팅</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- Research and Development Section -->
        <section id="research-development" class="py-20 bg-white">
            <div class="container mx-auto px-6">
                <h2 class="section-title">연구개발 (Research & Development)</h2>
                <p class="section-subtitle">미래 해양 기술을 선도하는 GRP Korea의 혁신적인 연구개발 프로젝트를 소개합니다.</p>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                    <!-- R&D Card 1: Text -->
                    <div class="bg-gray-50 p-8 rounded-lg shadow-md md:col-span-1">
                         <div class="flex items-center mb-4">
                            <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                <i data-lucide="atom"></i>
                            </div>
                            <h3 class="text-2xl font-bold">수소추진시스템</h3>
                        </div>
                        <p class="text-gray-600">
                            친환경 선박 기술의 핵심인 수소연료전지 기반 추진 시스템을 개발하고 있습니다. 
                            탄소 배출 없는 미래 해양 시대를 열어가기 위한 GRP Korea의 끊임없는 도전입니다.
                        </p>
                    </div>
                    <!-- R&D Card 2: Image -->
                    <div class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://github.com/kimi17-bot/GRPKorea/blob/main/stress%20calxulator.png?raw=true" alt="Pressure Vessel Design Tool" class="w-full h-64 object-contain p-4 bg-gray-100">
                         <div class="p-4 bg-white">
                            <h3 class="text-lg font-semibold text-center">압력 용기 설계 툴</h3>
                        </div>
                    </div>
                    <!-- R&D Card 3: Image -->
                    <div class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://github.com/kimi17-bot/GRPKorea/blob/main/pressure_cauculator.png?raw=true" alt="Hydrogen Storage Vessel Calculator" class="w-full h-64 object-contain p-4 bg-gray-100">
                        <div class="p-4 bg-white">
                            <h3 class="text-lg font-semibold text-center">수소 저장 용기 계산기</h3>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Products Section -->
        <section id="products" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title">제품 소개</h2>
                <p class="section-subtitle">다양한 임무와 환경에 최적화된 GRP Korea의 제품 라인업을 만나보세요.</p>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Product Card with adjusted image fit -->
                    <div
                        class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://github.com/kimi17-bot/GRPKorea/blob/main/670.png?raw=true" alt="GRP RHIB-650" class="w-full h-56 object-contain bg-gray-100">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">GRP RHIB-650</h3>
                            <p class="text-gray-600 mb-4">컴팩트한 사이즈와 뛰어난 기동성을 자랑하는 모델입니다.</p>
                            <ul class="text-sm text-gray-700 space-y-1">
                                <li><strong>전장:</strong> 6.5m</li>
                                <li><strong>최대속도:</strong> 40 Knots</li>
                            </ul>
                        </div>
                    </div>
                    <!-- Product Card with adjusted image fit -->
                    <div
                        class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://github.com/kimi17-bot/GRPKorea/blob/main/700.png?raw=true" alt="GRP RHIB-850" class="w-full h-56 object-contain bg-gray-100">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">GRP RHIB-850</h3>
                            <p class="text-gray-600 mb-4">다목적 임무 수행에 최적화된 베스트셀러 모델입니다.</p>
                            <ul class="text-sm text-gray-700 space-y-1">
                                <li><strong>전장:</strong> 9.2m</li>
                                <li><strong>최대속도:</strong> 47 Knots</li>
                            </ul>
                        </div>
                    </div>
                    <!-- Product Card with adjusted image fit -->
                    <div
                        class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://github.com/kimi17-bot/GRPKorea/blob/main/1100.png?raw=true" alt="GRP RHIB-1100" class="w-full h-56 object-contain bg-gray-100">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">GRP RHIB-1100</h3>
                            <p class="text-gray-600 mb-4">안정적인 운항 성능과 넓은 공간을 제공합니다.</p>
                            <ul class="text-sm text-gray-700 space-y-1">
                                <li><strong>전장:</strong> 11m</li>
                                <li><strong>최대속도:</strong> 40 Knots</li>
                            </ul>
                        </div>
                    </div>
                    <!-- Product Card with adjusted image fit -->
                    <div
                        class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://github.com/kimi17-bot/GRPKorea/blob/main/900.png?raw=true" alt="GRP RHIB-1400" class="w-full h-56 object-contain bg-gray-100">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">GRP RHIB-1400</h3>
                            <p class="text-gray-600 mb-4">장거리 및 특수 임무를 위한 플래그십 모델입니다.</p>
                            <ul class="text-sm text-gray-700 space-y-1">
                                <li><strong>전장:</strong> 14m</li>
                                <li><strong>최대속도:</strong> 40 Knots</li>
                            </ul>
                        </div>
                    </div>
                    <div
                        class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://placehold.co/400x300/94a3b8/ffffff?text=Foam+Fender" alt="Foam Fender" class="w-full h-56 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">폼 펜더</h3>
                            <p class="text-gray-600 mb-4">선박과 구조물을 보호하는 고성능 폼 충전식 펜더입니다.</p>
                        </div>
                    </div>
                    <div
                        class="bg-white rounded-lg shadow-lg overflow-hidden transform hover:-translate-y-2 transition duration-300">
                        <img src="https://placehold.co/400x300/94a3b8/ffffff?text=FRP+Panel" alt="FRP Panel" class="w-full h-56 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">FRP 복합 패널</h3>
                            <p class="text-gray-600 mb-4">경량이면서도 강도가 높은 다용도 복합소재 패널입니다.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Delivery Performance Section -->
        <section id="performance" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title">주요 납품 실적</h2>
                <p class="section-subtitle">정부 기관 및 국내외 유수 기업들이 GRP Korea의 기술력을 신뢰합니다.</p>
                <div class="max-w-5xl mx-auto overflow-x-auto">
                   <div class="shadow-lg rounded-lg overflow-hidden">
                        <table class="min-w-full leading-normal">
                            <thead>
                                <tr>
                                    <th class="px-5 py-3 border-b-2 border-gray-200 bg-gray-100 text-left text-xs font-semibold text-gray-700 uppercase tracking-wider">
                                        Year
                                    </th>
                                    <th class="px-5 py-3 border-b-2 border-gray-200 bg-gray-100 text-left text-xs font-semibold text-gray-700 uppercase tracking-wider">
                                        Order
                                    </th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2013. 11</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">Foam filled fender (27set)</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2013. 12</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">8 vessels of R.I.B for Korea Coast Guard</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2014. 01</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">14m R.I.B for Korea Coast Guard</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2014. 03</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">2 vessels of 8.5m R.I.B and 3 vessels of 6.5m R.I.B</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2014. 04</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">6 vessels of R.I.B for Korea Coast Guard</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2014. 04</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">Development of hull mold for Korea Coast Guard</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2014. 12</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">Water quality inspection boat</td>
                                </tr>
                                 <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2015. 03</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">13 vessels of 8.5m R.I.B for Korea Marine Corps.</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2015. 05</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">6 vessels of 10m R.I.B for Korea Coast Guard</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2016. 10</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">3 vessels of 8.5m RIB for West Sea Fisheries Management Service</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2016. 12</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">7 vessels of 10m R.I.B for Korea Coast Guard</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2016. 12</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">Fishery inspection R.I.B for Gunsansi</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2017. 11</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">3 vessels of R.I.B for West Sea Fisheries Management Service</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2017. 12</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">1 vessels of R.I.B for Korea Coast Guard(SSAT)</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2018. 01</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">6 vessels of 10m R.I.B for Korea Coast Guard</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2018. 08</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">1 vessels of R.I.B for Korea Navy</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2018. 11</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">8 vessels of R.I.B for East Sea Fisheries Management Service</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2019. 01</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">3 vessels of R.I.B for Korea Coast Guard</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2019. 11</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">5 vessels of R.I.B for Korea Navy</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2020. 03</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">Fishery inspection R.I.B for Muangun</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2020. 04</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">3 vessels of R.I.B for Korea Navy</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2020. 04</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">3 vessels of R.I.B for Republic of Korea Armed Forces</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2020. 09</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">RIGID BOUYANCY BOAT(OIL COMBAT) for SAMUDERA SHIPYARD(INDONESIA) 32 vessels built locally</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2020. 11</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">12 vessels of Patrol boat for CSBC COPORATION, TAIWAN</td>
                                </tr>
                                <tr class="bg-white hover:bg-gray-50">
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm font-medium text-gray-800">2023. 12</td>
                                    <td class="px-5 py-4 border-b border-gray-200 text-sm text-gray-700">1 vessels of working boat for CSBC COPORATION, TAIWAN</td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="py-20 bg-gray-800 text-white">
            <div class="container mx-auto px-6">
                <h2 class="section-title text-white">문의하기</h2>
                <p class="section-subtitle text-gray-300">프로젝트 문의, 기술 상담 등 무엇이든 편하게 연락주십시오.</p>
                <div class="grid md:grid-cols-2 gap-12">
                    <div class="bg-gray-700 p-8 rounded-lg">
                        <h3 class="text-2xl font-bold mb-6">메시지 보내기</h3>
                        <form action="#" method="POST">
                            <div class="mb-4">
                                <label for="name" class="block mb-2">이름</label>
                                <input type="text" id="name" name="name" class="w-full bg-gray-800 border border-gray-600 rounded-md py-2 px-3 focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                            </div>
                            <div class="mb-4">
                                <label for="email" class="block mb-2">이메일</label>
                                <input type="email" id="email" name="email" class="w-full bg-gray-800 border border-gray-600 rounded-md py-2 px-3 focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                            </div>
                            <div class="mb-4">
                                <label for="message" class="block mb-2">문의 내용</label>
                                <textarea id="message" name="message" rows="5" class="w-full bg-gray-800 border border-gray-600 rounded-md py-2 px-3 focus:outline-none focus:ring-2 focus:ring-blue-500" required></textarea>
                            </div>
                            <button type="submit" class="w-full bg-blue-600 text-white font-bold py-3 px-6 rounded-md hover:bg-blue-700 transition duration-300">전송</button>
                        </form>
                    </div>
                    <div class="space-y-6">
                        <div class="bg-gray-700 p-6 rounded-lg flex items-start space-x-4">
                            <i data-lucide="map-pin" class="text-blue-400 mt-1 flex-shrink-0"></i>
                            <div>
                                <h4 class="font-bold text-lg">본사 주소</h4>
                                <p class="text-gray-300">충청남도 천안시 동남구 풍세면 미죽로 152</p>
                            </div>
                        </div>
                        <div class="bg-gray-700 p-6 rounded-lg flex items-start space-x-4">
                            <i data-lucide="phone" class="text-blue-400 mt-1 flex-shrink-0"></i>
                            <div>
                                <h4 class="font-bold text-lg">연락처</h4>
                                <p class="text-gray-300">Tel: +82-41-577-7878</p>
                                <p class="text-gray-300">Fax: +82-41-573-7878</p>
                            </div>
                        </div>
                        <div class="bg-gray-700 p-6 rounded-lg flex items-start space-x-4">
                            <i data-lucide="mail" class="text-blue-400 mt-1 flex-shrink-0"></i>
                            <div>
                                <h4 class="font-bold text-lg">이메일</h4>
                                <p class="text-gray-300">grpkorea153@naver.com</p>
                            </div>
                        </div>
                        <div class="mt-6 h-64 rounded-lg overflow-hidden">
                            <iframe
                                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3200.756314841968!2d127.1030993152857!3d36.6570189799778!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x357b2f4477ffffff%3A0x6a36a7134375a610!2zKOyjvCnsoJXslpHtlZzrtoDri7g!5e0!3m2!1sko!2skr!4v1658800000000!5m2!1sko!2skr"
                                width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"
                                referrerpolicy="no-referrer-when-downgrade"></iframe>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white">
        <div class="container mx-auto px-6 py-8 text-center">
            <a href="#" class="text-2xl font-bold text-white mb-4 inline-block">GRP KOREA</a>
            <div class="flex justify-center space-x-6 mb-4">
                <a href="#about" class="text-gray-400 hover:text-white transition">회사소개</a>
                <a href="#technology" class="text-gray-400 hover:text-white transition">핵심기술</a>
                <a href="#products" class="text-gray-400 hover:text-white transition">제품소개</a>
                <a href="#contact" class="text-gray-400 hover:text-white transition">문의하기</a>
            </div>
            <p class="text-gray-500">&copy; 2024 GRP Korea Inc. All Rights Reserved.</p>
        </div>
    </footer>

    <script>
        lucide.createIcons();

        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);

                if(targetElement) {
                    targetElement.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
                
                // Close mobile menu on link click
                if (!mobileMenu.classList.contains('hidden')) {
                    mobileMenu.classList.add('hidden');
                }
            });
        });
        
        // Add fade-in animation to sections on scroll
        const faders = document.querySelectorAll('.fade-in');
        const sections = document.querySelectorAll('section');

        const appearOptions = {
            threshold: 0.2,
            rootMargin: "0px 0px -100px 0px"
        };

        const appearOnScroll = new IntersectionObserver(function(entries, appearOnScroll) {
            entries.forEach(entry => {
                if (!entry.isIntersecting) {
                    return;
                } else {
                    entry.target.classList.add('fade-in');
                    appearOnScroll.unobserve(entry.target);
                }
            });
        }, appearOptions);
        
        sections.forEach(section => {
            appearOnScroll.observe(section);
        });

        // Hero Video Sound Toggle
        const heroVideo = document.getElementById('hero-video');
        const soundButton = document.getElementById('sound-toggle-button');
        const soundOnIcon = document.getElementById('sound-on-icon');
        const soundOffIcon = document.getElementById('sound-off-icon');

        soundButton.addEventListener('click', () => {
            const isMuted = heroVideo.muted;
            heroVideo.muted = !isMuted;
            soundOffIcon.classList.toggle('hidden', !isMuted);
            soundOnIcon.classList.toggle('hidden', isMuted);
        });

    </script>
</body>

</html>

