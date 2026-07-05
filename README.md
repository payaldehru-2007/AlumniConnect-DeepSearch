# AlumniConnect - Deep Search Service

The backend search engine for **AlumniConnect** — a FastAPI service that finds real alumni profiles across the web using SerpAPI, with filtering and detailed profile lookup.

This is the module I independently designed and built for the AlumniConnect project. [Check out the full project here](https://github.com/payaldehru-2007/AlumniConnect).

## ✨ Features

- 🔍 **Search** — Find alumni profiles by name, company, or college
- 👤 **Profile Details** — Fetch detailed information for a specific profile
- 🎯 **Filters** — Narrow results by graduation year, company, location, and more
- ⚡ **7 REST API endpoints** built with FastAPI
- 🔌 Real-time data via **SerpAPI** integration

## 🛠️ Tech Stack

- **Framework:** FastAPI (Python)
- **Data Source:** SerpAPI
- **Language:** Python 3

## ⚙️ Setup & Installation

### 1. Clone the repo
```bash
git clone https://github.com/payaldehru-2007/AlumniConnect-DeepSearch.git
cd AlumniConnect-DeepSearch
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Set up environment variables
Create a `.env` file in the root directory:
```
SERPAPI_KEY=your_serpapi_key_here
```
Get a free API key from [SerpAPI](https://serpapi.com/).

### 4. Run the server
```bash
python main.py
```
Server runs on `http://localhost:8000`

## 📡 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/search` | Search alumni profiles by name/company/college |
| GET | `/profile/{id}` | Get detailed info for a specific profile |
| GET | `/filter` | Filter results by year, company, location |



## 🚧 Deployment Note

This service isn't currently deployed live — Railway requires a paid card for the always-on hosting this backend needs, and Vercel's serverless functions aren't suited for this kind of persistent API service. It runs fully and reliably locally using the steps above.

## 🔗 Related

Part of the larger [AlumniConnect](https://github.com/payaldehru-2007/AlumniConnect) project.

## 📄 License

This project is open for educational and portfolio purposes.