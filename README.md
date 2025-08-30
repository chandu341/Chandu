# Payroll System - Comprehensive Payroll Management

A modern, full-featured payroll management system built with React, TypeScript, and Tailwind CSS. This system provides role-based access control for administrators and employees, with comprehensive features for managing employee data, attendance tracking, salary calculations, and payslip generation.

## 🚀 Features

### Authentication & Role-Based Access
- **Administrator Access**: Complete system management capabilities
- **Employee Access**: Personal data and payslip viewing
- Secure login with demo accounts for testing

### Employee Management
- Add, edit, and delete employee records
- Store comprehensive employee information (personal details, position, department, salary)
- Professional employee listing with search and filter capabilities

### Attendance Tracking
- Manual attendance marking system
- Daily attendance status (Present, Late, Absent)
- Monthly attendance reports and statistics
- Attendance rate calculations

### Salary & Tax Management
- Automated salary calculations based on attendance
- Configurable tax rates for different employees
- Indian Rupee (₹) currency formatting
- Gross salary, tax deduction, and net salary calculations

### Payslip Generation
- Professional payslip design with company branding
- Detailed salary breakdown with tax information
- Print-ready format for physical copies
- PDF download capability (framework ready)

### Modern UI/UX
- Clean, professional interface design
- Responsive layout for desktop, tablet, and mobile
- Modern card-based layouts
- Smooth animations and hover effects
- Professional color scheme and typography

## 🛠️ Tech Stack

- **Frontend**: React 18, TypeScript, Tailwind CSS
- **Icons**: Lucide React
- **Build Tool**: Vite
- **Styling**: Modern CSS with gradients and animations
- **State Management**: React Context API
- **Data Persistence**: Local Storage (easily replaceable with backend)

## 📦 Installation & Setup

### Prerequisites
- Node.js (version 16 or higher)
- npm or yarn package manager

### Quick Start

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd payroll-system
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173` to access the application

## 👥 Demo Accounts

The system uses a secure email-based authentication system:

### First Time Setup
- When you first access the system, you'll be prompted to create an admin account
- This ensures secure access without default credentials
- The first registered user automatically becomes an administrator

### User Registration
- **Admin Registration**: Administrators can register new users (both admin and employee roles)
- **Role-Based Access**: Each user is assigned either Administrator or Employee role
- **Secure Authentication**: Passwords are hashed and stored securely

### Access Levels
- **Administrator Access**: Full system management, employee management, attendance tracking, payroll generation, user management
- **Employee Access**: Personal profile, attendance view, payslip access

## 🎯 Usage Guide

### Initial Setup

1. **First Visit**: Create your admin account when prompted
2. **User Management**: Add employee accounts through the User Management tab
3. **Employee Setup**: Add employee records with job details and salary information

### For Administrators

1. **Login** with your admin credentials
2. **Employee Management**: 
   - Add new employees with complete details
   - Edit existing employee information
   - Remove employees from the system
3. **Attendance Management**:
   - Mark daily attendance for all employees
   - View attendance statistics and reports
4. **Payroll Management**:
   - Generate monthly payslips for employees
   - View and download payslip reports
   - Monitor salary calculations and tax deductions
5. **User Management**:
   - Add new admin and employee user accounts
   - Manage user roles and permissions
   - Remove user accounts when needed

### For Employees

1. **Login** with employee credentials
2. **View Profile**: Check personal and job information
3. **Attendance Records**: View monthly attendance history and statistics
4. **Payslips**: Access and download generated payslips

## 🏗️ Project Structure

```
payroll-system/
├── src/
│   ├── components/           # React components
│   │   ├── Login.tsx        # Authentication component
│   │   ├── AdminDashboard.tsx
│   │   ├── EmployeeDashboard.tsx
│   │   ├── EmployeeList.tsx
│   │   ├── EmployeeForm.tsx
│   │   ├── AttendanceManagement.tsx
│   │   ├── AttendanceView.tsx
│   │   ├── PayrollReports.tsx
│   │   ├── PayslipView.tsx
│   │   ├── PayslipGenerator.tsx
│   │   └── UserManagement.tsx
│   ├── contexts/            # React Context providers
│   │   ├── AuthContext.tsx  # Authentication state
│   │   └── DataContext.tsx  # Application data state
│   ├── App.tsx             # Main application component
│   ├── App.css             # Global styles and animations
│   ├── index.css           # Tailwind CSS imports
│   └── main.tsx            # Application entry point
├── public/                 # Static assets
├── package.json           # Dependencies and scripts
├── tailwind.config.js     # Tailwind CSS configuration
├── vite.config.ts         # Vite build configuration
└── README.md              # Project documentation
```

## 🎨 Design Features

### Modern UI Elements
- **Gradient Backgrounds**: Professional blue-purple gradients
- **Card-Based Layout**: Clean, organized information display
- **Responsive Design**: Optimized for all screen sizes
- **Professional Typography**: Inter font family for readability
- **Smooth Animations**: Hover effects and transitions

### Color Scheme
- **Primary**: Blue (#2563eb) to Purple (#764ba2) gradients
- **Success**: Green (#059669) for positive actions
- **Warning**: Red (#dc2626) for alerts and deletions
- **Neutral**: Comprehensive gray scale for text and backgrounds

### Currency Formatting
- **Indian Rupee Symbol**: ₹ with proper formatting
- **Indian Number Format**: Comma separation following Indian standards
- **Consistent Display**: Uniform currency presentation across all components

## 🔐 Security Features

### Authentication Security
- **Password Hashing**: All passwords are hashed before storage
- **Role-Based Access Control**: Strict separation between admin and employee permissions
- **Session Management**: Secure user session handling
- **Input Validation**: Comprehensive validation for all user inputs

### Data Protection
- **Local Storage Encryption**: Sensitive data is properly formatted and stored
- **No Default Credentials**: System requires initial setup, no hardcoded passwords
- **User Management**: Admins can control user access and remove accounts

## 🔧 Customization

### Adding New Features
The modular architecture makes it easy to extend functionality:

1. **New Components**: Add to `src/components/`
2. **State Management**: Extend contexts in `src/contexts/`
3. **Styling**: Modify `src/App.css` for global styles
4. **Configuration**: Update `tailwind.config.js` for design tokens

### Backend Integration
The system is designed for easy backend integration:

1. Replace local storage with API calls in contexts
2. Add authentication tokens and session management
3. Implement real database connections
4. Add file upload capabilities for documents

## 🚀 Deployment

### Build for Production
```bash
npm run build
```

### Preview Production Build
```bash
npm run preview
```

The built files will be in the `dist/` directory, ready for deployment to any static hosting service.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🆘 Support

For support and questions:
- Email: support@payrollsystem.com
- Create an issue in the repository
- Check the documentation for common solutions

## 🔮 Future Enhancements

- **Backend Integration**: REST API with database
- **Advanced Reporting**: Charts and analytics
- **Email Notifications**: Automated payslip delivery
- **Mobile App**: React Native companion app
- **Multi-language Support**: Internationalization
- **Advanced Security**: Two-factor authentication
- **Bulk Operations**: CSV import/export functionality
- **LDAP Integration**: Enterprise directory services
- **Audit Logging**: Comprehensive activity tracking
- **Advanced Permissions**: Granular role-based permissions

---

**Payroll System** - Making payroll management simple, efficient, and professional.