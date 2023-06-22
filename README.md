# jwt_test_application
Application shares two public endpoints:
<ul>
  <li>/api/v1/auth/register</li>
  <li>/api/v1/auth/authenticate</li>
</ul>
Rest of the endpoints such as <i>/api/v1/auth/register</i> are secured with JWT. 

To register pass information like:
```
{
    "firstname": "piotr",
    "lastname": "piotr",
    "email": "piotrek1002@mail.com",
    "password": "abc123"
}
```
To authenticate pass information like:
```
{
    "email": "piotrek1002@mail.com",
    "password": "abc123"
}
```
Both of these endpoints return JWT token you can use to access secured endpoints.
Application written with <a href="https://www.youtube.com/watch?v=KxqlJblhzfI&ab_channel=Amigoscode"> YouTube tutorial</a> as an introductory exercise to Spring Security 
