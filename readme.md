# Multi-Language Translator & Transliterator with OCR

A powerful, AI-powered translation and transliteration application that supports 120+ languages with built-in OCR capabilities for PDFs and images.

![Languages](https://img.shields.io/badge/Languages-120+-blue)
![React](https://img.shields.io/badge/React-18+-61DAFB?logo=react)
![License](https://img.shields.io/badge/License-MIT-green)

## ✨ Features

### Core Features
- 🌍 **120+ Languages Support** - Translate between over 120 languages including major world languages and regional dialects
- 🔤 **Transliteration Mode** - Convert text from one script to another based on pronunciation (e.g., "Hello" → "हेलो")
- 📄 **PDF Text Extraction** - Upload PDF documents and extract text automatically
- 🖼️ **Image OCR** - Extract text from images (JPG, PNG, JPEG, etc.)
- 📝 **Text File Support** - Upload .txt files directly
- ⇄ **Language Swap** - Quickly swap source and target languages
- 📋 **Copy to Clipboard** - One-click copy of translated/transliterated text
- 💾 **Download Results** - Save translations/transliterations as .txt files
- 🎨 **Modern UI** - Clean, responsive interface with intuitive mode switching
- ⚡ **Real-time Processing** - Fast AI-powered translations, transliterations, and OCR

### Translation vs Transliteration

| Feature | Translation | Transliteration |
|---------|------------|-----------------|
| **Purpose** | Convert meaning | Convert script/sound |
| **Example 1** | "Hello" (EN) → "नमस्ते" (HI) | "Hello" (EN) → "हेलो" (HI) |
| **Example 2** | "Computer" (EN) → "कंप्यूटर" (HI meaning) | "Computer" (EN) → "कंप्यूटर" (HI sound) |
| **Use Case** | Understanding foreign text | Writing names, keeping pronunciation |

## 🌐 Supported Languages

The app supports translation and transliteration between any pair of the following 120+ languages:

Afrikaans, Albanian, Amharic, Arabic, Armenian, Assamese, Aymara, Azerbaijani, Bambara, Basque, Belarusian, Bengali, Bhojpuri, Bosnian, Bulgarian, Burmese, Catalan, Cebuano, Chinese (Simplified), Chinese (Traditional), Corsican, Croatian, Czech, Danish, Dhivehi, Dogri, Dutch, English, Esperanto, Estonian, Ewe, Filipino (Tagalog), Finnish, French, Frisian, Galician, Georgian, German, Greek, Guarani, Gujarati, Haitian Creole, Hausa, Hawaiian, Hebrew, Hindi, Hmong, Hungarian, Icelandic, Igbo, Ilocano, Indonesian, Irish, Italian, Japanese, Javanese, Kannada, Kazakh, Khmer, Kinyarwanda, Konkani, Korean, Krio, Kurdish (Kurmanji), Kurdish (Sorani), Kyrgyz, Lao, Latin, Latvian, Lingala, Lithuanian, Luganda, Luxembourgish, Macedonian, Maithili, Malagasy, Malay, Malayalam, Maltese, Maori, Marathi, Meiteilon (Manipuri), Mizo, Mongolian, Nepali, Norwegian, Odia (Oriya), Oromo, Pashto, Persian (Farsi), Polish, Portuguese, Punjabi, Quechua, Romanian, Russian, Samoan, Sanskrit, Scottish Gaelic, Sepedi, Serbian, Sesotho, Shona, Sindhi, Sinhala, Slovak, Slovenian, Somali, Spanish, Sundanese, Swahili, Swedish, Tajik, Tamil, Tatar, Telugu, Thai, Tigrinya, Tsonga, Turkish, Turkmen, Twi, Ukrainian, Urdu, Uyghur, Uzbek, Vietnamese, Welsh, Xhosa, Yiddish, Yoruba, and Zulu.

## 🚀 Getting Started

### Prerequisites

- Node.js 16+ installed
- React 18+
- Modern web browser

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/multilanguage-translator.git
cd multilanguage-translator
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

4. Open your browser and navigate to `http://localhost:3000`

## 📖 How to Use

### Choose Your Mode

**Step 1**: Select between two modes using the toggle buttons:
- **Translate Mode** - Convert meaning from one language to another
- **Transliterate Mode** - Convert script/pronunciation while keeping the sound

### Translation Mode

1. **Select Languages**: Choose your source and target languages from the dropdown menus
2. **Enter Text**: Type or paste text into the "Source Text" area
3. **Translate**: Click the "Translate" button
4. **Get Results**: View your translation in the "Translated Text" area

**Example**:
- Input: "Good morning" (English)
- Output: "Buenos días" (Spanish)

### Transliteration Mode

1. **Select Languages**: Choose your source and target scripts
2. **Enter Text**: Type text you want to convert to another script
3. **Transliterate**: Click the "Transliterate" button
4. **Get Results**: View the phonetic conversion in the target script

**Examples**:
- Input: "John" (English) → Output: "जॉन" (Hindi)
- Input: "Tokyo" (English) → Output: "টোকিও" (Bengali)
- Input: "Pizza" (English) → Output: "پیزا" (Urdu)

### Upload Files

#### Text Files (.txt)
- Click the "Text File (.txt)" button
- Select your .txt file
- Text will automatically populate in the source area

#### PDF Files
- Click the "PDF File" button
- Select your PDF document
- AI will extract all text from the PDF
- Extracted text appears in the source area

#### Images (OCR)
- Click the "Image (OCR)" button
- Select an image file (JPG, PNG, etc.)
- AI will perform OCR and extract visible text
- Extracted text appears in the source area

### Additional Features

- **Swap Languages**: Click the "⇄ Swap" button to quickly reverse source and target languages
- **Copy Result**: Click the "Copy" button to copy translated/transliterated text to clipboard
- **Download Result**: Click the "Download" button to save result as a .txt file

## 🛠️ Technical Details

### Built With

- **React** - Frontend framework
- **Lucide React** - Icons
- **Tailwind CSS** - Styling
- **Claude AI (Anthropic)** - Translation, transliteration, and OCR engine

### Architecture

The app uses Claude AI's API to perform:
- Text-to-text translation (meaning-based)
- Text-to-text transliteration (script/sound-based)
- PDF text extraction
- OCR from images
- Language and script detection

## 📝 File Format Support

| Format | Extension | Support |
|--------|-----------|---------|
| Text | .txt | ✅ Full |
| PDF | .pdf | ✅ Full |
| Images | .jpg, .jpeg, .png, .gif, .bmp | ✅ OCR |

## ⚙️ Configuration

### API Setup

The app requires access to the Anthropic API. The API endpoint is configured to use:
- Model: `claude-sonnet-4-20250514`
- Max tokens: 1000 per request

## 🎯 Use Cases

### Translation Use Cases
- **Travel**: Understand signs, menus, and documents in foreign countries
- **Business**: Translate business documents and communications
- **Education**: Study materials in multiple languages
- **Research**: Translate research papers and articles
- **Content Creation**: Localize content for global audiences

### Transliteration Use Cases
- **Names**: Write your name in different scripts (John → जॉन)
- **Branding**: Create brand names in local scripts while keeping pronunciation
- **Language Learning**: Learn how words are written in different alphabets
- **Social Media**: Post messages using different scripts
- **Documents**: Include foreign words/names in documents with proper script
- **Cultural Context**: Preserve pronunciation of cultural terms

### Real-World Examples

**Translation**:
- Restaurant menu: "Chicken Curry" → "चिकन करी" (meaning)
- Sign: "Exit" → "出口" (meaning in Chinese)

**Transliteration**:
- Brand name: "McDonald's" → "मैकडॉनल्ड्स" (sound in Hindi)
- Personal name: "Sarah" → "サラ" (sound in Japanese)
- Place: "London" → "লন্ডন" (sound in Bengali)

## 🔒 Privacy & Security

- All processing happens through secure API calls
- No text data is stored permanently
- Files are processed in-memory only
- No user data retention

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🐛 Known Issues

- Large PDF files (>10MB) may take longer to process
- Complex image layouts may affect OCR accuracy
- Very long texts may need to be processed in chunks
- Transliteration accuracy varies by language pair (best for major languages)

## 🗺️ Roadmap

- [ ] Add bulk file translation/transliteration
- [ ] Support for audio file transcription and translation
- [ ] Translation/transliteration history and favorites
- [ ] Offline mode for common languages
- [ ] Browser extension version
- [ ] Mobile app version
- [ ] Side-by-side comparison mode (translate + transliterate)
- [ ] Custom glossary support for consistent transliterations

## 💬 Support

For support, please open an issue in the GitHub repository or contact the maintainers.

## 🙏 Acknowledgments

- Anthropic for Claude AI
- Lucide for beautiful icons
- The open-source community

## 📊 Stats

- **Languages**: 120+
- **File Types**: 3 (Text, PDF, Images)
- **Translation Pairs**: 14,400+
- **Transliteration Pairs**: 14,400+
- **Modes**: 2 (Translate & Transliterate)
- **AI Model**: Claude Sonnet 4

## 🌟 Key Differentiators

Unlike other translation tools, this app offers:
1. **Dual Mode**: Switch between translation and transliteration
2. **Script Flexibility**: Convert text to 120+ different scripts
3. **OCR Support**: Extract and process text from images and PDFs
4. **No Storage**: Privacy-focused with no data retention
5. **AI-Powered**: Leverages advanced Claude AI for accurate results

---

Made with ❤️ by the community