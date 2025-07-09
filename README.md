<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Supreme Finance - Tailored Financial Solutions</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        :root {   
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --text-color: #333;
            --border-color: #ddd;
            --success-color: #27ae60;
            --whatsapp-green: #25D366;
            --facebook-blue: #1877F2;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f9f9f9;
            color: var(--text-color);
            line-height: 1.6;
            position: relative;
        }

        /* Header Styles */
        header {
            background-color: var(--primary-color);
            color: white;
            padding: 20px 0;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        .header-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            padding: 0 20px;
        }

        .logo-section {
            display: flex;
            align-items: center;
            gap: 20px;
        }

        #companyLogo {
            width: 80px;
            height: 80px;
            object-fit: contain;
            border: 2px solid var(--secondary-color);
            border-radius: 5px;
        }

        .company-info h1 {
            font-size: 28px;
            margin-bottom: 5px;
            color: white;
        }

        .tagline {
            font-style: italic;
            color: var(--light-color);
            font-size: 14px;
        }

        .contact-info {
            text-align: right;
        }

        .contact-info p {
            margin-bottom: 5px;
            font-size: 14px;
        }

        .social-icons {
            display: flex;
            justify-content: flex-end;
            gap: 10px;
            margin-top: 10px;
        }

        .social-icons a {
            color: white;
            font-size: 18px;
            transition: color 0.3s;
            display: flex;
            align-items: center;
            gap: 5px;
            text-decoration: none;
        }

        .social-icons a:hover {
            color: var(--secondary-color);
        }

        /* Navigation */
        nav {
            background-color: var(--secondary-color);
        }

        nav ul {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            list-style: none;
            padding: 0 20px;
        }

        nav li {
            flex: 1;
            text-align: center;
        }

        nav a {
            display: block;
            color: white;
            text-decoration: none;
            padding: 15px 10px;
            transition: background-color 0.3s;
        }

        nav a:hover {
            background-color: #2980b9;
        }

        nav i {
            margin-right: 8px;
        }

        /* Main Content */
        .main-container {
            max-width: 1200px;
            margin: 30px auto;
            display: flex;
            gap: 30px;
            padding: 0 20px;
        }

        .sidebar {
            flex: 0 0 300px;
        }

        .content-area {
            flex: 1;
        }

        /* Download Section */
        .download-section {
            background-color: white;
            border-radius: 5px;
            padding: 20px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
            margin-bottom: 20px;
        }

        .download-section h3 {
            color: var(--primary-color);
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 1px solid var(--border-color);
        }

        .form-list {
            list-style: none;
            margin-bottom: 20px;
        }

        .form-list li {
            margin-bottom: 10px;
        }

        .form-list a {
            display: block;
            padding: 10px;
            background-color: var(--light-color);
            color: var(--primary-color);
            text-decoration: none;
            border-radius: 4px;
            transition: background-color 0.3s;
        }

        .form-list a:hover {
            background-color: #d6eaf8;
        }

        .form-list i {
            margin-right: 10px;
            color: var(--accent-color);
        }

        /* Welcome Section */
        .welcome-section {
            background-color: white;
            border-radius: 5px;
            padding: 30px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
            margin-bottom: 30px;
            text-align: center;
        }

        .welcome-section h2 {
            color: var(--primary-color);
            margin-bottom: 15px;
        }

        .welcome-section p {
            margin-bottom: 25px;
            color: #555;
        }

        .cta-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
        }

        .primary-btn {
            background-color: var(--secondary-color);
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s;
        }

        .primary-btn:hover {
            background-color: #2980b9;
        }

        .secondary-btn {
            background-color: white;
            color: var(--secondary-color);
            border: 2px solid var(--secondary-color);
            padding: 12px 25px;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
            transition: all 0.3s;
        }

        .secondary-btn:hover {
            background-color: #f0f8ff;
        }

        /* Loan Calculator */
        .loan-calculator {
            background-color: white;
            border-radius: 5px;
            padding: 30px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
            margin-bottom: 30px;
        }

        .loan-calculator h3 {
            color: var(--primary-color);
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 1px solid var(--border-color);
        }

        .calculator-form {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
        }

        .loan-amount-slider {
            width: 100%;
            margin: 15px 0;
        }

        .loan-amount-values {
            display: flex;
            justify-content: space-between;
            margin-top: 5px;
            font-size: 14px;
            color: #555;
        }

        .current-amount {
            margin-top: 10px;
            font-weight: 600;
        }

        .fixed-term {
            padding: 10px;
            background-color: #f8f9fa;
            border-radius: 4px;
            text-align: center;
            font-weight: 600;
        }

        #calculateBtn {
            width: 100%;
        }

        .calculation-results {
            background-color: #f8f9fa;
            padding: 20px;
            border-radius: 4px;
            margin-top: 10px;
        }

        .result-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
            font-weight: 600;
        }

        .result-item span:first-child {
            color: #555;
        }

        /* Footer */
        footer {
            background-color: var(--primary-color);
            color: white;
            padding: 40px 0 20px;
        }

        .footer-container {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
            padding: 0 20px;
        }

        .footer-section {
            margin-bottom: 20px;
        }

        .footer-section h4 {
            margin-bottom: 20px;
            font-size: 18px;
            color: var(--light-color);
        }

        .footer-logo img {
            width: 100px;
            height: auto;
            margin-top: 15px;
        }

        .footer-section ul {
            list-style: none;
        }

        .footer-section li {
            margin-bottom: 10px;
        }

        .footer-section a {
            color: #bbb;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-section a:hover {
            color: white;
        }

        .footer-section p {
            margin-bottom: 10px;
            color: #bbb;
            font-size: 14px;
        }

        .footer-section i {
            margin-right: 8px;
            width: 20px;
            text-align: center;
        }

        .footer-social a {
            display: inline-block;
            margin-right: 10px;
            margin-bottom: 10px;
            padding: 8px 12px;
            border-radius: 4px;
            color: white;
            text-decoration: none;
        }

        .footer-social .whatsapp {
            background-color: var(--whatsapp-green);
        }

        .footer-social .facebook {
            background-color: var(--facebook-blue);
        }

        .footer-social .email {
            background-color: var(--secondary-color);
        }

        .copyright {
            text-align: center;
            padding-top: 20px;
            margin-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 14px;
            color: #bbb;
        }

        /* WhatsApp Float Button */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background-color: var(--whatsapp-green);
            color: white;
            padding: 15px 20px;
            border-radius: 50px;
            text-decoration: none;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            z-index: 100;
            display: flex;
            align-items: center;
            gap: 10px;
            font-weight: bold;
            transition: all 0.3s;
        }

        .whatsapp-float:hover {
            background-color: #128C7E;
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0,0,0,0.3);
        }

        .whatsapp-float i {
            font-size: 24px;
        }

        /* Responsive Design */
        @media (max-width: 992px) {
            .header-container {
                flex-direction: column;
                text-align: center;
            }
            
            .logo-section {
                flex-direction: column;
                margin-bottom: 20px;
            }
            
            .contact-info {
                text-align: center;
            }
            
            .social-icons {
                justify-content: center;
            }
            
            .main-container {
                flex-direction: column;
            }
            
            .sidebar {
                flex: 0 0 auto;
            }
            
            .footer-container {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
            }
            
            .cta-buttons {
                flex-direction: column;
            }

            .whatsapp-float {
                bottom: 20px;
                right: 20px;
                padding: 12px 15px;
                font-size: 14px;
            }
        }
    </style>
</head>
<body>
    <!-- WhatsApp Floating Button -->
    <a href="https://wa.me/67571547974" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i> Chat with Us
    </a>

    <header>
        <div class="header-container">
            <div class="logo-section">
                <img id="companyLogo" src="logo.png" alt="Supreme Finance Logo">
                <div class="company-info">
                    <h1>SUPREME FINANCE</h1>
                    <p class="tagline">Unleashing Your Financial Freedom through Tailored Financial Solutions</p>
                </div>
            </div>
            <div class="contact-info">
                <p><i class="fas fa-phone"></i> Phone: 77492090 / 71547974</p>
                <p><i class="fas fa-envelope"></i> Email: supremefinance24@gmail.com</p>
                <div class="social-icons">
                    <a href="https://wa.me/67571547974" target="_blank" title="Message us on WhatsApp">
                        <i class="fab fa-whatsapp"></i>
                    </a>
                    <a href="https://www.facebook.com/share/1CaVSzq2XD" target="_blank" title="Visit our Facebook page">
                        <i class="fab fa-facebook"></i>
                    </a>
                    <a href="mailto:supremefinance24@gmail.com" title="Send us an email">
                        <i class="fas fa-envelope"></i>
                    </a>
                </div>
            </div>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#"><i class="fas fa-home"></i> Home</a></li>
            <li><a href="#"><i class="fas fa-hand-holding-usd"></i> Loans</a></li>
            <li><a href="#"><i class="fas fa-file-alt"></i> Application Forms</a></li>
            <li><a href="#"><i class="fas fa-info-circle"></i> About Us</a></li>
            <li><a href="#"><i class="fas fa-envelope"></i> Contact</a></li>
        </ul>
    </nav>

    <div class="main-container">
        <aside class="sidebar">
            <div class="download-section">
                <h3><i class="fas fa-download"></i> Download Forms</h3>
                <ul class="form-list">
                    <li>
                        <a href="public-servants-loan-application.pdf" download="SupremeFinance_PublicServantsLoanApplication.pdf">
                            <i class="fas fa-file-pdf"></i> Public Servants Loan Application
                        </a>
                    </li>
                    <li>
                        <a href="teachers-loan-application.pdf" download="SupremeFinance_TeachersLoanApplication.pdf">
                            <i class="fas fa-file-pdf"></i> Teachers Loan Application
                        </a>
                    </li>
                    <li>
                        <a href="repayment-schedule.pdf" download="SupremeFinance_RepaymentSchedule.pdf">
                            <i class="fas fa-file-pdf"></i> Repayment Schedule
                        </a>
                    </li>
                    <li>
                        <a href="statec-form.pdf" download="SupremeFinance_StatecForm.pdf">
                            <i class="fas fa-file-pdf"></i> Statec Form
                        </a>
                    </li>
                    <li>
                        <a href="employee-deduction-advice.pdf" download="SupremeFinance_EmployeeDeductionAdvice.pdf">
                            <i class="fas fa-file-pdf"></i> Employee Deduction Advice
                        </a>
                    </li>
                </ul>
            </div>
        </aside>

        <main class="content-area">
            <section class="welcome-section">
                <h2>Online Loan Application</h2>
                <p>Complete our digital application form to apply for a loan with Supreme Finance. Our process is quick, secure, and designed to get you the financial solution you need.</p>
                <div class="cta-buttons">
                    <button id="startApplicationBtn" class="primary-btn"><i class="fas fa-rocket"></i> Start New Application</button>
                    <button id="continueDraftBtn" class="secondary-btn"><i class="fas fa-file-import"></i> Continue Draft</button>
                </div>
            </section>

            <section class="loan-calculator">
                <h3><i class="fas fa-calculator"></i> Loan Calculator</h3>
                <div class="calculator-form">
                    <div class="form-group">
                        <label for="loanAmount">Loan Amount (Kina)</label>
                        <input type="range" id="loanAmount" class="loan-amount-slider" min="500" max="5000" step="100" value="2500">
                        <div class="loan-amount-values">
                            <span>K500</span>
                            <span>K5,000</span>
                        </div>
                        <div class="current-amount">
                            Selected Amount: <span id="currentAmount">K2,500</span>
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label>Loan Term</label>
                        <div class="fixed-term">
                            20 Fortnights (10 months)
                        </div>
                    </div>
                    
                    <button id="calculateBtn" class="primary-btn"><i class="fas fa-calculator"></i> Calculate Repayments</button>
                    
                    <div class="calculation-results">
                        <div class="result-item">
                            <span>Fortnightly Repayment:</span>
                            <span id="fortnightlyPayment">K0.00</span>
                        </div>
                        <div class="result-item">
                            <span>Total Repayable:</span>
                            <span id="totalPayment">K0.00</span>
                        </div>
                    </div>
                </div>
            </section>
        </main>
    </div>

    <footer>
        <div class="footer-container">
            <div class="footer-section">
                <h4>Supreme Finance</h4>
                <p>Unleashing Your Financial Freedom through Tailored Financial Solutions</p>
                <div class="footer-logo">
                    <img id="footerLogo" src="logo.png" alt="Supreme Finance Logo">
                </div>
            </div>
            <div class="footer-section">
                <h4>Quick Links</h4>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Loan Products</a></li>
                    <li><a href="#">Application Process</a></li>
                    <li><a href="#">FAQ</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </div>
            <div class="footer-section">
                <h4>Contact Us</h4>
                <p><i class="fas fa-map-marker-alt"></i> PO BOX 1966, Boroko, Port Moresby, NCD, Papua New Guinea</p>
                <p><i class="fas fa-phone"></i> 77492090 / 71547974</p>
                <p><i class="fas fa-envelope"></i> supremefinance24@gmail.com</p>
                
                <div class="footer-social">
                    <a href="https://wa.me/67571547974" class="whatsapp" target="_blank">
                        <i class="fab fa-whatsapp"></i> WhatsApp
                    </a>
                    <a href="https://www.facebook.com/share/1CaVSzq2XD" class="facebook" target="_blank">
                        <i class="fab fa-facebook"></i> Facebook
                    </a>
                    <a href="mailto:supremefinance24@gmail.com" class="email">
                        <i class="fas fa-envelope"></i> Email
                    </a>
                </div>
            </div>
        </div>
        <div class="copyright">
            <p>&copy; 2025 Supreme Finance. All Rights Reserved.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Loan Calculator Functionality
            const loanAmountSlider = document.getElementById('loanAmount');
            const currentAmountDisplay = document.getElementById('currentAmount');
            const calculateBtn = document.getElementById('calculateBtn');
            const fortnightlyPaymentDisplay = document.getElementById('fortnightlyPayment');
            const totalPaymentDisplay = document.getElementById('totalPayment');
            
            // Update displayed amount when slider moves
            loanAmountSlider.addEventListener('input', function() {
                const amount = parseInt(this.value);
                currentAmountDisplay.textContent = 'K' + amount.toLocaleString();
            });
            
            // Calculate repayment when button clicked
            calculateBtn.addEventListener('click', function() {
                const amount = parseInt(loanAmountSlider.value);
                const term = 20; // Fixed at 20 fortnights
                
                if (amount < 500 || amount > 5000) {
                    alert('Please select an amount between K500 and K5,000');
                    return;
                }
                
                // Example calculation (replace with your actual formula)
                const totalRepayment = amount * 1.15; // 15% total cost
                const fortnightlyRepayment = totalRepayment / term;
                
                fortnightlyPaymentDisplay.textContent = 'K' + fortnightlyRepayment.toFixed(2);
                totalPaymentDisplay.textContent = 'K' + totalRepayment.toFixed(2);
            });
            
            // Application form toggle
            const startApplicationBtn = document.getElementById('startApplicationBtn');
            const continueDraftBtn = document.getElementById('continueDraftBtn');
            
            startApplicationBtn.addEventListener('click', function() {
                alert('Starting new application...');
                // In a real implementation, this would show the application form
            });
            
            continueDraftBtn.addEventListener('click', function() {
                alert('Loading saved draft...');
                // In a real application, this would load saved draft data
            });
        });
    </script>
</body>
</html>