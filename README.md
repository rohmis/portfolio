# Portfolio Project

This project consists of a Next.js frontend and an Express.js backend, with MongoDB as the database.

## Prerequisites

- Node.js (v14 or later)
- npm
- Docker and Docker Compose (for containerized setup)
- MongoDB (for local setup without Docker)

## Local Setup

### Frontend

1. Navigate to the frontend directory:

    ```sh
    cd frontend
    ```

2. Install dependencies:

    ```sh
    npm install
    ```

3. Create a `.env.local` file in the frontend directory and add necessary environment variables:

    ```env
    NEXT_PUBLIC_API_URL=http://localhost:5000
    ```

4. Start the development server:

    ```sh
    npm run dev
    ```

    The frontend will be available at [http://localhost:3000](http://localhost:3000).

### Backend

1. Navigate to the backend directory:

    ```sh
    cd backend
    ```

2. Install dependencies:

    ```sh
    npm install
    ```

3. Create a `.env` file in the backend directory and add necessary environment variables:

    ```env
    PORT=5000
    MONGODB_URI=mongodb://localhost:27017/portfolio
    JWT_SECRET=your_jwt_secret
    ```

4. Start the development server:

    ```sh
    npm run dev
    ```

    The backend API will be available at [http://localhost:5000](http://localhost:5000).

## Docker Setup

1. Ensure Docker and Docker Compose are installed on your system.
2. From the root directory of the project, build and start the containers:

    ```sh
    docker-compose up --build
    ```

    This will start the frontend, backend, and MongoDB services. The frontend will be available at [http://localhost:3000](http://localhost:3000), and the backend API at [http://localhost:5000](http://localhost:5000).

## Development

- Frontend code is in the `frontend/src` directory.
- Backend code is in the `backend/src` directory.
- Make sure to run `npm run build` in both frontend and backend directories before deploying to production.

## Testing

(Add instructions for running tests once they are set up)

## Deployment

(Add instructions for deploying to production, including any necessary environment variable setup)

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
