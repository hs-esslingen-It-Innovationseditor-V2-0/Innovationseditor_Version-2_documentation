# Innovationseditor_Version-2
A project to replace the Version 1 Editor-tool of "Hochschule Esslingen" to create, edit and bundle "abstracts" of students final theses into a book/pdf.


## Overview

This project contains a backend (Spring Boot), frontend (Angular), R-Proxy (Traefik) and is dockerized.

## Features
At the moment the following features are implemented:
- Writing text in an editor
- Adding Sources and Pictures in editor
- Saving text from editor into postgreSQL database
- authentication and authorization via an external Keycloak instance
- Basic API (documentation NOT up to date)


## Projektstruktur
Organisation: [ hs-esslingen-It-Innovationseditor-V2-0](https://github.com/hs-esslingen-It-Innovationseditor-V2-0https://github.com/hs-esslingen-It-Innovationseditor-V2-0)
```
IT-Innovationseditor-V2-0/
│
├── backend          # Spring Boot Backend (Java)
├── frontend         # Angular Frontend (TypeScript)
├── documentation    # Architektur, API und Datenmodell
├── pdf-worker       # Markdown to PDF Converter **NOT IMPLEMENTED**
└── setup-files      # docker-compose file for server setup
```


## Lizenz

Siehe [LICENSE](LICENSE).
