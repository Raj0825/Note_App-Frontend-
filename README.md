# Note_App-Frontend

### 2. Frontend Repository `README.md`
*Copy and paste this into the `README.md` file in your GitHub Pages repository.*

```markdown
# Note-Taking SPA (Frontend Client)

![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-Semantic-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-Responsive-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Deployed](https://img.shields.io/badge/Deployed-GitHub_Pages-121013?style=for-the-badge&logo=github&logoColor=white)

A zero-dependency, vanilla JavaScript Single Page Application (SPA) designed to interface with a secure Spring Boot REST API. The client manages its own routing, state, and asynchronous network requests to provide a seamless user experience.

## 🔗 Infrastructure & Environments
- **Production Client URL:** [Insert your GitHub Pages URL here]
- **API Server:** [Insert Backend Repository URL]
- **Hosting Provider:** GitHub Pages

## 🏗️ Technical Specifications
- **Architecture:** Decoupled client-side application.
- **Network Protocol:** Utilizes the native ES6 `fetch()` API for asynchronous HTTP requests.
- **State Management:** Leverages the browser's `localStorage` API for stateless session token management.
- **DOM Manipulation:** Native JavaScript rendering, bypassing the need for heavy frameworks like React or Angular for optimal performance.

## 🔐 Authentication Flow
1. User credentials are obfuscated via Base64 encoding (`btoa()`) on the client side.
2. The encoded string is appended to the `Authorization` header of outgoing HTTP requests.
3. Upon a `401 Unauthorized` response, the client automatically purges local state and redirects to the authentication gateway.

## ⚙️ Local Development Setup

Because this is a static asset repository, it requires no build pipeline or dependency installation.

### Execution
1. Clone the repository:
```bash
git clone [https://github.com/yourusername/your-frontend-repo.git](https://github.com/yourusername/your-frontend-repo.git)
cd your-frontend-repo
