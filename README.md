# 🛒 OZmap Challenge

# 🎯 Objective:

Develop a robust RESTful API for user and location management.

# 🖥️ Technologies used:

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Mongoose](https://img.shields.io/badge/mongooose-%234ea94b.svg?style=for-the-badge&logo=mongoose&logoColor=white)
![Mocha](https://img.shields.io/badge/-mocha-%238D6748?style=for-the-badge&logo=mocha&logoColor=white)
![Chai](https://img.shields.io/badge/chai-974942?style=for-the-badge&logo=chai&logoColor=white)
![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white)

## 📋 Prerequisites:

- Docker version 20.0.6
- Docker compose version v2.23.0

# 🛠️ How to Use:

1. Clone the repository to your machine using the command:

   `git clone git@github.com:leonardocbrand/ozmap-challenge.git`

2. Switch to the **leonardo-brandao** branch using the command:

   `git checkout leonardo-brandao`

3. Enter the repository folder and install the dependencies using the command:

   `npm install`

4. Create a **.env** file containing the same environment variables present in the **.env.example** file, or use the data from the example below:
<pre>
<code>DB_PORT=27017
API_PORT=3001 
MONGODB_URI=mongodb://db:27017/oz-tech-test?authSource=admin
GOOGLE_GEOCODING_REVERSE_URL=https://maps.googleapis.com/maps/api/geocode/json?latlng=
GOOGLE_GEOCODING_URL=https://maps.googleapis.com/maps/api/geocode/json?address=
GOOGLE_API_KEY=AIzaSyCOzyNvyVumnu8GmujVFfqr4WX2IUMdWVQ
</code></pre>

5. Open a terminal in the **repository root** and run the command <code>docker-compose up</code>;

6. Wait for all containers to be up and running;

7. To view the API request logs, run the command <code>docker logs -f ozimap-api</code>;

## 📷 Preview:

#### Documentation 1 (Swagger)

![alt text](./preview/swagger.png)

#### Documentation 2 (Swagger)

![alt text](./preview/swagger2.png)

#### Documentation 3 (Swagger)

![alt text](./preview/swagger3.png)

#### Test Coverage

![alt text](./preview/coverage.png)

## 💻 Application:

# Users

- Implement a complete CRUD for users.
- Ensure that each user contains essential information such as name, email, address, and coordinates.
- When creating a user, allow them to provide either an address or coordinates, showing an error if both or neither are provided.
- Use a geolocation service to resolve address ↔ coordinates, ensuring consistency in the information.
- When updating a user's address or coordinates, follow the same logic, maintaining data integrity.

# Regions

- Implement a complete CRUD for regions.
- Each region must have a name, coordinates, and a user who will be designated as the owner of the region.
- Enable the listing of regions containing a specific point.
- Allow the listing of regions at a certain distance from a point, offering the option to filter out regions not belonging to the user who made the request.

## Postman

If you prefer to make requests using Postman, there is a file called `postmanCollection.json` in the project root to import the collections with all the requests.
