# Basher Kella - Cybersecurity Dashboard

**Author**: [pesnik](https://github.com/pesnik)  
**Created**: February 2025  
**License**: MIT

Inspired by Titumir's Bamboo Fort, *Basher Kella* is a cybersecurity tool designed to provide a comprehensive, real-time web view of a server's security and health status. Built with a Go backend and React frontend, this project aims to empower users with critical insights into server concerns—think of it as a digital fortress for monitoring and defending your systems.

---

## Features
- **Server Health**: Monitor CPU, memory, and uptime.
- **Network Insights**: Track open ports and connections.
- **Security Alerts**: Detect anomalies like failed logins or suspicious processes.
- **Extensible**: Easily add new metrics or checks.

---

## Tech Stack
- **Backend**: Go (with Gorilla Mux for routing)
- **Frontend**: React (with Axios for API calls)
- **Future Plans**: Add charting (Recharts), authentication (JWT), and deployment options.

---

## Getting Started

### Prerequisites
- [Go](https://golang.org/dl/) (1.18+)
- [Node.js](https://nodejs.org/) (16+ with npm)

### Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/pesnik/basher-kella.git
   cd basher-kella
   ```

2. **Set Up the Backend**:
   ```bash
   cd backend
   go mod tidy
   go run main.go
   ```
   The API will run on `http://localhost:8080`.

3. **Set Up the Frontend**:
   ```bash
   cd ../frontend
   npm install
   npm start
   ```
   The dashboard will open at `http://localhost:3000`.

4. Ensure both backend and frontend are running simultaneously to see the dashboard in action.

---

## Usage
- Visit `http://localhost:3000` in your browser.
- The dashboard displays server stats fetched from the Go backend.
- Customize the backend (`backend/main.go`) to add more metrics or security checks tailored to your needs.

---

## Project Structure
```
basher-kella/
├── backend/      # Go backend code
├── frontend/     # React frontend code
├── docs/         # Documentation (optional)
└── README.md     # You're reading it!
```

---

## Contributing
Contributions are welcome! To get involved:
1. Fork the repo.
2. Create a feature branch (`git checkout -b feature/your-idea`).
3. Commit your changes (`git commit -m "Add your message"`).
4. Push to the branch (`git push origin feature/your-idea`).
5. Open a Pull Request.

Ideas? Open an issue or reach out to [pesnik](https://github.com/pesnik).

---

## License
This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

## Roadmap
- Add real-time server monitoring with `gopsutil`.
- Implement a sleek UI with Tailwind CSS or Material-UI.
- Secure the dashboard with JWT authentication.
- Deploy as a Dockerized app.

Built with <3 by pesnik. Let's fortify the digital world, one server at a time!
