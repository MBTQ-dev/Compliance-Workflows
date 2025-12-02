# Magician Platform: Advanced TypeScript Framework for VR4deaf Organizations

Magician Platform is an advanced TypeScript-based framework designed to streamline development workflows for innovative technology solutions. Leveraging cutting-edge integration tools, it enables seamless deployment and management of scalable systems tailored for developers and organizations, specifically designed to solve complex infrastructure and collaboration challenges for the Magicians system serving VR4deaf organizations' deaf customers.

![Magician Platform](https://business.360magicians.com)

## 🎯 Mission

This platform aims to provide comprehensive solutions for deaf entrepreneurs and VR4deaf organizations, offering:
- Streamlined business formation workflows
- Accessible interfaces with ASL support
- Integration with Vocational Rehabilitation (VR) services
- Scalable infrastructure for multiple projects

## 🚀 Features

### Core Magician Services
- **Business Magician**: Complete business formation and lifecycle support
- **Developer Magician**: Code scaffolding, tech recommendations, and development tools
- **Creative Magician**: Branding, ASL video production, and marketing solutions
- **Job Magician**: Resume building, job matching, and career development

### Accessibility & Integration
- **ASL Video Guidance**: Accessible content in American Sign Language
- **VR Counselor Integration**: Connect with Vocational Rehabilitation specialists
- **Real-time Translation Services**: Communication accessibility tools
- **Deaf-first Design**: All interfaces optimized for deaf users

### Business Tools
- **Document Management**: Storage and organization for business documents
- **Self-Employment Service Modules**: Comprehensive pricing tools
- **SBA Resource Library**: Access to Small Business Administration resources
- **AI-Powered Business Analytics**: Intelligent business planning and analysis

## 🔧 Technologies

- **Frontend**: React + TypeScript with Shadcn/UI components
- **Backend**: Express.js with TypeScript
- **Database**: PostgreSQL with Drizzle ORM
- **Dynamic Interactions**: HTMX for seamless UX
- **Cloud Storage**: Google Cloud Storage & Cloudflare R2 integration
- **Messaging**: Telegram bot and Slack integration
- **AI Services**: OpenAI & Anthropic integration
- **Deployment**: Vercel, Cloud Run, and Cloudflare Pages

## 📋 Requirements

- Node.js 20+
- PostgreSQL database (or use Docker)
- Google Cloud Storage account (for document storage)
- OpenAI API key (for AI features)

## 🏁 Getting Started

### Quick Start

1. Clone the repository
2. Run setup script:
   ```bash
   node scripts/setup.js
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

### Docker Setup

We provide a Docker Compose configuration for easy local development:

```bash
docker-compose up -d
```

Visit http://localhost:8080 to see the application.

## 🗄️ Environment Variables

Create a `.env` file in the project root with the following variables:

```
# Database connection
DATABASE_URL=postgres://username:password@localhost:5432/business_magician

# Google Cloud Storage
GOOGLE_CLOUD_PROJECT_ID=your-project-id
GOOGLE_CLOUD_BUCKET_NAME=your-bucket-name
GOOGLE_APPLICATION_CREDENTIALS=path-to-credentials.json

# OpenAI
OPENAI_API_KEY=your-openai-api-key

# Application settings
NODE_ENV=development
PORT=5000
```

## 📂 Project Structure

```
├── client/                  # Frontend React application
│   ├── src/
│   │   ├── components/      # UI components
│   │   ├── hooks/           # Custom React hooks
│   │   ├── lib/             # Utilities and API clients
│   │   ├── pages/           # Page components
├── server/                  # Backend Express application
│   ├── routes/              # API routes
│   ├── services/            # Business logic
│   ├── index.ts             # Server entry point
├── shared/                  # Shared code between client and server
│   ├── schema.ts            # Database schema definitions
├── scripts/                 # Utility scripts
```

## 🔄 Database Management

We use Drizzle ORM for database operations. Some useful commands:

```bash
# Push schema changes to database
npm run db:push

# Generate migration files
npm run db:generate

# Open Drizzle Studio (database UI)
npm run db:studio
```

## 📦 Deployment

The application is configured for deployment on Vercel:

```bash
node scripts/vercel-deploy.js
```

## 🤝 Contributing

Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on contributing to this project.

## 📄 License

[MIT License](LICENSE)

## 👥 Team

- 360 Magician Team
- VR4deaf Organization Partners

## 🔗 Related Documentation

- [Platform Integration Summary](PLATFORM-INTEGRATION-SUMMARY.md)
- [Implementation Plan](implementation-plan.md)
- [API Definition](api-definition.md)
- [GCP/Vercel Deployment Guide](gcp-vercel-deployment.md)
- [Repository Template](GITHUB-REPOSITORY-TEMPLATE.md)