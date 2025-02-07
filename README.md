# sam-scm-bitbucket-plugin

A Node.js/Express.js plugin that provides Source Control Management (SCM) functionalities for Bitbucket. This plugin connects to the Bitbucket API to offer operations such as listing repositories, branches, commits, and file content retrieval.

## Features

- Connects to Bitbucket API using personal access tokens.
- List and retrieve details of repositories.
- List branches and commits.
- Compare commits.
- Get file contents within a repository.
- Centralized error handling for API operations.
- Easily configurable via JSON configurations.

## Plugin Architecture

The plugin follows a modular architecture designed to run as a standalone service in a Docker container.

### Directory Structure

sam-scm-bitbucket-plugin/
├── src/
│   ├── v1/
│   │   ├── methods/        # Methods (actions) to perform SCM operations
│   │   ├── controllers/    # API controllers (e.g., Bitbucket controller)
│   │   ├── routes.js       # Express routes configuration
│   │   └── services/
│   │       └── bitbucket/     # Bitbucket provider related code
│   ├── app.js             # Express app initialization and middleware configuration
│   └── server.js          # Server bootstrapping
├── plugin.configs.json    # Plugin configuration file (Bitbucket settings only)
├── README.md              # Plugin documentation
└── plugin-root/          # Documentation

## Prerequisites

- Node.js (v14 or above recommended)
- npm (v6 or above)

## Installation

1. Clone this repository:

```bash
git clone https://bitbucket.com/SorenHQ/sam-scm-bitbucket-plugin.git
```

2. Change to the project directory:

```bash
cd  sam-scm-bitbucket-plugin
```

3. Install the dependencies:

```bash
npm install
```

4. Development & Usage:

```bash
npm start
```

Happy coding and enjoy using sam-scm-bitbucket-plugin!
