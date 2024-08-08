# Noor Php Framework

## Overview

Noor is a lightweight PHP framework designed for simplicity, performance, and ease of use. It aims to provide a minimalistic but functional environment for rapid web application development. Noor focuses on core functionalities and extensibility without imposing unnecessary complexity.

## Features

- **Minimalistic Design**: Core features with minimal dependencies.
- **Routing**: Simple and flexible routing system.
- **MVC Structure**: Support for Model-View-Controller architecture.
- **Database Abstraction**: Basic ORM for database interactions.
- **Template Engine**: Lightweight templating engine for views.
- **Request Handling**: Robust request and response handling.
- **Error Handling**: Simple error and exception handling.
- **Extensibility**: Easy to extend and integrate with third-party libraries.

## Directory Structure

The directory structure of Noor is designed to be intuitive and easy to navigate:

```
noor/
├── app/
│   ├── controllers/
│   ├── models/
│   ├── views/
│   ├── config/
├── public/
│   └── log.txt
│   └── assets/
├── vendor/
└── index.php
```

- `app/`: Contains application-specific logic.
  - `controllers/`: Controllers for handling requests.
  - `models/`: Models for interacting with the database.
  - `views/`: View templates.

- `routes`: Routes will be defined in index.php entrypoint
- `public/`: Publicly accessible files.
  - `assets/`: Static assets like CSS, JS, images.

- `vendor/`: Third-party dependencies (managed by Composer).

- `index.php`: The main entry point for the Noor framework, located at the root level for ease of access and Compatibility with apache-like servers alongside with php-server.

## Core Components

### Routing

The routing component is responsible for mapping HTTP requests to the appropriate controllers.

- **Route Definition**: Define routes in a configuration file or using a routing class.
- **Route Matching**: Match incoming requests to defined routes.
- **Route Parameters**: Support for dynamic route parameters.

### MVC Architecture

Noor follows the Model-View-Controller pattern:

- **Model**: Represents data and business logic. Interacts with the database.
- **View**: Handles presentation and user interface. Uses a templating engine.
- **Controller**: Manages user input and interacts with models and views.

### Database Abstraction (Low Priority)

Noor provides a basic ORM for database interactions:

- **Connection Management**: Establish and manage database connections.
- **CRUD Operations**: Basic create, read, update, delete operations.
- **Query Builder**: Simple query builder for constructing SQL queries.

### Template Engine

Noor includes a lightweight templating engine for rendering views:

- **Template Files**: Use `.php` files for templates.
- **Variables**: Pass variables from controllers to views.
- **Includes**: Support for including partial views.

### Request Handling

- **Request**: Handles incoming HTTP requests and extracts parameters.
- **Response**: Manages HTTP responses and status codes.
- **Middleware** (Low Priority): Process requests before they reach the controller.

### Error Handling

- **Error Reporting**: Display and log errors for debugging.
- **Exception Handling**: Handle exceptions gracefully and provide user-friendly error pages.

## Extensibility

Noor is designed to be easily extensible:

- **Plugins**: Add functionality through plugins.
- **Libraries**: Integrate third-party libraries using Composer.
- **Custom Middleware**: Define and use custom middleware.


## Getting Started

1. **Installation**: 
   - Clone the repository or download the source code.
   - Run `composer install` to install dependencies.

2. **Configuration**:
   - Edit the configuration files in the `app/config/` .

3. **Running the Application**:
   - Use a web server (e.g., Apache, Nginx, inbuilt PHP) to serve the `public/` directory.

4. **Creating Routes and Controllers**:
   - Define routes and create corresponding controllers in the `app/` directory.

## Conclusion

Noor is designed to be a simple, efficient, and extensible PHP framework. It provides essential features for web development while allowing developers to build upon and customize it as needed.
