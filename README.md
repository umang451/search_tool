# Research Tool

A powerful web-based research tool that helps you gather, analyze, and present information efficiently. This application uses AI-powered content generation, web crawling, and automatic presentation creation to streamline your research process.

## Features

- **Intelligent Web Crawling**: Automatically crawls relevant web pages to gather information about your research topic
- **AI-Powered Content Generation**: Uses Google's Gemini AI to generate comprehensive research summaries
- **Automatic Presentation Creation**: Generates PowerPoint presentations from your research findings
- **Data Persistence**: Stores research results using Supabase database
- **Modern React UI**: Clean and responsive user interface built with React and Vite

## Tech Stack

- **Frontend**: React.js with Vite
- **AI Integration**: Google Generative AI (Gemini)
- **Database**: Supabase
- **Web Crawling**: Crawlee
- **Presentation Generation**: pptxgenjs
- **Development**: TypeScript-ready environment

## Prerequisites

Before you begin, ensure you have:
- Node.js installed (v14 or higher)
- npm or yarn package manager
- A Supabase account and project
- A Google AI (Gemini) API key

## Setup

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory with the following variables:
   ```
   VITE_SUPABASE_URL=your_supabase_url
   VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
   VITE_GEMINI_API_KEY=your_gemini_api_key
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

## Usage

1. Enter your research query in the search box
2. Click "Search" to start the research process
3. The tool will:
   - Crawl relevant web pages
   - Generate an AI-powered summary
   - Create a downloadable presentation
   - Store the results in your Supabase database

## Project Structure

```
research_tool/
├── src/
│   ├── config/
│   │   ├── gemini.js       # Google Gemini AI configuration
│   │   ├── supabase.js     # Supabase client configuration
│   │   └── presentationGenerator.js
│   ├── utils/
│   │   └── presentationGenerator.js
│   ├── App.jsx            # Main application component
│   └── main.jsx          # Application entry point
├── supabase/
│   └── schema.sql        # Database schema
├── package.json
└── vite.config.js
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.