# Magic Background Generator

A simple web application that transforms your ideas into incredible animated backgrounds using the power of AI. Just describe what you imagine, and watch the magic happen.

This project was developed as part of the "Semana do Zero ao Programador Contratado" event.

## ✨ Features

- **AI-Powered Generation**: Describe the background you want in natural language.
- **Live Preview**: See the generated background applied instantly on the page.
- **Code Output**: Get the HTML and CSS code for the generated background.
- **Loading State**: A clear indicator shows when the AI is processing your request.
- **Responsive Design**: Works smoothly on both desktop and mobile devices.

## 🚀 How It Works

The application captures the user's text description and sends it to an n8n workflow via a webhook. The n8n workflow processes this description (likely using an AI model like GPT) to generate corresponding HTML and CSS code. This code is then sent back to the frontend, which dynamically injects it into the page to display the background and the code snippets.

1.  The user types a description (e.g., "a gentle blue gradient from light to dark").
2.  The frontend sends a `POST` request to an n8n webhook.
3.  The n8n workflow generates HTML and CSS.
4.  The frontend receives the code and:
    - Renders the HTML in the preview area.
    - Injects the CSS into a `<style>` tag in the document's `<head>`.
    - Displays the code in the HTML and CSS output boxes.

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Automation/Backend**: n8n.io
- **Fonts**: Google Fonts (Roboto Mono)

## 🔧 Getting Started

- Acess the project on: https://hpoirot22.github.io/fundo-magico/
