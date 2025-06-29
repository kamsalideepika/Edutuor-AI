# 🧠 EduTutor AI: Personalized Learning with Generative AI and LMS Integration

**Category:** Cloud Application Development
**Skills Required:** Python, Generative AI (Hugging Face Transformers), Gradio, PDF Processing

EduTutor AI is an AI-powered personalized education platform that revolutionizes the way students learn and educators assess progress. It provides dynamic quiz generation, student evaluation, and real-time feedback—all powered by **IBM Granite 3.3-2B Instruct LLM** (accessed via Hugging Face Transformers). Designed with modular architecture, this platform streamlines personalized education and enhances learning outcomes for students across academic levels.

---

### ✨ Key Features

EduTutor AI aims to make learning more accessible and personalized through its core functionalities:

* **🔐 User Authentication:** A straightforward login and registration system to manage individual student sessions.
* **📘 Dynamic Concept Explanations:** Enter any topic (e.g., "Photosynthesis", "Generative AI") and receive clear, age-appropriate, easy-to-understand explanations with examples.
* **🌍 Interactive Language Learning Support:** Choose a language (currently supports **English, Hindi, Spanish, Japanese, and French**) and get a tailored introduction with grammar, vocabulary, and usage tips.
* **📄 Automated Test Generation from PDFs:** Upload educational PDFs and get auto-generated **multiple-choice questions (MCQs)** formatted for use in quizzes and exams.
* **🧪 Custom Quiz Creator:** Enter a topic (e.g., "Machine Learning", "World War II") and receive a full 5-question quiz with options and correct answers.

---

### 🛠️ Tech Stack

* **Python:** The primary programming language for all application logic.
* **Hugging Face Transformers:** For integrating and utilizing the **IBM Granite 3.3B Instruct** Large Language Model.
* **Gradio:** Powers the intuitive and user-friendly web interface, enabling easy interaction with the AI functionalities.
* **PyPDF2:** Utilized for efficient parsing and text extraction from PDF documents, allowing the AI to generate content from uploaded study materials.
* **Torch:** Facilitates necessary LLM inference operations, especially when running on GPU.
* **BitsAndBytes:** (Used during development for potential model optimization and compatibility with `transformers`, though not explicitly for 4-bit loading in the final configuration).

---

### 📂 Project Structure

* `finalgenaifix.ipynb`: This is the main Jupyter Notebook containing all the core application logic, Gradio interface setup, and AI functionalities.
* `requirements.txt`: Lists all necessary Python packages for easy dependency management.
* `README.md`: This project overview, setup instructions, and feature explanations.

---

### 📦 Installation

To set up and run EduTutor AI, follow these steps:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/kamsalideepika/Edutuor-AI](https://github.com/kamsalideepika/Edutuor-AI)
    ```
2.  **Install Dependencies:**
    Navigate into the cloned directory and install the required Python packages using the `requirements.txt` file.
    ```bash
    cd Edutuor-AI
    pip install -r requirements.txt
    ```
    *(Note: Ensure you have `pip` installed and consider using a virtual environment for better project isolation.)*

---

### ▶️ Run the Application

You have two primary ways to run the `finalgenaifix.ipynb` notebook:

* **Option A: Google Colab (Recommended for ease of use and GPU access)**
    1.  Go to [Google Colab](https://colab.research.google.com/).
    2.  Click `File` > `Upload notebook` and select `finalgenaifix.ipynb` from your cloned repository.
    3.  Once opened, go to `Runtime` > `Change runtime type` and select `GPU` as the hardware accelerator (if available and desired), then click `Save`.
    4.  Run all cells (`Runtime` > `Run all`). The Gradio interface will launch directly in the output of the last cell, providing a public URL.

* **Option B: Local Jupyter Environment (Requires local Python/Jupyter setup)**
    1.  Ensure you have Jupyter Notebook or JupyterLab installed (`pip install notebook` or `pip install jupyterlab`).
    2.  Navigate to your cloned directory in your terminal.
    3.  Launch Jupyter:
        ```bash
        jupyter notebook
        ```
        or
        ```bash
        jupyter lab
        ```
    4.  Open `finalgenaifix.ipynb` from the Jupyter interface in your web browser.
    5.  Run all cells in the notebook.

---

### 🤖 Model Information

This project leverages the **IBM Granite 3.3B Instruct** model. It is an instruction-tuned Large Language Model specifically optimized for educational content generation and question-answering tasks, which is ideal for this platform's functionalities. The model is hosted via Hugging Face and seamlessly integrated into the application using their `transformers` library.

---

### 📚 Example Prompts

See EduTutor AI in action with these example interactions, ideal for demonstrating its capabilities for students of various academic levels:

* **Concept Explanation:** "Explain the concept of 'climate change' for a middle schooler."
* **Language Learning:** "Give me 10 common phrases in Japanese for tourists."
* **PDF Test Generation:** "Generate 3 multiple-choice questions from the uploaded science textbook chapter."
* **Custom Quiz Creation:** "Create a 5-question quiz about the solar system."

---

### 🌐 LMS Integration (Future Scope)

Looking ahead, EduTutor AI aims to evolve into an even more comprehensive learning tool. Future enhancements include:

* **Seamless Integration:** Connect with popular Learning Management Systems (LMS) like **Moodle or Google Classroom** to fit into existing educational workflows.
* **Progress Tracking:** Implement features to track student progress and performance over time.
* **Adaptive Learning:** Adapt AI-generated responses and content based on individual user learning history and identified areas for improvement, enabling truly personalized education experiences.
