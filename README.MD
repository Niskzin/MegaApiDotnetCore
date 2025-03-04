<h1 align="center">
  <br />
  <img src="https://i.imgur.com/lUyQJJZ.png" alt="Star Wars Planets API" width="150" />
  <br />
  <b>Star Wars Planets API</b>
  <br />
  <sub
    ><sup><b>(STAR-WARS-PLANETS)</b></sup></sub
  >
  <br />
  <a
    href="https://github.com/Niskzin/StarWarsPlanetsAPI/actions/workflows/build.yml"
  >
    <img
      src="https://github.com/Niskzin/StarWarsPlanetsAPI/actions/workflows/build.yml/badge.svg"
      alt=""
    />
  </a>
  <a href="https://github.com/Niskzin/StarWarsPlanetsAPI/releases/latest">
    <img
      src="https://img.shields.io/github/v/release/yourUsername/StarWarsPlanetsAPI"
      alt="Latest Release"
    />
  </a>
</h1>

<p align="center">
  This .NET Core API provides JSON data about planets from the Star Wars universe. Built with .NET Core 3.1, it utilizes modern technologies for data management and API responses.
  <br />
</p>

<p align="center">
  Developed using Entity Framework Core and other contemporary .NET tools, this project aims to offer a reliable API for accessing Star Wars planet information.
  <br />
</p>

<p align="center">
  <br />
  <img src="./_docs/assets/carbon.png" />
</p>

## API Endpoints

<table align="center">
  <tr>
    <th>Method</th>
    <th>Endpoint</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>GET</td>
    <td>/api/v1/planets</td>
    <td>Returns a list of all planets</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/api/v1/planets/{id}</td>
    <td>Returns details of a specific planet by ID</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/api/v1/planets</td>
    <td>Endpoint to create a new planet entry</td>
  </tr>
</table>

## Techniques Used

<p align="center">
  - <b>Entity Framework Core:</b> ORM for data management.<br />
  - <b>RESTful API Design:</b> Ensures clear and effective communication endpoints.<br />
  - <b>Dependency Injection:</b> Promotes loose coupling and enhanced testability.<br />
</p>

## Dependencies

<table align="center">
  <tr>
    <th>Package</th>
    <th>Version</th>
    <th>Link</th>
  </tr>
  <tr>
    <td>Microsoft.EntityFrameworkCore</td>
    <td>3.1.8</td>
    <td>
      <a href="https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8">NuGet</a>
    </td>
  </tr>
  <tr>
    <td>Microsoft.EntityFrameworkCore.Design</td>
    <td>3.1.8</td>
    <td>
      <a href="https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8">NuGet</a>
    </td>
  </tr>
  <tr>
    <td>Microsoft.EntityFrameworkCore.SqlServer</td>
    <td>3.1.8</td>
    <td>
      <a href="https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8">NuGet</a>
    </td>
  </tr>
  <tr>
    <td>Newtonsoft.Json</td>
    <td>12.0.2</td>
    <td>
      <a href="https://www.nuget.org/packages/Newtonsoft.Json/12.0.2">NuGet</a>
    </td>
  </tr>
</table>

## :gear: Arch

```🌐
src
├── 📂 Controllers      [Routes for endpoints]
├── 📂 Models           [Database models]
├── 📂 Services         [Business rules]
├── 📂 Middlewares      [Intermediate functions]
├── 📂 Database         [Database related structures]
│   ├── 📂 DTOs             [Data Transfer Objects]
│   ├── 📂 EntityFramework  [Entity Framework files]
│   │     ├── 📂 Context         [Entity context settings]
│   │     ├── 📂 Migrations      [Database migrations]
│   ├── 📂 Repositories     [Repository pattern]
