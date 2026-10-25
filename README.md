<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00622B,100:00C853&height=220&section=header&text=Ulises%20Montalvo&fontSize=58&fontColor=ffffff&fontAlignY=38&animation=fadeIn&desc=Backend%20Developer%20%7C%20C%23%20%26%20.NET&descSize=20&descAlignY=60" width="100%" alt="header" />

<a href="https://github.com/MizunoAC">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=1000&color=00C853&center=true&vCenter=true&width=700&lines=I+build+APIs+that+move+money+%F0%9F%92%B8;Stripe+%C2%B7+Google+Pay+%C2%B7+SQL+Server;Clean+architecture%2C+CQRS%2C+secure+by+default+%F0%9F%94%90;Legacy+to+microservices%2C+one+bounded+context+at+a+time;Now+exploring+mobile+with+React+Native+%F0%9F%93%B1" alt="Typing SVG" />
</a>

<br/>

![Profile views](https://komarev.com/ghpvc/?username=MizunoAC&label=Profile+views&color=00622B&style=for-the-badge)
![Followers](https://img.shields.io/github/followers/MizunoAC?label=Followers&style=for-the-badge&color=00A84F&logo=github)
![Repos](https://img.shields.io/badge/Public_repos-3-007F3A?style=for-the-badge&logo=github)

</div>

---

## 👨‍💻 About me

```csharp
var ulises = new Developer
{
    Role         = "C# Backend Developer",
    Focus        = new[] { "Payment systems", "Notification services", "RESTful APIs" },
    Architecture = new[] { "Clean Architecture", "CQRS", "Microservices" },
    Database     = "SQL Server (EF Core + ADO.NET + stored procedures)",
    Currently    = "Building a wildlife-tracking platform end to end 🌿",
    Learning     = "React Native + Expo",
    Philosophy   = "Make it work, make it secure, make it maintainable."
};
```

---

## 🛠️ Tech arsenal

<div align="center">

![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![EF Core](https://img.shields.io/badge/Entity_Framework_Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)

![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=for-the-badge&logo=stripe&logoColor=white)
![Google Pay](https://img.shields.io/badge/Google_Pay-4285F4?style=for-the-badge&logo=googlepay&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=for-the-badge&logo=twilio&logoColor=white)
![SendGrid](https://img.shields.io/badge/SendGrid-1A82E2?style=for-the-badge&logo=twilio&logoColor=white)
![JWT](https://img.shields.io/badge/JWT_RS256-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)

![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Expo](https://img.shields.io/badge/Expo-000020?style=for-the-badge&logo=expo&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Ionic](https://img.shields.io/badge/Ionic-3880FF?style=for-the-badge&logo=ionic&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

</div>

| 🧩 Area | 🔧 What I use |
|---|---|
| **Backend** | ASP.NET Core Web API & MVC · MediatR (CQRS) · Clean Architecture · Dependency Injection · NLog |
| **APIs** | RESTful design · DTOs · Request validation · Optional parameter handling · Structured error responses |
| **Data** | SQL Server · Entity Framework Core · ADO.NET · Stored procedures · Query optimization (`EXISTS` over subqueries) |
| **Payments** | Stripe · Google Pay · Secure token handling · Server-side payment flow |
| **Security** | JWT RS256 (access + refresh) · Role-based auth · BCrypt · Public/private key signing |
| **Integrations** | Twilio SMS · SendGrid & SMTP · RazorEngine templates · PuppeteerSharp (PDF) |
| **Workflow** | Git branching strategies · Conflict resolution · Remote sync · Docker · CI with GitHub Actions |
| **Mobile** | React Native · Expo Router · Ionic |

---

## 🌿 Featured project: FSP

> A wildlife sighting platform: users report animals with a photo and location, admins review and approve every record, and the community gets a species catalog with maps and PDF fact sheets.

```mermaid
flowchart LR
    A[📱 Mobile app<br/>React Native] -->|JWT| API
    B[🖼️ Admin gallery<br/>ASP.NET MVC] -->|JWT + Admin role| API
    C[⌨️ Console uploaders<br/>C#] -->|Bulk upload| API
    API[⚙️ FSP-API<br/>.NET 9 · MediatR] --> DB[(🗄️ SQL Server)]
    API --> M[✉️ Email<br/>notifications]
    API --> P[📄 PDF fact sheets]
```

<table>
  <tr>
    <td width="50%" valign="top">

### ⚙️ [FSP-API](https://github.com/MizunoAC/FSP-API)
REST API with **CQRS**, **JWT RS256** auth, an admin moderation flow, species catalog, sighting maps and PDF generation. Dockerized, with CI on GitHub Actions and 64+ commits of history.

`.NET 9` `MediatR` `SQL Server` `Docker` `Swagger`

    </td>
    <td width="50%" valign="top">

### 🖼️ [FSP-ImagenVisualizer](https://github.com/MizunoAC/FSP-ImagenVisualizer)
Admin-only image gallery built to browse hundreds of sighting photos.

- ✅ JWT login with token validation against the backend's public key
- ✅ Session handling and admin-only access
- ✅ Friendly image names (`fototrampaN`) instead of raw IDs
- ✅ Built-in view-only image viewer
- ✅ Branded green theme
- 🔜 Image listing served directly by the main API

`ASP.NET Core MVC` `.NET 8` `JWT`

    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">

### 📱 fsp-mobile *(in progress)*
Mobile client for reporting sightings, built from scratch with a nature-inspired green UI.

- ✅ Expo + Expo Router project setup (`src/app`, `src/components`)
- 🚧 Screen layouts and design
- 🔜 Integration with the C# API

`React Native` `Expo` `TypeScript`

    </td>
    <td width="50%" valign="top">

### 🧪 [proyectoFIonic](https://github.com/MizunoAC/proyectoFIonic)
First mobile prototype of the platform.

`Ionic` `TypeScript`

    </td>
  </tr>
</table>

Supporting tools: C# console apps that bulk-upload images to the API.

---

## 💼 What I do professionally

<details open>
<summary><b>💳 Payment systems</b></summary>
<br/>

- Integrated payment gateways (**Stripe** and **Google Pay**) with secure token management and a complete server-side payment flow
- Designed and maintained payment APIs, documented with XML comments for Swagger
- Hardened stored procedures to avoid subquery errors and improve performance

</details>

<details>
<summary><b>🏗️ Architecture & modernization</b></summary>
<br/>

- Migrated legacy projects to **microservices** using **CQRS** and SQL Server, improving scalability and modularity
- Built and maintained applications with **.NET C#**, **Entity Framework Core** and SQL Server, following clean architecture and maintainability best practices

</details>

<details>
<summary><b>🔌 API design</b></summary>
<br/>

- Designed, implemented and consumed **RESTful APIs**
- DTOs, request validation, optional parameter handling and structured error management

</details>

<details>
<summary><b>🔔 Notification services</b></summary>
<br/>

- Multi-channel delivery (SMS via Twilio, email via SendGrid) driven by user preferences
- Phone number validation with libphonenumber
- Clean service architecture using dependency injection

</details>

<details>
<summary><b>📧 Dynamic email templates</b></summary>
<br/>

- Invoice emails that adapt to variable amounts of data using RazorEngine
- Inline embedded images, so emails render without stray attachments

</details>

<details>
<summary><b>🔀 Team workflow</b></summary>
<br/>

- Git version control: branching, conflict resolution and remote synchronization

</details>

---

## 📊 GitHub stats

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=MizunoAC&show_icons=true&hide_border=true&bg_color=0d1117&title_color=00C853&icon_color=00C853&text_color=c9d1d9&ring_color=00C853" alt="stats" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MizunoAC&layout=compact&hide_border=true&bg_color=0d1117&title_color=00C853&text_color=c9d1d9" alt="top languages" />

<img src="https://streak-stats.demolab.com?user=MizunoAC&theme=dark&hide_border=true&background=0d1117&ring=00C853&fire=00C853&currStreakLabel=00C853&sideLabels=c9d1d9&currStreakNum=c9d1d9&sideNums=c9d1d9&dates=8b949e" alt="streak" />

</div>

---

## 🤝 Let's connect

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-MizunoAC-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MizunoAC)

*Open to feedback, collaboration and good coffee. ☕*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00622B,100:00C853&height=120&section=footer" width="100%" alt="footer" />

</div>