# YJPRBS
YJPRBS
<!DOCTYPE html>
<html lang="en">
<head>
    <base target="_self">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Journal of Yemeni Association of Plastic, Reconstructive and Burns Surgeons</title>
    <meta name="description" content="Official journal of the Yemeni Association of Plastic, Reconstructive and Burns Surgeons - Peer-reviewed research in plastic surgery, reconstructive surgery, and burns management.">
    <meta name="keywords" content="plastic surgery, reconstructive surgery, burns surgery, Yemen, medical journal, research, publications, subscribe, membership">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&family=Open+Sans:wght@300;400;600&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: "#1a365d",
                        secondary: "#2d3748",
                        accent: "#3182ce",
                        "accent-light": "#4299e1",
                        "medical-blue": "#1e40af",
                        "medical-teal": "#0d9488",
                        "journal-red": "#dc2626",
                        "asps-blue": "#003366",
                        "asps-gold": "#d4af37"
                    },
                    fontFamily: {
                        'heading': ['Montserrat', 'sans-serif'],
                        'body': ['Open Sans', 'sans-serif']
                    },
                    spacing: {
                        '128': '32rem',
                        '144': '36rem'
                    }
                }
            }
        }
    </script>
    <style>
        .hero-gradient {
            background: linear-gradient(135deg, #1a365d 0%, #2d3748 100%);
        }
        .card-hover {
            transition: all 0.3s ease;
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        .section-divider {
            border-bottom: 3px solid #3182ce;
            width: 60px;
            margin: 0 auto;
        }
        .modal {
            display: none;
            position: fixed;
            z-index: 1000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.5);
        }
        .modal-content {
            background-color: white;
            margin: 5% auto;
            padding: 0;
            width: 90%;
            max-width: 500px;
            border-radius: 10px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.2);
        }
        .tab-content {
            display: none;
        }
        .tab-content.active {
            display: block;
        }
        .tab-button.active {
            background-color: #3182ce;
            color: white;
        }
    </style>
</head>
<body class="font-body text-gray-700 bg-gray-50">
    <!-- Header & Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center py-4">
                <!-- Logo and Title -->
                <div class="flex items-center space-x-4 mb-4 md:mb-0">
                    <div class="w-16 h-16 bg-medical-blue rounded-full flex items-center justify-center">
                        <i class="fas fa-stethoscope text-white text-2xl"></i>
                    </div>
                    <div>
                        <h1 class="font-heading text-xl md:text-2xl font-bold text-primary">
                            Yemeni Association of Plastic, Reconstructive and Burns Surgeons
                        </h1>
                        <p class="text-sm text-gray-600">Official Journal</p>
                    </div>
                </div>

                <!-- User Actions -->
                <div class="flex items-center space-x-4 mb-4 md:mb-0">
                    <button id="signInBtn" class="text-accent hover:text-accent-light font-semibold">
                        <i class="fas fa-sign-in-alt mr-2"></i>Sign In
                    </button>
                    <button id="subscribeBtn" class="bg-accent text-white px-4 py-2 rounded-lg hover:bg-accent-light transition duration-300">
                        <i class="fas fa-crown mr-2"></i>Subscribe
                    </button>
                </div>

                <!-- Navigation -->
                <nav class="w-full md:w-auto">
                    <ul class="flex flex-wrap justify-center md:justify-end space-x-1 md:space-x-6">
                        <li><a href="#" class="nav-link text-medical-blue font-semibold">Home</a></li>
                        <li><a href="#" class="nav-link hover:text-medical-blue">Current Issue</a></li>
                        <li><a href="#" class="nav-link hover:text-medical-blue">Archives</a></li>
                        <li><a href="#" class="nav-link hover:text-medical-blue">Submit Paper</a></li>
                        <li><a href="#" class="nav-link hover:text-medical-blue">Editorial Board</a></li>
                        <li><a href="#" class="nav-link hover:text-medical-blue">For Members</a></li>
                        <li><a href="#" class="nav-link hover:text-medical-blue">About</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero-gradient text-white py-16 md:py-24">
        <div class="container mx-auto px-4">
            <div class="max-w-4xl mx-auto text-center">
                <h2 class="font-heading text-3xl md:text-5xl font-bold mb-6">
                    Journal of Yemeni Association of Plastic, Reconstructive and Burns Surgeons
                </h2>
                <p class="text-xl mb-8 opacity-90">
                    Advancing surgical excellence through peer-reviewed research and clinical innovations
                </p>
                <div class="flex flex-col sm:flex-row justify-center gap-4">
                    <button class="bg-white text-primary font-semibold py-3 px-8 rounded-lg hover:bg-gray-100 transition duration-300">
                        <i class="fas fa-book-open mr-2"></i>Browse Latest Issue
                    </button>
                    <button class="bg-accent text-white font-semibold py-3 px-8 rounded-lg hover:bg-accent-light transition duration-300">
                        <i class="fas fa-user-plus mr-2"></i>Join Association
                    </button>
                </div>
                <p class="mt-6 text-sm opacity-80">
                    <i class="fas fa-lock mr-2"></i>Secure access | 
                    <i class="fas fa-users mr-2 ml-4"></i>1,200+ Members | 
                    <i class="fas fa-globe mr-2 ml-4"></i>International Reach
                </p>
            </div>
        </div>
    </section>

    <!-- Subscription Banner -->
    <div class="bg-gradient-to-r from-asps-blue to-medical-blue text-white">
        <div class="container mx-auto px-4 py-4">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-4 md:mb-0">
                    <h3 class="font-heading text-xl font-bold">
                        <i class="fas fa-star mr-2"></i>Premium Journal Access
                    </h3>
                    <p class="text-sm opacity-90">Get full access to all articles, archives, and exclusive member content</p>
                </div>
                <div class="flex space-x-4">
                    <button class="bg-white text-asps-blue font-semibold px-6 py-2 rounded-lg hover:bg-gray-100 transition duration-300">
                        <i class="fas fa-eye mr-2"></i>View Subscription Options
                    </button>
                    <button class="bg-asps-gold text-asps-blue font-semibold px-6 py-2 rounded-lg hover:bg-yellow-500 transition duration-300">
                        <i class="fas fa-gem mr-2"></i>Become a Member
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- Main Content -->
    <main class="container mx-auto px-4 py-12">
        <!-- Featured Articles (with access badges) -->
        <section class="mb-16">
            <div class="text-center mb-12">
                <h2 class="font-heading text-3xl font-bold text-primary mb-4">Featured Articles</h2>
                <div class="section-divider"></div>
                <p class="text-gray-600 mt-4">Latest research - Access indicators show subscription requirements</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Article 1 - Free Access -->
                <div class="bg-white rounded-xl shadow-lg overflow-hidden card-hover">
                    <div class="relative">
                        <img 
                            src="https://picsum.photos/400/250?random=1" 
                            alt="Plastic surgery procedure" 
                            class="w-full h-48 object-cover"
                            loading="lazy"
                        >
                        <div class="absolute top-4 left-4 bg-green-500 text-white px-3 py-1 rounded-full text-sm font-semibold">
                            <i class="fas fa-unlock mr-1"></i>Free Access
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex items-center text-sm text-gray-500 mb-3">
                            <span class="bg-gray-100 px-2 py-1 rounded">Original Article</span>
                            <span class="mx-2">•</span>
                            <span>Dec 2023</span>
                        </div>
                        <h3 class="font-heading text-xl font-bold text-primary mb-3">
                            Microsurgical Reconstruction in Post-Traumatic Facial Defects
                        </h3>
                        <p class="text-gray-600 mb-4">
                            Comprehensive analysis of 50 cases of microsurgical reconstruction following traumatic facial injuries.
                        </p>
                        <div class="flex justify-between items-center">
                            <span class="text-sm text-gray-500">Dr. Ahmed Al-Mansoori et al.</span>
                            <a href="#" class="text-accent font-semibold hover:text-accent-light">Read Article →</a>
                        </div>
                    </div>
                </div>

                <!-- Article 2 - Member Only -->
                <div class="bg-white rounded-xl shadow-lg overflow-hidden card-hover border-2 border-asps-blue">
                    <div class="relative">
                        <img 
                            src="https://picsum.photos/400/250?random=2" 
                            alt="Burns treatment" 
                            class="w-full h-48 object-cover"
                            loading="lazy"
                        >
                        <div class="absolute top-4 left-4 bg-asps-blue text-white px-3 py-1 rounded-full text-sm font-semibold">
                            <i class="fas fa-crown mr-1"></i>Member Only
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex items-center text-sm text-gray-500 mb-3">
                            <span class="bg-gray-100 px-2 py-1 rounded">Clinical Study</span>
                            <span class="mx-2">•</span>
                            <span>Nov 2023</span>
                        </div>
                        <h3 class="font-heading text-xl font-bold text-primary mb-3">
                            Modern Burn Care Protocols in Resource-Limited Settings
                        </h3>
                        <p class="text-gray-600 mb-4">
                            Evaluation of adapted burn care protocols and their outcomes in Yemen's healthcare facilities.
                        </p>
                        <div class="flex justify-between items-center">
                            <span class="text-sm text-gray-500">Dr. Fatima Al-Hakimi et al.</span>
                            <button class="text-asps-blue font-semibold hover:text-asps-blue/80" onclick="showSignInModal()">
                                <i class="fas fa-lock mr-1"></i>Subscribe to Read
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Article 3 - Subscription Required -->
                <div class="bg-white rounded-xl shadow-lg overflow-hidden card-hover border-2 border-purple-600">
                    <div class="relative">
                        <img 
                            src="https://picsum.photos/400/250?random=3" 
                            alt="Reconstructive surgery" 
                            class="w-full h-48 object-cover"
                            loading="lazy"
                        >
                        <div class="absolute top-4 left-4 bg-purple-600 text-white px-3 py-1 rounded-full text-sm font-semibold">
                            <i class="fas fa-star mr-1"></i>Premium
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex items-center text-sm text-gray-500 mb-3">
                            <span class="bg-gray-100 px-2 py-1 rounded">Systematic Review</span>
                            <span class="mx-2">•</span>
                            <span>Oct 2023</span>
                        </div>
                        <h3 class="font-heading text-xl font-bold text-primary mb-3">
                            Craniofacial Reconstruction Techniques in Arab Populations
                        </h3>
                        <p class="text-gray-600 mb-4">
                            Systematic review of craniofacial reconstruction methods adapted for Middle Eastern populations.
                        </p>
                        <div class="flex justify-between items-center">
                            <span class="text-sm text-gray-500">Dr. Mohammed Al-Sayed et al.</span>
                            <button class="text-purple-600 font-semibold hover:text-purple-700" onclick="showSubscriptionModal()">
                                <i class="fas fa-gem mr-1"></i>Upgrade to Read
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Subscription Plans -->
        <section class="mb-16">
            <div class="text-center mb-12">
                <h2 class="font-heading text-3xl font-bold text-primary mb-4">Choose Your Access Level</h2>
                <div class="section-divider"></div>
                <p class="text-gray-600 mt-4">Modeled after American Society of Plastic Surgeons journal access tiers</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Free Tier -->
                <div class="bg-white rounded-xl shadow-lg p-8 border border-gray-200">
                    <div class="text-center mb-6">
                        <h3 class="font-heading text-2xl font-bold text-gray-700 mb-2">Free Reader</h3>
                        <div class="text-4xl font-bold text-primary mb-2">$0</div>
                        <div class="text-gray-500">per year</div>
                    </div>
                    <ul class="space-y-4 mb-8">
                        <li class="flex items-center">
                            <i class="fas fa-check text-green-500 mr-3"></i>
                            <span>Limited article access (3/month)</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-green-500 mr-3"></i>
                            <span>Basic newsletter</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-green-500 mr-3"></i>
                            <span>Table of contents alerts</span>
                        </li>
                        <li class="flex items-center text-gray-400">
                            <i class="fas fa-times mr-3"></i>
                            <span>No full-text archives</span>
                        </li>
                        <li class="flex items-center text-gray-400">
                            <i class="fas fa-times mr-3"></i>
                            <span>No member-only content</span>
                        </li>
                    </ul>
                    <button class="w-full bg-gray-100 text-primary font-semibold py-3 rounded-lg hover:bg-gray-200 transition duration-300" onclick="showSignInModal()">
                        <i class="fas fa-user mr-2"></i>Create Free Account
                    </button>
                </div>

                <!-- Individual Subscription -->
                <div class="bg-white rounded-xl shadow-lg p-8 border-2 border-accent relative">
                    <div class="absolute -top-4 left-1/2 transform -translate-x-1/2">
                        <span class="bg-accent text-white px-4 py-1 rounded-full text-sm font-semibold">
                            Most Popular
                        </span>
                    </div>
                    <div class="text-center mb-6">
                        <h3 class="font-heading text-2xl font-bold text-primary mb-2">Individual Subscription</h3>
                        <div class="text-4xl font-bold text-accent mb-2">$249</div>
                        <div class="text-gray-500">per year</div>
                    </div>
                    <ul class="space-y-4 mb-8">
                        <li class="flex items-center">
                            <i class="fas fa-check text-green-500 mr-3"></i>
                            <span>Unlimited article access</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-green-500 mr-3"></i>
                            <span>Full-text archives (5+ years)</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-green-500 mr-3"></i>
                            <span>Early view articles</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-green-500 mr-3"></i>
                            <span>PDF downloads</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-green-500 mr-3"></i>
                            <span>Mobile app access</span>
                        </li>
                    </ul>
                    <button class="w-full bg-accent text-white font-semibold py-3 rounded-lg hover:bg-accent-light transition duration-300" onclick="showSubscriptionModal()">
                        <i class="fas fa-credit-card mr-2"></i>Subscribe Now
                    </button>
                </div>

                <!-- Association Membership -->
                <div class="bg-white rounded-xl shadow-lg p-8 border-2 border-asps-gold">
                    <div class="text-center mb-6">
                        <h3 class="font-heading text-2xl font-bold text-primary mb-2">Full Membership</h3>
                        <div class="text-4xl font-bold text-asps-gold mb-2">$499</div>
                        <div class="text-gray-500">per year</div>
                    </div>
                    <ul class="space-y-4 mb-8">
                        <li class="flex items-center">
                            <i class="fas fa-crown text-asps-gold mr-3"></i>
                            <span>All subscription benefits</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-crown text-asps-gold mr-3"></i>
                            <span>Voting rights in association</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-crown text-asps-gold mr-3"></i>
                            <span>Conference discounts</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-crown text-asps-gold mr-3"></i>
                            <span>CME/CE credits</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-crown text-asps-gold mr-3"></i>
                            <span>Networking opportunities</span>
                        </li>
                    </ul>
                    <button class="w-full bg-asps-gold text-asps-blue font-semibold py-3 rounded-lg hover:bg-yellow-500 transition duration-300" onclick="showMembershipModal()">
                        <i class="fas fa-gem mr-2"></i>Join Association
                    </button>
                </div>
            </div>
        </section>

        <!-- Journal Features -->
        <section class="mb-16">
            <div class="bg-white rounded-xl shadow-lg p-8">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                    <div>
                        <h3 class="font-heading text-2xl font-bold text-primary mb-6">ASPS-Style Features</h3>
                        <div class="space-y-6">
                            <div class="flex items-start">
                                <div class="bg-blue-100 p-3 rounded-lg mr-4">
                                    <i class="fas fa-shield-alt text-blue-600 text-xl"></i>
                                </div>
                                <div>
                                    <h4 class="font-semibold text-lg mb-2">Secure Single Sign-On</h4>
                                    <p class="text-gray-600">One login for journal access, member portal, and conference registration</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <div class="bg-green-100 p-3 rounded-lg mr-4">
                                    <i class="fas fa-mobile-alt text-green-600 text-xl"></i>
                                </div>
                                <div>
                                    <h4 class="font-semibold text-lg mb-2">Mobile-Optimized</h4>
                                    <p class="text-gray-600">Access articles on any device with responsive design and dedicated mobile apps</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <div class="bg-purple-100 p-3 rounded-lg mr-4">
                                    <i class="fas fa-chart-line text-purple-600 text-xl"></i>
                                </div>
                                <div>
                                    <h4 class="font-semibold text-lg mb-2">Advanced Metrics</h4>
                                    <p class="text-gray-600">Track article usage, citations, and impact factors like leading medical journals</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div>
                        <h3 class="font-heading text-2xl font-bold text-primary mb-6">Institutional Access</h3>
                        <div class="bg-gradient-to-r from-blue-50 to-gray-50 p-6 rounded-lg">
                            <h4 class="font-semibold text-lg mb-4">For Hospitals & Universities</h4>
                            <p class="text-gray-600 mb-4">Provide access to your entire institution with our site license options:</p>
                            <ul class="space-y-3 mb-6">
                                <li class="flex items-center">
                                    <i class="fas fa-check text-green-500 mr-3"></i>
                                    <span>Unlimited concurrent users</span>
                                </li>
                                <li class="flex items-center">
                                    <i class="fas fa-check text-green-500 mr-3"></i>
                                    <span>IP-based access</span>
                                </li>
                                <li class="flex items-center">
                                    <i class="fas fa-check text-green-500 mr-3"></i>
                                    <span>Usage statistics and reports</span>
                                </li>
                                <li class="flex items-center">
                                    <i class="fas fa-check text-green-500 mr-3"></i>
                                    <span>Print subscriptions available</span>
                                </li>
                            </ul>
                            <button class="w-full bg-gray-800 text-white font-semibold py-3 rounded-lg hover:bg-gray-900 transition duration-300">
                                Request Institutional Quote
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Current Issue Preview -->
        <section>
            <div class="text-center mb-12">
                <h2 class="font-heading text-3xl font-bold text-primary mb-4">Current Issue Preview</h2>
                <div class="section-divider"></div>
                <p class="text-gray-600 mt-4">Volume 7, Issue 1 - March 2024</p>
            </div>

            <div class="bg-white rounded-xl shadow-lg overflow-hidden">
                <div class="md:flex">
                    <div class="md:w-1/3 p-8 bg-gradient-to-b from-primary to-secondary text-white flex flex-col justify-center">
                        <div class="text-center">
                            <div class="text-6xl font-bold mb-2">7</div>
                            <div class="text-2xl font-semibold mb-4">Volume 7, Issue 1</div>
                            <div class="text-xl mb-6">March 2024</div>
                            <div class="space-y-3">
                                <div class="flex items-center justify-center">
                                    <i class="fas fa-file-alt mr-2"></i>
                                    <span>12 Original Articles</span>
                                </div>
                                <div class="flex items-center justify-center">
                                    <i class="fas fa-comments mr-2"></i>
                                    <span>4 Review Articles</span>
                                </div>
                                <div class="flex items-center justify-center">
                                    <i class="fas fa-case mr-2"></i>
                                    <span>6 Case Reports</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="md:w-2/3 p-8">
                        <h3 class="font-heading text-2xl font-bold text-primary mb-6">Featured in This Issue</h3>
                        <div class="space-y-6">
                            <div class="border-l-4 border-accent pl-4">
                                <h4 class="font-semibold text-lg mb-2">Editor's Choice: Free Access</h4>
                                <p class="text-gray-600">"Innovative Flap Techniques in Yemeni Reconstructive Surgery" - Available to all readers</p>
                            </div>
                            <div class="border-l-4 border-asps-blue pl-4">
                                <h4 class="font-semibold text-lg mb-2">Member Exclusive</h4>
                                <p class="text-gray-600">"Five-Year Outcomes of Burn Reconstruction in Pediatric Patients" - Association members only</p>
                            </div>
                            <div class="border-l-4 border-purple-600 pl-4">
                                <h4 class="font-semibold text-lg mb-2">Subscription Required</h4>
                                <p class="text-gray-600">"Comparative Analysis of Microsurgical Techniques Across Arab Countries" - Full access needed</p>
                            </div>
                        </div>
                        <div class="mt-8 flex flex-wrap gap-4">
                            <button class="bg-accent text-white font-semibold px-6 py-3 rounded-lg hover:bg-accent-light transition duration-300">
                                <i class="fas fa-book-open mr-2"></i>Browse Table of Contents
                            </button>
                            <button class="bg-white border border-accent text-accent font-semibold px-6 py-3 rounded-lg hover:bg-blue-50 transition duration-300">
                                <i class="fas fa-shopping-cart mr-2"></i>Purchase Single Issue ($49)
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-primary text-white pt-12 pb-8">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-8">
                <!-- Quick Access -->
                <div>
                    <h4 class="font-heading text-xl font-bold mb-4">Quick Access</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300"><i class="fas fa-sign-in-alt mr-2"></i>Member Login</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300"><i class="fas fa-key mr-2"></i>Reset Password</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300"><i class="fas fa-question-circle mr-2"></i>Help Center</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300"><i class="fas fa-phone mr-2"></i>Contact Support</a></li>
                    </ul>
                </div>

                <!-- Resources -->
                <div>
                    <h4 class="font-heading text-xl font-bold mb-4">Resources</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300">Author Guidelines</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300">Reviewer Center</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300">Editorial Policies</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white transition duration-300">Copyright & Permissions</a></li>
                    </ul>
                </div>

                <!-- Contact -->
                <div>
                    <h4 class="font-heading text-xl font-bold mb-4">Contact</h4>
                    <ul class="space-y-3">
                        <li class="flex items-start">
                            <i class="fas fa-map-marker-alt mr-3 mt-1"></i>
                            <span class="text-gray-300">Editorial Office: Sana'a Medical Complex, Yemen</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-envelope mr-3"></i>
                            <span class="text-gray-300">subscriptions@yaps-journal.org</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-phone mr-3"></i>
                            <span class="text-gray-300">+967 1 234 5678 (Subscriptions)</span>
                        </li>
                    </ul>
                </div>

                <!-- Partners -->
                <div>
                    <h4 class="font-heading text-xl font-bold mb-4">Partners</h4>
                    <p class="text-gray-300 mb-4">In collaboration with:</p>
                    <div class="space-y-2">
                        <div class="flex items-center">
                            <i class="fas fa-handshake mr-3 text-asps-gold"></i>
                            <span class="text-gray-300">ASPS International Partners</span>
                        </div>
                        <div class="flex items-center">
                            <i class="fas fa-globe-americas mr-3 text-accent"></i>
                            <span class="text-gray-300">Middle East Plastic Surgery Federation</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Copyright -->
            <div class="border-t border-gray-700 pt-8 text-center">
                <p class="text-gray-400">
                    © 2024 Journal of Yemeni Association of Plastic, Reconstructive and Burns Surgeons. All rights reserved.
                </p>
                <p class="text-gray-400 text-sm mt-2">
                    ISSN: 2790-1234 | PubMed Indexed | Crossref Member | Published Quarterly
                </p>
                <div class="flex justify-center space-x-6 mt-4">
                    <a href="#" class="text-gray-400 hover:text-white text-sm">Privacy Policy</a>
                    <a href="#" class="text-gray-400 hover:text-white text-sm">Terms of Service</a>
                    <a href="#" class="text-gray-400 hover:text-white text-sm">Cookie Policy</a>
                    <a href="#" class="text-gray-400 hover:text-white text-sm">Accessibility</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Sign In Modal -->
    <div id="signInModal" class="modal">
        <div class="modal-content">
            <div class="bg-primary text-white p-6 rounded-t-lg">
                <div class="flex justify-between items-center">
                    <h3 class="font-heading text-2xl font-bold">Sign In to Your Account</h3>
                    <button class="text-white text-2xl" onclick="closeModal('signInModal')">&times;</button>
                </div>
                <p class="text-gray-300 mt-2">Access your subscriptions, saved articles, and member benefits</p>
            </div>
            <div class="p-6">
                <div class="flex border-b mb-6">
                    <button class="tab-button active flex-1 py-3 font-semibold" onclick="switchTab('signInTab', 'login')">Login</button>
                    <button class="tab-button flex-1 py-3 font-semibold" onclick="switchTab('signInTab', 'register')">Register</button>
                </div>
                
                <div id="login" class="tab-content active">
                    <form id="loginForm">
                        <div class="space-y-4">
                            <div>
                                <label class="block text-gray-700 mb-2">Email Address</label>
                                <input type="email" class="w-full px-4 py-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-accent" placeholder="your.email@example.com" required>
                            </div>
                            <div>
                                <label class="block text-gray-700 mb-2">Password</label>
                                <input type="password" class="w-full px-4 py-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-accent" placeholder="Enter your password" required>
                            </div>
                            <div class="flex items-center justify-between">
                                <label class="flex items-center">
                                    <input type="checkbox" class="mr-2">
                                    <span class="text-gray-600">Remember me</span>
                                </label>
                                <a href="#" class="text-accent hover:text-accent-light">Forgot password?</a>
                            </div>
                            <button type="submit" class="w-full bg-accent text-white font-semibold py-3 rounded-lg hover:bg-accent-light transition duration-300">
                                <i class="fas fa-sign-in-alt mr-2"></i>Sign In
                            </button>
                        </div>
                    </form>
                    <div class="mt-6 text-center">
                        <p class="text-gray-600">Or sign in with</p>
                        <div class="flex justify-center space-x-4 mt-4">
                            <button class="bg-blue-600 text-white p-3 rounded-lg hover:bg-blue-700">
                                <i class="fab fa-google"></i>
                            </button>
                            <button class="bg-blue-800 text-white p-3 rounded-lg hover:bg-blue-900">
                                <i class="fab fa-microsoft"></i>
                            </button>
                            <button class="bg-gray-800 text-white p-3 rounded-lg hover:bg-gray-900">
                                <i class="fab fa-orcid"></i>
                            </button>
                        </div>
                    </div>
                </div>
                
                <div id="register" class="tab-content">
                    <form id="registerForm">
                        <div class="space-y-4">
                            <div class="grid grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-gray-700 mb-2">First Name</label>
                                    <input type="text" class="w-full px-4 py-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-accent" required>
                                </div>
                                <div>
                                    <label class="block text-gray-700 mb-2">Last Name</label>
                                    <input type="text" class="w-full px-4 py-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-accent" required>
                                </div>
                            </div>
                            <div>
                                <label class="block text-gray-700 mb-2">Email Address</label>
                                <input type="email" class="w-full px-4 py-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-accent" required>
                            </div>
                            <div>
                                <label class="block text-gray-700 mb-2">Create Password</label>
                                <input type="password" class="w-full px-4 py-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-accent" required>
                            </div>
                            <div>
                                <label class="block text-gray-700 mb-2">Confirm Password</label>
                                <input type="password" class="w-full px-4 py-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-accent" required>
                            </div>
                            <div class="flex items-center">
                                <input type="checkbox" class="mr-2" required>
                                <span class="text-gray-600 text-sm">I agree to the <a href="#" class="text-accent">Terms of Service</a> and <a href="#" class="text-accent">Privacy Policy</a></span>
                            </div>
                            <button type="submit" class="w-full bg-accent text-white font-semibold py-3 rounded-lg hover:bg-accent-light transition duration-300">
                                <i class="fas fa-user-plus mr-2"></i>Create Free Account
                            </button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>

    <!-- Subscription Modal -->
    <div id="subscriptionModal" class="modal">
        <div class="modal-content">
            <div class="bg-gradient-to-r from-asps-blue to-medical-blue text-white p-6 rounded-t-lg">
                <div class="flex justify-between items-center">
                    <h3 class="font-heading text-2xl font-bold">Choose Your Subscription</h3>
                    <button class="text-white text-2xl" onclick="closeModal('subscriptionModal')">&times;</button>
                </div>
                <p class="text-gray-300 mt-2">Get full access to all journal content and member benefits</p>
            </div>
            <div class="p-6">
                <div class="space-y-6">
                    <div class="border border-accent rounded-lg p-6 hover:bg-blue-50 cursor-pointer" onclick="selectPlan('individual')">
                        <div class="flex justify-between items-center">
                            <div>
                                <h4 class="font-semibold text-lg mb-1">Individual Subscription</h4>
                                <p class="text-gray-600">Unlimited access to all articles</p>
                            </div>
                            <div class="text-right">
                                <div class="text-2xl font-bold text-accent">$249</div>
                                <div class="text-gray-500 text-sm">per year</div>
                            </div>
                        </div>
                    </div>
                    
                    <div class="border-2 border-asps-gold rounded-lg p-6 hover:bg-yellow-50 cursor-pointer" onclick="selectPlan('membership')">
                        <div class="flex justify-between items-center">
                            <div>
                                <div class="flex items-center">
                                    <h4 class="font-semibold text-lg mb-1">Full Association Membership</h4>
                                    <span class="ml-2 bg-asps-gold text-asps-blue px-2 py-1 rounded text-xs font-bold">BEST VALUE</span>
                                </div>
                                <p class="text-gray-600">All benefits plus voting rights and CME credits</p>
                            </div>
                            <div class="text-right">
                                <div class="text-2xl font-bold text-asps-gold">$499</div>
                                <div class="text-gray-500 text-sm">per year</div>
                            </div>
                        </div>
                    </div>
                    
                    <div class="border border-gray-300 rounded-lg p-6 hover:bg-gray-50 cursor-pointer" onclick="selectPlan('institutional')">
                        <div class="flex justify-between items-center">
                            <div>
                                <h4 class="font-semibold text-lg mb-1">Institutional License</h4>
                                <p class="text-gray-600">For hospitals, universities, and libraries</p>
                            </div>
                            <div class="text-right">
                                <div class="text-lg font-bold text-gray-700">Starting at $1,999</div>
                                <div class="text-gray-500 text-sm">per year</div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div id="paymentForm" class="mt-8 hidden">
                    <h4 class="font-heading text-xl font-bold mb-6">Payment Information</h4>
                    <form id="paymentDetailsForm">
                        <div class="space-y-4">
                            <div>
                                <label class="block text-gray-700 mb-2">Card Number</label>
                                <input type="text" class="w-full px-4 py-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-accent" placeholder="1234 5678 9012 3456" required>
                            </div>
                            <div class="grid grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-gray-700 mb-2">Expiry Date</label>
                                    <input type="text" class="w-full px-4 py-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-accent" placeholder="MM/YY" required>
                                </div>
                                <div>
                                    <label class="block text-gray-700 mb-2">CVV</label>
                                    <input type="text" class="w-full px-4 py-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-accent" placeholder="123" required>
                                </div>
                            </div>
                            <div>
                                <label class="block text-gray-700 mb-2">Billing Address</label>
                                <textarea class="w-full px-4 py-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-accent" rows="2" required></textarea>
                            </div>
                            <div class="flex items-center">
                                <input type="checkbox" class="mr-2" required>
                                <span class="text-gray-600 text-sm">I authorize annual renewal of this subscription</span>
                            </div>
                            <button type="submit" class="w-full bg-green-600 text-white font-semibold py-3 rounded-lg hover:bg-green-700 transition duration-300">
                                <i class="fas fa-lock mr-2"></i>Complete Secure Payment
                            </button>
                        </div>
                    </form>
                </div>
                
                <div class="mt-8 text-center">
                    <p class="text-gray-600 text-sm">
                        <i class="fas fa-lock mr-2"></i>Secure payment processed by Stripe
                        <br>
                        <i class="fas fa-shield-alt mr-2 mt-2"></i>30-day money-back guarantee
                    </p>
                </div>
            </div>
        </div>
    </div>

    <!-- Success Message -->
    <div id="successMessage" class="fixed bottom-4 right-4 bg-green-500 text-white p-4 rounded-lg shadow-lg hidden z-50">
        <div class="flex items-center">
            <i class="fas fa-check-circle text-2xl mr-3"></i>
            <div>
                <p class="font-semibold" id="successTitle">Success!</p>
                <p id="successText">Your action was completed successfully.</p>
            </div>
        </div>
    </div>

    <script>
        // Modal Functions
        function showSignInModal() {
            document.getElementById('signInModal').style.display = 'block';
        }

        function showSubscriptionModal() {
            document.getElementById('subscriptionModal').style.display = 'block';
        }

        function showMembershipModal() {
            showSubscriptionModal();
            setTimeout(() => selectPlan('membership'), 100);
        }

        function closeModal(modalId) {
            document.getElementById(modalId).style.display = 'none';
            document.getElementById('paymentForm').classList.add('hidden');
        }

        function switchTab(containerId, tabId) {
            // Update tab buttons
            document.querySelectorAll(`#${containerId} .tab-button`).forEach(btn => {
                btn.classList.remove('active');
            });
            event.target.classList.add('active');
            
            // Update tab content
            document.querySelectorAll(`#${containerId} .tab-content`).forEach(content => {
                content.classList.remove('active');
            });
            document.getElementById(tabId).classList.add('active');
        }

        function selectPlan(planType) {
            const paymentForm = document.getElementById('paymentForm');
            paymentForm.classList.remove('hidden');
            paymentForm.scrollIntoView({ behavior: 'smooth' });
            
            // Update form based on plan
            const formTitle = document.querySelector('#paymentForm h4');
            if (planType === 'individual') {
                formTitle.textContent = "Individual Subscription - $249/year";
            } else if (planType === 'membership') {
                formTitle.textContent = "Association Membership - $499/year";
            } else if (planType === 'institutional') {
                formTitle.textContent = "Institutional License - Starting at $1,999/year";
            }
        }

        // Form Submission Handlers
        document.addEventListener('DOMContentLoaded', function() {
            // Login Form
            document.getElementById('loginForm')?.addEventListener('submit', function(e) {
                e.preventDefault();
                closeModal('signInModal');
                showSuccess('Welcome back!', 'You have successfully signed in to your account.');
            });

            // Register Form
            document.getElementById('registerForm')?.addEventListener('submit', function(e) {
                e.preventDefault();
                closeModal('signInModal');
                showSuccess('Account Created!', 'Your free account has been created. Check your email for verification.');
            });

            // Payment Form
            document.getElementById('paymentDetailsForm')?.addEventListener('submit', function(e) {
                e.preventDefault();
                closeModal('subscriptionModal');
                showSuccess('Subscription Activated!', 'Your subscription is now active. You have full access to all journal content.');
            });

            // Navigation click handlers
            document.querySelectorAll('.nav-link').forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    const page = this.textContent;
                    alert(`Navigating to ${page} section (simulated)`);
                });
            });

            // Button click handlers
            document.querySelectorAll('button').forEach(button => {
                if (button.textContent.includes('Browse') || button.textContent.includes('View') || button.textContent.includes('Join')) {
                    if (!button.onclick) {
                        button.addEventListener('click', function() {
                            const action = this.textContent.trim();
                            showSuccess('Action Triggered', `${action} functionality would open here.`);
                        });
                    }
                }
            });

            // Close modals when clicking outside
            window.addEventListener('click', function(e) {
                if (e.target.classList.contains('modal')) {
                    e.target.style.display = 'none';
                }
            });
        });

        function showSuccess(title, message) {
            const successMsg = document.getElementById('successMessage');
            document.getElementById('successTitle').textContent = title;
            document.getElementById('successText').textContent = message;
            successMsg.classList.remove('hidden');
            
            setTimeout(() => {
                successMsg.classList.add('hidden');
            }, 5000);
        }

        // User state management
        const userState = {
            isLoggedIn: false,
            subscriptionLevel: null,
            membershipType: null,
            savedArticles: [],
            preferences: {}
        };

        // Article access simulation
        function checkArticleAccess(articleType) {
            if (articleType === 'free') return true;
            if (articleType === 'member' && userState.membershipType) return true;
            if (articleType === 'premium' && userState.subscriptionLevel) return true;
            return false;
        }

        // Data for articles
        const articles = [
            {
                id: 1,
                title: "Microsurgical Reconstruction in Post-Traumatic Facial Defects",
                author: "Dr. Ahmed Al-Mansoori et al.",
                access: "free",
                category: "Original Article",
                date: "Dec 2023"
            },
            {
                id: 2,
                title: "Modern Burn Care Protocols in Resource-Limited Settings",
                author: "Dr. Fatima Al-Hakimi et al.",
                access: "member",
                category: "Clinical Study",
                date: "Nov 2023"
            },
            {
                id: 3,
                title: "Craniofacial Reconstruction Techniques in Arab Populations",
                author: "Dr. Mohammed Al-Sayed et al.",
                access: "premium",
                category: "Systematic Review",
                date: "Oct 2023"
            }
        ];

        // Subscription plans
        const subscriptionPlans = [
            {
                id: "free",
                name: "Free Reader",
                price: 0,
                features: ["3 articles/month", "Newsletter", "TOC alerts"]
            },
            {
                id: "individual",
                name: "Individual Subscription",
                price: 249,
                features: ["Unlimited articles", "Full archives", "PDF downloads", "Mobile app"]
            },
            {
                id: "membership",
                name: "Full Membership",
                price: 499,
                features: ["All subscription benefits", "Voting rights", "Conference discounts", "CME credits"]
            }
        ];
    </script>
</body>
</html>
