# Text-to-Speech App

A simple and efficient Text-to-Speech (TTS) web application built using **Next.js**. This app allows users to convert text into speech using various AI models hosted on Hugging Face.

## Features

- Select from multiple TTS models
- Convert text to high-quality speech
- Seamless integration with Hugging Face API

## Tech Stack

- **Frontend & Backend:** Next.js
- **UI Components:** shadcn/ui, Tailwind CSS
- **API Integration:** Hugging Face Inference API

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/text-to-speech-app.git
   cd text-to-speech-app
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Set up environment variables:
   - Create a `.env.local` file in the root directory
   - Add the following:
     ```sh
     HUGGING_FACE_TOKEN=your_huggingface_api_token
     ```
4. Run the development server:
   ```sh
   npm run dev
   ```

## Usage

1. Open the app in your browser.
2. Select a sound model from the dropdown.
3. Enter text in the input field.
4. Click submit to generate speech.
5. Download the generated audio.

## API Endpoint

- **POST /api/generate-audio**
  - **Request Body:**
    ```json
    {
      "modelUrl": "https://api-inference.huggingface.co/models/example-model",
      "input": "Hello, world!"
    }
    ```
  - **Response:** Audio file in `audio/mpeg` format

## License

This project is free to use without restrictions.

---

Feel free to contribute and enhance the app! 🚀

