# <center>Golden Owl - Coding Test (Backend)</center>


## 1. What does this project have?
This is an API for viewing and searching results of serveral candidates in the national entrance exam.

Some features:

- Search score by registration number
- Export report with 4 levels (=8 points, 8 points > && >=6 points, 6 points > && >= 4 points, < 4 points)
    - Statistics of the number of students with scores in the above 4 levels by subjects.
- List top 10 students of group A including (math, physics, chemistry)

## 2. How to run this project?

### Run using Docker
- Install and start Docker on your machine

- Start Docker Compose

```shell
docker compose up
```

- Migrate and seed data
```shell
make migrate
make seed
```

### Run manually
- Install NodeJS, Make Utils on your machine

- Start PostgeSQL Database

- Create `.env` file

```
DB_HOST=<YOUR_HOST>
DB_USER=<YOUR_USERNAME>
DB_PASSWORD=<YOUR_PASSWORD>
DB=<YOUR_DB_NAME>
DB_DIALECT=postgres
DB_PORT=<YOUR_DB_PORT>
SSL_MODE=<YOUR_SSL>
NODE_ENV=development
```

- Install dependencies
```shell
npm install
```

- Edit the `config/config.json` file to match your database configuration

- Migrate and seed data 
```shell
make migrate
make seed
```

- Start NodeJS Backend
```shell
npm run dev
```

## 3. Deployment
The backend is deploy to [this url](link).