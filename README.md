# Personal Website

This is a personal website built with [Next.js](https://nextjs.org/), [React](https://reactjs.org/), [Tailwind CSS](https://tailwindcss.com/), and [Stackbit](https://www.stackbit.com/).

## Tech Stack

* **Framework**: [Next.js](https://nextjs.org/)
* **Styling**: [Tailwind CSS](https://tailwindcss.com/)
* **Content Management**: [Stackbit](https://www.stackbit.com/)
* **Deployment**: [Netlify](https://www.netlify.com/)

## Getting Started

### Prerequisites

* [Node.js](https://nodejs.org/en/) (version 18 or higher)
* [npm](https://www.npmjs.com/)

### Installation

1. Clone the repository and navigate to the project directory.
2. Install the dependencies:
   ```bash
   npm install
   ```

### Running the Development Server

To start the development server, you need to run two commands in parallel in separate terminal windows:

1.  Run the Next.js development server:
    ```bash
    npm run dev
    ```
2.  Run the Stackbit development server for the visual editor:
    ```bash
    npx stackbit dev
    ```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result, and `localhost:8090` to use the Stackbit editor.

## Project Structure

The project is structured as follows:

* **`content/`**: Contains the content of the website, managed by Stackbit.
* **`public/`**: Contains static assets, such as images.
* **`src/`**: Contains the source code of the application.
  * **`components/`**: Contains the React components, organized into atoms, molecules, sections, and layouts.
  * **`pages/`**: Contains the Next.js pages. The `[[...slug]].tsx` file is a dynamic route that handles all pages based on the content from Stackbit.
  * **`css/`**: Contains the main CSS file.
  * **`utils/`**: Contains utility functions.
* **`stackbit.config.ts`**: The configuration file for Stackbit.

## Content Management

This project uses [Stackbit](https://www.stackbit.com/) for content management. The content models are defined in the `.stackbit/models` directory. The content itself is stored in the `content` directory.

You can edit the content locally or use the Stackbit visual editor.

## Deployment

This project is configured for deployment on [Netlify](https://www.netlify.com/). The `netlify.toml` file contains the deployment settings. To deploy the project, you can connect your Git repository to Netlify.
