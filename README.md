# SendZen Monorepo

This is a monorepo for the SendZen project, containing multiple applications that share common code.

## Project Structure

*   `packages/public-app`: The public-facing Next.js application.
*   `packages/private-app`: The private/internal Next.js application.
*   `packages/shared-ui`: A shared library of UI components used by both applications.

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

*   Node.js (v18 or newer)
*   pnpm package manager. If you don't have it, install it with:
    ```sh
    npm install -g pnpm
    ```

### Installation

1.  **Clone the repository:**
    ```sh
    git clone <YOUR_REPOSITORY_URL>
    cd sendzen-test
    ```

2.  **Install dependencies:**
    Run this command from the root of the project to install dependencies for all packages.
    ```sh
    pnpm install
    ```

### Running the Applications

You can run each application's development server from the root of the project.

*   **To run the public app:**
    ```sh
    pnpm run dev:public
    ```
    This will start the public app, usually on `http://localhost:3000`.

*   **To run the private app:**
    ```sh
    pnpm run dev:private
    ```
    This will start the private app, usually on `http://localhost:3001`.

## How It Works

This project uses [pnpm workspaces](https://pnpm.io/workspaces) to manage the monorepo. Changes made in the `shared-ui` package are automatically available in `public-app` and `private-app` because they are linked locally. When you commit and push changes, you are updating the entire repository at once.
"# test-private" 
"# test-private" 
