<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>کلینیک زیبایی Clinic 7 - لوکس و مینیمال</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&family=Montserrat:wght@300;400;500;600;700&family=Vazirmatn:wght@300;400;500;600;700&family=Shabnam:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --luxury-black: #000000;
            --luxury-gold: #FFD700;
            --pure-white: #FFFFFF;
            --dark-gray: #1C1C1C;
        }
        
        * {
            font-family: 'Vazirmatn', 'Shabnam', 'Tahoma', sans-serif;
            direction: rtl;
            text-align: right;
        }
        
        body {
            direction: rtl;
            text-align: right;
        }
        
        .luxury-title {
            font-family: 'Vazirmatn', 'Shabnam', serif;
            font-weight: 700;
        }
        
        .luxury-accent {
            font-family: 'Vazirmatn', 'Shabnam', sans-serif;
            font-weight: 500;
        }
        
        .persian-text {
            font-family: 'Vazirmatn', 'Shabnam', 'Tahoma', sans-serif;
            direction: rtl;
            text-align: right;
            line-height: 1.8;
        }
        
        .english-text {
            font-family: 'Montserrat', sans-serif;
            direction: ltr;
            text-align: center;
        }
        
        .gold-gradient {
            background: linear-gradient(135deg, #FFD700, #FFA500, #FFD700);
        }
        
        .gold-text {
            color: #FFD700;
        }
        
        .gold-shadow {
            box-shadow: 0 8px 32px rgba(255, 215, 0, 0.3);
        }
        
        .luxury-card {
            background: rgba(28, 28, 28, 0.8);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 215, 0, 0.1);
        }
        
        .hover-gold:hover {
            background: linear-gradient(135deg, #FFA500, #FFD700);
            transform: translateY(-4px);
            box-shadow: 0 12px 40px rgba(255, 215, 0, 0.4);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .luxury-border {
            border: 1px solid #1C1C1C;
        }
        
        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.5s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .accordion-content.active {
            max-height: 300px;
        }
        
        .calendar-grid {
            display: grid;
            grid-template-columns: repeat(7, 1fr);
            gap: 12px;
        }
        
        .calendar-day {
            aspect-ratio: 1;
            display: flex;
            align-items: center;
            justify-content: center;
            background: #1C1C1C;
            border: 1px solid rgba(255, 215, 0, 0.2);
            cursor: pointer;
            transition: all 0.3s ease;
            color: #FFFFFF;
            font-weight: 500;
        }
        
        .calendar-day:hover {
            background: rgba(255, 215, 0, 0.1);
            border-color: #FFD700;
            transform: scale(1.05);
        }
        
        .calendar-day.selected {
            background: linear-gradient(135deg, #FFD700, #FFA500);
            color: #000000;
            font-weight: 700;
            box-shadow: 0 4px 20px rgba(255, 215, 0, 0.5);
        }
        
        .luxury-input {
            background: #1C1C1C;
            border: 1px solid rgba(255, 215, 0, 0.3);
            color: #FFFFFF;
            transition: all 0.3s ease;
        }
        
        .luxury-input:focus {
            border-color: #FFD700;
            box-shadow: 0 0 20px rgba(255, 215, 0, 0.2);
            outline: none;
        }
        
        .luxury-input::placeholder {
            color: rgba(255, 255, 255, 0.5);
        }
        
        .section-divider {
            height: 1px;
            background: linear-gradient(90deg, transparent, #1C1C1C, transparent);
            margin: 4rem 0;
        }
    </style>
</head>
<body style="background-color: #000000; color: #FFFFFF;" class="min-h-screen">
    <!-- Header -->
    <header class="relative overflow-hidden py-20">
        <div class="absolute inset-0 bg-gradient-to-br from-transparent via-gray-900/10 to-transparent"></div>
        <div class="relative container mx-auto px-6 text-center">
            <h1 class="luxury-title english-text text-7xl font-bold mb-6" style="color: #FFD700;">Clinic 7</h1>
            <div class="w-24 h-1 gold-gradient mx-auto mb-6"></div>
            <p class="luxury-accent persian-text text-2xl mb-8 text-center" style="color: #FFFFFF;">زیبایی بی‌نهایت، تجربه‌ای لوکس</p>
            
            <!-- Additional Persian Content -->
            <div style="
              direction: rtl;
              text-align: right;
              font-family: Tahoma, sans-serif;
              line-height: 1.8;
              max-width: 600px;
              margin: 2rem auto;
              padding: 2rem;
              background: rgba(28, 28, 28, 0.6);
              border-radius: 16px;
              border: 1px solid rgba(255, 215, 0, 0.2);
            ">
              <h2 style="writing-mode: horizontal-tb; white-space: nowrap; color: gold; text-align: center; margin-bottom: 1rem; font-size: 2rem;">
                کلینیک زیبایی سون
              </h2>
              <p style="writing-mode: horizontal-tb; white-space: normal; font-size: 16px; color: #ffffff; text-align: center;">
                ارائه‌دهنده خدمات زیبایی، تزریقات و جوانسازی با بهترین کیفیت و جدیدترین متدهای روز.
              </p>
            </div>
            <div class="flex justify-center space-x-8 space-x-reverse">
                <span class="text-5xl" style="color: #FFD700;">✨</span>
                <span class="text-5xl" style="color: #FFD700;">💉</span>
                <span class="text-5xl" style="color: #FFD700;">👨‍⚕️</span>
            </div>
        </div>
    </header>

    <div class="section-divider"></div>

    <!-- About Us -->
    <section class="py-20">
        <div class="container mx-auto px-6">
            <h2 class="luxury-title persian-text text-5xl font-bold text-center mb-4" style="color: #FFD700;">درباره کلینیک</h2>
            <div class="w-16 h-1 gold-gradient mx-auto mb-12"></div>
            <div class="max-w-4xl mx-auto text-center">
                <p class="persian-text text-xl leading-relaxed" style="color: #FFFFFF;">
                    در کلینیک زیبایی Clinic 7، ما تجربه‌ای لوکس و بی‌نظیر از خدمات زیبایی ارائه می‌دهیم. 
                    با بهره‌گیری از پیشرفته‌ترین تکنولوژی‌ها و متخصصان برتر، زیبایی شما را به سطحی جدید می‌رسانیم.
                </p>
            </div>
        </div>
    </section>

    <div class="section-divider"></div>

    <!-- Services -->
    <section class="py-20">
        <div class="container mx-auto px-6">
            <h2 class="luxury-title persian-text text-5xl font-bold text-center mb-4" style="color: #FFD700;">خدمات لوکس</h2>
            <div class="w-16 h-1 gold-gradient mx-auto mb-16"></div>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="luxury-card p-8 rounded-2xl hover:scale-105 transition-all duration-500">
                    <div class="text-5xl mb-6 text-center" style="color: #FFD700;">💉</div>
                    <h3 class="luxury-accent persian-text text-2xl font-semibold mb-4 text-center" style="color: #FFD700;">بوتاکس پریمیوم</h3>
                    <p class="persian-text text-center" style="color: #FFFFFF;">جوانسازی طبیعی با بالاترین کیفیت</p>
                </div>
                
                <div class="luxury-card p-8 rounded-2xl hover:scale-105 transition-all duration-500">
                    <div class="text-5xl mb-6 text-center" style="color: #FFD700;">💋</div>
                    <h3 class="luxury-accent persian-text text-2xl font-semibold mb-4 text-center" style="color: #FFD700;">فیلر لوکس</h3>
                    <p class="persian-text text-center" style="color: #FFFFFF;">حجم‌دهی هنرمندانه لب و صورت</p>
                </div>
                
                <div class="luxury-card p-8 rounded-2xl hover:scale-105 transition-all duration-500">
                    <div class="text-5xl mb-6 text-center" style="color: #FFD700;">✨</div>
                    <h3 class="luxury-accent persian-text text-2xl font-semibold mb-4 text-center" style="color: #FFD700;">تزریق چربی</h3>
                    <p class="persian-text text-center" style="color: #FFFFFF;">جوانسازی طبیعی با تکنولوژی پیشرفته</p>
                </div>
                
                <div class="luxury-card p-8 rounded-2xl hover:scale-105 transition-all duration-500">
                    <div class="text-5xl mb-6 text-center" style="color: #FFD700;">🛏️</div>
                    <h3 class="luxury-accent persian-text text-2xl font-semibold mb-4 text-center" style="color: #FFD700;">مزوتراپی VIP</h3>
                    <p class="persian-text text-center" style="color: #FFFFFF;">تقویت و درخشندگی پوست</p>
                </div>
                
                <div class="luxury-card p-8 rounded-2xl hover:scale-105 transition-all duration-500">
                    <div class="text-5xl mb-6 text-center" style="color: #FFD700;">🔥</div>
                    <h3 class="luxury-accent persian-text text-2xl font-semibold mb-4 text-center" style="color: #FFD700;">لیزر پیشرفته</h3>
                    <p class="persian-text text-center" style="color: #FFFFFF;">حذف موهای زائد با دستگاه‌های لوکس</p>
                </div>
                
                <div class="luxury-card p-8 rounded-2xl hover:scale-105 transition-all duration-500">
                    <div class="text-5xl mb-6 text-center" style="color: #FFD700;">👨‍⚕️</div>
                    <h3 class="luxury-accent persian-text text-2xl font-semibold mb-4 text-center" style="color: #FFD700;">مشاوره تخصصی</h3>
                    <p class="persian-text text-center" style="color: #FFFFFF;">مشاوره رایگان با متخصصان برتر</p>
                </div>
            </div>
        </div>
    </section>

    <div class="section-divider"></div>

    <!-- Accordion Section -->
    <section class="py-20">
        <div class="container mx-auto px-6">
            <div class="max-w-4xl mx-auto">
                <div class="luxury-card rounded-2xl overflow-hidden">
                    <button class="accordion-btn w-full p-8 text-right flex justify-between items-center hover:bg-gray-900/50 transition-all duration-300" onclick="toggleAccordion()">
                        <span class="luxury-accent persian-text text-2xl font-semibold flex items-center" style="color: #FFD700;">
                            <span class="ml-4 text-4xl">💉</span>
                            خدمات ویژه کلینیک
                        </span>
                        <span class="accordion-icon text-3xl transition-transform duration-500" style="color: #FFD700;">⊕</span>
                    </button>
                    <div class="accordion-content" style="background-color: #1C1C1C;">
                        <div class="p-8 space-y-6">
                            <div class="flex items-center" style="color: #FFFFFF;">
                                <span class="ml-4 text-2xl" style="color: #FFD700;">•</span>
                                <span class="persian-text text-lg">بوتاکس پریمیوم – رفع چین و چروک با دوام بالا</span>
                            </div>
                            <div class="flex items-center" style="color: #FFFFFF;">
                                <span class="ml-4 text-2xl" style="color: #FFD700;">•</span>
                                <span class="persian-text text-lg">فیلر لوکس – طراحی هنرمندانه چهره</span>
                            </div>
                            <div class="flex items-center" style="color: #FFFFFF;">
                                <span class="ml-4 text-2xl" style="color: #FFD700;">•</span>
                                <span class="persian-text text-lg">تزریق چربی – جوانسازی کاملاً طبیعی</span>
                            </div>
                            <div class="flex items-center" style="color: #FFFFFF;">
                                <span class="ml-4 text-2xl" style="color: #FFD700;">•</span>
                                <span class="persian-text text-lg">مزوتراپی VIP – تقویت عمقی پوست و مو</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <div class="section-divider"></div>

<!-- Appointment Booking -->
<section class="py-20">
  <div class="container mx-auto px-6">
    <h2 class="luxury-title persian-text text-4xl md:text-5xl font-bold text-center mb-4 text-[#FFD700]">
      رزرو نوبت VIP
    </h2>
    <div class="w-16 h-1 gold-gradient mx-auto mb-4"></div>
    <p class="persian-text text-center text-lg md:text-xl mb-16 text-white">
      تجربه‌ای لوکس در انتظار شماست
    </p>

    <div class="max-w-3xl mx-auto">
      <div id="booking-form" class="space-y-12">

        <!-- Step 1: Service Selection -->
        <div id="step1" class="booking-step">
          <h3 class="luxury-accent persian-text text-2xl font-semibold mb-8 text-center text-[#FFD700]">
            ۱. انتخاب خدمت لوکس
          </h3>
          <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
            <button class="service-btn luxury-card flex flex-row items-center gap-3 p-6 rounded-xl hover-gold transition-all duration-500 w-full justify-center" data-service="بوتاکس پریمیوم">
              <span class="text-3xl text-[#FFD700]">💉</span>
              <span class="luxury-accent persian-text font-medium text-white">بوتاکس پریمیوم</span>
            </button>
            <button class="service-btn luxury-card flex flex-row items-center gap-3 p-6 rounded-xl hover-gold transition-all duration-500 w-full justify-center" data-service="فیلر لوکس">
              <span class="text-3xl text-[#FFD700]">💋</span>
              <span class="luxury-accent persian-text font-medium text-white">فیلر لوکس</span>
            </button>
            <button class="service-btn luxury-card flex flex-row items-center gap-3 p-6 rounded-xl hover-gold transition-all duration-500 w-full justify-center" data-service="لیزر پیشرفته">
              <span class="text-3xl text-[#FFD700]">🔥</span>
              <span class="luxury-accent persian-text font-medium text-white">لیزر پیشرفته</span>
            </button>
            <button class="service-btn luxury-card flex flex-row items-center gap-3 p-6 rounded-xl hover-gold transition-all duration-500 w-full justify-center" data-service="مشاوره تخصصی">
              <span class="text-3xl text-[#FFD700]">👩⚕️</span>
              <span class="luxury-accent persian-text font-medium text-white">مشاوره تخصصی</span>
            </button>
          </div>
        </div>

        <!-- Step 2: Doctor Selection -->
        <div id="step2" class="booking-step hidden">
          <h3 class="luxury-accent persian-text text-2xl font-semibold mb-8 text-center text-[#FFD700]">
            ۲. انتخاب متخصص
          </h3>
          <div class="grid grid-cols-1 gap-6">
            <button class="doctor-btn luxury-card flex flex-row items-center gap-3 p-6 rounded-xl hover-gold transition-all duration-500 w-full justify-center" data-doctor="دکتر احمدی">
              <span class="text-3xl text-[#FFD700]">👨⚕️</span>
              <span class="luxury-accent persian-text font-medium text-white">دکتر احمدی - پوست و زیبایی</span>
            </button>
            <button class="doctor-btn luxury-card flex flex-row items-center gap-3 p-6 rounded-xl hover-gold transition-all duration-500 w-full justify-center" data-doctor="دکتر محمدی">
              <span class="text-3xl text-[#FFD700]">👩⚕️</span>
              <span class="luxury-accent persian-text font-medium text-white">دکتر محمدی - جراحی زیبایی</span>
            </button>
          </div>
        </div>

        <!-- Step 3: Date & Time Selection -->
        <div id="step3" class="booking-step hidden">
          <h3 class="luxury-accent persian-text text-2xl font-semibold mb-8 text-center text-[#FFD700]">
            ۳. انتخاب تاریخ و زمان
          </h3>
          <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
            <div>
              <h4 class="luxury-accent persian-text text-xl mb-6 text-[#FFD700]">تاریخ مراجعه</h4>
              <div class="calendar-grid text-sm font-medium grid grid-cols-7 gap-2">
                <div class="calendar-day font-bold text-[#FFD700]">ش</div>
                <div class="calendar-day font-bold text-[#FFD700]">ی</div>
                <div class="calendar-day font-bold text-[#FFD700]">د</div>
                <div class="calendar-day font-bold text-[#FFD700]">س</div>
                <div class="calendar-day font-bold text-[#FFD700]">چ</div>
                <div class="calendar-day font-bold text-[#FFD700]">پ</div>
                <div class="calendar-day font-bold text-[#FFD700]">ج</div>
                <div class="calendar-day opacity-30">28</div>
                <div class="calendar-day opacity-30">29</div>
                <div class="calendar-day opacity-30">30</div>
                <div class="calendar-day" onclick="selectDate(this)">1</div>
                <div class="calendar-day" onclick="selectDate(this)">2</div>
                <div class="calendar-day" onclick="selectDate(this)">3</div>
                <div class="calendar-day" onclick="selectDate(this)">4</div>
                <div class="calendar-day" onclick="selectDate(this)">5</div>
                <div class="calendar-day" onclick="selectDate(this)">6</div>
              </div>
            </div>
            <div>
              <h4 class="luxury-accent persian-text text-xl mb-6 text-[#FFD700]">ساعت مراجعه</h4>
              <div class="grid grid-cols-2 gap-3">
                <button class="time-btn luxury-card p-4 rounded-lg hover-gold transition-all duration-300 luxury-accent font-medium w-full" onclick="selectTime(this)">09:00</button>
                <button class="time-btn luxury-card p-4 rounded-lg hover-gold transition-all duration-300 luxury-accent font-medium w-full" onclick="selectTime(this)">10:30</button>
                <button class="time-btn luxury-card p-4 rounded-lg hover-gold transition-all duration-300 luxury-accent font-medium w-full" onclick="selectTime(this)">14:00</button>
                <button class="time-btn luxury-card p-4 rounded-lg hover-gold transition-all duration-300 luxury-accent font-medium w-full" onclick="selectTime(this)">15:30</button>
              </div>
            </div>
          </div>
        </div>

        <!-- Step 4: Personal Information -->
        <div id="step4" class="booking-step hidden">
          <h3 class="luxury-accent persian-text text-2xl font-semibold mb-8 text-center text-[#FFD700]">
            ۴. اطلاعات شخصی
          </h3>
          <div class="space-y-6">
            <input type="text" id="fullName" placeholder="نام و نام خانوادگی" class="w-full p-5 luxury-input persian-text rounded-xl text-lg">
            <input type="tel" id="phone" placeholder="شماره تماس" class="w-full p-5 luxury-input persian-text rounded-xl text-lg">
            <input type="email" id="email" placeholder="ایمیل (اختیاری)" class="w-full p-5 luxury-input persian-text rounded-xl text-lg">
          </div>
        </div>

        <!-- Navigation Buttons -->
        <div class="flex flex-col sm:flex-row justify-between gap-4 pt-8">
          <button id="prevBtn" class="px-8 py-4 luxury-card rounded-xl hover:bg-gray-800 transition-all luxury-accent persian-text font-medium hidden" onclick="previousStep()">قبلی</button>
          <button id="nextBtn" class="px-8 py-4 gold-gradient rounded-xl hover-gold luxury-accent persian-text font-bold text-black gold-shadow" onclick="nextStep()">بعدی</button>
          <button id="submitBtn" class="px-8 py-4 gold-gradient rounded-xl hover-gold luxury-accent persian-text font-bold text-black gold-shadow hidden" onclick="submitBooking()">رزرو نوبت</button>
        </div>

      </div>

      <!-- Success Message -->
      <div id="success-message" class="hidden text-center p-12 luxury-card rounded-2xl">
        <div class="text-6xl mb-6 text-[#FFD700]">✅</div>
        <h3 class="luxury-title persian-text text-3xl font-bold mb-4 text-[#FFD700]">نوبت شما با موفقیت ثبت شد</h3>
        <p class="persian-text text-xl text-white">تیم ما به زودی جهت هماهنگی با شما تماس خواهد گرفت.</p>
      </div>
    </div>
  </div>
</section>

<!-- Booking Script -->
<script>
  let currentStep = 1;
  let bookingData = {};

  function showStep(step) {
    document.querySelectorAll(".booking-step").forEach((el, index) => {
      el.classList.add("hidden");
      if (index === step - 1) el.classList.remove("hidden");
    });
    document.getElementById("prevBtn").classList.toggle("hidden", step === 1);
    document.getElementById("nextBtn").classList.toggle("hidden", step === 4);
    document.getElementById("submitBtn").classList.toggle("hidden", step !== 4);
  }

  function nextStep() {
    if (currentStep < 4) {
      currentStep++;
      showStep(currentStep);
    }
  }

  function previousStep() {
    if (currentStep > 1) {
      currentStep--;
      showStep(currentStep);
    }
  }

  // انتخاب سرویس
  document.querySelectorAll(".service-btn").forEach(btn => {
    btn.addEventListener("click", () => {
      bookingData.service = btn.dataset.service;
      nextStep();
    });
  });

  // انتخاب دکتر
  document.querySelectorAll(".doctor-btn").forEach(btn => {
    btn.addEventListener("click", () => {
      bookingData.doctor = btn.dataset.doctor;
      nextStep();
    });
  });

  // انتخاب تاریخ
  function selectDate(el) {
    document.querySelectorAll(".calendar-day").forEach(day => day.classList.remove("selected"));
    el.classList.add("selected");
    bookingData.date = el.innerText;
  }

  // انتخاب ساعت
  function selectTime(el) {
    document.querySelectorAll(".time-btn").forEach(time => time.classList.remove("selected"));
    el.classList.add("selected");
    bookingData.time = el.innerText;
  }

  // ثبت اطلاعات
  function submitBooking() {
    bookingData.fullName = document.getElementById("fullName").value;
    bookingData.phone = document.getElementById("phone").value;
    bookingData.email = document.getElementById("email").value;

    if (!bookingData.fullName || !bookingData.phone) {
      alert("لطفا نام و شماره تماس را وارد کنید");
      return;
    }

    document.getElementById("booking-form").classList.add("hidden");
    document.getElementById("success-message").classList.remove("hidden");

    console.log("اطلاعات رزرو:", bookingData);
  }

  window.selectDate = selectDate;
  window.selectTime = selectTime;
  window.previousStep = previousStep;
  window.nextStep = nextStep;
  window.submitBooking = submitBooking;

  showStep(currentStep);
</script>
