# Team Management Backend

This is a backend API for managing teams and their members, built with **IBM Loopback 3** and using **PostgreSQL** as the database. The API includes functionalities to manage teams and members, along with their job descriptions. 

## Requirements

Make sure you have the following installed on your machine:

- Node.js (version 12 or lower)
- PostgreSQL (with a running instance)
- Git
- npm (Node Package Manager)

## Installation

### 1. Clone the Repository

First, clone this repository to your local machine:

```bash
git clone https://github.com/your-username/team-management-backend.git
cd team-management-backend
```

### 2. Install Dependencies

Install the necessary dependencies by running the following command:

```bash
npm install
```

### 3. Configure the Environment Variables

Create a `.env` file in the root directory of the project with the following content:

```env
POSTGRES_HOST=localhost
POSTGRES_PORT=5432
POSTGRES_DB=team_management
POSTGRES_USER=my_db_user
POSTGRES_PASSWORD=your_password_here
```

Replace `your_password_here` with the actual password for the PostgreSQL user.

### 4. Setup the Database

Before running the application, you need to set up the database schema.

To automatically create tables and migrate schema, run:

```bash
node . --migrate
```

### 5. Running the Application

Once everything is set up, you can run the backend using:

```bash
node .
```

This will start the server on `http://localhost:3000`. You can explore the API through LoopBack's built-in **API Explorer** at `http://localhost:3000/explorer`.

## Troubleshooting

- **Error: password authentication failed for user `my_db_user`**
  - Ensure the PostgreSQL database is running and you have the correct credentials in the `.env` file.
  - Verify that the `pg_hba.conf` file in PostgreSQL is correctly configured to allow password authentication.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

Make sure to replace placeholders such as `your_password_here` and `https://github.com/your-username/team-management-backend.git` with information appropriate to your project.
