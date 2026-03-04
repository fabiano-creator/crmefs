@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Inter', sans-serif;
  font-size: 14px;
  line-height: 1.6;
  color: #2d3436;
  background: #f8f9fa;
}

/* Login Screen */
.login-screen {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  padding: 20px;
}

.login-container {
  background: white;
  border-radius: 20px;
  box-shadow: 0 20px 40px rgba(0,0,0,0.15);
  width: 100%;
  max-width: 420px;
  padding: 50px 40px;
  animation: fadeInUp 0.5s ease;
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.login-header {
  text-align: center;
  margin-bottom: 40px;
}

.login-icon {
  font-size: 48px;
  color: #667eea;
  margin-bottom: 20px;
  display: inline-block;
}

.login-header h1 {
  font-size: 28px;
  font-weight: 700;
  color: #2d3436;
  margin-bottom: 8px;
}

.login-header p {
  color: #636e72;
  font-size: 14px;
}

.login-form .form-group {
  margin-bottom: 24px;
}

.login-form label {
  display: block;
  font-weight: 500;
  margin-bottom: 8px;
  color: #2d3436;
}

.login-form label i {
  margin-right: 8px;
  color: #667eea;
}

.login-form input {
  width: 100%;
  padding: 14px 16px;
  border: 2px solid #e1e8ed;
  border-radius: 10px;
  font-size: 14px;
  transition: all 0.3s ease;
  font-family: inherit;
}

.login-form input:focus {
  outline: none;
  border-color: #667eea;
  box-shadow: 0 0 0 3px rgba(102, 126, 234, 0.1);
}

.login-info {
  text-align: center;
  margin-top: 20px;
  padding: 12px;
  background: #f8f9fa;
  border-radius: 8px;
}

.login-info small {
  color: #636e72;
}

/* Buttons */
.btn-primary {
  background: linear-gradient(135deg, #667eea 0%, #5568d3 100%);
  color: white;
  border: none;
  padding: 16px;
  border-radius: 10px;
  font-size: 16px;
  font-weight: 500;
  cursor: pointer;
  transition: all 0.3s ease;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
}

.btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}

/* Main App */
.main-app {
  display: flex;
  min-height: 100vh;
}

/* Sidebar */
.sidebar {
  width: 260px;
  background: linear-gradient(180deg, #1a1f36 0%, #2d3561 100%);
  color: white;
  position: fixed;
  height: 100vh;
  left: 0;
  top: 0;
  display: flex;
  flex-direction: column;
  box-shadow: 0 10px 25px rgba(0,0,0,0.1);
  z-index: 1000;
}

.sidebar-header {
  padding: 24px 20px;
  border-bottom: 1px solid rgba(255,255,255,0.1);
  display: flex;
  align-items: center;
  gap: 12px;
}

.sidebar-header i {
  font-size: 28px;
  color: #feca57;
}

.sidebar-title {
  font-size: 18px;
  font-weight: 700;
}

.sidebar-nav {
  flex: 1;
  padding: 20px 0;
  overflow-y: auto;
}

.nav-item {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 14px 24px;
  color: rgba(255,255,255,0.7);
  text-decoration: none;
  transition: all 0.3s ease;
  border-left: 3px solid transparent;
}

.nav-item:hover {
  background: rgba(255,255,255,0.05);
  color: white;
  border-left-color: #f093fb;
}

.nav-item.active {
  background: rgba(255,255,255,0.1);
  color: white;
  border-left-color: #feca57;
}

.nav-item i {
  font-size: 18px;
  width: 24px;
}

.sidebar-footer {
  padding: 20px;
  border-top: 1px solid rgba(255,255,255,0.1);
}

.btn-logout {
  width: 100%;
  background: rgba(255,255,255,0.1);
  color: white;
  border: 1px solid rgba(255,255,255,0.2);
  padding: 12px;
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.btn-logout:hover {
  background: rgba(255,255,255,0.15);
}

/* Main Content */
.main-content {
  flex: 1;
  margin-left: 260px;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.main-header {
  background: white;
  padding: 20px 30px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  box-shadow: 0 2px 4px rgba(0,0,0,0.05);
  position: sticky;
  top: 0;
  z-index: 100;
}

.menu-toggle {
  display: none;
  background: none;
  border: none;
  font-size: 24px;
  color: #2d3436;
  cursor: pointer;
}

.header-title h2 {
  font-size: 24px;
  font-weight: 600;
  color: #2d3436;
}

.header-user {
  display: flex;
  align-items: center;
  gap: 12px;
  color: #636e72;
}

.header-user i {
  font-size: 28px;
  color: #667eea;
}

.content-container {
  flex: 1;
  padding: 30px;
}

.page-content {
  display: none;
}

.page-content.active {
  display: block;
  animation: fadeIn 0.3s ease;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

/* Cards */
.card {
  background: white;
  border-radius: 12px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.07);
  margin-bottom: 24px;
  overflow: hidden;
}

.card-header {
  padding: 20px 24px;
  border-bottom: 1px solid #e1e8ed;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.card-header h3 {
  font-size: 18px;
  font-weight: 600;
  color: #2d3436;
  display: flex;
  align-items: center;
  gap: 10px;
}

.card-header h3 i {
  color: #667eea;
}

/* Dashboard Cards */
.dashboard-cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  margin-bottom: 30px;
}

.metric-card {
  display: flex;
  align-items: center;
  gap: 20px;
  padding: 24px !important;
}

.card-icon {
  width: 64px;
  height: 64px;
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 28px;
  color: white;
  flex-shrink: 0;
}

.metric-card .card-content {
  padding: 0;
}

.metric-card h3 {
  font-size: 14px;
  font-weight: 500;
  color: #636e72;
  margin-bottom: 8px;
}

.metric-value {
  font-size: 28px;
  font-weight: 700;
  color: #2d3436;
  margin-bottom: 4px;
}

.metric-subtitle {
  font-size: 12px;
  color: #b2bec3;
}

/* Responsive */
@media (max-width: 968px) {
  .sidebar {
    transform: translateX(-100%);
    transition: transform 0.3s ease;
  }
  
  .sidebar.active {
    transform: translateX(0);
  }
  
  .main-content {
    margin-left: 0;
  }
  
  .menu-toggle {
    display: block;
  }
  
  .dashboard-cards {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 640px) {
  .content-container {
    padding: 16px;
  }
  
  .main-header {
    padding: 16px 20px;
  }
  
  .header-title h2 {
    font-size: 18px;
  }
  
  .login-container {
    padding: 40px 30px;
  }
}
