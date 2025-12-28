# Career Catalyst

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js](https://img.shields.io/badge/Node.js-18+-green.svg)](https://nodejs.org/)
[![Express.js](https://img.shields.io/badge/Express.js-4.x-lightgrey.svg)](https://expressjs.com/)

## Description

**Career Catalyst** is an intelligent job portal designed to empower candidates. It moves beyond simple keyword matching by using machine learning to analyze your uploaded resume and match you with opportunities based on deep skills similarity, improving job matching accuracy by an estimated 25%.

A job board that works for the candidate. It analyzes your uploaded resume and matches you with jobs based on skills similarity, not just keyword matching.

## Key Features

*   **Intelligent Resume Parser:** Extracts skills, experience, and education from diverse resume formats (PDF, DOCX, including image-based PDFs via integrated OCR).
*   **ML-Driven Job Recommendations:** Utilizes advanced algorithms to match candidates with jobs based on semantic skill similarity, not just keyword overlap.
*   **Skill Gap Analysis:** Provides insights into the skills you have versus the skills required for your target roles, helping you focus your professional development.
*   **Auto-Apply Bot:** (Feature in development) Streamlines the application process for highly relevant job postings.
*   **Interview Prep Mode:** Offers tailored questions and resources based on the specific job description and your resume profile.

## Tech Stack

*   **Backend Framework:** [Express.js](https://expressjs.com/) (v4.x)
*   **Machine Learning & NLP:** [Google Gemini API](https://ai.google.dev/gemini-api) for text analysis, understanding, and semantic matching.
*   **File Parsing:** Custom parser with integrated OCR solution (e.g., Tesseract.js or a dedicated service) for handling image-based PDFs and various document formats.
*   **Runtime:** [Node.js](https://nodejs.org/) (v18 or higher)

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

*   **Node.js** (v18 or later) and **npm** installed.
*   A **Google Cloud Project** with the **Gemini API** enabled.
*   A Gemini API key.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/jumaan1st/CareerCatalyst.git
    cd CareerCatalyst
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Environment Configuration:**
    Create a `.env` file in the root directory based on the provided `.env.example` (if available) or create one with the following variables:
    ```env
    PORT=3000
    GEMINI_API_KEY=your_google_gemini_api_key_here
    # Add any other configuration variables (e.g., database URL, OCR service key)
    ```
    Replace `your_google_gemini_api_key_here` with your actual API key.

4.  **Start the development server:**
    ```bash
    npm start
    # or for development with auto-restart (if configured):
    # npm run dev
    ```
    The application should now be running on `http://localhost:3000` (or the port you specified).

## Usage

*(Screenshots and detailed usage instructions will be added here as the UI/UX is finalized.)*

1.  **Upload Your Resume:** Navigate to the upload section and submit your resume (PDF, DOCX).
2.  **View Your Profile:** The system will parse your resume and display your extracted skills and experience.
3.  **Explore Jobs:** Browse job listings that have been intelligently ranked based on compatibility with your profile.
4.  **Analyze Gaps:** Use the Skill Gap Analysis tool to see where you can improve for your dream role.
5.  **Prepare for Interviews:** Activate Interview Prep Mode for a specific job to get customized questions.

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

Please ensure your code adheres to the existing style and includes appropriate tests.

## License

Distributed under the MIT License. See the `LICENSE` file for more information.