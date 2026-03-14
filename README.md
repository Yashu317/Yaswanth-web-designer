# Yaswanth-web-designer
good services
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="utf-8">
    <meta content="width=device-width, initial-scale=1, shrink-to-fit=no" name="viewport">
    <title>Yaswanth - Web Designer</title>

    <link href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.6.0/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/sweetalert2@11/dist/sweetalert2.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap" rel="stylesheet">

    <style>
        /* --- GLOBAL DESIGN --- */
        html {
            overflow-x: hidden;
            max-width: 100%;
        }
        
        body { 
            background-color: #c20975;
            background-image: radial-gradient(#2fb95d 1px, transparent 1px);
            background-size: 20px 20px;
            font-family: 'Poppins', sans-serif; 
            overflow-x: hidden; 
            max-width: 100%;
            margin: 0;
            padding: 0;
            color: #c0960d;
        }

        /* --- UTILITY --- */
        .view-section { display: none; } 
        .view-section.active { display: block; animation: fadeIn 0.5s; } 
        @keyframes fadeIn { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }

        /* --- HEADER --- */
        .main-header { 
            background: rgba(6, 173, 42, 0.95); 
            backdrop-filter: blur(10px);
            box-shadow: 0 4px 20px rgba(0,0,0,0.05); 
            padding: 15px 0; 
            position: sticky; 
            top: 0; 
            z-index: 1000; 
        }
        .nav-link { font-weight: 600; color: #555 !important; margin-left: 15px; cursor: pointer; transition: 0.3s; }
        .nav-link:hover { color: #4e54c8 !important; }
        
        /* Button Styles */
        .thm-btn { 
            background: linear-gradient(45deg, #ffc107, #ff9800); 
            color: #fff !important; 
            padding: 10px 25px; 
            border-radius: 30px; 
            font-weight: 600; 
            text-decoration: none; 
            border: none; 
            cursor: pointer; 
            transition: 0.3s; 
            display: inline-block; 
            box-shadow: 0 5px 15px rgba(255, 152, 0, 0.3);
        }
        .thm-btn:hover { transform: translateY(-3px); box-shadow: 0 8px 20px rgba(255, 152, 0, 0.4); text-decoration: none; }

        .thm-btn-outline {
            background: transparent;
            color: #ff9800 !important;
            border: 2px solid #ff9800;
            padding: 8px 25px;
            border-radius: 30px;
            font-weight: 600;
            cursor: pointer;
            transition: 0.3s;
            display: inline-block;
        }
        .thm-btn-outline:hover { background: #ff9800; color: #fff !important; transform: translateY(-3px); }

        /* Mobile Nav & Super Look Styles (Optimized for Phone) */
        @media (max-width: 767px) {
            .mobile-active {
                display: flex !important;
                flex-direction: column;
                position: absolute;
                top: 75px;
                left: 10px;
                right: 10px;
                background: rgba(255, 255, 255, 0.98);
                padding: 20px;
                box-shadow: 0 10px 30px rgba(0,0,0,0.2);
                border-radius: 20px;
                text-align: center;
                z-index: 1000;
            }
            .mobile-active .nav-link { margin-left: 0; margin-bottom: 15px; font-size: 1.1rem; color: #333 !important; }
            .mobile-active .thm-btn, .mobile-active .thm-btn-outline { margin: 10px auto !important; width: 80%; display: block; }
            
            /* Mobile Enhancements */
            .hero-content { text-align: center; }
            .hero-content h1 { font-size: 2.2rem !important; margin-top: 10px; }
            .hero-profile-img { width: 220px !important; height: 220px !important; margin-top: 30px; border-width: 4px !important; }
            .hero-section { min-height: auto !important; padding: 40px 15px !important; border-bottom-left-radius: 30px !important; border-bottom-right-radius: 30px !important; }
            .login-box { padding: 30px 20px !important; margin: 30px 15px !important; max-width: 100%; }
            .section-title h2 { font-size: 26px !important; }
            .sidebar { width: 100% !important; margin-bottom: 20px; }
            .main-content { padding-left: 0 !important; }
            .course-progress-box { padding: 20px !important; text-align: center; }
            .course-progress-box .text-right { text-align: center !important; margin-top: 15px; }
            .section-padding { padding: 50px 0 !important; }
        }

        /* --- HERO SECTION --- */
        .hero-section {
            background: linear-gradient(135deg, #4e54c8 0%, #8f94fb 100%);
            height: auto;
            min-height: 580px;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
            padding: 50px 0;
            border-bottom-left-radius: 50px;
            border-bottom-right-radius: 50px;
            box-shadow: 0 10px 30px rgba(78, 84, 200, 0.2);
        }
        .hero-overlay {
            position: absolute;
            top: 0; left: 0; right: 0; bottom: 0;
            background: url('https://www.transparenttextures.com/patterns/cubes.png');
            opacity: 0.2;
        }
        .hero-content h1 { color: #fff; font-weight: 800; font-size: 3.5rem; text-shadow: 0 5px 15px rgba(0,0,0,0.2); line-height: 1.2; }
        .hero-content p { color: rgba(255,255,255,0.9); font-size: 1.2rem; margin-bottom: 30px; margin-top: 15px; }
        .hero-image-wrapper { text-align: center; }
        .hero-profile-img { width: 320px; height: 320px; object-fit: cover; border-radius: 50%; border: 6px solid rgba(255,255,255,0.3); box-shadow: 0 15px 40px rgba(0,0,0,0.2); transition: transform 0.3s; }
        .hero-profile-img:hover { transform: scale(1.05); }

        /* --- SECTIONS --- */
        .section-padding { padding: 80px 0; background-color: rgba(244, 247, 246, 0.8); }
        .bg-white-box { background-color: #ffffff !important; border-radius: 30px; margin: 20px; box-shadow: 0 10px 40px rgba(0,0,0,0.03); }
        .section-title { text-align: center; margin-bottom: 50px; }
        .section-title span { color: #4e54c8; text-transform: uppercase; letter-spacing: 2px; font-weight: 700; font-size: 14px; display: block; margin-bottom: 5px; }
        .section-title h2 { font-weight: 800; font-size: 36px; color: #1a1a1a; }
        .courses-one__single { background: #fff; border-radius: 20px; box-shadow: 0 15px 40px rgba(0,0,0,0.08); margin-bottom: 30px; overflow: hidden; transition: all 0.4s ease; border: 1px solid #f0f0f0; }
        .courses-one__single:hover { transform: translateY(-10px); box-shadow: 0 20px 50px rgba(0,0,0,0.12); }
        .courses-one__img img { width: 100%; height: 220px; object-fit: cover; }
        .courses-one__content { padding: 25px; }
        
        /* Tool Box */
        .tool-box { background: #fff; padding: 30px; border-radius: 15px; box-shadow: 0 5px 20px rgba(0,0,0,0.05); transition: 0.3s; border: 1px solid #eee; text-align: center; height: 100%; }
        .tool-box:hover { transform: translateY(-5px); border-color: #4e54c8; box-shadow: 0 15px 30px rgba(78, 84, 200, 0.1); }
        .tool-icon-wrapper { width: 70px; height: 70px; background: #f0f2f5; border-radius: 50%; display: flex; align-items: center; justify-content: center; margin: 0 auto 20px; font-size: 30px; color: #4e54c8; transition: 0.3s; }
        .tool-box:hover .tool-icon-wrapper { background: #4e54c8; color: #fff; }
        .earning-potential { font-weight: 700; color: #28a745; margin-top: 10px; display: block; }
        
        /* --- DASHBOARD STYLES --- */
        .dashboard-container { display: flex; min-height: 100vh; margin-top: 30px; margin-bottom: 30px; flex-wrap: wrap; }
        .sidebar { width: 260px; background: #fff; border-radius: 15px; box-shadow: 0 10px 30px rgba(0,0,0,0.05); overflow: hidden; height: fit-content; }
        .sidebar a { display: block; color: #555; padding: 18px 25px; text-decoration: none; border-left: 4px solid transparent; font-weight: 500; transition: 0.2s; }
        .sidebar a:hover, .sidebar a.active { background: #f4f7f6; color: #4e54c8; border-left: 4px solid #4e54c8; font-weight: 700; }
        .main-content { flex: 1; padding-left: 30px; }
        .dash-card { background: #fff; padding: 25px; border-radius: 15px; box-shadow: 0 5px 20px rgba(0,0,0,0.05); margin-bottom: 25px; border: 1px solid #f0f0f0; }
        
        /* Progress Bar */
        .course-progress-box { padding: 30px; background: linear-gradient(135deg, #4e54c8 0%, #8f94fb 100%); color: #fff; border-radius: 15px; margin-bottom: 30px; box-shadow: 0 10px 20px rgba(78, 84, 200, 0.2); }
        .progress { height: 10px; border-radius: 10px; background: rgba(255,255,255,0.3); }
        .progress-bar { background: #ffc107; }

        /* --- LOGIN & REGISTER BOX --- */
        .login-box { 
            max-width: 450px; 
            margin: 60px auto; 
            background: rgba(255, 255, 255, 0.95); 
            backdrop-filter: blur(10px);
            padding: 40px 40px; 
            border-radius: 20px; 
            box-shadow: 0 20px 60px rgba(0,0,0,0.2); 
            text-align: center; 
            border: 1px solid rgba(255,255,255,0.5);
        }
        .form-control { height: 50px; border-radius: 10px; margin-bottom: 20px; border: 1px solid #e0e0e0; background: #fdfdfd; padding-left: 20px; transition: 0.3s; }
        .form-control:focus { border-color: #4e54c8; box-shadow: 0 0 10px rgba(78, 84, 200, 0.1); }
        
        /* Login Tabs */
        .login-tabs { display: flex; margin-bottom: 30px; background: #f0f2f5; border-radius: 30px; padding: 5px; }
        .login-tab { flex: 1; padding: 10px; border-radius: 30px; font-weight: 600; cursor: pointer; transition: 0.3s; color: #555; }
        .login-tab.active { background: #4e54c8; color: #fff; box-shadow: 0 5px 15px rgba(78,84,200,0.3); }

        /* Footer */
        .site-footer { background: #0f1016; color: #fff; padding: 80px 0 30px; border-top-left-radius: 50px; border-top-right-radius: 50px; margin-top: 40px; }
        .footer-links a { color: #888; display: block; margin-bottom: 10px; transition: 0.3s; }
        .footer-links a:hover { color: #ffc107; padding-left: 5px; text-decoration: none; }
        .copyright { border-top: 1px solid #222; padding-top: 30px; margin-top: 50px; text-align: center; color: #666; font-size: 14px; }
        
        .admin-sidebar { background: #2c3e50; }
        .admin-sidebar a { color: #bdc3c7; }
        .admin-sidebar a:hover, .admin-sidebar a.active { background: #34495e; color: #fff; border-color: #e74c3c; }
        
        /* Status Badge */
        .status-badge { padding: 6px 12px; border-radius: 30px; font-size: 11px; text-transform: uppercase; font-weight: 700; }
        .bg-pending { background: #fff8e1; color: #f39c12; }
        .bg-success { background: #e8f5e9; color: #27ae60; }
    </style>
</head>

<body>

    <header class="main-header">
        <div class="container">
            <div class="d-flex justify-content-between align-items-center">
                <a class="navbar-brand d-flex align-items-center" href="#" onclick="showLanding()">
                    <img alt="Yaswanth" height="50" style="border-radius: 50%; object-fit: cover; width: 50px; margin-right: 10px; border: 2px solid #4e54c8;" onerror="this.style.display='none'; document.getElementById('logo-txt').style.display='block';" src="IMG-20240928-WA0042.jpg" />
                    <span id="logo-txt" style="color: black; font-weight: 800; font-size: 24px;">Yaswanth</span>
                </a>
                <div id="publicNav" class="d-none d-md-block">
                    <a class="nav-link d-inline-block" onclick="showLanding()">Home</a>
                    <a class="nav-link d-inline-block" onclick="navTo('#tools')">My Skills</a>
                    <a class="nav-link d-inline-block" onclick="navTo('#why-me')">My Process</a>
                    <a class="nav-link d-inline-block" onclick="navTo('#courses')">Services</a>
                    <a class="thm-btn ml-3" onclick="showLogin()"><i class="fas fa-sign-in-alt"></i> Login</a>
                    <a class="thm-btn-outline ml-2" onclick="showRegister()"><i class="fas fa-user-plus"></i> Register</a>
                </div>
                <button class="btn d-md-none" style="color: #333;" onclick="toggleMobileMenu()"><i class="fas fa-bars fa-2x"></i></button>

                <div id="authNav" style="display: none;">
                    <span class="font-weight-bold mr-3" id="welcomeName" style="color: #333;">User</span>
                    <button class="btn btn-sm btn-outline-danger rounded-pill px-3" onclick="logout()">Logout</button>
                </div>
            </div>
        </div>
    </header>

    <div class="view-section active" id="view-landing">
        <section class="hero-section">
            <div class="hero-overlay"></div>
            <div class="container position-relative">
                <div class="row align-items-center">
                    <div class="col-lg-7 hero-content">
                        <span style="color: #ffc107; font-weight: 700; letter-spacing: 2px;"><i class="fas fa-code"></i> WEB DEVELOPER & DESIGNER</span>
                        <h1>Hi, I'm Yaswanth.<br>Let's Build the Web.</h1>
                        <p>With a B.Tech background in Mechanical Engineering, I bring strong problem-solving skills to digital spaces. I specialize in front-end and back-end web development, crafting clean code using HTML, CSS, and Java.</p>
                        <a class="thm-btn mt-3" onclick="navTo('#tools')">Explore My Work</a>
                        <a class="thm-btn-outline mt-3 ml-2 text-white border-white" onclick="navTo('#contact')" style="color: #fff !important; border-color: #fff;">Hire Me</a>
                    </div>
                    <div class="col-lg-5 text-center mt-5 mt-lg-0 hero-image-wrapper">
                        <div class="separator" style="clear: both;">
                            <a href="#" style="display: block; text-align: center;">
                                <img alt="Yaswanth" class="hero-profile-img" src="IMG-20240928-WA0042.jpg" onerror="this.src='https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhSIqKHeTaJKoRKT9Q_qjPx392w8-N9t33H6kadCxsvEi_MNMulYSKBKwmK-aatcb3FgR0l-ADoEBA1uMZGS-QEJn8NbqfohtQs_-r5-nzz6ojOqih2yrcCDiu1k6E4kNkI867IKjmit3equRMO3OufZm2JbPO_6rqv9TGHwxbqscrOOCY72iXggsJSigOD/s200/WhatsApp%20Image%202026-03-13%20at%2011.18.51%20AM.jpeg';"/>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section class="section-padding bg-white-box" id="tools">
            <div class="container">
                <div class="section-title">
                    <span>What I Do</span>
                    <h2>My Core <span>Technical Skills</span></h2>
                </div>
                <div class="row">
                    <div class="col-md-3 mb-4">
                        <div class="tool-box">
                            <div class="tool-icon-wrapper"><i class="fab fa-html5"></i></div>
                            <h5>HTML & CSS</h5>
                            <p class="text-muted small">Building structured, semantic, and modern web pages from scratch.</p>
                            <span class="earning-potential text-primary">Front-End Dev</span>
                        </div>
                    </div>
                    <div class="col-md-3 mb-4">
                        <div class="tool-box">
                            <div class="tool-icon-wrapper"><i class="fab fa-java"></i></div>
                            <h5>Java</h5>
                            <p class="text-muted small">Creating robust logic, secure applications, and functional backends.</p>
                            <span class="earning-potential text-primary">Back-End Dev</span>
                        </div>
                    </div>
                    <div class="col-md-3 mb-4">
                        <div class="tool-box">
                            <div class="tool-icon-wrapper"><i class="fas fa-mobile-alt"></i></div>
                            <h5>Responsive Design</h5>
                            <p class="text-muted small">Ensuring layouts look perfect on phones, tablets, and desktop screens.</p>
                            <span class="earning-potential text-primary">UI/UX Focus</span>
                        </div>
                    </div>
                    <div class="col-md-3 mb-4">
                        <div class="tool-box">
                            <div class="tool-icon-wrapper"><i class="fas fa-cogs"></i></div>
                            <h5>Problem Solving</h5>
                            <p class="text-muted small">Applying my engineering background to solve complex logic challenges.</p>
                            <span class="earning-potential text-primary">Engineering Mindset</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section class="section-padding" id="why-me">
            <div class="container">
                <div class="section-title">
                    <span style="color: #fff;">Why Choose Me</span>
                    <h2 style="color: #fff;">My <span>Working Process</span></h2>
                </div>
                <div class="row text-center">
                    <div class="col-md-4 mb-4">
                        <div class="p-4 bg-white rounded shadow-sm h-100" style="border-top: 4px solid #ffc107;">
                            <i class="fas fa-search fa-3x text-warning mb-3 mt-2"></i>
                            <h4 class="font-weight-bold" style="color: #333;">1. Research & Plan</h4>
                            <p class="text-muted small">Understanding your requirements, target audience, and business goals deeply before writing a single line of code.</p>
                        </div>
                    </div>
                    <div class="col-md-4 mb-4">
                        <div class="p-4 bg-white rounded shadow-sm h-100" style="border-top: 4px solid #4e54c8;">
                            <i class="fas fa-laptop-code fa-3x text-primary mb-3 mt-2"></i>
                            <h4 class="font-weight-bold" style="color: #333;">2. Design & Develop</h4>
                            <p class="text-muted small">Crafting intuitive UI/UX and building robust, scalable web applications using the latest web technologies.</p>
                        </div>
                    </div>
                    <div class="col-md-4 mb-4">
                        <div class="p-4 bg-white rounded shadow-sm h-100" style="border-top: 4px solid #28a745;">
                            <i class="fas fa-rocket fa-3x text-success mb-3 mt-2"></i>
                            <h4 class="font-weight-bold" style="color: #333;">3. Testing & Launch</h4>
                            <p class="text-muted small">Rigorous testing across devices to ensure zero bugs, followed by a smooth and successful project deployment.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section class="section-padding bg-white-box" id="courses">
            <div class="container">
                <div class="section-title">
                    <span>Portfolio</span>
                    <h2>Featured <span>Services</span></h2>
                </div>
                <div class="row justify-content-center">
                    <div class="col-md-5">
                        <div class="courses-one__single">
                            <div class="courses-one__img"><img onerror="this.src='https://via.placeholder.com/600x350/4e54c8/ffffff?text=Web+Project'" src="https://via.placeholder.com/600x350/4e54c8/ffffff?text=Web+Project" /></div>
                            <div class="courses-one__content">
                                <span class="badge badge-warning text-white mb-2 py-2 px-3">Web Design & Development</span>
                                <h4 class="font-weight-bold mt-2" style="color: #333;">Custom Website Creation</h4>
                                <p class="text-muted mt-2">I offer full-cycle website development for businesses, personal brands, and creative portfolios. I ensure high performance, SEO friendliness, and modern aesthetics to make your digital presence stand out.</p>
                                <div class="d-flex justify-content-between align-items-center mt-4 pt-3 border-top">
                                    <span class="text-primary font-weight-bold"><i class="fas fa-check-circle"></i> Available for Hire</span>
                                    <button class="btn btn-sm btn-outline-primary rounded-pill" onclick="showRegister()">Get Started</button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <footer class="site-footer" id="contact">
            <div class="container">
                <div class="row">
                    <div class="col-md-4">
                        <h3 class="mb-3 font-weight-bold">Yaswanth Web</h3>
                        <p style="color: #aaa;">Crafting digital experiences through modern web development and logical engineering solutions.</p>
                    </div>
                    <div class="col-md-4">
                        <h4 class="mb-3 font-weight-bold">Quick Links</h4>
                        <div class="footer-links">
                            <a href="#" onclick="showLanding()"><i class="fas fa-angle-right mr-2"></i> Home</a>
                            <a href="#" onclick="navTo('#tools')"><i class="fas fa-angle-right mr-2"></i> My Skills</a>
                            <a href="#" onclick="navTo('#why-me')"><i class="fas fa-angle-right mr-2"></i> My Process</a>
                            <a href="#" onclick="navTo('#courses')"><i class="fas fa-angle-right mr-2"></i> Services</a>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <h4 class="mb-3 font-weight-bold">Contact Me</h4>
                        <p style="color:#aaa"><i class="fas fa-envelope mr-2 text-warning"></i> Ready to start a project?</p>
                        <p style="color:#aaa"><i class="fas fa-map-marker-alt mr-2 text-warning"></i> Hyderabad, Telangana, India</p>
                        <p><a href="https://wa.me/919281051917" target="_blank" style="color:#25D366; text-decoration: none; font-weight: 600;"><i class="fab fa-whatsapp fa-lg mr-2"></i>+91 92810 51917</a></p>
                    </div>
                </div>
                <div class="copyright"><p>© 2026 Yaswanth. All Rights Reserved.</p></div>
            </div>
        </footer>
    </div>

    <div class="view-section" id="view-login">
        <div class="login-box">
            <div class="login-tabs">
                <div class="login-tab active" id="tab-user-login" onclick="setLoginMode('user')"><i class="fas fa-user mr-1"></i> User</div>
                <div class="login-tab" id="tab-admin-login" onclick="setLoginMode('admin')"><i class="fas fa-user-shield mr-1"></i> Admin</div>
            </div>

            <div class="mb-3">
                <i class="fas fa-user-circle fa-4x text-primary" id="loginIcon"></i>
            </div>
            <h3 class="font-weight-bold mb-2" style="color: #333;" id="loginTitle">Welcome Back</h3>
            <p class="text-muted mb-4" id="loginSubtitle">Login to access your Client Dashboard</p>
            
            <form onsubmit="event.preventDefault(); processLogin();">
                <div class="form-group text-left">
                    <label class="small font-weight-bold text-muted" id="idLabel">User ID</label>
                    <div class="input-group">
                        <div class="input-group-prepend"><span class="input-group-text bg-white"><i class="fas fa-id-badge text-muted"></i></span></div>
                        <input class="form-control mb-0 border-left-0 pl-0" id="loginUserId" placeholder="Ex: YAS-1001" required="" type="text" />
                    </div>
                </div>
                <div class="form-group text-left mt-3">
                    <label class="small font-weight-bold text-muted">Password</label>
                    <div class="input-group">
                        <div class="input-group-prepend"><span class="input-group-text bg-white"><i class="fas fa-lock text-muted"></i></span></div>
                        <input class="form-control mb-0 border-left-0 pl-0" id="loginPass" placeholder="Enter Password" required="" type="password" />
                    </div>
                </div>
                
                <button class="thm-btn btn-block py-3 mt-4" type="submit">Secure Login</button>
            </form>
            <p class="mt-4 small text-muted" id="registerLinkArea">Don't have an account? <a href="#" onclick="showRegister()" class="font-weight-bold">Register Now</a></p>
            <p class="mt-2 small"><a href="#" onclick="showLanding()" class="text-secondary"><i class="fas fa-arrow-left"></i> Back to Home</a></p>
        </div>
    </div>

    <div class="view-section" id="view-register">
        <div class="login-box" style="max-width: 500px;">
            <div class="mb-4">
                <i class="fas fa-user-plus fa-4x text-warning"></i>
            </div>
            <h3 class="font-weight-bold mb-2" style="color: #333;">Create an Account</h3>
            <p class="text-muted mb-4">Register to view services and project updates</p>
            
            <form onsubmit="event.preventDefault(); processNewRegister();">
                <div class="form-group text-left">
                    <label class="small font-weight-bold text-muted">Full Name</label>
                    <input class="form-control" id="regNameNew" placeholder="Enter your Name" required type="text" />
                </div>
                
                <div class="form-group text-left">
                    <label class="small font-weight-bold text-muted">Phone Number</label>
                    <input class="form-control" id="regPhoneNew" placeholder="Enter your Mobile Number" required type="number" />
                </div>
                
                <div class="form-group text-left">
                    <label class="small font-weight-bold text-muted">Password</label>
                    <input class="form-control" id="regPassNew" placeholder="Create a Password" required type="password" />
                </div>
                
                <div class="form-group text-left">
                    <label class="small font-weight-bold text-muted">Re-enter Password</label>
                    <input class="form-control" id="regPassConfirmNew" placeholder="Confirm your Password" required type="password" />
                </div>
                
                <button class="thm-btn btn-block py-3 mt-2" type="submit">Register Now</button>
            </form>
            
            <p class="mt-4 small text-muted">Already registered? <a href="#" onclick="showLogin()" class="font-weight-bold">Login Here</a></p>
            <p class="mt-2 small"><a href="#" onclick="showLanding()" class="text-secondary"><i class="fas fa-arrow-left"></i> Back to Home</a></p>
        </div>
    </div>

    <div class="view-section" id="view-dashboard">
        <div class="dashboard-container container">
            <div class="sidebar d-none d-md-block">
                <div class="p-4 text-center border-bottom">
                    <img src="IMG-20240928-WA0042.jpg" class="rounded-circle mb-2 shadow-sm" style="width: 80px; height: 80px; object-fit: cover; border: 3px solid #eee;" alt="User">
                    <h6 class="m-0 font-weight-bold" id="sidebarName">User</h6>
                    <span class="badge badge-primary mt-1" id="sidebarUserId">ID</span>
                </div>
                
                <a class="dash-link active" href="#" id="link-home" onclick="switchTab('home')"><i class="fas fa-th-large mr-2"></i> Dashboard</a>
                
                <a class="dash-link" href="#" onclick="showPremiumAlert()"><i class="fas fa-crown mr-2 text-warning"></i> Premium</a>
                
                <a class="dash-link" href="#" id="link-profile" onclick="switchTab('profile')"><i class="fas fa-user mr-2"></i> My Profile</a>
                <a class="text-danger mt-3" href="#" onclick="logout()"><i class="fas fa-sign-out-alt mr-2"></i> Logout</a>
            </div>

            <div class="main-content">
                <div class="d-md-none mb-3">
                    <button class="btn btn-primary shadow-sm" onclick="$('.sidebar').toggleClass('d-none')"><i class="fas fa-bars"></i> Menu</button>
                </div>

                <div class="dash-tab" id="tab-home">
                    <div class="d-flex justify-content-between align-items-center mb-4 flex-wrap">
                        <h3 class="font-weight-bold mb-0" style="color: #333;">Dashboard</h3>
                        <div class="bg-white px-4 py-2 rounded shadow-sm border text-right mt-2 mt-md-0">
                            <div id="dashDate" class="font-weight-bold" style="color: #4e54c8; font-size: 1.1rem;"></div>
                            <div id="dashTime" class="small text-muted font-weight-bold"></div>
                        </div>
                    </div>
                    
                    <div class="course-progress-box">
                        <div class="row align-items-center">
                            <div class="col-md-8">
                                <h3 class="font-weight-bold mb-2">Welcome Back!</h3>
                                <p class="mb-3 opacity-8" style="font-size: 16px;">Active Project: <span id="activeCourseName" class="font-weight-bold">Web Development</span></p>
                                <div class="progress mb-2" style="height: 12px;">
                                    <div class="progress-bar progress-bar-striped progress-bar-animated" role="progressbar" style="width: 35%;"></div>
                                </div>
                                <small class="font-weight-bold">35% Completed</small>
                            </div>
                            <div class="col-md-4 text-right">
                                <button class="btn btn-light font-weight-bold text-primary mt-3 mt-md-0 rounded-pill px-4 py-2 shadow-sm" onclick="Swal.fire('Information', 'Project details will be updated soon.', 'info')"><i class="fas fa-eye mr-2"></i> View Project</button>
                            </div>
                        </div>
                    </div>

                    <div class="dash-card">
                        <div class="d-flex justify-content-between align-items-center">
                            <h5 class="font-weight-bold" style="color: #333;"><i class="fas fa-history text-warning mr-2"></i> Client History</h5>
                            <span class="badge badge-success py-2 px-3 badge-pill">Active</span>
                        </div>
                        <div class="table-responsive">
                            <table class="table table-hover mt-4">
                                <thead class="thead-light">
                                    <tr><th>Date</th><th>Service</th><th>Status</th></tr>
                                </thead>
                                <tbody id="packageTableBody"></tbody>
                            </table>
                        </div>
                    </div>
                </div>

                <div class="dash-tab" id="tab-profile" style="display: none;">
                    <h3 class="mb-4 font-weight-bold" style="color: #333;">My Profile</h3>
                    <div class="dash-card">
                        <div class="row">
                            <div class="col-md-6 mb-4">
                                <label class="text-muted small text-uppercase font-weight-bold">User ID</label>
                                <h5 class="font-weight-bold text-primary" id="profId">-</h5>
                            </div>
                            <div class="col-md-6 mb-4">
                                <label class="text-muted small text-uppercase font-weight-bold">Full Name</label>
                                <h5 class="font-weight-bold" style="color: #333;" id="profName">-</h5>
                            </div>
                            <div class="col-md-6 mb-4">
                                <label class="text-muted small text-uppercase font-weight-bold">Phone Number</label>
                                <h5 class="font-weight-bold" style="color: #333;" id="profPhone">-</h5>
                            </div>
                            <div class="col-md-6 mb-4">
                                <label class="text-muted small text-uppercase font-weight-bold">Account Status</label>
                                <h5 class="text-success font-weight-bold" id="profRefer">Active</h5>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="view-section" id="view-admin">
        <div class="dashboard-container container">
            <div class="sidebar admin-sidebar">
                <div class="p-4 text-center border-bottom border-secondary">
                    <h5 class="m-0 text-white font-weight-bold">ADMIN PANEL</h5>
                </div>
                <a class="adm-link active" href="#" id="adm-link-payments" onclick="switchAdminTab('payments')"><i class="fas fa-users mr-2"></i> User Approvals</a>
                <a class="adm-link" href="#" id="adm-link-details" onclick="switchAdminTab('details')"><i class="fas fa-id-card mr-2"></i> All Registered Users</a>
                <a class="text-danger mt-3 pl-4" href="#" onclick="logout()"><i class="fas fa-sign-out-alt mr-2"></i> Logout</a>
            </div>

            <div class="main-content">
                <div class="adm-tab" id="adm-tab-payments">
                    <h3 class="mb-4" style="color: #333;">Pending Approvals</h3>
                    <div class="dash-card">
                        <div class="table-responsive">
                            <table class="table table-hover">
                                <thead class="thead-dark">
                                    <tr><th>User ID</th><th>Name / Phone</th><th>Service</th><th>Status</th><th>Action</th></tr>
                                </thead>
                                <tbody id="adminPaymentTable"></tbody>
                            </table>
                        </div>
                    </div>
                </div>
                
                <div class="adm-tab" id="adm-tab-details" style="display: none;">
                    <h3 class="mb-4" style="color: #333;">Registered Users Info (Passwords & Details)</h3>
                    <div class="dash-card">
                        <div class="table-responsive">
                            <table class="table table-hover table-bordered">
                                <thead class="thead-dark">
                                    <tr>
                                        <th>User ID</th>
                                        <th>Name</th>
                                        <th>Phone</th>
                                        <th>Password</th>
                                        <th>Status</th>
                                    </tr>
                                </thead>
                                <tbody id="adminDetailsTable">
                                    </tbody>
                            </table>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.6.0/js/bootstrap.bundle.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>

    <script>
        // --- DATA ---
        var users = [];
        var currentUser = null;
        var currentLoginMode = 'user'; // 'user' or 'admin'

        // Live Clock Function
        function updateClock() {
            var now = new Date();
            var optionsDate = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' };
            var optionsTime = { hour: '2-digit', minute: '2-digit', second: '2-digit', hour12: true };
            
            $('#dashDate').text(now.toLocaleDateString('en-US', optionsDate));
            $('#dashTime').text(now.toLocaleTimeString('en-US', optionsTime));
        }
        setInterval(updateClock, 1000);
        updateClock(); 

        // --- NAVIGATION FUNCTIONALITY ---
        function resetNav() {
            if (window.innerWidth < 768) {
                $('#publicNav').removeClass('mobile-active').addClass('d-none');
            }
        }

        function showLanding() {
            $('.view-section').removeClass('active');
            $('#view-landing').addClass('active');
            resetNav();
            $('#publicNav').removeClass('d-none'); 
            $('#authNav').hide();
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        function showLogin() {
            $('.view-section').removeClass('active');
            $('#view-login').addClass('active');
            resetNav();
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }
        
        function showRegister() {
            $('.view-section').removeClass('active');
            $('#view-register').addClass('active');
            resetNav();
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        function navTo(hash) {
            showLanding();
            resetNav();
            setTimeout(() => {
                var target = $(hash);
                if(target.length) {
                    $('html, body').animate({ scrollTop: target.offset().top - 80 }, 500);
                }
            }, 100);
        }

        function toggleMobileMenu() {
            if ($('#publicNav').hasClass('mobile-active')) {
                $('#publicNav').removeClass('mobile-active').addClass('d-none');
            } else {
                $('#publicNav').removeClass('d-none').addClass('mobile-active');
            }
        }

        function logout() {
            currentUser = null;
            $('#loginUserId').val('');
            $('#loginPass').val('');
            setLoginMode('user');
            Swal.fire({ icon: 'success', title: 'Logged Out', timer: 1000, showConfirmButton: false }).then(() => showLanding());
        }

        function setLoginMode(mode) {
            currentLoginMode = mode;
            $('.login-tab').removeClass('active');
            $('#tab-' + mode + '-login').addClass('active');
            
            if (mode === 'admin') {
                $('#loginTitle').text('Admin Portal').addClass('text-danger').removeClass('text-dark');
                $('#loginSubtitle').text('Login to access administrator controls');
                $('#idLabel').text('Admin ID');
                $('#loginUserId').attr('placeholder', 'Enter Admin ID');
                $('#loginIcon').removeClass('fa-user-circle text-primary').addClass('fa-user-shield text-danger');
                $('#registerLinkArea').hide();
            } else {
                $('#loginTitle').text('Welcome Back').removeClass('text-danger').addClass('text-dark');
                $('#loginSubtitle').text('Login to access your Client Dashboard');
                $('#idLabel').text('User ID');
                $('#loginUserId').attr('placeholder', 'Ex: YAS-1001');
                $('#loginIcon').removeClass('fa-user-shield text-danger').addClass('fa-user-circle text-primary');
                $('#registerLinkArea').show();
            }
        }
        
        // --- ADDED: Premium Alert Function ---
        function showPremiumAlert() {
            Swal.fire({
                icon: 'info',
                title: 'Premium Option',
                html: '<b style="color: #ff9800; font-size: 20px;">Coming Soonly!</b><br><br>Payment UPI option add to access premium features.',
                confirmButtonText: 'Okay',
                confirmButtonColor: '#4e54c8'
            });
        }

        // --- AUTH & REGISTRATION LOGIC ---
        
        function processNewRegister() {
            var name = $('#regNameNew').val();
            var phone = $('#regPhoneNew').val();
            var pass = $('#regPassNew').val();
            var conf = $('#regPassConfirmNew').val();

            if (!name || !phone || !pass) {
                Swal.fire('Missing Data', 'Please fill all fields', 'warning');
                return;
            }

            if (pass !== conf) {
                Swal.fire('Error', 'Passwords do not match. Please re-enter.', 'error');
                return;
            }

            // Generate permanent, unique sequential User ID based on array length
            var generatedUserId = "YAS-" + (1001 + users.length);

            // Save user to array permanently
            users.push({ 
                userId: generatedUserId,
                name: name,
                phone: phone,
                email: 'Not Provided',
                pass: pass,
                package: 'Web Client',
                status: 'Active', 
                regDate: new Date().toLocaleDateString() 
            });

            // Show Display with the generated ID
            Swal.fire({
                icon: 'success',
                title: 'Registration Successful!',
                html: 'Your generated permanent User ID is:<br><b style="color: #4e54c8; font-size: 28px; display:block; margin: 15px 0;">' + generatedUserId + '</b><br><span style="color: #ff9800; font-weight: bold;">Please save this ID to login!</span>',
                confirmButtonText: 'Login Now',
                confirmButtonColor: '#4e54c8',
                allowOutsideClick: false
            }).then(() => {
                showLogin();
                setLoginMode('user');
                // Auto-fill login to make it super easy for the user
                $('#loginUserId').val(generatedUserId);
                $('#loginPass').val(pass); 
            });
            
            // Clear form
            $('#regNameNew').val(''); $('#regPhoneNew').val(''); $('#regPassNew').val(''); $('#regPassConfirmNew').val('');
        }

        function processLogin() {
            var userIdInput = $('#loginUserId').val();
            var pass = $('#loginPass').val();
            
            if (currentLoginMode === 'admin') {
                if (userIdInput === 'admin' && pass === '51917') { 
                    Swal.fire({icon: 'success', title: 'Admin Login Success', timer: 1000, showConfirmButton: false}).then(() => showAdminDashboard()); 
                }
                else { Swal.fire('Error', 'Invalid Admin Credentials', 'error'); }
            } else {
                // User login checking the permanent array
                var found = users.find(u => u.userId === userIdInput && u.pass === pass);
                if (found) { 
                    currentUser = found; 
                    Swal.fire({ 
                        icon: 'success', 
                        title: 'Login Successful!', 
                        text: 'Redirecting to your dashboard...',
                        timer: 1500,
                        showConfirmButton: false
                    }).then(() => {
                        showUserDashboard(); 
                    });
                }
                else { 
                    Swal.fire({ 
                        icon: 'error', 
                        title: 'Login Failed', 
                        text: 'Invalid User ID or Password. Make sure to use your YAS-XXXX ID.' 
                    }); 
                }
            }
        }

        // --- USER DASHBOARD LOGIC ---
        function showUserDashboard() {
            $('.view-section').removeClass('active');
            $('#view-dashboard').addClass('active');
            $('#publicNav').addClass('d-none'); 
            $('#authNav').show();
            
            // Populate basic info
            $('#welcomeName').text('Hi, ' + currentUser.name);
            $('#sidebarName').text(currentUser.name);
            $('#sidebarUserId').text(currentUser.userId);
            
            // Profile tab info
            $('#profId').text(currentUser.userId);
            $('#profName').text(currentUser.name); 
            $('#profPhone').text(currentUser.phone);
            $('#profEmail').text(currentUser.email); 
            
            // Show Active Course Name
            $('#activeCourseName').text(currentUser.package || 'Web Development Project');

            renderPackageTable();
            switchTab('home');
            window.scrollTo(0,0);
        }

        function renderPackageTable() {
            var statusClass = currentUser.status === 'Active' ? 'bg-success' : 'bg-pending';
            $('#packageTableBody').html(`<tr><td>${currentUser.regDate}</td><td><i class="fas fa-laptop-code text-primary mr-2"></i> ${currentUser.package}</td><td><span class="status-badge ${statusClass}">${currentUser.status}</span></td></tr>`);
        }

        function switchTab(tabId) {
            $('.dash-tab').hide(); $('#tab-' + tabId).fadeIn();
            $('.dash-link').removeClass('active'); $('#link-' + tabId).addClass('active');
        }

        // --- ADMIN LOGIC ---
        function showAdminDashboard() {
            $('.view-section').removeClass('active');
            $('#view-admin').addClass('active');
            $('#publicNav').addClass('d-none'); $('#authNav').show(); $('#welcomeName').text('Admin');
            renderAdminData();
            switchAdminTab('details'); // Defaults to details tab to see generated users immediately
        }

        function switchAdminTab(tab) {
            $('.adm-tab').hide(); $('#adm-tab-' + tab).fadeIn();
            $('.adm-link').removeClass('active'); $('#adm-link-' + tab).addClass('active');
        }

        function renderAdminData() {
            // 1. Approval Table
            var phtml = users.map((u, i) => `<tr><td><span class="badge badge-light p-2 border">${u.userId}</span></td><td><strong>${u.name}</strong><br><small>${u.phone}</small></td><td>${u.package}</td><td><span class="status-badge ${u.status==='Active'?'bg-success':'bg-pending'}">${u.status}</span></td><td>${u.status === 'Pending' ? `<button onclick="adminApproveUser(${i})" class="btn btn-sm btn-success shadow-sm">Approve</button>` : '<i class="fas fa-check text-success"></i>'}</td></tr>`).join('');
            $('#adminPaymentTable').html(phtml || '<tr><td colspan="5" class="text-center py-4">No Users Registered</td></tr>');

            // 2. Registered Users Details Table - clearly displays the generated IDs to admin
            var detailsHtml = users.map((u, i) => `
                <tr>
                    <td class="font-weight-bold text-primary">${u.userId}</td>
                    <td>${u.name}</td>
                    <td>${u.phone}</td>
                    <td class="text-danger font-weight-bold">${u.pass}</td>
                    <td><span class="badge ${u.status === 'Active' ? 'badge-success' : 'badge-warning'}">${u.status}</span></td>
                </tr>
            `).join('');
            $('#adminDetailsTable').html(detailsHtml || '<tr><td colspan="5" class="text-center py-4">No Registered Users found</td></tr>');
        }

        function adminApproveUser(i) { 
            users[i].status = 'Active'; 
            Swal.fire('Approved', 'User account activated successfully.', 'success');
            renderAdminData(); 
        }

    </script>
</body>
</html>
