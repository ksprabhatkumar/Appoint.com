# Appoint.com - Appointment Booking System

A modern, full-stack appointment booking platform built with Next.js that allows users to create business services and manage appointments seamlessly.

## 🚀 Features

### User Management
- **User Registration & Authentication**: Secure user registration and login system
- **Social Login**: Integration with GitHub and Google OAuth providers
- **User Profiles**: Personalized user accounts with profile management

### Business Management
- **Business Creation**: Users can create and manage their own service businesses
- **Service Listings**: Comprehensive service catalog with detailed descriptions
- **Business Dashboard**: Dedicated interface for business owners to manage their services

### Appointment System
- **Appointment Booking**: Users can book appointments with preferred date and time
- **Real-time Availability**: Dynamic calendar showing available time slots
- **Appointment Management**: View, modify, and cancel appointments

### User Dashboard
- **Upcoming Appointments**: View all scheduled appointments
- **Reservation Management**: Business owners can manage customer reservations
- **Business Overview**: Comprehensive view of business services and bookings

### Search & Discovery
- **Location-based Search**: Find services by geographic location
- **Category Filtering**: Filter services by business categories
- **Advanced Search**: Comprehensive search functionality

### Responsive Design
- **Mobile-first**: Optimized for all device sizes
- **Modern UI**: Clean, intuitive user interface
- **Accessibility**: WCAG compliant design

## 🛠️ Tech Stack

- **Frontend**: Next.js 13 with App Router, React 18, TypeScript
- **Styling**: Tailwind CSS, CSS Modules
- **Authentication**: NextAuth.js with multiple providers
- **Database**: MongoDB with Prisma ORM
- **Image Handling**: Cloudinary integration
- **Maps**: React Leaflet for location services
- **Forms**: React Hook Form for form management
- **Date Handling**: React Date Range, Date-fns
- **UI Components**: React Icons, React Spinners, React Hot Toast

## 📦 Installation

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- MongoDB database
- Git

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd SE_Project
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   Create a `.env` file in the root directory:
   ```env
   DATABASE_URL="your-mongodb-connection-string"
   NEXTAUTH_SECRET="your-nextauth-secret"
   NEXTAUTH_URL="http://localhost:3000"
   
   # OAuth Providers
   GITHUB_ID="your-github-client-id"
   GITHUB_SECRET="your-github-client-secret"
   GOOGLE_CLIENT_ID="your-google-client-id"
   GOOGLE_CLIENT_SECRET="your-google-client-secret"
   
   # Cloudinary (for image uploads)
   NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME="your-cloudinary-cloud-name"
   ```

4. **Database Setup**
   ```bash
   npx prisma generate
   npx prisma db push
   ```

5. **Start Development Server**
   ```bash
   npm run dev
   ```

   The application will be available at `http://localhost:3000`

## 🏗️ Project Structure

```
├── app/                    # Next.js App Router
│   ├── actions/           # Server actions
│   ├── api/               # API routes
│   ├── components/        # React components
│   ├── hooks/             # Custom React hooks
│   ├── libs/              # Utility libraries
│   └── providers/         # Context providers
├── pages/                 # NextAuth configuration
├── prisma/                # Database schema and migrations
├── public/                # Static assets
└── @types/                # TypeScript type definitions
```

## 🔧 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

## 🗄️ Database Schema

The application uses MongoDB with Prisma ORM. Key models include:

- **User**: User authentication and profile data
- **Account**: OAuth account linking
- **Business**: Business service information
- **Reservation**: Appointment booking data

## 🔐 Authentication

Authentication is handled by NextAuth.js with support for:
- Email/Password credentials
- GitHub OAuth
- Google OAuth

## 🎨 Styling

The application uses Tailwind CSS for styling with:
- Responsive design utilities
- Custom CSS classes in [`globals.css`](app/globals.css)
- Tailwind configuration in [`tailwind.config.js`](tailwind.config.js)

## 🚀 Deployment

The application is configured for deployment on Vercel:

1. Connect your GitHub repository to Vercel
2. Set environment variables in Vercel dashboard
3. Deploy automatically on push to main branch

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For support and questions, please open an issue in the GitHub repository.

---

Built with ❤️ using Next.js and modern web technologies.
