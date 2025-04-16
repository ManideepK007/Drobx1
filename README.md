# Drobx1
# DropBoxify – Mini Dropbox Clone

**Goal**: Build a mini Dropbox-like file storage and sharing system with basic distributed system features like replication, fault tolerance, and metadata tracking.

## 🛠️ Tech Stack
- **Backend**: Python (Flask/FastAPI)
- **Database**: PostgreSQL / SQLite
- **File Storage**: Simulated local storage nodes (folders) or AWS S3
- **Frontend**: HTML/JS or React (optional)
- **DevOps**: Docker, GitHub Actions (CI/CD), Postman for testing

## 📋 Features
### 🟢 Phase 1: MVP – Basic Upload/Download/Delete
- [ ] Create Flask backend with file upload endpoint
- [ ] Store file in a local directory
- [ ] Save metadata (filename, size, timestamp) to DB
- [ ] Endpoint to download file by ID
- [ ] Endpoint to delete file
- [ ] Test using Postman

### 🔵 Phase 2: Simulated Distributed Storage
- [ ] Create 3 local “storage nodes” (just folders like `/node1`, `/node2`, `/node3`)
- [ ] Add file replication logic (e.g., file gets copied to 2 nodes)
- [ ] Simulate node failure by deleting a folder — app should still retrieve files
- [ ] Log storage activity for transparency

### 🟣 Phase 3: Extra Features
- [ ] User authentication (JWT or simple login)
- [ ] File versioning (track changes)
- [ ] Shareable file links (UUIDs)
- [ ] Basic web frontend for upload/download
- [ ] Real-time sync (polling every X seconds for new files)

## 📂 Folder Structure

dropboxify/ ├── app/ │ ├── api/ │ │ ├── routes.py │ ├── services/ │ │ ├── storage_handler.py │ ├── models/ │ │ ├── file_metadata.py │ ├── main.py ├── storage/ │ ├── node1/ │ ├── node2/ │ ├── node3/ ├── database/ │ ├── schema.sql ├── tests/ │ ├── test_api.py ├── Dockerfile ├── requirements.txt



## 🗓️ Milestones & Timeline

| Week | Task                                      |
|------|-------------------------------------------|
| 1    | Set up Flask app + upload/download APIs   |
| 2    | Implement metadata DB + file storage      |
| 3    | Add replication + simulate node failures  |
| 4    | Test + document the API                   |
| 5    | Optional features (auth, versioning, etc.)|
| 6    | Polish, Dockerize, deploy (if desired)    |

## 🌐 GitHub Setup Checklist
- [ ] Create GitHub repo
- [ ] Add `README.md` with:
  - Project intro
  - Features
  - Setup instructions
  - API endpoints
- [ ] Include system architecture diagram (use draw.io or Excalidraw)
- [ ] Deployment guide (Docker or AWS)

## 📚 Helpful Resources:
- [Flask Documentation](https://flask.palletsprojects.com/)
- [PostgreSQL Docs](https://www.postgresql.org/docs/)
- [Docker Docs](https://docs.docker.com/)
