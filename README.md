# 🍔 Swiggy Clone

![Status](https://img.shields.io/badge/Status-Active-success)
![React](https://img.shields.io/badge/React-18.x-61DAFB?logo=react)
![Vite](https://img.shields.io/badge/Vite-5.x-646CFF?logo=vite)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.x-38B2AC?logo=tailwind-css)
![JavaScript](https://img.shields.io/badge/JavaScript-93.8%25-yellow)

A fully functional food delivery application clone inspired by Swiggy, built with modern web technologies. This project demonstrates proficiency in React, Vite, TailwindCSS, and DevOps practices.

## 🌟 Features

- **🏠 Home Page**: Browse restaurants and food items with an intuitive interface
- **🔍 Search Functionality**: Search for restaurants, cuisines, and dishes
- **🛒 Shopping Cart**: Add items to cart with real-time updates
- **🍽️ Restaurant Menu**: Detailed restaurant pages with menu items
- **📱 Responsive Design**: Fully responsive UI that works on all devices
- **⚡ Fast Performance**: Built with Vite for lightning-fast hot module replacement
- **🎨 Modern UI/UX**: Styled with TailwindCSS for a clean, modern look
- **🐳 Dockerized**: Easy deployment with Docker and Docker Compose
- **🔄 CI/CD Pipeline**: Automated build and deployment with Jenkins

## 🛠️ Technologies Used

### Frontend
- **React 18.x**: Component-based UI library
- **Vite**: Next-generation frontend build tool
- **TailwindCSS**: Utility-first CSS framework
- **JavaScript (ES6+)**: Modern JavaScript features
- **ESLint**: Code quality and consistency

### DevOps & Deployment
- **Docker**: Containerization
- **Docker Compose**: Multi-container orchestration
- **Jenkins**: CI/CD automation
- **Nginx**: Web server (in production)

### Database
- **SQL**: Database for storing application data

## 📁 Project Structure

```
swiggy-clone/
├── public/                 # Static assets
├── src/                    # Source files
│   ├── components/         # React components
│   ├── pages/             # Page components
│   ├── utils/             # Utility functions
│   ├── assets/            # Images, icons, etc.
│   ├── App.jsx            # Main App component
│   └── main.jsx           # Entry point
├── Dockerfile             # Docker configuration
├── docker-compose.yaml    # Docker Compose setup
├── Jenkinsfile           # Jenkins pipeline
├── init.sql              # Database initialization
├── tailwind.config.js    # Tailwind configuration
├── vite.config.js        # Vite configuration
├── eslint.config.js      # ESLint configuration
├── package.json          # Dependencies
└── README.md             # Documentation
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- Docker (optional, for containerized deployment)
- Git

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/Ankitpandey321/swiggy-clone.git
   cd swiggy-clone
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. **Open your browser**
   - Navigate to `http://localhost:5173`

### Building for Production

```bash
npm run build
# or
yarn build
```

The production-ready files will be in the `dist` directory.

### Preview Production Build

```bash
npm run preview
# or
yarn preview
```

## 🐳 Docker Deployment

### Using Docker Compose

1. **Build and run the application**
   ```bash
   docker-compose up --build
   ```

2. **Access the application**
   - Navigate to `http://localhost:80`

### Using Docker

1. **Build the Docker image**
   ```bash
   docker build -t swiggy-clone .
   ```

2. **Run the container**
   ```bash
   docker run -p 80:80 swiggy-clone
   ```

## 🔄 CI/CD Pipeline

This project includes a Jenkins pipeline configuration for automated:
- Code linting and quality checks
- Building the application
- Running tests
- Creating Docker images
- Deploying to production

## 📊 Database Setup

Initialize the database using the provided SQL script:

```bash
# For MySQL/PostgreSQL
mysql -u username -p database_name < init.sql
# or
psql -U username -d database_name -f init.sql
```

## 🎨 Customization

### Tailwind Configuration

Modify `tailwind.config.js` to customize:
- Colors
- Fonts
- Spacing
- Breakpoints
- And more...

### Vite Configuration

Edit `vite.config.js` to configure:
- Build options
- Plugins
- Development server settings

## 📱 Features Breakdown

### Home Page
- Restaurant listings with images and ratings
- Popular cuisines carousel
- Search bar for quick access
- Filter options (rating, delivery time, cost)

### Restaurant Page
- Restaurant details (name, cuisine, ratings)
- Menu categorization
- Add to cart functionality
- Special offers and discounts

### Cart
- View all added items
- Update quantities
- Remove items
- Calculate total with taxes

## 🧪 Running Tests

```bash
npm run test
# or
yarn test
```

## 📈 Performance Optimization

- **Code Splitting**: Dynamic imports for route-based code splitting
- **Lazy Loading**: Images and components loaded on demand
- **Caching**: Service worker implementation for offline support
- **Minification**: Production builds are minified and optimized

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Code Style

This project uses ESLint for code quality. Run the linter:

```bash
npm run lint
# or
yarn lint
```

## 🐛 Known Issues

- None at the moment. Please report issues in the GitHub repository.

## 🔮 Future Enhancements

- [ ] User authentication and authorization
- [ ] Payment gateway integration
- [ ] Order tracking system
- [ ] Restaurant partner dashboard
- [ ] Real-time notifications
- [ ] Delivery location tracking
- [ ] Review and rating system
- [ ] Favorites and order history

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Ankit Pandey**

- GitHub: [@Ankitpandey321](https://github.com/Ankitpandey321)
- Project Repository: [swiggy-clone](https://github.com/Ankitpandey321/swiggy-clone)

## 🙏 Acknowledgments

- Inspired by [Swiggy](https://www.swiggy.com)
- Built as a learning project to demonstrate full-stack development skills
- Thanks to the React, Vite, and TailwindCSS communities

## 📞 Support

If you have any questions or need help, please:
- Open an issue in the GitHub repository
- Contact me through GitHub

---

⭐ **If you found this project helpful, please give it a star!**

## 📸 Screenshots

> Add screenshots of your application here to showcase the UI

### Home Page
![Home Page](#)

### Restaurant Menu
![Restaurant Menu](#)

### Shopping Cart
![Shopping Cart](#)

---

**Note**: This is a clone project built for educational purposes. All rights to the original Swiggy brand and design belong to their respective owners.
