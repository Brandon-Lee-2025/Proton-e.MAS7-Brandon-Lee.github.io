# Proton-e.MAS7-Brandon-Lee.github.io
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Brandon Lee | Proton e.MAS Sales Specialist</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --professional-blue: #0C4DA2;
            --light-blue: #3A7BDB;
            --accent-gold: #D4AF37;
            --dark-text: #333333;
            --light-text: #FFFFFF;
            --light-bg: #F5F9FF;
            --card-shadow: 0 10px 30px rgba(12, 77, 162, 0.15);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: var(--dark-text);
            overflow-x: hidden;
            background-color: var(--light-bg);
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        .bilingual {
            display: flex;
            flex-direction: column;
        }
        
        .chinese {
            font-weight: 500;
        }
        
        .english {
            font-size: 0.85em;
            color: #666;
            font-style: italic;
            margin-top: 3px;
        }
        
        /* 头部导航 */
        header {
            background-color: white;
            box-shadow: 0 2px 15px rgba(12, 77, 162, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
            animation: slideDown 0.5s ease-out;
        }
        
        @keyframes slideDown {
            from { transform: translateY(-100%); }
            to { transform: translateY(0); }
        }
        
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .logo-img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            border: 2px solid var(--professional-blue);
            object-fit: cover;
            transition: transform 0.3s ease;
        }
        
        .logo-img:hover {
            transform: rotate(10deg);
        }
        
        .logo-text {
            font-weight: 700;
            font-size: 1.5rem;
            color: var(--professional-blue);
        }
        
        .logo-text span {
            color: var(--accent-gold);
        }
        
        /* GitHub部署说明部分 */
        .github-section {
            background-color: #f8f9fa;
            padding: 40px 0;
            border-top: 1px solid #eaeaea;
            border-bottom: 1px solid #eaeaea;
            margin: 30px 0;
        }
        
        .github-steps {
            background: white;
            border-radius: 10px;
            padding: 25px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            max-width: 800px;
            margin: 0 auto;
        }
        
        .github-steps h2 {
            color: var(--professional-blue);
            text-align: center;
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 2px solid var(--accent-gold);
        }
        
        .step {
            margin-bottom: 20px;
            padding: 15px;
            border-left: 3px solid var(--accent-gold);
            background: rgba(12, 77, 162, 0.03);
        }
        
        .step-number {
            display: inline-block;
            width: 30px;
            height: 30px;
            background: var(--accent-gold);
            color: white;
            border-radius: 50%;
            text-align: center;
            line-height: 30px;
            margin-right: 10px;
            font-weight: bold;
        }
        
        .step-content {
            display: inline-block;
            width: calc(100% - 40px);
            vertical-align: top;
        }
        
        .code-block {
            background: #2d2d2d;
            color: #f8f8f2;
            padding: 15px;
            border-radius: 5px;
            font-family: 'Courier New', monospace;
            margin: 10px 0;
            overflow-x: auto;
        }
        
        .terminal {
            position: relative;
        }
        
        .terminal::before {
            content: '$';
            position: absolute;
            left: 10px;
            top: 15px;
            color: #50fa7b;
        }
        
        .terminal pre {
            padding-left: 20px;
        }
        
        .note {
            background: #fff9db;
            border-left: 4px solid #ffd43b;
            padding: 10px 15px;
            margin: 15px 0;
            border-radius: 0 4px 4px 0;
        }
        
        /* 首屏区域 */
        .hero {
            background: linear-gradient(rgba(12, 77, 162, 0.9), rgba(12, 77, 162, 0.85)), url('https://images.unsplash.com/photo-1617347454431-f49d7ff5c3b1?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            color: var(--light-text);
            padding: 100px 0 80px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at center, transparent 0%, rgba(12, 77, 162, 0.8) 100%);
            z-index: 1;
        }
        
        .hero-content {
            max-width: 900px;
            margin: 0 auto;
            position: relative;
            z-index: 2;
        }
        
        .advisor-card {
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 30px;
            max-width: 500px;
            margin: 0 auto 40px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease;
        }
        
        .advisor-card:hover {
            transform: translateY(-5px);
        }
        
        .advisor-avatar {
            width: 140px;
            height: 140px;
            border-radius: 50%;
            border: 3px solid var(--accent-gold);
            margin: 0 auto 20px;
            object-fit: cover;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            transition: all 0.3s ease;
        }
        
        .advisor-avatar:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 20px rgba(212, 175, 55, 0.4);
        }
        
        .hero h1 {
            font-size: 2.8rem;
            margin-bottom: 20px;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.3);
            animation: fadeInUp 1s ease;
        }
        
        .hero p {
            font-size: 1.3rem;
            margin-bottom: 30px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
            animation: fadeInUp 1s ease 0.2s;
            animation-fill-mode: both;
        }
        
        .hero-buttons {
            animation: fadeInUp 1s ease 0.4s;
            animation-fill-mode: both;
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .btn {
            display: inline-block;
            background-color: var(--accent-gold);
            color: var(--dark-text);
            padding: 15px 35px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            border: 2px solid var(--accent-gold);
            box-shadow: 0 4px 10px rgba(0,0,0,0.15);
            position: relative;
            overflow: hidden;
        }
        
        .btn::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(255, 255, 255, 0.2);
            transform: translateX(-100%);
            transition: transform 0.3s ease;
        }
        
        .btn:hover {
            background-color: transparent;
            color: white;
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0,0,0,0.25);
        }
        
        .btn:hover::after {
            transform: translateX(100%);
        }
        
        .btn-outline {
            background: transparent;
            border: 2px solid white;
            color: white;
            margin-left: 15px;
        }
        
        .btn-outline:hover {
            background: white;
            color: var(--professional-blue);
        }
        
        /* 痛点区域 */
        .pain-points {
            padding: 80px 0;
            background-color: white;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }
        
        .section-title h2 {
            font-size: 2.2rem;
            color: var(--professional-blue);
            display: inline-block;
            padding-bottom: 15px;
        }
        
        .section-title h2:after {
            content: '';
            position: absolute;
            width: 80px;
            height: 3px;
            background: var(--accent-gold);
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            animation: lineGrow 1.5s ease;
        }
        
        @keyframes lineGrow {
            from { width: 0; }
            to { width: 80px; }
        }
        
        .points-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .point-card {
            background: white;
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 5px 20px rgba(12, 77, 162, 0.08);
            transition: all 0.4s ease;
            text-align: center;
            border: 1px solid rgba(12, 77, 162, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        .point-card:hover {
            transform: translateY(-10px);
            box-shadow: var(--card-shadow);
            border-color: var(--light-blue);
        }
        
        .point-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: var(--accent-gold);
            transform: scaleX(0);
            transform-origin: left;
            transition: transform 0.4s ease;
        }
        
        .point-card:hover::before {
            transform: scaleX(1);
        }
        
        .point-icon {
            font-size: 2.5rem;
            color: var(--professional-blue);
            margin-bottom: 20px;
            background: rgba(12, 77, 162, 0.05);
            width: 80px;
            height: 80px;
            line-height: 80px;
            border-radius: 50%;
            margin: 0 auto 20px;
            transition: all 0.3s ease;
        }
        
        .point-card:hover .point-icon {
            background: rgba(12, 77, 162, 0.1);
            transform: rotate(10deg);
        }
        
        /* 服务流程 */
        .process {
            padding: 80px 0;
            background: var(--light-bg);
        }
        
        .timeline {
            position: relative;
            max-width: 1000px;
            margin: 50px auto;
        }
        
        .timeline:before {
            content: '';
            position: absolute;
            width: 4px;
            background: linear-gradient(to bottom, var(--accent-gold), var(--professional-blue));
            top: 0;
            bottom: 0;
            left: 50%;
            margin-left: -2px;
            animation: lineGrowVertical 2s ease;
        }
        
        @keyframes lineGrowVertical {
            from { height: 0; }
            to { height: 100%; }
        }
        
        .timeline-item {
            padding: 20px 40px;
            position: relative;
            width: 50%;
            box-sizing: border-box;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 0.6s ease forwards;
        }
        
        .timeline-item:nth-child(1) { animation-delay: 0.2s; }
        .timeline-item:nth-child(2) { animation-delay: 0.4s; }
        .timeline-item:nth-child(3) { animation-delay: 0.6s; }
        .timeline-item:nth-child(4) { animation-delay: 0.8s; }
        
        .timeline-item:nth-child(odd) {
            left: 0;
            text-align: right;
        }
        
        .timeline-item:nth-child(even) {
            left: 50%;
        }
        
        .timeline-content {
            padding: 25px;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(12, 77, 162, 0.08);
            border-left: 4px solid var(--professional-blue);
            position: relative;
            transition: all 0.3s ease;
        }
        
        .timeline-content:hover {
            transform: translateX(5px);
            box-shadow: var(--card-shadow);
        }
        
        .timeline-content h3 {
            color: var(--professional-blue);
            margin-bottom: 10px;
        }
        
        /* 车型展示 */
        .vehicle-showcase {
            padding: 80px 0;
            background: white;
        }
        
        .vehicles-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 40px;
            margin-top: 50px;
        }
        
        .vehicle-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: all 0.4s ease;
            position: relative;
        }
        
        .vehicle-card:hover {
            transform: translateY(-10px);
            box-shadow: var(--card-shadow);
        }
        
        .vehicle-image {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-bottom: 3px solid var(--accent-gold);
            transition: transform 0.5s ease;
        }
        
        .vehicle-card:hover .vehicle-image {
            transform: scale(1.05);
        }
        
        .vehicle-details {
            padding: 25px;
            text-align: center;
            position: relative;
            z-index: 2;
            background: white;
        }
        
        .vehicle-details h3 {
            color: var(--professional-blue);
            font-size: 1.8rem;
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
        }
        
        .vehicle-details h3::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 100%;
            height: 2px;
            background: var(--accent-gold);
            transform: scaleX(0);
            transition: transform 0.3s ease;
        }
        
        .vehicle-card:hover .vehicle-details h3::after {
            transform: scaleX(1);
        }
        
        .vehicle-features {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
            margin: 20px 0;
            text-align: left;
        }
        
        .feature-item {
            display: flex;
            align-items: center;
        }
        
        .feature-icon {
            color: var(--accent-gold);
            margin-right: 10px;
            font-size: 1.2rem;
            min-width: 20px;
        }
        
        /* 技术亮点 */
        .tech-highlights {
            padding: 80px 0;
            background: var(--light-bg);
        }
        
        .tech-container {
            display: flex;
            gap: 40px;
            max-width: 1200px;
            margin: 0 auto;
            align-items: center;
        }
        
        .tech-content {
            flex: 1;
        }
        
        .tech-visual {
            flex: 1;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: var(--card-shadow);
        }
        
        .tech-video {
            width: 100%;
            height: 400px;
            border: none;
            border-radius: 15px;
        }
        
        .motor-card {
            background: white;
            border-radius: 15px;
            padding: 30px;
            box-shadow: var(--card-shadow);
            margin-top: 40px;
            text-align: center;
        }
        
        .motor-image {
            max-width: 100%;
            border-radius: 10px;
            margin: 20px 0;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            border: 1px solid rgba(12, 77, 162, 0.1);
        }
        
        .tech-title {
            color: var(--professional-blue);
            margin-bottom: 20px;
            font-size: 1.8rem;
            position: relative;
            display: inline-block;
        }
        
        .tech-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 100%;
            height: 3px;
            background: var(--accent-gold);
        }
        
        .tech-features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .tech-feature-card {
            background: rgba(12, 77, 162, 0.03);
            border-radius: 10px;
            padding: 25px;
            text-align: center;
            border: 1px solid rgba(12, 77, 162, 0.08);
            transition: all 0.3s ease;
        }
        
        .tech-feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            border-color: var(--accent-gold);
        }
        
        .tech-feature-icon {
            font-size: 2.5rem;
            color: var(--accent-gold);
            margin-bottom: 15px;
        }
        
        /* 顾问介绍 */
        .about-advisor {
            padding: 80px 0;
            background: var(--light-bg);
        }
        
        .about-container {
            display: flex;
            align-items: center;
            gap: 50px;
            max-width: 1100px;
            margin: 0 auto;
        }
        
        .about-avatar {
            flex: 1;
            text-align: center;
            perspective: 1000px;
        }
        
        .about-avatar img {
            width: 100%;
            max-width: 400px;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.15);
            border: 2px solid var(--accent-gold);
            transition: transform 0.5s ease;
            transform-style: preserve-3d;
        }
        
        .about-avatar:hover img {
            transform: rotateY(10deg);
        }
        
        .about-content {
            flex: 1;
        }
        
        .about-content h2 {
            color: var(--professional-blue);
            margin-bottom: 20px;
            font-size: 2rem;
            position: relative;
            display: inline-block;
        }
        
        .about-content h2::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 100%;
            height: 3px;
            background: var(--accent-gold);
        }
        
        .about-content h3 {
            color: var(--accent-gold);
            margin-bottom: 15px;
            font-size: 1.4rem;
        }
        
        .contact-info {
            margin-top: 30px;
            padding-top: 20px;
            border-top: 1px solid rgba(12, 77, 162, 0.1);
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
            transition: transform 0.3s ease;
        }
        
        .contact-item:hover {
            transform: translateX(5px);
        }
        
        .contact-icon {
            width: 40px;
            height: 40px;
            background: rgba(12, 77, 162, 0.05);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            color: var(--professional-blue);
            transition: all 0.3s ease;
        }
        
        .contact-item:hover .contact-icon {
            background: var(--professional-blue);
            color: white;
        }
        
        /* 表单区域 */
        .cta-section {
            background: linear-gradient(to right, var(--professional-blue), #093a7e);
            padding: 80px 0;
            color: white;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .cta-section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M11 18c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm48 25c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm-43-7c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm63 31c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM34 90c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm56-76c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM12 86c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm28-65c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm23-11c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-6 60c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm29 22c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zM32 63c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm57-13c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-9-21c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM60 91c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM35 41c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM12 60c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2z' fill='%23093a7e' fill-opacity='0.1' fill-rule='evenodd'/%3E%3C/svg%3E");
            opacity: 0.1;
            z-index: 1;
        }
        
        .form-container {
            max-width: 600px;
            margin: 40px auto 0;
            background: rgba(255,255,255,0.1);
            padding: 40px;
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
            position: relative;
            z-index: 2;
            transition: transform 0.3s ease;
        }
        
        .form-container:hover {
            transform: scale(1.01);
        }
        
        .form-group {
            margin-bottom: 25px;
            text-align: left;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            color: white;
        }
        
        .form-group input, 
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 15px;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            background: rgba(255,255,255,0.9);
            transition: all 0.3s ease;
            border: 2px solid transparent;
        }
        
        .form-group input:focus, 
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--accent-gold);
            box-shadow: 0 0 0 3px rgba(212, 175, 55, 0.3);
        }
        
        /* 页脚 */
        footer {
            background: linear-gradient(to right, #0a2a5c, #08306b);
            color: white;
            padding: 60px 0 30px;
            position: relative;
            overflow: hidden;
        }
        
        footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M11 18c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm48 25c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm-43-7c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm63 31c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM34 90c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm56-76c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM12 86c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm28-65c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm23-11c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-6 60c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm29 22c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zM32 63c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm57-13c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-9-21c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM60 91c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM35 41c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM12 60c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2z' fill='%23D4AF37' fill-opacity='0.1' fill-rule='evenodd'/%3E%3C/svg%3E");
            opacity: 0.1;
            z-index: 1;
        }
        
        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            position: relative;
            z-index: 2;
        }
        
        .contact-info-footer h3 {
            color: var(--accent-gold);
            margin-bottom: 20px;
            position: relative;
            display: inline-block;
        }
        
        .contact-info-footer h3::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 100%;
            height: 2px;
            background: var(--accent-gold);
        }
        
        .contact-item-footer {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
            transition: transform 0.3s ease;
        }
        
        .contact-item-footer:hover {
            transform: translateX(5px);
        }
        
        .contact-icon-footer {
            margin-right: 15px;
            color: var(--accent-gold);
            min-width: 20px;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .social-icon {
            display: inline-block;
            width: 40px;
            height: 40px;
            background: rgba(255,255,255,0.1);
            border-radius: 50%;
            text-align: center;
            line-height: 40px;
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }
        
        .social-icon::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--accent-gold);
            transform: translateY(100%);
            transition: transform 0.3s ease;
            z-index: -1;
        }
        
        .social-icon:hover {
            background: transparent;
            transform: translateY(-5px);
            color: var(--dark-text);
        }
        
        .social-icon:hover::before {
            transform: translateY(0);
        }
        
        .copyright {
            text-align: center;
            padding-top: 40px;
            margin-top: 40px;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: rgba(255,255,255,0.7);
            position: relative;
            z-index: 2;
        }
        
        /* 安全认证 */
        .safety-section {
            padding: 80px 0;
            background: white;
        }
        
        .safety-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }
        
        .safety-badge {
            width: 200px;
            height: 200px;
            margin: 0 auto 30px;
            background: #fff;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            border: 5px solid var(--accent-gold);
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }
        
        .safety-badge i {
            font-size: 6rem;
            color: var(--professional-blue);
        }
        
        /* 响应式设计 */
        @media (max-width: 992px) {
            .about-container {
                flex-direction: column;
                text-align: center;
            }
            
            .contact-item {
                justify-content: center;
            }
            
            .timeline:before {
                left: 31px;
            }
            
            .timeline-item {
                width: 100%;
                padding-left: 70px;
                padding-right: 25px;
                text-align: left !important;
            }
            
            .timeline-item:nth-child(even) {
                left: 0;
            }
            
            .tech-container {
                flex-direction: column;
            }
        }
        
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero .btn {
                display: block;
                margin: 10px auto;
                max-width: 300px;
            }
            
            .btn-outline {
                margin-left: 0;
                margin-top: 15px;
            }
            
            .vehicle-features {
                grid-template-columns: 1fr;
            }
            
            .hero p {
                font-size: 1.1rem;
            }
            
            .tech-video {
                height: 300px;
            }
        }
        
        /* 地址链接样式 */
        .address-link {
            color: inherit;
            text-decoration: none;
            transition: all 0.3s ease;
        }
        
        .address-link:hover {
            color: var(--accent-gold);
            text-decoration: underline;
        }
        
        .address-link i {
            margin-right: 5px;
        }
    </style>
</head>
<body>
    <!-- 导航栏 -->
    <header>
        <div class="container">
            <nav class="navbar">
                <div class="logo">
                    <img src="https://i.ibb.co/rfxTf7pH/download.png" alt="Brandon Lee Logo" class="logo-img">
                    <div class="logo-text">Brandon<span>Lee</span></div>
                </div>
                <div class="contact-header">
                    <a href="tel:+60198067373" class="btn">
                        <i class="fas fa-phone"></i> 立即致电 (Call Now)
                    </a>
                </div>
            </nav>
        </div>
    </header>

    <!-- 首屏区域 -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <div class="advisor-card">
                    <img src="https://i.ibb.co/39sJs9jN/Whats-App-Image-2025-07-12-at-12-30-16-Photoroom.png" alt="Brandon Lee" class="advisor-avatar">
                    <h3>Brandon Lee Yan Siung</h3>
                    <p>高级专业汽车销售顾问<br><span style="font-size: 0.9em;">(Senior Professional Car Sales Consultant)</span></p>
                </div>
                
                <h1>解锁您的完美Proton e.MAS购车方案<br><span style="font-size: 0.7em; display: block; margin-top: 15px;">Unlock Your Perfect Proton e.MAS Purchase Plan</span></h1>
                <p>一对一专业顾问服务 • 精准配置推荐 • 最优贷款方案 • 政府补贴申请无忧<br>
                <span style="font-size: 0.9em;">One-on-One Consultation • Precise Configuration Recommendation • Best Loan Solutions • Hassle-Free Government Subsidy Application</span></p>
                <div class="hero-buttons">
                    <a href="#cta" class="btn">获取免费专属方案<br><span style="font-size: 0.8em;">Get Free Personalized Plan</span></a>
                    <a href="tel:+60198067373" class="btn btn-outline">
                        <i class="fas fa-phone"></i> 019-806 7373
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- 痛点区域 -->
    <section class="pain-points">
        <div class="container">
            <div class="section-title">
                <h2>您在选购Proton e.MAS时是否遇到这些问题？<br><span style="font-size: 0.7em; display: block; margin-top: 10px;">Do You Face These Issues When Choosing Proton e.MAS?</span></h2>
            </div>
            <div class="points-grid">
                <div class="point-card">
                    <div class="point-icon">
                        <i class="fas fa-cogs"></i>
                    </div>
                    <div class="bilingual">
                        <div class="chinese">配置选择困难症</div>
                        <div class="english">Configuration Selection Difficulty</div>
                    </div>
                    <p>Prime版还是Premium版？不知道哪款最适合您的生活需求和预算？<br>
                    <span style="font-size: 0.85em; color: #666; font-style: italic;">Prime or Premium? Not sure which suits your lifestyle and budget best?</span></p>
                </div>
                
                <div class="point-card">
                    <div class="point-icon">
                        <i class="fas fa-calculator"></i>
                    </div>
                    <div class="bilingual">
                        <div class="chinese">贷款方案复杂</div>
                        <div class="english">Complex Loan Options</div>
                    </div>
                    <p>面对不同银行的利率和条款，不知如何选择最划算的方案？担心审批不通过？<br>
                    <span style="font-size: 0.85em; color: #666; font-style: italic;">Facing various bank rates and terms, unsure how to choose the best option? Worried about approval?</span></p>
                </div>
                
                <div class="point-card">
                    <div class="point-icon">
                        <i class="fas fa-file-invoice-dollar"></i>
                    </div>
                    <div class="bilingual">
                        <div class="chinese">补贴申请困惑</div>
                        <div class="english">Subsidy Application Confusion</div>
                    </div>
                    <p>不了解最新的电动车补贴政策？担心错过可享受的数千元优惠？<br>
                    <span style="font-size: 0.85em; color: #666; font-style: italic;">Unaware of latest EV subsidy policies? Worried about missing thousands in benefits?</span></p>
                </div>
            </div>
        </div>
    </section>

    <!-- 服务流程 -->
    <section class="process">
        <div class="container">
            <div class="section-title">
                <h2>简单四步 轻松拥有您的e.MAS<br><span style="font-size: 0.7em; display: block; margin-top: 10px;">Simple 4 Steps to Own Your e.MAS</span></h2>
            </div>
            
            <div class="timeline">
                <div class="timeline-item">
                    <div class="timeline-content">
                        <div class="bilingual">
                            <div class="chinese"><i class="fas fa-comments"></i> 1. 免费咨询</div>
                            <div class="english">Free Consultation</div>
                        </div>
                        <p>告诉我们您的需求和预算，解答所有疑问<br>
                        <span style="font-size: 0.9em; font-style: italic;">Share your needs and budget, get all questions answered</span></p>
                    </div>
                </div>
                
                <div class="timeline-item">
                    <div class="timeline-content">
                        <div class="bilingual">
                            <div class="chinese"><i class="fas fa-clipboard-list"></i> 2. 定制方案</div>
                            <div class="english">Customized Solution</div>
                        </div>
                        <p>为您量身推荐Prime或Premium配置方案<br>
                        <span style="font-size: 0.9em; font-style: italic;">Personalized recommendation for Prime or Premium configuration</span></p>
                    </div>
                </div>
                
                <div class="timeline-item">
                    <div class="timeline-content">
                        <div class="bilingual">
                            <div class="chinese"><i class="fas fa-file-signature"></i> 3. 手续办理</div>
                            <div class="english">Documentation Processing</div>
                        </div>
                        <p>我们协助完成贷款申请、补贴申领及所有文书工作<br>
                        <span style="font-size: 0.9em; font-style: italic;">We assist with loan application, subsidy claims and paperwork</span></p>
                    </div>
                </div>
                
                <div class="timeline-item">
                    <div class="timeline-content">
                        <div class="bilingual">
                            <div class="chinese"><i class="fas fa-car"></i> 4. 喜提爱车</div>
                            <div class="english">Enjoy Your New Car</div>
                        </div>
                        <p>享受无缝交车体验，开启您的Emas电动之旅<br>
                        <span style="font-size: 0.9em; font-style: italic;">Seamless delivery experience to start your e.MAS journey</span></p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- 车型展示 -->
    <section class="vehicle-showcase">
        <div class="container">
            <div class="section-title">
                <h2>探索 Proton e.MAS 系列<br><span style="font-size: 0.7em; display: block; margin-top: 10px;">Explore Proton e.MAS Series</span></h2>
                <p>选择最适合您的电动车型<br><span style="font-size: 0.9em; font-style: italic;">Choose the EV that best suits you</span></p>
            </div>
            
            <div class="vehicles-grid">
                <div class="vehicle-card">
                    <img src="https://i.ibb.co/PffxhHh/e-MAS7-PRIME.png" alt="Proton e.MAS7 Prime" class="vehicle-image">
                    <div class="vehicle-details">
                        <h3>e.MAS7 Prime</h3>
                        <p>智能电动SUV，完美平衡性能与经济性<br>
                        <span style="font-size: 0.9em; font-style: italic;">Smart Electric SUV, Perfect Balance of Performance & Economy</span></p>
                        
                        <div class="vehicle-features">
                            <div class="feature-item">
                                <div class="feature-icon">
                                    <i class="fas fa-bolt"></i>
                                </div>
                                <div>最大功率 160kW<br><span style="font-size: 0.9em; font-style: italic;">Max Power 160kW</span></div>
                            </div>
                            <div class="feature-item">
                                <div class="feature-icon">
                                    <i class="fas fa-road"></i>
                                </div>
                                <div>续航 345km<br><span style="font-size: 0.9em; font-style: italic;">Range 345km</span></div>
                            </div>
                            <div class="feature-item">
                                <div class="feature-icon">
                                    <i class="fas fa-charging-station"></i>
                                </div>
                                <div>快充 30分钟<br><span style="font-size: 0.9em; font-style: italic;">Fast Charge 30min</span></div>
                            </div>
                            <div class="feature-item">
                                <div class="feature-icon">
                                    <i class="fas fa-users"></i>
                                </div>
                                <div>5座舒适空间<br><span style="font-size: 0.9em; font-style: italic;">5-Seat Comfort Space</span></div>
                            </div>
                        </div>
                        
                        <a href="#cta" class="btn" style="background: var(--professional-blue); color: white;">
                            咨询Prime详情<br>
                            <span style="font-size: 0.8em;">Inquire About Prime</span>
                        </a>
                    </div>
                </div>
                
                <div class="vehicle-card">
                    <img src="https://i.ibb.co/HDcy9qfT/e-MAS7-PREMIUM-1024x396.png" alt="Proton e.MAS7 Premium" class="vehicle-image">
                    <div class="vehicle-details">
                        <h3>e.MAS7 Premium</h3>
                        <p>豪华电动SUV，尊享高端科技与舒适体验<br>
                        <span style="font-size: 0.9em; font-style: italic;">Luxury Electric SUV with Premium Tech & Comfort</span></p>
                        
                        <div class="vehicle-features">
                            <div class="feature-item">
                                <div class="feature-icon">
                                    <i class="fas fa-bolt"></i>
                                </div>
                                <div>最大功率 160kW<br><span style="font-size: 0.9em; font-style: italic;">Max Power 160kW</span></div>
                            </div>
                            <div class="feature-item">
                                <div class="feature-icon">
                                    <i class="fas fa-road"></i>
                                </div>
                                <div>续航 410km<br><span style="font-size: 0.9em; font-style: italic;">Range 410km</span></div>
                            </div>
                            <div class="feature-item">
                                <div class="feature-icon">
                                    <i class="fas fa-sun"></i>
                                </div>
                                <div>全景天窗<br><span style="font-size: 0.9em; font-style: italic;">Panoramic Sunroof</span></div>
                            </div>
                            <div class="feature-item">
                                <div class="feature-icon">
                                    <i class="fas fa-tachometer-alt"></i>
                                </div>
                                <div>16粒Flyme Auto Speaker<br><span style="font-size: 0.9em; font-style: italic;">16 Flyme Auto Speakers</span></div>
                            </div>
                        </div>
                        
                        <a href="#cta" class="btn" style="background: var(--accent-gold); color: #333;">
                            咨询Premium详情<br>
                            <span style="font-size: 0.8em;">Inquire About Premium</span>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- 技术亮点 -->
    <section class="tech-highlights">
        <div class="container">
            <div class="section-title">
                <h2>核心技术亮点<br><span style="font-size: 0.7em; display: block; margin-top: 10px;">Core Technical Highlights</span></h2>
                <p>Proton e.MAS 的先进技术解析<br><span style="font-size: 0.9em; font-style: italic;">Advanced Technology of Proton e.MAS</span></p>
            </div>
            
            <!-- 神盾短刀电池视频 -->
            <div class="tech-container">
                <div class="tech-content">
                    <h3 class="tech-title">神盾短刀电池技术<br><span style="font-size: 0.7em; display: block; margin-top: 5px;">Shen Dun Blade Battery Technology</span></h3>
                    <p>Proton e.MAS 采用创新的神盾短刀电池技术，提供行业领先的安全性能和续航能力：<br>
                    <span style="font-size: 0.9em; font-style: italic;">Proton e.MAS features innovative Shen Dun Blade Battery technology, offering industry-leading safety and range:</span></p>
                    <ul style="list-style-type: none; padding: 20px 0;">
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 超强热管理系统，防止过热风险<br><span style="font-size: 0.9em; font-style: italic;">Advanced thermal management system prevents overheating risks</span></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 军工级防护结构，通过严苛安全测试<br><span style="font-size: 0.9em; font-style: italic;">Military-grade protection structure passes rigorous safety tests</span></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 快速充电技术：30分钟充至80%<br><span style="font-size: 0.9em; font-style: italic;">Fast charging: 30 minutes to 80% capacity</span></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 超长电池寿命：921次充放电后仍保持90%容量<br><span style="font-size: 0.9em; font-style: italic;">Long battery life: retains 90% capacity after 921 cycles</span></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> IP68防水防尘等级，适应各种气候条件<br><span style="font-size: 0.9em; font-style: italic;">IP68 waterproof/dustproof rating for all climates</span></li>
                    </ul>
                </div>
                
                <div class="tech-visual">
                    <!-- 修正后的电池视频嵌入代码 -->
                    <iframe class="tech-video" src="https://www.youtube.com/embed/Wjt4pLqLMWs" 
                            title="神盾短刀电池技术介绍" frameborder="0" 
                            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                            allowfullscreen></iframe>
                </div>
            </div>
            
            <!-- Asian NCAP 五星安全认证 -->
            <div class="tech-container" style="margin-top: 60px;">
                <div class="tech-visual">
                    <!-- 添加的Asian NCAP安全认证视频 -->
                    <iframe class="tech-video" src="https://www.youtube.com/embed/gjWEHKaE2Cc" 
                            title="Proton e.MAS Asian NCAP 五星安全认证" frameborder="0" 
                            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                            allowfullscreen></iframe>
                </div>
                
                <div class="tech-content">
                    <h3 class="tech-title">Asian NCAP 五星安全认证<br><span style="font-size: 0.7em; display: block; margin-top: 5px;">5-Star Asian NCAP Safety Rating</span></h3>
                    <p>Proton e.MAS 荣获最高安全评级，为您的每次出行提供全方位保护：<br>
                    <span style="font-size: 0.9em; font-style: italic;">Proton e.MAS achieves the highest safety rating, providing comprehensive protection for every journey:</span></p>
                    <ul style="list-style-type: none; padding: 20px 0;">
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 成人乘员保护：94.4分（满分100）<br><span style="font-size: 0.9em; font-style: italic;">Adult Occupant Protection: 94.4/100</span></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 儿童乘员保护：89.5分（满分100）<br><span style="font-size: 0.9em; font-style: italic;">Child Occupant Protection: 89.5/100</span></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 安全辅助系统：81.9分（满分100）<br><span style="font-size: 0.9em; font-style: italic;">Safety Assist: 81.9/100</span></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 行人保护：78.9分（满分100）<br><span style="font-size: 0.9em; font-style: italic;">Pedestrian Protection: 78.9/100</span></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 6个安全气囊 + 主动安全系统<br><span style="font-size: 0.9em; font-style: italic;">6 Airbags + Active Safety Systems</span></li>
                    </ul>
                </div>
            </div>
            
            <!-- 电机技术介绍 -->
            <div class="motor-card">
                <h3 class="tech-title">高效永磁同步电机<br><span style="font-size: 0.7em; display: block; margin-top: 5px;">High-Efficiency Permanent Magnet Synchronous Motor</span></h3>
                <p>Proton e.MAS 采用最新一代永磁同步电机技术，提供强劲动力与高效能表现<br>
                <span style="font-size: 0.9em; font-style: italic;">Proton e.MAS features next-gen PMSM technology for powerful and efficient performance</span></p>
                
                <!-- 修正后的电机图片链接 -->
                <img src="https://i.ibb.co/Wvkgtcpj/Whats-App-Image-2025-07-12-at-12-46-21.jpg" alt="Proton e.MAS Motor" class="motor-image">
                
                <div class="tech-specs" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-top: 20px;">
                    <div class="spec-item">
                        <div class="spec-value" style="font-size: 2rem; color: var(--professional-blue); font-weight: bold;">160kW</div>
                        <div class="spec-label">最大功率<br><span style="font-size: 0.9em; font-style: italic;">Max Power</span></div>
                    </div>
                    <div class="spec-item">
                        <div class="spec-value" style="font-size: 2rem; color: var(--professional-blue); font-weight: bold;">320N·m</div>
                        <div class="spec-label">峰值扭矩<br><span style="font-size: 0.9em; font-style: italic;">Peak Torque</span></div>
                    </div>
                    <div class="spec-item">
                        <div class="spec-value" style="font-size: 2rem; color: var(--professional-blue); font-weight: bold;">95%</div>
                        <div class="spec-label">能源效率<br><span style="font-size: 0.9em; font-style: italic;">Energy Efficiency</span></div>
                    </div>
                    <div class="spec-item">
                        <div class="spec-value" style="font-size: 2rem; color: var(--professional-blue); font-weight: bold;">0-100km/h 6.9s</div>
                        <div class="spec-label">加速性能<br><span style="font-size: 0.9em; font-style: italic;">Acceleration</span></div>
                    </div>
                </div>
                
                <p style="margin-top: 20px; text-align: left;">
                    <strong>技术优势：</strong> 电机采用油冷技术确保持续高性能输出，集成式设计减少能量损失，智能控制系统根据不同驾驶条件自动优化动力分配，实现性能与效率的完美平衡。<br>
                    <span style="font-size: 0.9em; font-style: italic;"><strong>Technical Advantages:</strong> Oil-cooled motor ensures sustained high performance, integrated design minimizes energy loss, intelligent control optimizes power distribution for perfect balance of performance and efficiency.</span>
                </p>
            </div>
        </div>
    </section>
    
    <!-- 安全特性 -->
    <section class="safety-section">
        <div class="container">
            <div class="section-title">
                <h2>全方位安全保障<br><span style="font-size: 0.7em; display: block; margin-top: 10px;">Comprehensive Safety Features</span></h2>
                <p>为您的每一次出行保驾护航<br><span style="font-size: 0.9em; font-style: italic;">Protecting every journey you take</span></p>
            </div>
            
            <div class="safety-content">
                <div class="safety-badge">
                    <i class="fas fa-shield-alt"></i>
                </div>
                
                <div class="tech-features">
                    <div class="tech-feature-card">
                        <div class="tech-feature-icon">
                            <i class="fas fa-car-crash"></i>
                        </div>
                        <h3>高强度车身结构</h3>
                        <p>超高强度钢占比72%，关键部位使用热成型钢<br>
                        <span style="font-size: 0.9em; font-style: italic;">72% ultra-high-strength steel, hot-formed steel in key areas</span></p>
                    </div>
                    
                    <div class="tech-feature-card">
                        <div class="tech-feature-icon">
                            <i class="fas fa-air-freshener"></i>
                        </div>
                        <h3>6安全气囊系统</h3>
                        <p>全方位保护驾驶员和乘客安全<br>
                        <span style="font-size: 0.9em; font-style: italic;">Comprehensive protection for driver and passengers</span></p>
                    </div>
                    
                    <div class="tech-feature-card">
                        <div class="tech-feature-icon">
                            <i class="fas fa-robot"></i>
                        </div>
                        <h3>高级驾驶辅助系统</h3>
                        <p>包含自适应巡航、车道保持等安全功能<br>
                        <span style="font-size: 0.9em; font-style: italic;">Includes adaptive cruise control, lane keeping assist</span></p>
                    </div>
                    
                    <div class="tech-feature-card">
                        <div class="tech-feature-icon">
                            <i class="fas fa-braille"></i>
                        </div>
                        <h3>智能安全监测</h3>
                        <p>360°全景影像 + 盲点监测系统<br>
                        <span style="font-size: 0.9em; font-style: italic;">360° camera + blind spot monitoring</span></p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- 顾问介绍 -->
    <section class="about-advisor">
        <div class="container">
            <div class="section-title">
                <h2>关于您的专属顾问<br><span style="font-size: 0.7em; display: block; margin-top: 10px;">About Your Personal Consultant</span></h2>
            </div>
            
            <div class="about-container">
                <div class="about-avatar">
                    <img src="https://i.ibb.co/39sJs9jN/Whats-App-Image-2025-07-12-at-12-30-16-Photoroom.png" alt="Brandon Lee Professional Advisor">
                </div>
                
                <div class="about-content">
                    <h2>Brandon Lee</h2>
                    <h3>汽车销售顾问<br><span style="font-size: 0.8em;">Sales Specialist</span></h3>
                    
                    <p>作为Ngu Motor Sdn Bhd（授权Proton e.MAS经销商）的专业顾问，我拥有丰富的电动汽车销售经验和专业知识。我致力于为客户提供省心又安心的购车体验，确保您获得最适合的Proton e.MAS配置和最优的购车方案。<br>
                    <span style="font-size: 0.9em; font-style: italic;">As a professional consultant at Ngu Motor Sdn Bhd (authorized Proton e.MAS dealer), I have extensive experience and expertise in electric vehicle sales. I'm committed to providing a hassle-free car buying experience, ensuring you get the most suitable Proton e.MAS configuration and the best purchase plan.</span></p>
                    
                    <p>我专注于：<br><span style="font-size: 0.9em; font-style: italic;">I specialize in:</span></p>
                    <ul style="list-style-type: none; padding-left: 20px;">
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 个性化购车方案定制<br><span style="font-size: 0.9em; font-style: italic;">Personalized car purchase solutions</span></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 政府电动车补贴申请<br><span style="font-size: 0.9em; font-style: italic;">Government EV subsidy applications</span></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 最优贷款方案匹配<br><span style="font-size: 0.9em; font-style: italic;">Optimal loan solution matching</span></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-gold); margin-right: 10px;"></i> 全流程购车指导<br><span style="font-size: 0.9em; font-style: italic;">Full-process car purchase guidance</span></li>
                    </ul>
                    
                    <div class="contact-info">
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-building"></i>
                            </div>
                            <div>
                                <strong>Ngu Motor Sdn Bhd</strong><br>
                                <a href="https://maps.app.goo.gl/Qv83T3CqxsTB27rs9" target="_blank" class="address-link">
                                    <i class="fas fa-map-marker-alt"></i> Lot 4019, Block 3, Jalan Ulu Oya<br>
                                    96000 Sibu, Sarawak
                                </a>
                            </div>
                        </div>
                        
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-phone"></i>
                            </div>
                            <div>+60 19-806 7373</div>
                        </div>
                        
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-envelope"></i>
                            </div>
                            <div>sa.brandon@ngumotor.com</div>
                        </div>

                        <!-- Facebook链接 -->
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fab fa-facebook-f"></i>
                            </div>
                            <div>
                                <a href="https://www.facebook.com/share/1EnvuS2A8h/?mibextid=wwXIfr" target="_blank" style="color: var(--professional-blue); text-decoration: none;">
                                    在Facebook上关注我<br>
                                    <span style="font-size: 0.9em; font-style: italic;">Follow Me on Facebook</span>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 行动号召表单 -->
    <section class="cta-section" id="cta">
        <div class="container">
            <h2 style="font-size: 2.2rem;">限时福利：先到先得<br><span style="font-size: 0.7em; display: block; margin-top: 10px;">Limited Time Offer: First Come, First Served</span></h2>
            <p style="font-size: 1.4rem; margin: 20px 0;">免费获得专属充电套装！<br><span style="font-size: 0.9em; font-style: italic;">Get Free Exclusive Charging Kit!</span></p>
            
            <div class="form-container">
                <form id="consultation-form">
                    <div class="form-group">
                        <label for="name">您的姓名 / Your Name</label>
                        <input type="text" id="name" required placeholder="例如：ADAM / e.g. ADAM">
                    </div>
                    
                    <div class="form-group">
                        <label for="phone">手机号码 / Phone Number</label>
                        <input type="tel" id="phone" required placeholder="例如：012-345 6789 / e.g. 012-345 6789">
                    </div>
                    
                    <div class="form-group">
                        <label for="model">感兴趣的车型 / Model Interested In</label>
                        <select id="model">
                            <option value="">请选择车型 / Please Select Model</option>
                            <option value="prime">e.MAS Prime</option>
                            <option value="premium">e.MAS Premium</option>
                            <option value="notsure">尚未决定 / Not Sure Yet</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="question">您最关心的问题 / Your Main Concern</label>
                        <textarea id="question" rows="3" placeholder="例如：贷款方案、政府补贴、充电设施等 / e.g. Loan options, government subsidies, charging facilities" style="width: 100%; padding: 15px; border: none; border-radius: 8px; font-size: 1rem; background: rgba(255,255,255,0.9);"></textarea>
                    </div>
                    
                    <button type="submit" class="btn" style="width: 100%; background: #FFB347; color: #333; font-weight: bold;">
                        <i class="fas fa-paper-plane"></i> 提交获取专属方案<br>
                        <span style="font-size: 0.8em;">Submit to Get Personalized Plan</span>
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- 页脚 -->
    <footer>
        <div class="container">
            <div class="footer-grid">
                <div class="contact-info-footer">
                    <h3>联系您的专属顾问<br><span style="font-size: 0.8em;">Contact Your Personal Consultant</span></h3>
                    <div class="contact-item-footer">
                        <div class="contact-icon-footer">
                            <i class="fas fa-user"></i>
                        </div>
                        <div>Brandon Lee</div>
                    </div>
                    <div class="contact-item-footer">
                        <div class="contact-icon-footer">
                            <i class="fas fa-phone"></i>
                        </div>
                        <div>+60 19-806 7373</div>
                    </div>
                    <div class="contact-item-footer">
                        <div class="contact-icon-footer">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <div>sa.brandon@ngumotor.com</div>
                    </div>
                    <div class="contact-item-footer">
                        <div class="contact-icon-footer">
                            <i class="fas fa-map-marker-alt"></i>
                        </div>
                        <div>
                            <a href="https://maps.app.goo.gl/Qv83T3CqxsTB27rs9" target="_blank" class="address-link">
                                <i class="fas fa-map-marker-alt"></i> Lot 4019, Block 3, Jalan Ulu Oya, 96000 Sibu, Sarawak
                            </a>
                        </div>
                    </div>
                    
                    <div class="social-links">
                        <a href="https://www.facebook.com/share/1EnvuS2A8h/?mibextid=wwXIfr" target="_blank" class="social-icon">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="https://wa.me/60198067373" target="_blank" class="social-icon">
                            <i class="fab fa-whatsapp"></i>
                        </a>
                        <a href="mailto:sa.brandon@ngumotor.com" class="social-icon">
                            <i class="fas fa-envelope"></i>
                        </a>
                    </div>
                </div>
                
                <div class="service-hours">
                    <h3>服务时间<br><span style="font-size: 0.8em;">Service Hours</span></h3>
                    <p>周一至周六: 8:00 AM - 6:00 PM<br><span style="font-size: 0.9em; font-style: italic;">Mon-Sat: 8:00 AM - 6:00 PM</span></p>
                    <p>周日: 10:00 AM - 5:00 PM<br><span style="font-size: 0.9em; font-style: italic;">Sun: 10:00 AM - 5:00 PM</span></p>
                    <p style="margin-top: 20px; color: #D4AF37;">
                        <i class="fas fa-exclamation-circle"></i> 紧急咨询可24小时致电<br>
                        <span style="font-size: 0.9em; font-style: italic;">Emergency Consultation Available 24/7</span>
                    </p>
                    
                    <h3 style="margin-top: 30px;">授权经销商<br><span style="font-size: 0.8em;">Authorized Dealer</span></h3>
                    <p>Ngu Motor Sdn Bhd</p>
                    <p>202401043297 (1589143-H)</p>
                    <p>Proton e.MAS 官方授权经销商<br>
                    <span style="font-size: 0.9em; font-style: italic;">Official Authorized Proton e.MAS Dealer</span></p>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2025 Brandon Lee - Proton e.MAS专业顾问 | 品质生活，触手可及<br>
                <span style="font-size: 0.9em; font-style: italic;">Brandon Lee - Proton e.MAS Professional Consultant | Quality Life Within Reach</span></p>
            </div>
        </div>
    </footer>

    <script>
        // 表单提交处理
        document.getElementById('consultation-form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // 表单验证
            const name = document.getElementById('name').value;
            const phone = document.getElementById('phone').value;
            
            if(!name || !phone) {
                alert('请填写姓名和手机号码 / Please fill in your name and phone number');
                return;
            }
            
            // 模拟提交成功
            alert(`感谢 ${name} 的咨询！我们将于15分钟内联系您（${phone}），请保持电话畅通。\nThank you for your inquiry, ${name}! We will contact you within 15 minutes (${phone}), please keep your phone available.`);
            this.reset();
        });
        
        // 滚动动画
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = 1;
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, {
            threshold: 0.1
        });
        
        // 观察所有需要动画的元素
        document.querySelectorAll('.timeline-item, .point-card, .vehicle-card, .tech-container, .motor-card, .tech-feature-card, .safety-badge').forEach(el => {
            el.style.opacity = 0;
            el.style.transform = 'translateY(30px)';
            el.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
            observer.observe(el);
        });
    </script>
</body>
</html>
