<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EzAssign - Elite UK Academic Support & Mentorship Platform</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            navy: '#0f172a',
                            blue: '#1e40af',
                            lightBlue: '#2563eb',
                            green: '#059669',
                            gold: '#d97706',
                            bg: '#f8fafc'
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        body { font-family: 'Inter', sans-serif; }
        .bg-grid-pattern {
            background-image: radial-gradient(rgba(37, 99, 235, 0.08) 1px, transparent 1px);
            background-size: 24px 24px;
        }
        .custom-scrollbar::-webkit-scrollbar {
            width: 6px;
        }
        .custom-scrollbar::-webkit-scrollbar-track {
            background: #f1f5f9;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background: #cbd5e1;
            border-radius: 4px;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 antialiased selection:bg-blue-600 selection:text-white">

    <!-- Top Announcement Bar -->
    <div class="bg-gradient-to-r from-brand-navy via-slate-900 to-brand-navy text-white text-xs sm:text-sm py-2 px-4 border-b border-slate-800">
        <div class="max-w-7xl mx-mx auto flex justify-between items-center px-2 sm:px-6">
            <div class="flex items-center space-x-2">
                <span class="bg-emerald-500 text-white text-[10px] font-extrabold uppercase px-2 py-0.5 rounded-full tracking-wider animate-pulse">Limited Offer</span>
                <span class="hidden sm:inline">Get <strong class="text-amber-400">30% OFF</strong> + 5% Cashback on your first order!</span>
                <span class="sm:hidden text-xs">Save <strong class="text-amber-400">30% OFF</strong> today!</span>
            </div>
            <div class="flex items-center space-x-4 text-xs">
                <a href="tel:+919256466594" class="hover:text-amber-400 transition flex items-center gap-1 font-medium">
                    <i data-lucide="phone" class="w-3.5 h-3.5 text-amber-400"></i> +91-9256466594
                </a>
                <span class="text-slate-600">|</span>
                <a href="https://wa.me/919256466594?text=Hi%20EzAssign%20team,%20I%20need%20help%20with%20my%20assignment" target="_blank" class="hover:text-emerald-400 transition flex items-center gap-1 font-medium text-emerald-400">
                    <i data-lucide="message-square" class="w-3.5 h-3.5"></i> WhatsApp Direct
                </a>
            </div>
        </div>
    </div>

    <!-- Sticky Navigation Header -->
    <header class="sticky top-0 z-50 bg-white/95 backdrop-blur-md border-b border-slate-200/80 shadow-sm transition-all duration-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <!-- Brand Logo -->
                <a href="#" class="flex items-center space-x-3 group">
                    <div class="w-11 h-11 bg-gradient-to-tr from-blue-700 to-indigo-600 rounded-xl flex items-center justify-center text-white font-black text-2xl shadow-lg shadow-blue-500/20 group-hover:scale-105 transition-transform">
                        Ez
                    </div>
                    <div>
                        <span class="text-2xl font-black tracking-tight text-slate-900 group-hover:text-blue-600 transition">EzAssign<span class="text-blue-600">.uk</span></span>
                        <p class="text-[10px] text-slate-500 tracking-wider uppercase font-semibold">Academic Excellence Partner</p>
                    </div>
                </a>

                <!-- Desktop Nav Links -->
                <nav class="hidden md:flex items-center space-x-8 text-sm font-semibold text-slate-600">
                    <a href="#calculator" class="hover:text-blue-600 transition">Order Form</a>
                    <a href="#how-it-works" class="hover:text-blue-600 transition">How It Works</a>
                    <a href="#why-us" class="hover:text-blue-600 transition">Why Us</a>
                    <a href="#subjects" class="hover:text-blue-600 transition">100+ Domains</a>
                    <a href="#freebies" class="hover:text-blue-600 transition">Free Services</a>
                    <a href="#faqs" class="hover:text-blue-600 transition">FAQs</a>
                </nav>

                <!-- Header Actions -->
                <div class="hidden sm:flex items-center space-x-3">
                    <a href="tel:+919256466594" class="px-4 py-2.5 rounded-xl text-xs font-bold text-slate-700 hover:bg-slate-100 border border-slate-300 transition flex items-center gap-1.5">
                        <i data-lucide="headphone-off" class="w-4 h-4 text-blue-600"></i> Support
                    </a>
                    <a href="#calculator" class="px-5 py-2.5 rounded-xl text-xs font-bold text-white bg-gradient-to-r from-blue-600 to-indigo-600 hover:from-blue-700 hover:to-indigo-700 shadow-md shadow-blue-500/20 transition flex items-center gap-1.5">
                        <i data-lucide="file-edit" class="w-4 h-4"></i> Get Quote Now
                    </a>
                </div>

                <!-- Mobile menu button -->
                <button id="mobileMenuBtn" class="md:hidden p-2 rounded-lg text-slate-600 hover:text-slate-900 hover:bg-slate-100">
                    <i data-lucide="menu" class="w-6 h-6"></i>
                </button>
            </div>
        </div>

        <!-- Mobile Drawer Menu -->
        <div id="mobileDrawer" class="hidden md:hidden border-b border-slate-200 bg-white px-4 pt-2 pb-6 space-y-3">
            <a href="#calculator" class="mobile-link block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50">Order Form</a>
            <a href="#how-it-works" class="mobile-link block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50">How It Works</a>
            <a href="#why-us" class="mobile-link block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50">Why Choose Us</a>
            <a href="#subjects" class="mobile-link block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50">100+ Subjects</a>
            <a href="#freebies" class="mobile-link block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50">Freebies</a>
            <a href="#faqs" class="mobile-link block px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:bg-slate-50">FAQs</a>
            <div class="pt-4 border-t border-slate-100 flex flex-col gap-2">
                <a href="tel:+919256466594" class="w-full text-center px-4 py-3 rounded-xl text-sm font-bold text-slate-700 bg-slate-100">Call Support: +91-9256466594</a>
                <a href="#calculator" class="w-full text-center px-4 py-3 rounded-xl text-sm font-bold text-white bg-blue-600">Get Instant Order Quote</a>
            </div>
        </div>
    </header>

    <!-- Hero Section with Live Interactive Calculator -->
    <section class="relative bg-slate-900 text-white pt-10 pb-16 lg:pt-16 lg:pb-24 overflow-hidden bg-grid-pattern">
        <!-- Ambient background glows -->
        <div class="absolute top-1/4 -left-20 w-96 h-96 bg-blue-600/20 rounded-full filter blur-3xl pointer-events-none"></div>
        <div class="absolute bottom-10 right-0 w-96 h-96 bg-emerald-500/10 rounded-full filter blur-3xl pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <!-- Hero Left Column: Pitch & Trust Badges -->
                <div class="lg:col-span-7 space-y-6">
                    <div class="inline-flex items-center gap-2 px-3 py-1.5 rounded-full bg-blue-950/80 border border-blue-500/30 text-blue-300 text-xs font-semibold backdrop-blur-sm">
                        <i data-lucide="shield-check" class="w-4 h-4 text-emerald-400"></i>
                        <span>Verified UK & Global Academic Mentorship</span>
                    </div>

                    <h1 class="text-3xl sm:text-4xl lg:text-5xl font-black tracking-tight leading-tight text-white">
                        Crushing under deadline pressure? <span class="bg-gradient-to-r from-blue-400 via-indigo-300 to-emerald-400 bg-clip-text text-transparent">Get expert Assignment Help now!</span>
                    </h1>

                    <p class="text-base sm:text-lg text-slate-300 font-normal leading-relaxed">
                        At <strong class="text-white font-bold">EzAssign</strong>, we connect you with top-tier subject-matter experts who help you handle academic stress. If you're stuck under never-ending academic challenges, simply say <em class="text-amber-300 italic font-semibold">"do my assignment"</em>. You get complete, error-free, plagiarism-free solutions that elevate your performance.
                    </p>

                    <!-- Core Guarantee Pill Grid -->
                    <div class="grid grid-cols-2 sm:grid-cols-4 gap-3 pt-2">
                        <div class="bg-slate-800/80 border border-slate-700/60 p-3 rounded-xl flex items-center gap-2.5 backdrop-blur-sm">
                            <i data-lucide="award" class="w-5 h-5 text-amber-400 shrink-0"></i>
                            <div>
                                <p class="text-xs font-bold text-white">Guaranteed</p>
                                <p class="text-[10px] text-slate-400">Grade or Refund</p>
                            </div>
                        </div>
                        <div class="bg-slate-800/80 border border-slate-700/60 p-3 rounded-xl flex items-center gap-2.5 backdrop-blur-sm">
                            <i data-lucide="bot-off" class="w-5 h-5 text-emerald-400 shrink-0"></i>
                            <div>
                                <p class="text-xs font-bold text-white">0% AI Content</p>
                                <p class="text-[10px] text-slate-400">100% Human Writers</p>
                            </div>
                        </div>
                        <div class="bg-slate-800/80 border border-slate-700/60 p-3 rounded-xl flex items-center gap-2.5 backdrop-blur-sm">
                            <i data-lucide="clock" class="w-5 h-5 text-blue-400 shrink-0"></i>
                            <div>
                                <p class="text-xs font-bold text-white">24/7 Live Support</p>
                                <p class="text-[10px] text-slate-400">Instant Queries</p>
                            </div>
                        </div>
                        <div class="bg-slate-800/80 border border-slate-700/60 p-3 rounded-xl flex items-center gap-2.5 backdrop-blur-sm">
                            <i data-lucide="users" class="w-5 h-5 text-purple-400 shrink-0"></i>
                            <div>
                                <p class="text-xs font-bold text-white">1.5M+ Happy</p>
                                <p class="text-[10px] text-slate-400">Students Served</p>
                            </div>
                        </div>
                    </div>

                    <!-- Social Proof Avatar Bar -->
                    <div class="flex items-center gap-4 pt-2 border-t border-slate-800">
                        <div class="flex -space-x-2 overflow-hidden">
                            <img class="inline-block h-9 w-9 rounded-full ring-2 ring-slate-900" src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=100&q=80" alt="Student">
                            <img class="inline-block h-9 w-9 rounded-full ring-2 ring-slate-900" src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?auto=format&fit=crop&w=100&q=80" alt="Student">
                            <img class="inline-block h-9 w-9 rounded-full ring-2 ring-slate-900" src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?auto=format&fit=crop&w=100&q=80" alt="Student">
                            <img class="inline-block h-9 w-9 rounded-full ring-2 ring-slate-900" src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?auto=format&fit=crop&w=100&q=80" alt="Student">
                        </div>
                        <div>
                            <div class="flex items-center gap-1 text-amber-400">
                                <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
                                <span class="text-white text-xs font-bold ml-1">4.9/5</span>
                            </div>
                            <p class="text-xs text-slate-400">Trusted by UK, US & Global Scholars</p>
                        </div>
                    </div>
                </div>

                <!-- Hero Right Column: Interactive Order Form -->
                <div id="calculator" class="lg:col-span-5">
                    <div class="bg-white rounded-2xl shadow-2xl p-5 sm:p-7 border border-slate-200 text-slate-900 relative">
                        
                        <!-- Discount Badge Header -->
                        <div class="absolute -top-3.5 left-1/2 transform -translate-x-1/2 bg-gradient-to-r from-amber-500 to-orange-500 text-white font-extrabold text-xs px-4 py-1 rounded-full shadow-md tracking-wider uppercase flex items-center gap-1">
                            <i data-lucide="sparkles" class="w-3.5 h-3.5"></i> 30% OFF FIRST ORDER
                        </div>

                        <h2 class="text-xl font-bold text-slate-900 mb-1 text-center mt-1">Get Instant Assignment Quote</h2>
                        <p class="text-xs text-slate-500 text-center mb-5">Zero hidden fees • Plagiarism-free report included</p>

                        <form id="assignmentForm" class="space-y-4">
                            <!-- Service Type Selector Tabs -->
                            <div>
                                <label class="block text-xs font-bold text-slate-700 uppercase tracking-wider mb-1.5">1. Select Service Type</label>
                                <div class="grid grid-cols-3 gap-2 p-1 bg-slate-100 rounded-xl" id="serviceTabs">
                                    <button type="button" data-service="Writing" class="service-btn active py-2 text-xs font-bold rounded-lg transition bg-blue-600 text-white shadow-sm flex items-center justify-center gap-1">
                                        <i data-lucide="pen-tool" class="w-3.5 h-3.5"></i> Writing
                                    </button>
                                    <button type="button" data-service="Technical" class="service-btn py-2 text-xs font-bold rounded-lg transition text-slate-600 hover:text-slate-900 flex items-center justify-center gap-1">
                                        <i data-lucide="code" class="w-3.5 h-3.5"></i> Technical
                                    </button>
                                    <button type="button" data-service="Online Class" class="service-btn py-2 text-xs font-bold rounded-lg transition text-slate-600 hover:text-slate-900 flex items-center justify-center gap-1">
                                        <i data-lucide="laptop" class="w-3.5 h-3.5"></i> Online Class
                                    </button>
                                </div>
                            </div>

                            <!-- Email & Course Code -->
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                                <div>
                                    <label class="block text-xs font-semibold text-slate-700 mb-1">Email Address*</label>
                                    <input type="email" id="userEmail" required placeholder="student@university.ac.uk" class="w-full px-3 py-2 text-xs border border-slate-300 rounded-lg focus:ring-2 focus:ring-blue-600 focus:border-blue-600 outline-none transition">
                                </div>
                                <div>
                                    <label class="block text-xs font-semibold text-slate-700 mb-1">Subject / Course Code*</label>
                                    <input type="text" id="courseCode" required placeholder="e.g. CS101 / LAW602" class="w-full px-3 py-2 text-xs border border-slate-300 rounded-lg focus:ring-2 focus:ring-blue-600 focus:border-blue-600 outline-none transition">
                                </div>
                            </div>

                            <!-- Deadline & Page/Word Count Row -->
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                                <div>
                                    <label class="block text-xs font-semibold text-slate-700 mb-1">Target Delivery Time</label>
                                    <select id="deadlineTime" class="w-full px-3 py-2 text-xs border border-slate-300 rounded-lg focus:ring-2 focus:ring-blue-600 focus:border-blue-600 outline-none transition bg-white">
                                        <option value="6">Urgent (6 Hours)</option>
                                        <option value="12">12 Hours</option>
                                        <option value="24" selected>24 Hours (Standard)</option>
                                        <option value="48">2 Days</option>
                                        <option value="72">3 Days</option>
                                        <option value="120">5+ Days</option>
                                    </select>
                                </div>

                                <div>
                                    <label class="block text-xs font-semibold text-slate-700 mb-1">Length / Word Count</label>
                                    <div class="flex items-center border border-slate-300 rounded-lg overflow-hidden">
                                        <button type="button" id="btnPageMinus" class="px-3 py-2 bg-slate-100 hover:bg-slate-200 text-slate-700 font-bold text-xs">-</button>
                                        <div id="pageDisplay" class="flex-1 text-center text-xs font-bold text-slate-800">
                                            1 Page / 250 Words
                                        </div>
                                        <button type="button" id="btnPagePlus" class="px-3 py-2 bg-slate-100 hover:bg-slate-200 text-slate-700 font-bold text-xs">+</button>
                                    </div>
                                </div>
                            </div>

                            <!-- Phone with International Country Pickers -->
                            <div>
                                <label class="block text-xs font-semibold text-slate-700 mb-1">Phone Number (For Instant WhatsApp Update)</label>
                                <div class="flex gap-2">
                                    <select id="countryCode" class="w-2/5 px-2 py-2 text-xs border border-slate-300 rounded-lg focus:ring-2 focus:ring-blue-600 focus:border-blue-600 outline-none bg-white">
                                        <option value="+44">UK (+44)</option>
                                        <option value="+91" selected>IN (+91)</option>
                                        <option value="+1">US/CA (+1)</option>
                                        <option value="+61">AU (+61)</option>
                                        <option value="+971">UAE (+971)</option>
                                        <option value="+353">IE (+353)</option>
                                        <option value="+65">SG (+65)</option>
                                        <option value="+49">DE (+49)</option>
                                        <option value="+33">FR (+33)</option>
                                    </select>
                                    <input type="tel" id="phoneNumber" placeholder="9256466594" class="w-3/5 px-3 py-2 text-xs border border-slate-300 rounded-lg focus:ring-2 focus:ring-blue-600 focus:border-blue-600 outline-none transition">
                                </div>
                            </div>

                            <!-- Attachment & Brief -->
                            <div>
                                <label class="block text-xs font-semibold text-slate-700 mb-1">Description / Brief Instructions</label>
                                <textarea id="briefNotes" rows="2" placeholder="Paste guidelines, grading rubric requirements or specific professor instructions..." class="w-full px-3 py-2 text-xs border border-slate-300 rounded-lg focus:ring-2 focus:ring-blue-600 focus:border-blue-600 outline-none transition resize-none"></textarea>
                            </div>

                            <!-- Mock File Upload UI -->
                            <div class="border-2 border-dashed border-slate-200 hover:border-blue-400 rounded-xl p-2.5 text-center transition cursor-pointer bg-slate-50" id="uploadArea">
                                <i data-lucide="upload-cloud" class="w-5 h-5 mx-auto text-blue-500 mb-1"></i>
                                <p class="text-[11px] text-slate-600 font-medium">Attach Prompt / Rubrics (PDF, DOCX, ZIP)</p>
                                <span class="text-[9px] text-slate-400">Max size 25MB • 100% Encrypted</span>
                                <input type="file" id="fileInput" class="hidden">
                            </div>

                            <!-- Terms Checkbox -->
                            <div class="flex items-start gap-2 pt-1">
                                <input type="checkbox" id="termsCheck" checked class="mt-0.5 rounded text-blue-600 focus:ring-blue-500 h-3.5 w-3.5">
                                <label for="termsCheck" class="text-[11px] text-slate-500 leading-tight">
                                    I accept the <a href="#" class="text-blue-600 underline">Terms & Conditions</a>, and agree to receive updates & special discounts.
                                </label>
                            </div>

                            <!-- Price Summary & Submit CTA -->
                            <div class="pt-2 border-t border-slate-100 flex items-center justify-between">
                                <div>
                                    <span class="text-[10px] text-slate-400 uppercase font-bold block">Estimated Price</span>
                                    <div class="flex items-baseline gap-1.5">
                                        <span id="calculatedPrice" class="text-2xl font-black text-slate-900">£18.00</span>
                                        <span id="originalPrice" class="text-xs text-slate-400 line-through">£25.00</span>
                                    </div>
                                </div>
                                <button type="submit" class="px-6 py-3 bg-gradient-to-r from-emerald-600 to-teal-600 hover:from-emerald-700 hover:to-teal-700 text-white font-extrabold text-sm rounded-xl shadow-lg shadow-emerald-600/20 transition transform active:scale-95 flex items-center gap-2">
                                    <span>Do My Assignment</span>
                                    <i data-lucide="arrow-right" class="w-4 h-4"></i>
                                </button>
                            </div>
                        </form>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Trust Strip Banner -->
    <section class="bg-white border-y border-slate-200 py-6">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-2 md:grid-cols-4 gap-6 text-center">
                <div class="flex flex-col items-center">
                    <div class="w-10 h-10 rounded-full bg-blue-50 text-blue-600 flex items-center justify-center mb-2">
                        <i data-lucide="shield-check" class="w-5 h-5"></i>
                    </div>
                    <h3 class="text-sm font-bold text-slate-900">100% Genuine Human Work</h3>
                    <p class="text-xs text-slate-500">No AI-generated text or templates</p>
                </div>
                <div class="flex flex-col items-center">
                    <div class="w-10 h-10 rounded-full bg-emerald-50 text-emerald-600 flex items-center justify-center mb-2">
                        <i data-lucide="badge-check" class="w-5 h-5"></i>
                    </div>
                    <h3 class="text-sm font-bold text-slate-900">Grade Guarantee or Refund</h3>
                    <p class="text-xs text-slate-500">Strict quality assurance criteria</p>
                </div>
                <div class="flex flex-col items-center">
                    <div class="w-10 h-10 rounded-full bg-purple-50 text-purple-600 flex items-center justify-center mb-2">
                        <i data-lucide="file-check-2" class="w-5 h-5"></i>
                    </div>
                    <h3 class="text-sm font-bold text-slate-900">Free Turnitin Report</h3>
                    <p class="text-xs text-slate-500">Comprehensive plagiarism proof</p>
                </div>
                <div class="flex flex-col items-center">
                    <div class="w-10 h-10 rounded-full bg-amber-50 text-amber-600 flex items-center justify-center mb-2">
                        <i data-lucide="lock" class="w-5 h-5"></i>
                    </div>
                    <h3 class="text-sm font-bold text-slate-900">100% Encrypted & Private</h3>
                    <p class="text-xs text-slate-500">Strict data protection protocols</p>
                </div>
            </div>
        </div>
    </section>

    <!-- How to Access Services Section (3 Steps) -->
    <section id="how-it-works" class="py-16 lg:py-24 bg-slate-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-xs font-extrabold uppercase tracking-widest text-blue-600 bg-blue-100/80 px-3 py-1 rounded-full">Streamlined Process</span>
                <h2 class="text-3xl font-black text-slate-900 mt-3">How To Access Our Online Assignment Services</h2>
                <p class="text-slate-600 text-sm sm:text-base mt-2">Get high-scoring university assignments delivered in 3 simple, stress-free steps.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 relative">
                <!-- Connector line for desktop -->
                <div class="hidden md:block absolute top-1/2 left-0 w-full h-0.5 bg-slate-200 -z-0 transform -translate-y-6"></div>

                <!-- Step 1 -->
                <div class="bg-white rounded-2xl p-8 border border-slate-200 shadow-sm relative z-10 hover:shadow-md transition">
                    <div class="w-12 h-12 bg-blue-600 text-white rounded-2xl flex items-center justify-center font-black text-xl mb-6 shadow-md shadow-blue-500/20">
                        1
                    </div>
                    <h3 class="text-xl font-bold text-slate-900 mb-3">Drop In Your Brief</h3>
                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        Upload your assignment prompt, grading rubrics, and reading lists directly into our secure portal. Don't worry about messy formatting—just send over whatever guidelines your professor gave you, along with your target deadline.
                    </p>
                </div>

                <!-- Step 2 -->
                <div class="bg-white rounded-2xl p-8 border border-slate-200 shadow-sm relative z-10 hover:shadow-md transition">
                    <div class="w-12 h-12 bg-emerald-600 text-white rounded-2xl flex items-center justify-center font-black text-xl mb-6 shadow-md shadow-emerald-500/20">
                        2
                    </div>
                    <h3 class="text-xl font-bold text-slate-900 mb-3">Secure Match & Escrow</h3>
                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        Process your fully encrypted payment to immediately commission a verified, subject-specific authority who will begin crafting your blueprint with continuous progress tracking.
                    </p>
                </div>

                <!-- Step 3 -->
                <div class="bg-white rounded-2xl p-8 border border-slate-200 shadow-sm relative z-10 hover:shadow-md transition">
                    <div class="w-12 h-12 bg-purple-600 text-white rounded-2xl flex items-center justify-center font-black text-xl mb-6 shadow-md shadow-purple-500/20">
                        3
                    </div>
                    <h3 class="text-xl font-bold text-slate-900 mb-3">Academic Delivery</h3>
                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        Download your comprehensive, citation-verified draft alongside an exhaustive institutional-quality checklist and free Turnitin plagiarism report.
                    </p>
                </div>
            </div>

            <div class="text-center mt-12">
                <a href="#calculator" class="inline-flex items-center gap-2 px-8 py-4 bg-slate-900 hover:bg-slate-800 text-white font-bold text-sm rounded-xl shadow-lg transition">
                    <span>Order Your Assignment Now</span>
                    <i data-lucide="arrow-right" class="w-4 h-4"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- Why Students Choose EzAssign Section (6 Grid Cards) -->
    <section id="why-us" class="py-16 lg:py-24 bg-white border-t border-slate-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-xs font-extrabold uppercase tracking-widest text-emerald-600 bg-emerald-100/80 px-3 py-1 rounded-full">Unmatched Quality</span>
                <h2 class="text-3xl font-black text-slate-900 mt-3">Why Students Choose Our University Assignment Help</h2>
                <p class="text-slate-600 text-sm sm:text-base mt-2">Unlock our 100% AI-free, human-written assignment solutions designed to secure top academic scores.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Card 1 -->
                <div class="p-6 rounded-2xl bg-slate-50 border border-slate-200 hover:border-blue-400 transition group">
                    <div class="w-12 h-12 rounded-xl bg-blue-100 text-blue-600 flex items-center justify-center mb-5 group-hover:scale-110 transition-transform">
                        <i data-lucide="user-check" class="w-6 h-6"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 mb-2">Genuine, Human-Written Work</h3>
                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        Authentic scholarship refuses to follow a template. Our human experts structure arguments manually, keeping the human element intact for papers completely free of automated robotic patterns.
                    </p>
                </div>

                <!-- Card 2 -->
                <div class="p-6 rounded-2xl bg-slate-50 border border-slate-200 hover:border-emerald-400 transition group">
                    <div class="w-12 h-12 rounded-xl bg-emerald-100 text-emerald-600 flex items-center justify-center mb-5 group-hover:scale-110 transition-transform">
                        <i data-lucide="file-spreadsheet" class="w-6 h-6"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 mb-2">Custom Rubric Matching</h3>
                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        Your assigned writer closely reviews your specific department guidelines, grading rubrics, and course expectations to tailor every section to what professors expect.
                    </p>
                </div>

                <!-- Card 3 -->
                <div class="p-6 rounded-2xl bg-slate-50 border border-slate-200 hover:border-purple-400 transition group">
                    <div class="w-12 h-12 rounded-xl bg-purple-100 text-purple-600 flex items-center justify-center mb-5 group-hover:scale-110 transition-transform">
                        <i data-lucide="book-open-check" class="w-6 h-6"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 mb-2">Deep Scholarly Research</h3>
                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        We skip shallow summaries. Our writers pull evidence directly from credible, peer-reviewed databases including PubMed, Scopus, and JSTOR for maximum depth.
                    </p>
                </div>

                <!-- Card 4 -->
                <div class="p-6 rounded-2xl bg-slate-50 border border-slate-200 hover:border-amber-400 transition group">
                    <div class="w-12 h-12 rounded-xl bg-amber-100 text-amber-600 flex items-center justify-center mb-5 group-hover:scale-110 transition-transform">
                        <i data-lucide="headphone-off" class="w-6 h-6"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 mb-2">24/7 Dedicated Support</h3>
                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        Our support team is always online. Whether you need to make a last-minute instruction change or ask a quick question, someone is here to help right away.
                    </p>
                </div>

                <!-- Card 5 -->
                <div class="p-6 rounded-2xl bg-slate-50 border border-slate-200 hover:border-indigo-400 transition group">
                    <div class="w-12 h-12 rounded-xl bg-indigo-100 text-indigo-600 flex items-center justify-center mb-5 group-hover:scale-110 transition-transform">
                        <i data-lucide="line-chart" class="w-6 h-6"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 mb-2">Track Your Progress</h3>
                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        You are never left in the dark. With milestone tracking, see exactly how your paper is coming along and upload additional lecture notes at any stage.
                    </p>
                </div>

                <!-- Card 6 -->
                <div class="p-6 rounded-2xl bg-slate-50 border border-slate-200 hover:border-teal-400 transition group">
                    <div class="w-12 h-12 rounded-xl bg-teal-100 text-teal-600 flex items-center justify-center mb-5 group-hover:scale-110 transition-transform">
                        <i data-lucide="clock" class="w-6 h-6"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 mb-2">On-Time Guaranteed Delivery</h3>
                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        By using a fast, multi-stage writing process, our team consistently delivers your work ahead of schedule, leaving plenty of time for review before turning it in.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- FREEBIES BANNER (Highlighted in Emerald Green) -->
    <section id="freebies" class="py-12 bg-gradient-to-r from-emerald-800 via-emerald-700 to-teal-800 text-white relative overflow-hidden shadow-inner">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="flex flex-col lg:flex-row items-center justify-between gap-8">
                <div>
                    <span class="bg-amber-400 text-slate-950 font-black text-xs px-3 py-1 rounded-full uppercase tracking-wider">Compulsory Free Add-ons</span>
                    <h2 class="text-2xl sm:text-3xl font-black mt-2">Unlock Our Premium Academic Freebies</h2>
                    <p class="text-emerald-100 text-xs sm:text-sm mt-1">Every assignment order comes loaded with £80+ worth of complimentary academic tools.</p>
                </div>

                <!-- Freebies Grid Pills -->
                <div class="grid grid-cols-2 sm:grid-cols-3 gap-3 w-full lg:w-auto">
                    <div class="bg-white/10 backdrop-blur-md px-4 py-3 rounded-xl border border-white/20 flex items-center gap-2">
                        <i data-lucide="check-circle-2" class="w-5 h-5 text-amber-300"></i>
                        <div>
                            <p class="text-xs font-bold">Citing & Referencing</p>
                            <span class="text-[10px] text-amber-300 font-extrabold uppercase">FREE</span>
                        </div>
                    </div>
                    <div class="bg-white/10 backdrop-blur-md px-4 py-3 rounded-xl border border-white/20 flex items-center gap-2">
                        <i data-lucide="check-circle-2" class="w-5 h-5 text-amber-300"></i>
                        <div>
                            <p class="text-xs font-bold">Plagiarism Report</p>
                            <span class="text-[10px] text-amber-300 font-extrabold uppercase">FREE</span>
                        </div>
                    </div>
                    <div class="bg-white/10 backdrop-blur-md px-4 py-3 rounded-xl border border-white/20 flex items-center gap-2">
                        <i data-lucide="check-circle-2" class="w-5 h-5 text-amber-300"></i>
                        <div>
                            <p class="text-xs font-bold">Study Samples</p>
                            <span class="text-[10px] text-amber-300 font-extrabold uppercase">FREE</span>
                        </div>
                    </div>
                    <div class="bg-white/10 backdrop-blur-md px-4 py-3 rounded-xl border border-white/20 flex items-center gap-2">
                        <i data-lucide="check-circle-2" class="w-5 h-5 text-amber-300"></i>
                        <div>
                            <p class="text-xs font-bold">Editing & Proofing</p>
                            <span class="text-[10px] text-amber-300 font-extrabold uppercase">FREE</span>
                        </div>
                    </div>
                    <div class="bg-white/10 backdrop-blur-md px-4 py-3 rounded-xl border border-white/20 flex items-center gap-2">
                        <i data-lucide="check-circle-2" class="w-5 h-5 text-amber-300"></i>
                        <div>
                            <p class="text-xs font-bold">Limitless Corrections</p>
                            <span class="text-[10px] text-amber-300 font-extrabold uppercase">FREE</span>
                        </div>
                    </div>
                    <a href="#calculator" class="bg-amber-400 hover:bg-amber-300 text-slate-950 px-4 py-3 rounded-xl font-bold text-xs flex items-center justify-center gap-1 shadow-md transition">
                        <span>Claim Freebies</span>
                        <i data-lucide="arrow-right" class="w-4 h-4"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- 100+ Subjects Covered Section -->
    <section id="subjects" class="py-16 lg:py-24 bg-slate-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <span class="text-xs font-extrabold uppercase tracking-widest text-blue-600 bg-blue-100/80 px-3 py-1 rounded-full">Exhaustive Expertise</span>
                <h2 class="text-3xl font-black text-slate-900 mt-3">Spanning 100+ Distinct Academic Domains</h2>
                <p class="text-slate-600 text-sm sm:text-base mt-2">Our expansive network of 5,000+ scholarly experts delivers precise solutions across all major university disciplines.</p>
            </div>

            <!-- Domain Tag Cloud Grid -->
            <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-6 gap-3">
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="book-open" class="w-4 h-4 text-blue-500"></i> English Literature
                </div>
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="calculator" class="w-4 h-4 text-emerald-500"></i> Mathematics
                </div>
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="code-2" class="w-4 h-4 text-purple-500"></i> Programming & CS
                </div>
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="landmark" class="w-4 h-4 text-amber-500"></i> Law & Jurisprudence
                </div>
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="bar-chart-3" class="w-4 h-4 text-indigo-500"></i> Finance & Accounts
                </div>
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="cpu" class="w-4 h-4 text-red-500"></i> Engineering
                </div>
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="heart-pulse" class="w-4 h-4 text-pink-500"></i> Nursing & Healthcare
                </div>
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="globe" class="w-4 h-4 text-teal-500"></i> Social Science
                </div>
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="pie-chart" class="w-4 h-4 text-orange-500"></i> Economics
                </div>
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="binary" class="w-4 h-4 text-blue-600"></i> SPSS & Stata
                </div>
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="coffee" class="w-4 h-4 text-amber-700"></i> Java & C++ Help
                </div>
                <div class="bg-white p-3.5 rounded-xl border border-slate-200 text-center font-semibold text-xs text-slate-700 hover:border-blue-500 hover:text-blue-600 transition shadow-sm flex items-center justify-center gap-2">
                    <i data-lucide="briefcase" class="w-4 h-4 text-indigo-700"></i> MBA Coursework
                </div>
            </div>
        </div>
    </section>

    <!-- Thought Leadership & Human Expertise Section -->
    <section class="py-16 lg:py-24 bg-white border-t border-slate-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <div class="lg:col-span-7 space-y-5">
                    <span class="text-xs font-extrabold uppercase tracking-widest text-blue-600 bg-blue-50 px-3 py-1 rounded-full">Human vs Automated AI</span>
                    <h2 class="text-3xl font-black text-slate-900 leading-tight">
                        Why Verified Human Scholars Are Essential For UK Academic Success
                    </h2>
                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        In an era of automated content generation, human scholarship remains irreplaceable. AI tools sound repetitive and lack the ability to synthesize competing academic schools of thought or apply complex university rubrics effectively.
                    </p>
                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        At <strong>EzAssign</strong>, our dedicated specialists understand theoretical frameworks, empirical data collection, and rigorous referencing standards across UK higher education.
                    </p>

                    <!-- Scholar Citation Box -->
                    <div class="bg-slate-50 border-l-4 border-blue-600 p-5 rounded-r-2xl mt-4">
                        <p class="text-xs sm:text-sm text-slate-700 italic font-medium">
                            "I observe that many post-graduate students face challenges in executing the Point-Evidence-Explanation-Link (PEEL) framework, which directly depresses marks. We help them shift to analytical prose and cohesive structure for high-scoring submissions."
                        </p>
                        <div class="mt-3 flex items-center gap-3">
                            <div class="w-8 h-8 rounded-full bg-blue-600 text-white font-bold text-xs flex items-center justify-center">
                                AJ
                            </div>
                            <div>
                                <p class="text-xs font-bold text-slate-900">Alexis Jiang</p>
                                <p class="text-[10px] text-slate-500">Senior Academic Mentor & Literature Lead</p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Case Study Box -->
                <div class="lg:col-span-5">
                    <div class="bg-gradient-to-br from-slate-900 to-slate-800 text-white p-7 rounded-2xl shadow-xl border border-slate-700">
                        <div class="flex items-center gap-2 mb-4">
                            <i data-lucide="microscope" class="w-5 h-5 text-emerald-400"></i>
                            <span class="text-xs font-bold text-emerald-400 uppercase tracking-wider">Academic Case Insight</span>
                        </div>
                        <h3 class="text-lg font-bold text-white mb-2">Nike Supply Chain Management Analysis</h3>
                        <p class="text-slate-300 text-xs leading-relaxed mb-4">
                            Our real-time researchers analyze real-world frameworks. In our Nike case study, we demonstrate how demand planning, centralized data warehousing, and inventory forecasting maintain optimal customer balances in volatile markets.
                        </p>
                        <div class="pt-3 border-t border-slate-700 flex justify-between items-center text-xs">
                            <span class="text-slate-400">Sample Citation: Scopus & PubMed</span>
                            <a href="#calculator" class="text-emerald-400 font-bold hover:underline flex items-center gap-1">
                                Request Case Sample <i data-lucide="chevron-right" class="w-3.5 h-3.5"></i>
                            </a>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Transparent Hub & Urgent Help Section -->
    <section class="py-16 bg-slate-900 text-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
                
                <div>
                    <span class="text-xs font-extrabold uppercase tracking-widest text-emerald-400 bg-emerald-950 border border-emerald-800 px-3 py-1 rounded-full">Transparent Ecosystem</span>
                    <h2 class="text-2xl sm:text-3xl font-black mt-3">A Transparent Hub For Higher Education</h2>
                    <ul class="mt-6 space-y-4 text-xs sm:text-sm text-slate-300">
                        <li class="flex items-start gap-3">
                            <i data-lucide="check-circle" class="w-5 h-5 text-emerald-400 shrink-0 mt-0.5"></i>
                            <span><strong>Continuous Project Tracking:</strong> Monitor performance and milestones at each writing stage.</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <i data-lucide="check-circle" class="w-5 h-5 text-emerald-400 shrink-0 mt-0.5"></i>
                            <span><strong>Direct Scholar Interface:</strong> Communicate directly with your assignment helper for updates.</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <i data-lucide="check-circle" class="w-5 h-5 text-emerald-400 shrink-0 mt-0.5"></i>
                            <span><strong>Confidential Storage Ecosystem:</strong> 256-bit encryption protects research and payment details.</span>
                        </li>
                    </ul>
                </div>

                <div class="bg-gradient-to-tr from-blue-900/60 to-indigo-900/60 p-8 rounded-2xl border border-blue-500/30 backdrop-blur-sm">
                    <div class="flex items-center gap-3 mb-4">
                        <div class="p-3 bg-amber-500 text-slate-950 rounded-xl font-bold">
                            <i data-lucide="zap" class="w-6 h-6"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-white">Beat The Clock: Urgent Help</h3>
                            <p class="text-xs text-blue-200">Same-day turnaround available 24/7</p>
                        </div>
                    </div>
                    <p class="text-xs sm:text-sm text-slate-300 leading-relaxed mb-6">
                        Facing a deadline in 6 to 24 hours? Don't let time constraints ruin your GPA. Hand over the heavy lifting to our rapid-response urgent support team.
                    </p>
                    <a href="#calculator" class="w-full inline-block text-center px-6 py-3.5 bg-emerald-500 hover:bg-emerald-400 text-slate-950 font-black text-sm rounded-xl shadow-lg transition">
                        Order Urgent Assignment Now
                    </a>
                </div>

            </div>
        </div>
    </section>

    <!-- Interactive FAQs Accordion -->
    <section id="faqs" class="py-16 lg:py-24 bg-slate-50">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <span class="text-xs font-extrabold uppercase tracking-widest text-blue-600 bg-blue-100/80 px-3 py-1 rounded-full">Got Questions?</span>
                <h2 class="text-3xl font-black text-slate-900 mt-3">Frequently Asked Questions</h2>
                <p class="text-slate-600 text-xs sm:text-sm mt-2">Everything you need to know about EzAssign's academic support services.</p>
            </div>

            <div class="space-y-4" id="faqAccordion">
                
                <!-- FAQ Item 1 -->
                <div class="bg-white border border-slate-200 rounded-xl overflow-hidden transition">
                    <button class="faq-btn w-full p-5 text-left font-bold text-sm sm:text-base text-slate-900 flex justify-between items-center gap-4 hover:bg-slate-50">
                        <span>Can your online assignment maker handle specialized subjects like Law or Engineering?</span>
                        <i data-lucide="chevron-down" class="w-5 h-5 text-slate-400 transition-transform"></i>
                    </button>
                    <div class="faq-content hidden px-5 pb-5 text-xs sm:text-sm text-slate-600 border-t border-slate-100 pt-3 leading-relaxed">
                        Yes, absolutely. We pair students with domain-specific specialists holding advanced degrees in fields ranging from Law, Computer Science, and Engineering to Nursing and Financial Analysis.
                    </div>
                </div>

                <!-- FAQ Item 2 -->
                <div class="bg-white border border-slate-200 rounded-xl overflow-hidden transition">
                    <button class="faq-btn w-full p-5 text-left font-bold text-sm sm:text-base text-slate-900 flex justify-between items-center gap-4 hover:bg-slate-50">
                        <span>What makes EzAssign different from AI-generated alternatives?</span>
                        <i data-lucide="chevron-down" class="w-5 h-5 text-slate-400 transition-transform"></i>
                    </button>
                    <div class="faq-content hidden px-5 pb-5 text-xs sm:text-sm text-slate-600 border-t border-slate-100 pt-3 leading-relaxed">
                        Every single submission from EzAssign is written entirely from scratch by verified human academics. We guarantee zero AI content, providing full Turnitin plagiarism and AI reports with your delivery.
                    </div>
                </div>

                <!-- FAQ Item 3 -->
                <div class="bg-white border border-slate-200 rounded-xl overflow-hidden transition">
                    <button class="faq-btn w-full p-5 text-left font-bold text-sm sm:text-base text-slate-900 flex justify-between items-center gap-4 hover:bg-slate-50">
                        <span>How do I know the assignment will match my professor's grading rubric?</span>
                        <i data-lucide="chevron-down" class="w-5 h-5 text-slate-400 transition-transform"></i>
                    </button>
                    <div class="faq-content hidden px-5 pb-5 text-xs sm:text-sm text-slate-600 border-t border-slate-100 pt-3 leading-relaxed">
                        Your assigned scholar rigorously analyzes your prompt files, syllabus rubrics, and guidelines to ensure every argument aligns precisely with institutional expectations and marking criteria.
                    </div>
                </div>

                <!-- FAQ Item 4 -->
                <div class="bg-white border border-slate-200 rounded-xl overflow-hidden transition">
                    <button class="faq-btn w-full p-5 text-left font-bold text-sm sm:text-base text-slate-900 flex justify-between items-center gap-4 hover:bg-slate-50">
                        <span>Can you deliver urgent assignments on the same day?</span>
                        <i data-lucide="chevron-down" class="w-5 h-5 text-slate-400 transition-transform"></i>
                    </button>
                    <div class="faq-content hidden px-5 pb-5 text-xs sm:text-sm text-slate-600 border-t border-slate-100 pt-3 leading-relaxed">
                        Yes! Our team operates 24/7 across multiple time zones. We offer expedited turnarounds as fast as 6 hours for tight deadline situations without compromising quality.
                    </div>
                </div>

                <!-- FAQ Item 5 -->
                <div class="bg-white border border-slate-200 rounded-xl overflow-hidden transition">
                    <button class="faq-btn w-full p-5 text-left font-bold text-sm sm:text-base text-slate-900 flex justify-between items-center gap-4 hover:bg-slate-50">
                        <span>Is my personal and order data kept confidential?</span>
                        <i data-lucide="chevron-down" class="w-5 h-5 text-slate-400 transition-transform"></i>
                    </button>
                    <div class="faq-content hidden px-5 pb-5 text-xs sm:text-sm text-slate-600 border-t border-slate-100 pt-3 leading-relaxed">
                        Strict confidentiality is our top priority. We never share student data, documents, or payment details with third parties under any circumstances.
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Floating WhatsApp Action CTA -->
    <a href="https://wa.me/919256466594?text=Hi%20EzAssign,%20I%20want%20to%20order%20my%20assignment" target="_blank" class="fixed bottom-6 right-6 z-50 bg-emerald-500 hover:bg-emerald-600 text-white p-4 rounded-full shadow-2xl flex items-center gap-3 transition transform hover:scale-105 group border-2 border-white">
        <i data-lucide="message-square" class="w-6 h-6"></i>
        <span class="hidden sm:inline text-xs font-black tracking-wide pr-1">Need Urgent Help? Chat Now</span>
    </a>

    <!-- Footer Section -->
    <footer class="bg-slate-950 text-slate-400 text-xs border-t border-slate-800 pt-16 pb-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-5 gap-8 pb-12 border-b border-slate-800">
                
                <!-- Col 1: Brand Info -->
                <div class="lg:col-span-2 space-y-4">
                    <a href="#" class="flex items-center space-x-2">
                        <div class="w-9 h-9 bg-blue-600 rounded-lg flex items-center justify-center text-white font-black text-xl">Ez</div>
                        <span class="text-xl font-bold text-white">EzAssign.uk</span>
                    </a>
                    <p class="text-slate-400 leading-relaxed pr-4">
                        EzAssign is an elite academic support and mentorship platform operated by EZASSIGN LLP, assisting university students across the UK, Europe, and globally with 100% human-written coursework guidance.
                    </p>
                    <div class="space-y-1 text-slate-300 font-medium">
                        <p class="flex items-center gap-2"><i data-lucide="phone" class="w-4 h-4 text-emerald-400"></i> Helpline: +91-9256466594</p>
                        <p class="flex items-center gap-2"><i data-lucide="globe" class="w-4 h-4 text-blue-400"></i> Website: ezassign.uk</p>
                    </div>
                </div>

                <!-- Col 2: Subjects -->
                <div class="space-y-3">
                    <h4 class="text-white font-bold text-sm uppercase tracking-wider">Top Subjects</h4>
                    <ul class="space-y-2">
                        <li><a href="#calculator" class="hover:text-white transition">Law Assignment Help</a></li>
                        <li><a href="#calculator" class="hover:text-white transition">Finance & Accounts</a></li>
                        <li><a href="#calculator" class="hover:text-white transition">Nursing & Healthcare</a></li>
                        <li><a href="#calculator" class="hover:text-white transition">Computer Science & Java</a></li>
                        <li><a href="#calculator" class="hover:text-white transition">SPSS & Stata Help</a></li>
                    </ul>
                </div>

                <!-- Col 3: Quick Links -->
                <div class="space-y-3">
                    <h4 class="text-white font-bold text-sm uppercase tracking-wider">Useful Links</h4>
                    <ul class="space-y-2">
                        <li><a href="#how-it-works" class="hover:text-white transition">How It Works</a></li>
                        <li><a href="#why-us" class="hover:text-white transition">Why Choose Us</a></li>
                        <li><a href="#freebies" class="hover:text-white transition">Free Academic Add-ons</a></li>
                        <li><a href="#faqs" class="hover:text-white transition">FAQ & Support</a></li>
                    </ul>
                </div>

                <!-- Col 4: Trust Badge & Legal -->
                <div class="space-y-3">
                    <h4 class="text-white font-bold text-sm uppercase tracking-wider">Guaranteed Quality</h4>
                    <p class="text-slate-400 text-[11px] leading-normal">
                        Every order comes with 100% money-back grade assurance, strict privacy encryption, and verified institutional compliance.
                    </p>
                    <div class="pt-2 flex items-center gap-2">
                        <span class="bg-slate-800 text-slate-300 px-2 py-1 rounded text-[10px] font-bold border border-slate-700">100% Encrypted</span>
                        <span class="bg-slate-800 text-emerald-400 px-2 py-1 rounded text-[10px] font-bold border border-slate-700">0% AI Content</span>
                    </div>
                </div>
            </div>

            <!-- Disclaimer & Legal Disclaimer -->
            <div class="pt-8 space-y-4">
                <p class="text-[11px] text-slate-500 leading-relaxed">
                    <strong>Disclaimer:</strong> Reference papers and solution blueprints provided by EzAssign (ezassign.uk) serve strictly as model research materials and reference guides for students. These papers are intended to be utilized for study and academic referencing purposes only.
                </p>

                <div class="flex flex-col sm:flex-row justify-between items-center gap-4 text-[11px] text-slate-500 pt-4 border-t border-slate-900">
                    <p>© 2026 EZASSIGN LLP. Registered in Jaipur, Rajasthan, India. All rights reserved.</p>
                    <div class="flex gap-4">
                        <a href="#" class="hover:underline">Terms of Use</a>
                        <a href="#" class="hover:underline">Privacy Policy</a>
                        <a href="#" class="hover:underline">Revision Policy</a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <!-- Interactive JavaScript Logic -->
    <script>
        // Initialize Lucide Icons
        lucide.createIcons();

        // State variables for Order Form Calculator
        let currentPageCount = 1;
        const basePricePerPage = 18.00; // Base rate in £ GBP

        const pageDisplay = document.getElementById('pageDisplay');
        const calculatedPrice = document.getElementById('calculatedPrice');
        const originalPrice = document.getElementById('originalPrice');
        const btnMinus = document.getElementById('btnPageMinus');
        const btnPlus = document.getElementById('btnPagePlus');

        // Update Calculator UI
        function updateCalculator() {
            const words = currentPageCount * 250;
            pageDisplay.textContent = `${currentPageCount} ${currentPageCount === 1 ? 'Page' : 'Pages'} / ${words} Words`;
            
            const currentTotal = (currentPageCount * basePricePerPage).toFixed(2);
            const strikethroughTotal = (currentPageCount * (basePricePerPage * 1.4)).toFixed(2);

            calculatedPrice.textContent = `£${currentTotal}`;
            originalPrice.textContent = `£${strikethroughTotal}`;
        }

        btnPlus.addEventListener('click', () => {
            currentPageCount++;
            updateCalculator();
        });

        btnMinus.addEventListener('click', () => {
            if (currentPageCount > 1) {
                currentPageCount--;
                updateCalculator();
            }
        });

        // Service Tab Selection
        const serviceBtns = document.querySelectorAll('.service-btn');
        serviceBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                serviceBtns.forEach(b => {
                    b.classList.remove('bg-blue-600', 'text-white', 'shadow-sm');
                    b.classList.add('text-slate-600');
                });
                btn.classList.add('bg-blue-600', 'text-white', 'shadow-sm');
                btn.classList.remove('text-slate-600');
            });
        });

        // Mobile Menu Drawer Toggle
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mobileDrawer = document.getElementById('mobileDrawer');
        const mobileLinks = document.querySelectorAll('.mobile-link');

        mobileMenuBtn.addEventListener('click', () => {
            mobileDrawer.classList.toggle('hidden');
        });

        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileDrawer.classList.add('hidden');
            });
        });

        // Interactive FAQs Accordion Toggle
        const faqButtons = document.querySelectorAll('.faq-btn');
        faqButtons.forEach(btn => {
            btn.addEventListener('click', () => {
                const content = btn.nextElementSibling;
                const icon = btn.querySelector('i');
                
                content.classList.toggle('hidden');
                if (icon) {
                    icon.classList.toggle('rotate-180');
                }
            });
        });

        // File Upload Trigger Handler
        const uploadArea = document.getElementById('uploadArea');
        const fileInput = document.getElementById('fileInput');

        uploadArea.addEventListener('click', () => {
            fileInput.click();
        });

        fileInput.addEventListener('change', (e) => {
            if (e.target.files.length > 0) {
                uploadArea.querySelector('p').textContent = `Attached: ${e.target.files[0].name}`;
                uploadArea.classList.add('border-emerald-500', 'bg-emerald-50');
            }
        });

        // Form Submission Directing to WhatsApp Order Desk
        const assignmentForm = document.getElementById('assignmentForm');
        assignmentForm.addEventListener('submit', (e) => {
            e.preventDefault();
            
            const email = document.getElementById('userEmail').value;
            const code = document.getElementById('courseCode').value;
            const deadline = document.getElementById('deadlineTime').value;
            const phone = document.getElementById('countryCode').value + document.getElementById('phoneNumber').value;
            const brief = document.getElementById('briefNotes').value;

            const msg = `Hi EzAssign Team,%0A%0AI want to order an assignment:%0A- Email: ${email}%0A- Subject Code: ${code}%0A- Deadline: ${deadline} Hours%0A- Length: ${currentPageCount} Page(s) (${currentPageCount*250} Words)%0A- Phone: ${phone}%0A- Brief: ${encodeURIComponent(brief)}`;
            
            window.open(`https://wa.me/919256466594?text=${msg}`, '_blank');
        });
    </script>
</body>
</html>
