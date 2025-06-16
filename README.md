# Spaces - Accessible Tool Generator

An AI-powered web application that generates customized accessible digital tools from natural language descriptions. Built for social impact to help people with physical, cognitive, or technological barriers access digital tools.

## 🌟 Features

- **AI-Powered Generation**: Describe any tool you need in plain language and get a fully functional accessible tool
- **Voice Input**: Hands-free interaction with speech recognition
- **Template System**: 6 pre-built accessibility tool templates
- **WCAG 2.1 AA Compliant**: All generated tools follow accessibility best practices
- **Smart Fallback**: Demo tools when API quota is exceeded
- **Responsive Design**: Works on mobile, tablet, and desktop

## 🚀 Live Demo

The application automatically generates tools like:
- Voice-controlled daily planners
- Large-button timers with audio announcements
- Communication boards with text-to-speech
- Memory aids with visual and audio cues
- Accessible calculators
- Note-taking tools with speech-to-text

## 🛠️ Tech Stack

- **Frontend**: React 18, TypeScript, Tailwind CSS, shadcn/ui
- **Backend**: Node.js, Express, TypeScript
- **AI**: OpenAI GPT-4o for tool generation
- **Storage**: In-memory storage (easily configurable for PostgreSQL)
- **Build**: Vite for development and production

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/spaces-accessible-tools.git
cd spaces-accessible-tools
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
# Copy the example file
cp .env.example .env

# Add your OpenAI API key
OPENAI_API_KEY=your_openai_api_key_here
```

4. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

## 🔧 Configuration

### Environment Variables

- `OPENAI_API_KEY`: Your OpenAI API key for tool generation
- `NODE_ENV`: Set to `development` or `production`

### Database Setup (Optional)

The application uses in-memory storage by default. To use PostgreSQL:

1. Install PostgreSQL
2. Update the database configuration in `drizzle.config.ts`
3. Run migrations: `npm run db:push`

## 🏗️ Project Structure

```
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # UI components
│   │   ├── pages/          # Route pages
│   │   ├── hooks/          # Custom React hooks
│   │   └── lib/            # Utilities and configurations
├── server/                 # Express backend
│   ├── services/           # Business logic
│   └── routes.ts           # API endpoints
├── shared/                 # Shared types and schemas
└── public/                 # Static assets
```

## 🎯 Usage

### Basic Usage

1. **Describe Your Tool**: Type or speak what you need
   - "I need a large-button timer for cooking"
   - "Create a task planner I can control with my voice"

2. **Select Accessibility Needs**: Choose from:
   - Screen reader support
   - Voice control
   - High contrast colors
   - Large text options

3. **Choose Device Preference**: Mobile, desktop, or both

4. **Generate**: Get your custom accessible tool instantly

### Voice Input

Click the microphone button and speak your tool description. The application will convert your speech to text automatically.

### Template Examples

Choose from pre-built templates:
- Voice-Controlled Planner
- Visual Reminder System
- Accessible Calculator
- Voice Note Taker
- Communication Board
- Memory Aid Tool

## 🔒 API Keys

To use the full AI generation capabilities, you need an OpenAI API key:

1. Go to [OpenAI Platform](https://platform.openai.com/api-keys)
2. Create a new API key
3. Add it to your `.env` file or environment variables

**Note**: The application includes smart fallback demo tools when API quotas are exceeded.

## 🚀 Deployment

### Replit Deployment

This project is optimized for Replit:

1. Import the repository to Replit
2. Add your `OPENAI_API_KEY` as a secret
3. Run the project - it will automatically start

### Other Platforms

For other deployment platforms:

1. Build the project: `npm run build`
2. Start the server: `npm start`
3. Ensure environment variables are set

## 🤝 Contributing

We welcome contributions! Please:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes following our coding standards
4. Test your changes thoroughly
5. Submit a pull request

### Development Guidelines

- Follow TypeScript best practices
- Use Tailwind CSS for styling
- Ensure accessibility compliance (WCAG 2.1 AA)
- Add tests for new features
- Update documentation

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🌍 Social Impact

This project aims to make digital tools accessible to everyone, regardless of their abilities or technical knowledge. By using AI to generate customized accessible tools, we're breaking down barriers and creating a more inclusive digital world.

## 🙏 Acknowledgments

- Built with modern web technologies and accessibility in mind
- Inspired by the need for universal design in digital tools
- Thanks to the open-source community for excellent tools and libraries

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/yourusername/spaces-accessible-tools/issues) page
2. Create a new issue with detailed information
3. For security issues, please email directly

---

Built with ❤️ for accessibility and inclusion.
