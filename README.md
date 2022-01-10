# __API CHALLENGE ALKEMY BACKEND__
=================================================================================================


1 *En tu consola favorita*:

>**git clone https://github.com/Flavio3312/backend-alkemy.git**

>**cd backend-alkemy**

>|npm install|
  

>listo, el siguiente comando es para correr la **API** en modo de desarrollo:

>|npm run dev|

=================================================================================================

2 *Configurar prisma schema*

>2.a  |npx prisma generate|
>     ||
>2.b  |npx prisma migrate dev --20211227230013_frist_one --create-only|
>     ||
>2.c  |npx prisma migrate dev|
>     ||
>2.d  |prisma db push|
>     ||




3 *Recorda crear tu archivo .env con la conexion a tu base de datos por ejemplo postgresql*
>DATABASE_URL="postgresql://usuario:contraseña@localhost:5432/nombrebasededatos?schema=public"
>PORT=""
>SECRET=""
>DATABASE_URL_PROD=""
>DATABASE_URL_DEV=""
>DATABASE_URL_TEST=""


===============================================================================================================================================================================================================================================
### *API REST*

-**POST http://localhost:3001/api/records**
>Content-Type: application/json
>Authorization: bearer 2cJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImVtYWlsdGVzdDE1QGdtYWlsLmNvbSIsImlkIjoiYWJjOGNkNGUtMGJlOC00ZmNhLTk3YjctMjAzZGE4MTQ2OTFhIiwiaWF0IjoxNjE5MzgxODQ0fQ.veAaUY-VB5KCRujuEbPvzjvuEdq7Vkm00zlOqBM6BH7
>
>{
>    "concept": "home",
>    "amount": 20,
>    "category": "casa",
>    "isIncome": false,
>    "date": "2012-01-01"
>}



-**POST http://localhost:3001/api/users**
>Content-type: application/json
>
>{
>    "email": algo@gmail.com",
>    "password": "12345678"
>}


-**GET  http://localhost:3001/api/users**
>Content-Type: application/json
>Authorization: bearer 2cJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImVtYWlsdGVzdDE1QGdtYWlsLmNvbSIsImlkIjoiYWJjOGNkNGUtMGJlOC00ZmNhLTk3YjctMjAzZGE4MTQ2OTFhIiwiaWF0IjoxNjE5MzgxODQ0fQ.veAaUY-VB5KCRujuEbPvzjvuEdq7Vkm00zlOqBM6BH7
>
>POST http://localhost:3001/api/login
>Content-type: application/json
>
>{
>    "email": "algo@gmail.com",
>    "password": "12345678"
>}






