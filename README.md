# GitHub Batch Upload Tool with AI Documentation

A comprehensive web application that streamlines the process of uploading multiple files to GitHub while automatically generating professional documentation using AI.

## Description

This tool provides a complete workflow for developers who want to quickly set up a new GitHub repository with proper documentation. It allows you to:

1. Configure your GitHub repository and AI model settings
2. Upload multiple source files to the application
3. Generate comprehensive documentation (README.md, CONTRIBUTING.md, LICENSE, .gitignore, CHANGELOG.md) using AI
4. Preview and edit all files before committing
5. Upload everything to GitHub in a single operation

The application uses OpenRouter's AI models to analyze your source code and generate contextually relevant documentation.

## Features

### 🚀 Core Functionality
- **Batch file upload** - Upload multiple files at once
- **AI-powered documentation generation** - Automatically creates professional documentation
- **Repository validation** - Tests GitHub connection and repository access
- **Content preview and editing** - Review and modify files before upload
- **Progress tracking** - Visual progress bars for all operations
- **Comprehensive logging** - Detailed status messages throughout the process

### 📚 Documentation Generation
- **README.md** - Project overview and instructions
- **CONTRIBUTING.md** - Guidelines for contributors
- **LICENSE** - Open source license text
- **.gitignore** - Git ignore patterns for your tech stack
- **CHANGELOG.md** - Version history tracking

### 🔧 Technical Features
- **Multiple AI model support** - Works with any OpenRouter-compatible model
- **Base64 file encoding** - Proper handling of binary and text files
- **Error handling** - Comprehensive error messages and recovery
- **Responsive design** - Works on desktop and mobile devices
- **Secure token handling** - Local processing of sensitive credentials

## File Structure

The application is a single HTML file (`version1(patch-fixed).html`) that contains:

- **HTML Structure** - Complete user interface with step-by-step workflow
- **CSS Styling** - Modern, responsive design with GitHub-inspired aesthetics
- **JavaScript Logic** - All functionality including file handling, AI integration, and GitHub API calls

### Key Components

1. **Configuration Card** (`config-card`) - Set up GitHub tokens, AI model, and repository details
2. **Upload Card** (`upload-card`) - Select and process files for upload
3. **AI Generation Card** (`ai-card`) - Configure AI documentation generation
4. **Preview Card** (`preview-card`) - Review and edit all files before upload
5. **Log Card** (`log-card`) - View detailed status messages

## Getting Started

### Prerequisites

1. **GitHub Personal Access Token** with `repo` scope
2. **OpenRouter API Key** (free tier available)
3. **Existing GitHub Repository** (must be created manually before using the tool)
4. **Source files** you want to upload

### Setup Instructions

1. **Download the Application**
   ```bash
   # Download the HTML file
   curl -O https://raw.githubusercontent.com/your-repo/version1(patch-fixed).html
   ```

2. **Open in Browser**
   - Double-click the HTML file or open it in any modern web browser
   - No server setup required - it runs entirely in the browser

3. **Configure Settings** (Step 1)
   - Enter your GitHub Personal Access Token
   - Enter your OpenRouter API Key
   - Specify your preferred AI model ID (default: `mistralai/mistral-7b-instruct:free`)
   - Provide your existing repository URL
   - Set target branch and commit message

4. **Upload Files** (Step 2)
   - Select the files you want to upload
   - Click "Upload Files to App" to process them

5. **Generate Documentation** (Step 3)
   - Describe your project purpose, target audience, and tech stack
   - Add any custom instructions for the AI
   - Click "Generate Documentation"

6. **Review and Upload** (Step 4)
   - Preview all files and generated documentation
   - Edit any content as needed
   - Click "Upload All to GitHub" to commit everything

### Configuration Options

#### AI Models
The tool supports any OpenRouter-compatible model. Some popular options:

- `mistralai/mistral-7b-instruct:free` - Free, good for basic documentation
- `openai/gpt-3.5-turbo` - Fast and affordable
- `openai/gpt-4` - Most capable, higher cost
- `anthropic/claude-3-sonnet` - Excellent for technical writing

#### GitHub Repository Requirements
- Repository must exist before using the tool
- Your PAT must have access to the repository
- Target branch must exist (default: `main`)

### Security Notes

- All file processing happens locally in your browser
- API keys are stored only in memory during the session
- No files are uploaded to external servers (except your final GitHub repository)
- Always use a secure connection (HTTPS) when possible

### Troubleshooting

**Common Issues:**

1. **Repository not found**: Ensure the repository exists and your token has access
2. **AI generation fails**: Check your OpenRouter API key and model ID
3. **File upload errors**: Verify files are not too large (recommended under 10MB each)
4. **Authentication errors**: Double-check your GitHub PAT has the `repo` scope

**Error Messages:**
- Red alerts indicate errors that must be resolved
- Green alerts confirm successful operations
- The log panel provides detailed technical information

The application is designed to be self-contained and requires no additional dependencies or server setup.