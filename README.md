<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meet With William Levy | Book Your Meeting Fan Experience</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#8a2be2',
                        secondary: '#ff6b6b',
                        accent: '#4ecdc4',
                        dark: '#1a1a2e',
                        light: '#f8f9fa'
                    },
                    animation: {
                        'pulse-slow': 'pulse 3s cubic-bezier(0.4, 0, 0.6, 1) infinite'
                    }
                }
            }
        }
    </script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            color: #f8f9fa;
            overflow-x: hidden;
        }
        
        .card {
            transition: all 0.3s ease;
            transform-style: preserve-3d;
        }
        
        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.3), 0 10px 10px -5px rgba(0, 0, 0, 0.2);
        }
        
        .card.vip {
            border-top: 4px solid #ffd166;
        }
        
        .card.vvip {
            border-top: 4px solid #ff6b6b;
        }
        
        .card.regular {
            border-top: 4px solid #4ecdc4;
        }
        
        .gradient-text {
            background: linear-gradient(90deg, #ff6b6b, #ffd166, #4ecdc4);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .hero-pattern {
            background: radial-gradient(circle, rgba(138,43,226,0.1) 0%, rgba(26,26,46,0) 70%);
        }
        
        .membership-card {
            background: linear-gradient(135deg, rgba(26,26,46,0.8) 0%, rgba(22,33,62,0.9) 100%);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.1);
        }
        
        .price-tag {
            position: absolute;
            top: -15px;
            right: 20px;
            background: linear-gradient(90deg, #ff6b6b, #ffd166);
            padding: 5px 15px;
            border-radius: 20px;
            font-weight: 600;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        
        .feature-list li {
            margin-bottom: 10px;
            display: flex;
            align-items: flex-start;
        }
        
        .feature-list li:before {
            content: "✓";
            color: #4ecdc4;
            font-weight: bold;
            margin-right: 10px;
        }
        
        .testimonials {
            background: rgba(26, 26, 46, 0.5);
            backdrop-filter: blur(5px);
        }
        
        .btn-primary {
            background: linear-gradient(90deg, #8a2be2, #ff6b6b);
            transition: all 0.3s ease;
        }
        
        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(138, 43, 226, 0.3);
        }
        
        .btn-secondary {
            background: linear-gradient(90deg, #4ecdc4, #8a2be2);
            transition: all 0.3s ease;
        }
        
        .btn-secondary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(78, 205, 196, 0.3);
        }
        
        .form-input {
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            color: white;
        }
        
        .form-input:focus {
            outline: none;
            border-color: #8a2be2;
            box-shadow: 0 0 0 3px rgba(138, 43, 226, 0.3);
        }
        
        .form-input::placeholder {
            color: rgba(255, 255, 255, 0.5);
        }
        
        .stars {
            color: #ffd166;
        }
        
        .nav-link {
            position: relative;
            padding: 5px 0;
        }
        
        .nav-link:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background: linear-gradient(90deg, #ff6b6b, #ffd166);
            transition: width 0.3s ease;
        }
        
        .nav-link:hover:after {
            width: 100%;
        }
        
        .floating {
            animation: floating 3s ease-in-out infinite;
        }
        
        @keyframes floating {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
        
        /* Modal styles */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            z-index: 1000;
            overflow-y: auto;
        }
        
        .modal-content {
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            margin: 5% auto;
            padding: 30px;
            border-radius: 15px;
            max-width: 700px;
            width: 90%;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .close-modal {
            position: absolute;
            top: 15px;
            right: 25px;
            font-size: 28px;
            font-weight: bold;
            color: #fff;
            cursor: pointer;
            transition: all 0.3s;
        }
        
        .close-modal:hover {
            color: #ff6b6b;
        }
        
        .payment-option {
            display: flex;
            align-items: center;
            padding: 15px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            margin-bottom: 15px;
            cursor: pointer;
            transition: all 0.3s;
        }
        
        .payment-option:hover {
            border-color: #8a2be2;
            background: rgba(138, 43, 226, 0.1);
        }
        
        .payment-option.selected {
            border-color: #8a2be2;
            background: rgba(138, 43, 226, 0.2);
        }
        
        .payment-icon {
            font-size: 30px;
            margin-right: 15px;
            width: 50px;
            text-align: center;
        }
        
        .payment-logo {
            height: 30px;
            margin-right: 15px;
        }
    </style>
</head>
<body class="min-h-screen">
    <!-- Navigation -->
    <nav class="fixed w-full z-50 bg-dark bg-opacity-90 backdrop-blur-sm py-4 px-6">
        <div class="max-w-7xl mx-auto flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="w-10 h-10 rounded-full bg-gradient-to-r from-primary to-secondary flex items-center justify-center">
                    <i class="fas fa-star text-white"></i>
                </div>
                <span class="text-xl font-bold gradient-text">Star Experience</span>
            </div>
            
            <div class="hidden md:flex space-x-8">
                <a href="#home" class="nav-link">Home</a>
                <a href="#experiences" class="nav-link">Experiences</a>
                <a href="#memberships" class="nav-link">Memberships</a>
                <a href="#testimonials" class="nav-link">Testimonials</a>
                <a href="#contact" class="nav-link">Contact</a>
            </div>
            
            <button class="md:hidden text-white">
                <i class="fas fa-bars text-2xl"></i>
            </button>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="pt-32 pb-20 px-6 hero-pattern">
        <div class="max-w-7xl mx-auto grid md:grid-cols-2 gap-12 items-center">
            <div class="text-center md:text-left">
                <h1 class="text-4xl md:text-6xl font-bold mb-6 leading-tight">
                    Exclusive Fan <span class="gradient-text">Experiences With William Levy</span>
                </h1>
                <p class="text-xl text-gray-300 mb-8 max-w-2xl">
                    Get closer to your favorite star with our exclusive meet and greet packages, VIP access, and fan membership cards.
                </p>
                <div class="flex flex-col sm:flex-row gap-4 justify-center md:justify-start">
                    <a href="#experiences" class="btn-primary py-3 px-8 rounded-full font-semibold text-center">
                        Book Experience
                    </a>
                    <a href="#memberships" class="btn-secondary py-3 px-8 rounded-full font-semibold text-center">
                        View Memberships
                    </a>
                </div>
            </div>
            
            <div class="flex justify-center">
                <div class="relative">
                    <div class="w-64 h-64 md:w-80 md:h-80 rounded-full bg-gradient-to-r from-primary to-secondary opacity-20 absolute -top-6 -left-6"></div>
                    <div class="w-64 h-64 md:w-80 md:h-80 rounded-full bg-gradient-to-r from-secondary to-accent opacity-20 absolute -bottom-6 -right-6"></div>
                    <div class="relative z-10 w-64 h-64 md:w-80 md:h-80 rounded-full overflow-hidden border-4 border-white border-opacity-20 floating">
                        <div class="bg-gray-200 border-2 border-dashed rounded-xl w-full h-full" />
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experiences Section -->
    <section id="experiences" class="py-20 px-6">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Exclusive <span class="gradient-text">Fan Experiences</span></h2>
                <p class="text-gray-400 max-w-2xl mx-auto">
                    Choose from our range of fan experiences to get closer to your favorite star William Levy
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Meet and Greet -->
                <div class="card bg-dark bg-opacity-50 rounded-xl p-6 membership-card">
                    <div class="price-tag">From $750</div>
                    <div class="text-center mb-6">
                        <div class="w-16 h-16 rounded-full bg-gradient-to-r from-primary to-secondary flex items-center justify-center mx-auto mb-4">
                            <i class="fas fa-handshake text-white text-2xl"></i>
                        </div>
                        <h3 class="text-2xl font-bold mb-2">Meet & Greet</h3>
                    </div>
                    <ul class="feature-list text-gray-300 mb-8">
                        <li>15-minute personal meeting</li>
                        <li>Photo opportunity</li>
                        <li>Autograph session</li>
                        <li>Exclusive merchandise</li>
                        <li>Priority seating for 1 event</li>
                    </ul>
                    <button class="w-full py-3 bg-gradient-to-r from-primary to-secondary rounded-lg font-semibold book-now-btn" data-package="Meet & Greet" data-price="750">
                        Book Now
                    </button>
                </div>
                
                <!-- VVIP Meeting -->
                <div class="card bg-dark bg-opacity-50 rounded-xl p-6 membership-card">
                    <div class="price-tag">From $1000</div>
                    <div class="text-center mb-6">
                        <div class="w-16 h-16 rounded-full bg-gradient-to-r from-secondary to-accent flex items-center justify-center mx-auto mb-4">
                            <i class="fas fa-crown text-white text-2xl"></i>
                        </div>
                        <h3 class="text-2xl font-bold mb-2">VVIP Meeting</h3>
                    </div>
                    <ul class="feature-list text-gray-300 mb-8">
                        <li>30-minute exclusive session</li>
                        <li>Private photo shoot</li>
                        <li>Personalized gifts</li>
                        <li>Backstage access</li>
                        <li>VIP seating for all events</li>
                        <li>Complimentary refreshments</li>
                    </ul>
                    <button class="w-full py-3 bg-gradient-to-r from-secondary to-accent rounded-lg font-semibold book-now-btn" data-package="VVIP Meeting" data-price="1000">
                        Book Now
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Memberships Section -->
    <section id="memberships" class="py-20 px-6 bg-dark bg-opacity-30">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Fan <span class="gradient-text">Membership Cards</span></h2>
                <p class="text-gray-400 max-w-2xl mx-auto">
                    Become a member and enjoy exclusive benefits throughout the year
                </p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Regular Fan Card -->
                <div class="card regular rounded-xl p-8 membership-card">
                    <div class="price-tag">$250/year</div>
                    <div class="text-center mb-8">
                        <div class="w-20 h-20 rounded-full bg-gradient-to-r from-accent to-primary flex items-center justify-center mx-auto mb-6">
                            <i class="fas fa-ticket-alt text-white text-3xl"></i>
                        </div>
                        <h3 class="text-2xl font-bold mb-2">Regular Fan</h3>
                        <p class="text-gray-400">Perfect for casual fans</p>
                    </div>
                    <ul class="feature-list text-gray-300 mb-8">
                        <li>Early ticket access</li>
                        <li>10% discount on merchandise</li>
                        <li>Monthly fan content</li>
                        <li>Fan club newsletter</li>
                        <li>Exclusive fan events</li>
                    </ul>
                    <button class="w-full py-3 bg-gradient-to-r from-accent to-primary rounded-lg font-semibold join-now-btn" data-package="Regular Fan Membership" data-price="250">
                        Join Now
                    </button>
                </div>
                
                <!-- VIP Fan Card -->
                <div class="card vip rounded-xl p-8 membership-card transform md:scale-105">
                    <div class="price-tag">$500/year</div>
                    <div class="text-center mb-8">
                        <div class="w-20 h-20 rounded-full bg-gradient-to-r from-yellow-400 to-yellow-600 flex items-center justify-center mx-auto mb-6">
                            <i class="fas fa-star text-white text-3xl"></i>
                        </div>
                        <h3 class="text-2xl font-bold mb-2">VIP Fan</h3>
                        <p class="text-gray-400">For devoted fans</p>
                    </div>
                    <ul class="feature-list text-gray-300 mb-8">
                        <li>All Regular benefits</li>
                        <li>Priority ticket access</li>
                        <li>20% discount on merchandise</li>
                        <li>Exclusive meet & greets (2/year)</li>
                        <li>VIP seating at events</li>
                        <li>Behind-the-scenes content</li>
                        <li>Personalized birthday messages</li>
                    </ul>
                    <button class="w-full py-3 bg-gradient-to-r from-yellow-400 to-yellow-600 rounded-lg font-semibold join-now-btn" data-package="VIP Fan Membership" data-price="500">
                        Join Now
                    </button>
                </div>
                
                <!-- VVIP Fan Card -->
                <div class="card vvip rounded-xl p-8 membership-card">
                    <div class="price-tag">$1000/year</div>
                    <div class="text-center mb-8">
                        <div class="w-20 h-20 rounded-full bg-gradient-to-r from-red-500 to-pink-500 flex items-center justify-center mx-auto mb-6">
                            <i class="fas fa-crown text-white text-3xl"></i>
                        </div>
                        <h3 class="text-2xl font-bold mb-2">VVIP Fan</h3>
                        <p class="text-gray-400">Ultimate fan experience</p>
                    </div>
                    <ul class="feature-list text-gray-300 mb-8">
                        <li>All VIP benefits</li>
                        <li>First access to tickets</li>
                        <li>30% discount on merchandise</li>
                        <li>Exclusive meet & greets (4/year)</li>
                        <li>Backstage passes</li>
                        <li>Personal video messages</li>
                        <li>Annual exclusive dinner</li>
                        <li>Personalized gifts</li>
                    </ul>
                    <button class="w-full py-3 bg-gradient-to-r from-red-500 to-pink-500 rounded-lg font-semibold join-now-btn" data-package="VVIP Fan Membership" data-price="1000">
                        Join Now
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section id="testimonials" class="py-20 px-6">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Fan <span class="gradient-text">Experiences</span></h2>
                <p class="text-gray-400 max-w-2xl mx-auto">
                    Hear from fans who have experienced our exclusive packages
                </p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="testimonials rounded-xl p-6">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-200 border-2 border-dashed"></div>
                        <div class="ml-4">
                            <h4 class="font-bold">Sarah Johnson</h4>
                            <div class="flex stars">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-300 italic">
                        "The VVIP meeting was absolutely incredible! I got to spend 30 minutes with my favorite star and even got backstage access. Worth every penny!"
                    </p>
                </div>
                
                <div class="testimonials rounded-xl p-6">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-200 border-2 border-dashed"></div>
                        <div class="ml-4">
                            <h4 class="font-bold">Michael Chen</h4>
                            <div class="flex stars">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-300 italic">
                        "As a VIP member for two years, I've had access to exclusive content and events that regular fans can only dream of. Highly recommend!"
                    </p>
                </div>
                
                <div class="testimonials rounded-xl p-6">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-200 border-2 border-dashed"></div>
                        <div class="ml-4">
                            <h4 class="font-bold">Emma Rodriguez</h4>
                            <div class="flex stars">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star-half-alt"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-300 italic">
                        "The meet and greet package was perfect for my birthday gift. The photo session was amazing and the autograph is now framed in my room!"
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 px-6 bg-dark bg-opacity-50">
        <div class="max-w-4xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Get <span class="gradient-text">In Touch</span></h2>
                <p class="text-gray-400 max-w-2xl mx-auto">
                    Have questions about booking experiences or memberships? Reach out to us!
                </p>
            </div>
            
            <div class="bg-dark rounded-2xl p-8 md:p-12">
                <form class="space-y-6">
                    <div class="grid md:grid-cols-2 gap-6">
                        <div>
                            <label class="block text-gray-300 mb-2">Full Name</label>
                            <input type="text" class="w-full form-input py-3 px-4 rounded-lg">
                        </div>
                        <div>
                            <label class="block text-gray-300 mb-2">Email Address</label>
                            <input type="email" class="w-full form-input py-3 px-4 rounded-lg">
                        </div>
                    </div>
                    
                    <div>
                        <label class="block text-gray-300 mb-2">Subject</label>
                        <input type="text" class="w-full form-input py-3 px-4 rounded-lg">
                    </div>
                    
                    <div>
                        <label class="block text-gray-300 mb-2">Your Message</label>
                        <textarea rows="5" class="w-full form-input py-3 px-4 rounded-lg"></textarea>
                    </div>
                    
                    <button type="submit" class="w-full py-4 bg-gradient-to-r from-primary to-secondary rounded-lg font-semibold text-lg">
                        Send Message
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-12 px-6 border-t border-gray-800">
        <div class="max-w-7xl mx-auto">
            <div class="grid md:grid-cols-4 gap-8">
                <div>
                    <div class="flex items-center space-x-2 mb-6">
                        <div class="w-10 h-10 rounded-full bg-gradient-to-r from-primary to-secondary flex items-center justify-center">
                            <i class="fas fa-star text-white"></i>
                        </div>
                        <span class="text-xl font-bold gradient-text">Star Experience</span>
                    </div>
                    <p class="text-gray-400 mb-6">
                        Connecting fans with their favorite stars through exclusive experiences and memberships.
                    </p>
                    <div class="flex space-x-4">
                        <a href="#" class="w-10 h-10 rounded-full bg-dark flex items-center justify-center hover:bg-primary transition">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-dark flex items-center justify-center hover:bg-primary transition">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-dark flex items-center justify-center hover:bg-primary transition">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-dark flex items-center justify-center hover:bg-primary transition">
                            <i class="fab fa-tiktok"></i>
                        </a>
                    </div>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-6">Quick Links</h4>
                    <ul class="space-y-3">
                        <li><a href="#home" class="text-gray-400 hover:text-white transition">Home</a></li>
                        <li><a href="#experiences" class="text-gray-400 hover:text-white transition">Experiences</a></li>
                        <li><a href="#memberships" class="text-gray-400 hover:text-white transition">Memberships</a></li>
                        <li><a href="#testimonials" class="text-gray-400 hover:text-white transition">Testimonials</a></li>
                        <li><a href="#contact" class="text-gray-400 hover:text-white transition">Contact</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-6">Experiences</h4>
                    <ul class="space-y-3">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Meet & Greet</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">VVIP Meeting</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Backstage Access</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Private Concert</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Video Call Session</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-6">Newsletter</h4>
                    <p class="text-gray-400 mb-4">
                        Subscribe to get special offers and updates
                    </p>
                    <div class="flex">
                        <input type="email" placeholder="Your email" class="form-input py-3 px-4 rounded-l-lg flex-grow">
                        <button class="bg-gradient-to-r from-primary to-secondary py-3 px-6 rounded-r-lg font-semibold">
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </div>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 text-center text-gray-500">
                <p>&copy; 2023 Star Experience. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Floating Action Button -->
    <div class="fixed bottom-8 right-8 z-50">
        <button class="w-14 h-14 rounded-full bg-gradient-to-r from-primary to-secondary flex items-center justify-center shadow-lg hover:from-secondary hover:to-primary transition">
            <i class="fas fa-comments text-white text-xl"></i>
        </button>
    </div>

    <!-- Booking Modal -->
    <div id="bookingModal" class="modal">
        <div class="modal-content relative">
            <span class="close-modal">&times;</span>
            <h2 class="text-2xl md:text-3xl font-bold mb-6 text-center gradient-text" id="modalTitle">Book Your Experience</h2>
            
            <form id="bookingForm" class="space-y-6">
                <input type="hidden" id="packageType">
                <input type="hidden" id="packagePrice">
                
                <div class="grid md:grid-cols-2 gap-6">
                    <div>
                        <label class="block text-gray-300 mb-2">First Name <span class="text-red-500">*</span></label>
                        <input type="text" id="firstName" class="w-full form-input py-3 px-4 rounded-lg" required>
                    </div>
                    <div>
                        <label class="block text-gray-300 mb-2">Last Name <span class="text-red-500">*</span></label>
                        <input type="text" id="lastName" class="w-full form-input py-3 px-4 rounded-lg" required>
                    </div>
                </div>
                
                <div class="grid md:grid-cols-2 gap-6">
                    <div>
                        <label class="block text-gray-300 mb-2">Email Address <span class="text-red-500">*</span></label>
                        <input type="email" id="email" class="w-full form-input py-3 px-4 rounded-lg" required>
                    </div>
                    <div>
                        <label class="block text-gray-300 mb-2">Phone Number <span class="text-red-500">*</span></label>
                        <input type="tel" id="phone" class="w-full form-input py-3 px-4 rounded-lg" required>
                    </div>
                </div>
                
                <div>
                    <label class="block text-gray-300 mb-2">Street Address <span class="text-red-500">*</span></label>
                    <input type="text" id="street" class="w-full form-input py-3 px-4 rounded-lg" required>
                </div>
                
                <div class="grid md:grid-cols-3 gap-6">
                    <div>
                        <label class="block text-gray-300 mb-2">House/Apartment Number <span class="text-red-500">*</span></label>
                        <input type="text" id="houseNumber" class="w-full form-input py-3 px-4 rounded-lg" required>
                    </div>
                    <div>
                        <label class="block text-gray-300 mb-2">City <span class="text-red-500">*</span></label>
                        <input type="text" id="city" class="w-full form-input py-3 px-4 rounded-lg" required>
                    </div>
                    <div>
                        <label class="block text-gray-300 mb-2">Zip/Postal Code <span class="text-red-500">*</span></label>
                        <input type="text" id="zipCode" class="w-full form-input py-3 px-4 rounded-lg" required>
                    </div>
                </div>
                
                <div class="grid md:grid-cols-2 gap-6">
                    <div>
                        <label class="block text-gray-300 mb-2">Country <span class="text-red-500">*</span></label>
                        <select id="country" class="w-full form-input py-3 px-4 rounded-lg" required>
                            <option value="">Select Country</option>
                            <option value="US">United States</option>
                            <option value="UK">United Kingdom</option>
                            <option value="CA">Canada</option>
                            <option value="AU">Australia</option>
                            <option value="DE">Germany</option>
                            <option value="FR">France</option>
                            <option value="JP">Japan</option>
                            <option value="BR">Brazil</option>
                            <option value="IN">India</option>
                            <option value="MX">Mexico</option>
                            <option value="other">Other</option>
                        </select>
                    </div>
                    <div id="otherCountryContainer" class="hidden">
                        <label class="block text-gray-300 mb-2">Other Country <span class="text-red-500">*</span></label>
                        <input type="text" id="otherCountry" class="w-full form-input py-3 px-4 rounded-lg">
                    </div>
                </div>
                
                <div class="border-t border-gray-700 pt-6">
                    <h3 class="text-xl font-bold mb-4">Payment Information</h3>
                    <div class="space-y-4">
                        <div class="payment-option" data-payment="credit">
                            <div class="payment-icon">
                                <i class="far fa-credit-card"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">Credit/Debit Card</h4>
                                <p class="text-sm text-gray-400">Pay with Visa, Mastercard, or American Express</p>
                            </div>
                        </div>
                        
                        <div class="payment-option" data-payment="paypal">
                            <div class="payment-icon">
                                <i class="fab fa-paypal"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">PayPal</h4>
                                <p class="text-sm text-gray-400">Pay with your PayPal account</p>
                            </div>
                        </div>
                        
                        <div class="payment-option" data-payment="bank">
                            <div class="payment-icon">
                                <i class="fas fa-university"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">Bank Transfer</h4>
                                <p class="text-sm text-gray-400">Direct bank transfer</p>
                            </div>
                        </div>
                    </div>
                    
                    <div id="creditCardForm" class="hidden mt-6 space-y-4">
                        <div class="grid md:grid-cols-2 gap-4">
                            <div>
                                <label class="block text-gray-300 mb-2">Card Number <span class="text-red-500">*</span></label>
                                <input type="text" class="w-full form-input py-3 px-4 rounded-lg" placeholder="1234 5678 9012 3456">
                            </div>
                            <div>
                                <label class="block text-gray-300 mb-2">Card Holder Name <span class="text-red-500">*</span></label>
                                <input type="text" class="w-full form-input py-3 px-4 rounded-lg" placeholder="John Doe">
                            </div>
                        </div>
                        
                        <div class="grid md:grid-cols-3 gap-4">
                            <div>
                                <label class="block text-gray-300 mb-2">Expiry Date <span class="text-red-500">*</span></label>
                                <input type="text" class="w-full form-input py-3 px-4 rounded-lg" placeholder="MM/YY">
                            </div>
                            <div>
                                <label class="block text-gray-300 mb-2">CVV <span class="text-red-500">*</span></label>
                                <input type="text" class="w-full form-input py-3 px-4 rounded-lg" placeholder="123">
                            </div>
                        </div>
                    </div>
                    
                    <div id="bankTransferInfo" class="hidden mt-6 bg-dark p-4 rounded-lg">
                        <h4 class="font-bold mb-2">Bank Transfer Instructions</h4>
                        <p class="text-gray-400 text-sm mb-2">Please transfer the amount to the following account:</p>
                        <div class="space-y-2">
                            <p class="text-gray-300"><span class="font-medium">Bank Name:</span> International Star Bank</p>
                            <p class="text-gray-300"><span class="font-medium">Account Name:</span> Star Experience LLC</p>
                            <p class="text-gray-300"><span class="font-medium">Account Number:</span> 123456789</p>
                            <p class="text-gray-300"><span class="font-medium">IBAN:</span> US33 1234 5678 9012 3456 7890</p>
                            <p class="text-gray-300"><span class="font-medium">SWIFT/BIC:</span> INTLUS33</p>
                        </div>
                        <p class="text-gray-400 text-sm mt-4">Please include your full name as reference.</p>
                    </div>
                </div>
                
                <div class="border-t border-gray-700 pt-6">
                    <div class="flex justify-between items-center mb-4">
                        <span class="text-gray-300">Package:</span>
                        <span class="font-bold" id="summaryPackage">Meet & Greet</span>
                    </div>
                    <div class="flex justify-between items-center mb-4">
                        <span class="text-gray-300">Price:</span>
                        <span class="font-bold" id="summaryPrice">$750</span>
                    </div>
                    <div class="flex justify-between items-center text-lg font-bold">
                        <span>Total:</span>
                        <span id="summaryTotal">$750</span>
                    </div>
                </div>
                
                <div class="pt-6">
                    <div class="flex items-start mb-4">
                        <input type="checkbox" id="terms" class="mt-1 mr-2" required>
                        <label for="terms" class="text-gray-300 text-sm">I agree to the <a href="#" class="text-primary hover:underline">Terms & Conditions</a> and <a href="#" class="text-primary hover:underline">Privacy Policy</a></label>
                    </div>
                    
                    <button type="submit" class="w-full py-4 bg-gradient-to-r from-primary to-secondary rounded-lg font-semibold text-lg">
                        Complete Booking
                    </button>
                </div>
            </form>
        </div>
    </div>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Simple form submission handling
        const forms = document.querySelectorAll('form');
        forms.forEach(form => {
            form.addEventListener('submit', function(e) {
                e.preventDefault();
                alert('Thank you for your message! We will get back to you soon.');
                form.reset();
            });
        });

        // Card hover effects
        const cards = document.querySelectorAll('.card');
        cards.forEach(card => {
            card.addEventListener('mouseenter', () => {
                card.style.transform = 'translateY(-10px)';
            });
            card.addEventListener('mouseleave', () => {
                card.style.transform = 'translateY(0)';
            });
        });

        // Modal functionality
        const modal = document.getElementById("bookingModal");
        const bookNowBtns = document.querySelectorAll(".book-now-btn, .join-now-btn");
        const closeModal = document.querySelector(".close-modal");
        const bookingForm = document.getElementById("bookingForm");
        const packageTypeInput = document.getElementById("packageType");
        const packagePriceInput = document.getElementById("packagePrice");
        const modalTitle = document.getElementById("modalTitle");
        const summaryPackage = document.getElementById("summaryPackage");
        const summaryPrice = document.getElementById("summaryPrice");
        const summaryTotal = document.getElementById("summaryTotal");
        const countrySelect = document.getElementById("country");
        const otherCountryContainer = document.getElementById("otherCountryContainer");
        const otherCountryInput = document.getElementById("otherCountry");
        const paymentOptions = document.querySelectorAll(".payment-option");
        const creditCardForm = document.getElementById("creditCardForm");
        const bankTransferInfo = document.getElementById("bankTransferInfo");

        // Open modal when Book Now/Join Now is clicked
        bookNowBtns.forEach(btn => {
            btn.addEventListener("click", function() {
                const package = this.getAttribute("data-package");
                const price = this.getAttribute("data-price");
                
                packageTypeInput.value = package;
                packagePriceInput.value = price;
                
                modalTitle.textContent = package.includes("Membership") ? "Join Membership" : "Book Your Experience";
                summaryPackage.textContent = package;
                summaryPrice.textContent = `$${price}`;
                summaryTotal.textContent = `$${price}`;
                
                modal.style.display = "block";
                document.body.style.overflow = "hidden";
            });
        });

        // Close modal
        closeModal.addEventListener("click", function() {
            modal.style.display = "none";
            document.body.style.overflow = "auto";
        });

        // Close modal when clicking outside
        window.addEventListener("click", function(event) {
            if (event.target === modal) {
                modal.style.display = "none";
                document.body.style.overflow = "auto";
            }
        });

        // Handle country selection
        countrySelect.addEventListener("change", function() {
            if (this.value === "other") {
                otherCountryContainer.classList.remove("hidden");
                otherCountryInput.required = true;
            } else {
                otherCountryContainer.classList.add("hidden");
                otherCountryInput.required = false;
            }
        });

        // Handle payment option selection
        paymentOptions.forEach(option => {
            option.addEventListener("click", function() {
                // Remove selected class from all options
                paymentOptions.forEach(opt => {
                    opt.classList.remove("selected");
                });
                
                // Add selected class to clicked option
                this.classList.add("selected");
                
                // Show relevant payment form
                const paymentType = this.getAttribute("data-payment");
                
                creditCardForm.classList.add("hidden");
                bankTransferInfo.classList.add("hidden");
                
                if (paymentType === "credit") {
                    creditCardForm.classList.remove("hidden");
                } else if (paymentType === "bank") {
                    bankTransferInfo.classList.remove("hidden");
                }
            });
        });

        // Handle booking form submission
        bookingForm.addEventListener("submit", function(e) {
            e.preventDefault();
            
            // Validate payment method is selected
            const selectedPayment = document.querySelector(".payment-option.selected");
            if (!selectedPayment) {
                alert("Please select a payment method");
                return;
            }
            
            // Validate credit card form if selected
            if (selectedPayment.getAttribute("data-payment") === "credit") {
                const cardInputs = creditCardForm.querySelectorAll("input[required]");
                let valid = true;
                
                cardInputs.forEach(input => {
                    if (!input.value.trim()) {
                        valid = false;
                    }
                });
                
                if (!valid) {
                    alert("Please fill in all required credit card details");
                    return;
                }
            }
            
            // Here you would typically send the form data to your server
            // For this demo, we'll just show a success message
            alert(`Thank you for your booking! Your ${packageTypeInput.value} has been confirmed.`);
            
            // Reset form and close modal
            this.reset();
            modal.style.display = "none";
            document.body.style.overflow = "auto";
            
            // Reset payment options
            paymentOptions.forEach(opt => {
                opt.classList.remove("selected");
            });
            creditCardForm.classList.add("hidden");
            bankTransferInfo.classList.add("hidden");
        });
    </script>
</body>
</html>
