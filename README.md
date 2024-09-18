# GemUnite

GemUnite is a web application designed for IT enthusiasts to collaborate on projects within their areas of interest. Users can search for or create small to medium-sized groups and work together on projects like machine learning, web development, cybersecurity, IoT, and more.

## Features

- **User Registration:** Users sign up with their personal information and select their areas of interest.
- **Project Proposals:** Users can view project proposals in their areas of interest on the homepage, see group members, and request to join.
- **Project Creation:** Registered users can create a project, set group size, and provide a description of the project idea.
- **Project Management:** Members can track project progress through checkpoints, manage tasks, and communicate via a built-in chat. Github repositories can be linked via the Github API.
- **Member Management:** Project creators can accept/reject requests, remove members, and edit project information.

## Tech Stack

- **Ruby on Rails:** Web framework
- **SQLite:** Database
- **Github API:** To manage repositories for projects
- **ActionCable:** Real-time chat functionality

## Getting Started

### Prerequisites

Ensure that you have the following installed:

- [Ruby](https://www.ruby-lang.org/en/) (version 3.0.0 or above)
- [Ruby on Rails](https://rubyonrails.org/) (version 6.1 or above)

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/RiccardoEbene/GemUnite.git
    cd GemUnite
    ```

2. Install dependencies:

    ```bash
    bundle install
    yarn install
    ```

3. Set up the database:

    ```bash
    rails db:create
    rails db:migrate
    ```

4. Set up environment variables:

    You'll need to configure a `.env` file with your Github API credentials and any other necessary environment variables:

    ```bash
    GITHUB_CLIENT_ID=your_github_client_id
    GITHUB_CLIENT_SECRET=your_github_client_secret
    ```

5. Run the server:

    ```bash
    rails server
    ```

6. Navigate to `http://localhost:3000` in your browser.

### Running Tests

Run the following command to execute tests:

```bash
rails test
```

### API Integration

GemUnite uses the [Github API](https://docs.github.com/en/rest) to manage project repositories. Make sure you have a valid Github API token for repository creation and linking.

