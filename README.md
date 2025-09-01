# AI Study Buddy 🚀

A comprehensive AI-powered learning companion with document analysis, image processing, and personalized study assistance capabilities.

## 🌟 Features

### Core Capabilities
- **Multi-Modal Learning Support**: Text, PDF, and image analysis
- **Context-Aware Conversations**: Maintains conversation history and adapts to learning patterns
- **Document Summarization**: PDF processing with educational summaries
- **Study Material Generation**: Flashcards, quizzes, and study outlines
- **Image Analysis**: Educational image interpretation and analysis
- **Multi-Student Support**: Separate memory and context for different student personas

### Advanced Features
- **Real-time WebSocket Communication**: Instant responses and typing indicators
- **Markdown Rendering**: Rich text formatting with mathematical expressions
- **Diagram Visualization**: Enhanced display for scientific and mathematical diagrams
- **Progress Tracking**: Document processing with visual progress indicators
- **Responsive Design**: Modern, tech-themed UI with glassmorphism effects

## 🏗️ Architecture

### Backend Components
- **FastAPI Server** (`ui/backend_server.py`): WebSocket-based API server
- **Study Buddy Agent** (`study_buddy_agent_phase6.py`): Core AI agent with Bedrock integration
- **Tool System**: Modular tools for various educational tasks

### Frontend
- **Modern Web UI** (`ui/web_ui_connected.html`): Single-page application with real-time features
- **Tech-themed Design**: Cyan/blue gradient theme with Nunito fonts
- **Responsive Layout**: Sidebar navigation with main chat interface

## 🛠️ Tools & Integrations

### Educational Tools
1. **Calculator** - Mathematical expression evaluation
2. **Web Search** - Current information and news
3. **Academic Search** - Educational resources and academic content
4. **Study Planner** - Personalized study plan creation
5. **Progress Analyzer** - Learning progress analysis and recommendations

### Document Processing
6. **PDF Processor** - Text extraction from PDF documents
7. **Document Summarizer** - Educational summary generation
8. **Study Material Generator** - Flashcards, quizzes, and outlines
9. **File Handler** - Document storage and retrieval

### Media Analysis
10. **Image Analyzer** - Educational image analysis with custom prompts
11. **Memory Manager** - Student information and adaptive recommendations

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- AWS Account with Bedrock access
- Required Python packages (see installation)

### Installation

1. **Clone the repository**
```bash
git clone <repository-url>
cd strand-bedrock-agent
```

2. **Install dependencies**
```bash
pip install fastapi uvicorn websockets strands boto3 python-dotenv
pip install pdfplumber PyPDF2  # For PDF processing
```

3. **Set up environment variables**
Create a `.env` file:
```env
AWS_REGION=us-east-1
AWS_ACCESS_KEY_ID=your_access_key
AWS_SECRET_ACCESS_KEY=your_secret_key
```

4. **Run the application**
```bash
python3 ui/backend_server.py
```

5. **Access the interface**
Open `http://localhost:8003` in your browser

## 📱 Usage

### Student Management
- **Change Student ID**: Click "Change Student ID" button in sidebar
- **Multiple Personas**: Each student ID maintains separate memory and context
- **Context Persistence**: Conversation history and learning preferences saved per student

### Document Analysis
1. Click PDF button or drag-and-drop PDF files
2. Select summary type (Comprehensive, Quick, Study Guide)
3. Generate study materials from summaries

### Image Analysis
1. Click image button to upload images
2. Add custom analysis prompts
3. Get educational insights and explanations

### Chat Interface
- **Markdown Support**: Rich text formatting in responses
- **Emoji Integration**: Emotional expressions in AI responses
- **Real-time Feedback**: Typing indicators and progress bars

## 🎨 UI Features

### Design Elements
- **Modern Typography**: Nunito font family for readability
- **Tech Theme**: Cyan/blue gradient color scheme
- **Glassmorphism**: Backdrop blur effects and transparency
- **Responsive Layout**: Adapts to different screen sizes

### Interactive Components
- **Gradient Buttons**: Hover effects and smooth transitions
- **Animated Icons**: Scale effects on hover
- **Progress Indicators**: Visual feedback for long operations
- **Status Indicators**: Connection status and document counts

## 🧠 AI Capabilities

### Context Awareness
- **Conversation Memory**: Maintains chat history per student
- **Learning Style Detection**: Adapts to student preferences
- **Topic Tracking**: Connects related concepts across sessions
- **Document Context**: References uploaded documents in conversations

### Response Features
- **Markdown Formatting**: Structured, readable responses
- **Emoji Integration**: Emotional expressions when appropriate
- **Code Highlighting**: Syntax highlighting for technical content
- **Mathematical Rendering**: MathJax support for equations

## 📁 File Structure

```
strand-bedrock-agent/
├── ui/
│   ├── backend_server.py          # FastAPI WebSocket server
│   └── web_ui_connected.html      # Frontend interface
├── tools/                         # Educational tool modules
│   ├── calculator.py
│   ├── web_search.py
│   ├── pdf_processor.py
│   ├── document_summarizer.py
│   ├── image_analyzer_base64.py
│   ├── memory_manager.py
│   └── file_handler.py
├── study_buddy_agent_phase6.py    # Main AI agent
└── README.md                      # This file
```

## 🔧 Configuration

### Model Settings
- **Model**: Claude 3 Sonnet (Anthropic via AWS Bedrock)
- **Region**: US East 1
- **Context Window**: Optimized for educational conversations

### Memory Management
- **Conversation History**: Last 20 exchanges per student
- **Context Summary**: Last 5 exchanges for immediate context
- **Document Storage**: Persistent summary storage with retrieval

## 🚨 Troubleshooting

### Common Issues
1. **WebSocket Connection**: Check server is running on port 8003
2. **AWS Credentials**: Verify Bedrock access and credentials
3. **PDF Processing**: Ensure PDF files are under 50MB
4. **Image Upload**: Check image format compatibility

### Debug Features
- **Server Logs**: Detailed logging for troubleshooting
- **Connection Status**: Real-time connection indicators
- **Error Messages**: User-friendly error reporting

## 🔮 Future Enhancements

### Planned Features
- **Voice Integration**: Speech-to-text and text-to-speech
- **Advanced Analytics**: Learning progress visualization
- **Collaborative Features**: Multi-student study sessions
- **Mobile App**: Native mobile application
- **Plugin System**: Extensible tool architecture

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📞 Support

For issues and questions:
- Create an issue in the repository
- Check the troubleshooting section
- Review server logs for detailed error information

---

**Built with ❤️ for enhanced learning experiences**
