# 🏥 CCTV Clinic Tracker - Multi-Portal System

A comprehensive college clinic management system with multiple portals for different user roles, featuring gate pass approvals, attendance tracking, and visit management.

## 🌟 Features

### Multi-Portal Access
- **👨‍⚕️ Clinic Portal** - Manage visits, attendance, and gate passes
- **👨‍🏫 Faculty Portal** - Review and track student visits
- **👨‍🎓 Student Portal** - Submit gate pass requests and view history
- **👔 HOD Portal** - Approve/decline gate pass requests

### Core Functionality
- ✅ Gate Pass Request & Approval System
- ✅ Digital Attendance Tracking
- ✅ Visit History Management
- ✅ Multi-role Authentication & Authorization
- ✅ Real-time Status Updates
- ✅ Responsive UI Design

## 🚀 Tech Stack

### Frontend
- HTML5, CSS3, JavaScript (Vanilla)
- Responsive Design
- AJAX for API communication

### Backend Options
- **Node.js** (Express.js + MongoDB + Mongoose)
- **Java** (Spring Boot 3.5.0 + MongoDB)

### Database
- MongoDB

### Deployment
- Vercel (Frontend & Node.js API)
- Render (Alternative deployment)

## 📁 Project Structure

```
CCTV-local-full/
├── cctv/                          # Main application directory
│   ├── index.html                 # Main portal page
│   ├── login-signup.html          # Authentication page
│   ├── script.js                  # Frontend logic
│   ├── styles.css                 # Styling
│   ├── server.js                  # Node.js backend
│   ├── db.js                      # MongoDB connection
│   ├── package.json               # Node dependencies
│   ├── models/                    # MongoDB models
│   │   ├── User.js
│   │   ├── Visit.js
│   │   ├── GatePass.js
│   │   ├── Attendance.js
│   │   └── Section.js
│   ├── server-java/               # Java Spring Boot backend
│   │   ├── pom.xml
│   │   └── src/
│   ├── scripts/                   # Database utilities
│   └── seed/                      # Seed data
├── vercel.json                    # Vercel configuration
├── render.yaml                    # Render configuration
└── Documentation/                 # Comprehensive guides
```

## 🛠️ Installation & Setup

### Prerequisites
- Node.js (v16+)
- MongoDB (local or Atlas)
- Java 21 (for Java backend)
- Maven (for Java backend)

### Quick Start (Node.js Backend)

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd CCTV-local-full/cctv
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment variables**
   Create a `.env` file in the `cctv` directory:
   ```env
   MONGO_URI=your_mongodb_connection_string
   PORT=8080
   ```

4. **Start the server**
   ```bash
   npm start
   ```

5. **Access the application**
   - Open browser: `http://localhost:8080`

### Java Backend Setup

1. **Navigate to Java server directory**
   ```bash
   cd cctv/server-java
   ```

2. **Configure application.properties**
   ```properties
   spring.data.mongodb.uri=your_mongodb_connection_string
   server.port=8081
   ```

3. **Build and run**
   ```bash
   mvn clean install
   java -jar target/clinic-server-0.0.1-SNAPSHOT.jar
   ```

## 🔐 Default Credentials

| Role    | Email                  | Password    |
|---------|------------------------|-------------|
| Clinic  | clinic@klh.edu.in      | clinic123   |
| Faculty | faculty@klh.edu.in     | faculty123  |
| Student | student@klh.edu.in     | student123  |
| HOD     | hod@klh.edu.in         | hod123      |

> ⚠️ **Change these in production!**

## 📚 Documentation

Comprehensive documentation is available in the project:

- **[00-START-HERE.md](cctv/00-START-HERE.md)** - Project overview
- **[HOW-TO-RUN-TEST.md](cctv/HOW-TO-RUN-TEST.md)** - Testing guide
- **[DOCUMENTATION-INDEX.md](cctv/DOCUMENTATION-INDEX.md)** - All documentation
- **[QUICK-REFERENCE.md](cctv/QUICK-REFERENCE.md)** - Quick commands
- **[API_DEBUG_GUIDE.md](cctv/API_DEBUG_GUIDE.md)** - Debugging help

## 🚀 Deployment

### Vercel Deployment
```bash
npm install -g vercel
vercel --prod
```

### Render Deployment
- Push to GitHub
- Connect repository to Render
- Deploy using `render.yaml` configuration

## 🧪 Testing

Run the complete test suite:
```bash
# Follow steps in HOW-TO-RUN-TEST.md
```

Test checklist includes:
- ✅ User authentication
- ✅ Gate pass creation
- ✅ Approval workflow
- ✅ Attendance tracking
- ✅ Multi-portal access

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- **Your Name** - *Initial work*

## 🙏 Acknowledgments

- Built for college clinic management
- Inspired by real-world healthcare tracking needs
- Designed for scalability and ease of use

## 📧 Support

For issues, questions, or contributions:
- Create an issue in the repository
- Contact: [your-email@example.com]

## 🔄 Version History

- **v1.0.0** - Initial release
  - Multi-portal system
  - Gate pass approval workflow
  - Attendance tracking
  - Dual backend support (Node.js + Java)

---

Made with ❤️ for efficient clinic management
