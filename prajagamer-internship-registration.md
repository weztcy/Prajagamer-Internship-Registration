# Portfolio Project Data — Prajagamer - Internship Registration

- **Category:** `web-development` (`Web Development`)
- **Accent Color:** `cyan`
- **Target Assets Folder:** `public/images/projects/prajagamer_internship_registration/`
- **Required Local Images:** `banner.webp`, `image01.webp` .. `image07.webp`

## TypeScript Data (`ProjectCaseStudy`)

```typescript
{
  "id": "prajagamer-internship-registration",
  "code": "PRO-42 // WEB-06",
  "title": "Prajagamer - Internship Registration",
  "category": "web-development",
  "categoryLabel": "Website",
  "year": "2024",
  "status": "Completed",
  "accentColor": "cyan",
  "repoUrl": "https://github.com/weztcy/Prajagamer-Internship-Registration",
  "license": "MIT License",
  "banner": "/images/projects/prajagamer_internship_registration/banner.webp",
  "summary": "Full-stack internship registration and applicant review portal built for Disdukcapil Kota Semarang using React, Express, Prisma, and SQLite.",
  "projectDescription": "Full-stack internship portal for Disdukcapil Kota Semarang featuring NIK/NIP role authentication, multi-step document submission, live recruitment banner updates, WhatsApp status notifications, and an admin dashboard with Excel export powered by React, Express, Prisma, and SQLite.",
  "architectureSummary": "Decoupled React + Vite + Redux Persist SPA communicating over REST with an Express 5 backend backed by Prisma ORM, SQLite, and Multer file storage.",
  "techStack": [
    "React",
    "Vite",
    "Tailwind CSS",
    "Redux Toolkit",
    "Redux Persist",
    "React Router",
    "Axios",
    "Express",
    "Prisma",
    "SQLite",
    "Multer",
    "SheetJS",
    "Cropper.js"
  ],
  "telemetryMatrix": {
    "projectType": "Full-Stack Web Application",
    "targetPlatform": "Web Browser & Node.js Runtime",
    "primaryDomain": "Public Sector Internship Portal",
    "architecturePipeline": "React SPA -> Express API -> Prisma SQLite",
    "testingAndAudit": "Passed",
    "projectStatus": "Completed",
    "projectYear": "2024"
  },
  "projectInfo": {
    "projectType": "Full-Stack Web Portal",
    "developmentStatus": "Completed",
    "developmentYear": "2024",
    "platform": "Web (Responsive Desktop & Mobile)",
    "projectCategory": "Web Development"
  },
  "projectBackground": "Managing student internship intakes at Disdukcapil Kota Semarang previously relied on fragmented manual document intake and disconnected spreadsheets. Prajagamer unifies public program information, candidate registration, academic document uploads, and staff screening into one auditable web platform.",
  "problemStatements": [
    {
      "title": "Fragmented Applicant Intake & Verification",
      "description": "Collecting student identity data, university records, recommendation letters, CVs, and transcripts manually slowed screening across administrative staff.",
      "issueCode": "ISSUE_01"
    },
    {
      "title": "Lack of Real-Time Application Tracking",
      "description": "Administrators lacked a centralized dashboard to monitor pending, accepted, and rejected candidate counts or export structured rosters.",
      "issueCode": "ISSUE_02"
    },
    {
      "title": "Static Recruitment Announcements",
      "description": "Updating public internship open-recruitment banners required manual code edits rather than an administrative upload workflow.",
      "issueCode": "ISSUE_03"
    }
  ],
  "projectObjectives": [
    {
      "title": "Digitize End-to-End Registration",
      "description": "Deliver a guided multi-step workflow enabling students to register with NIK, complete profiles, and upload required PDFs and photos online.",
      "targetTag": "TARGET_01"
    },
    {
      "title": "Centralize Administrative Screening",
      "description": "Equip Disdukcapil staff with KPI counters, search/sort/pagination controls, document preview links, WhatsApp triggers, and .xlsx export.",
      "targetTag": "TARGET_02"
    },
    {
      "title": "Enable Self-Service Banner & Staff Management",
      "description": "Provide authenticated admins with dynamic recruitment banner replacement and CRUD management of administrator NIP accounts.",
      "targetTag": "TARGET_03"
    }
  ],
  "coreFeatures": [
    {
      "title": "Applicant Registration & Profile Portal",
      "description": "Supports NIK-based login, multipart registration with photo, CV, and transcript uploads, plus profile editing with Cropper.js and Emsifa regency lookup.",
      "badge": "Applicant Flow"
    },
    {
      "title": "Two-Step Internship Application Form",
      "description": "Validates placement willingness, enforces a minimum 30-day internship period, and submits recommendation letters, CVs, and portfolios via Multer.",
      "badge": "Submission"
    },
    {
      "title": "Admin Analytics & Status Screening",
      "description": "Displays Total, Verifying, Accepted, and Rejected metrics with searchable, sortable tables and one-click Accept/Reject status transitions.",
      "badge": "Admin Console"
    },
    {
      "title": "SheetJS Export & WhatsApp Dispatch",
      "description": "Generates formatted .xlsx workbooks of user and applicant datasets client-side and launches pre-filled wa.me status notifications.",
      "badge": "Operations"
    },
    {
      "title": "Dynamic Banner & Staff CRUD",
      "description": "Allows administrators to upload live Lowongan recruitment banners and create or remove NIP-authenticated admin accounts.",
      "badge": "Content & Access"
    }
  ],
  "interfaceShowcase": [
    {
      "imageUrl": "/images/projects/prajagamer_internship_registration/image01.webp"
    },
    {
      "imageUrl": "/images/projects/prajagamer_internship_registration/image02.webp"
    },
    {
      "imageUrl": "/images/projects/prajagamer_internship_registration/image03.webp"
    },
    {
      "imageUrl": "/images/projects/prajagamer_internship_registration/image04.webp"
    },
    {
      "imageUrl": "/images/projects/prajagamer_internship_registration/image05.webp"
    },
    {
      "imageUrl": "/images/projects/prajagamer_internship_registration/image06.webp"
    },
    {
      "imageUrl": "/images/projects/prajagamer_internship_registration/image07.webp"
    }
  ],
  "userFlow": {
    "summary": "Students register with NIK and academic documents, authenticate into a persisted Redux session, verify personal details, and submit a two-stage internship application, while administrators sign in via NIP to review files, update statuses, and export rosters.",
    "steps": [
      {
        "step": "01",
        "title": "Account Registration & Document Upload",
        "description": "Applicant submits NIK, NIM, university, major, and initial photo, CV, and transcript files to /api/user/register.",
        "actorOrNode": "Register.jsx -> /api/user/register"
      },
      {
        "step": "02",
        "title": "NIK Authentication & Session Persistence",
        "description": "Applicant signs in via /api/user/login and receives a bearer token stored in Redux Persist.",
        "actorOrNode": "Login.jsx -> Redux Persist"
      },
      {
        "step": "03",
        "title": "Two-Stage Internship Submission",
        "description": "User confirms placement availability in step 1, selects a 30+ day period and uploads recommendation letter and portfolio in step 2.",
        "actorOrNode": "FormPendaftaran1 & 2 -> /api/apply-internship"
      },
      {
        "step": "04",
        "title": "Admin Screening, Export & Notification",
        "description": "Admin logs in via NIP, inspects KPI cards and documents, updates status via PUT /api/users/status, exports .xlsx, or opens wa.me.",
        "actorOrNode": "DashboardAdmin & DataPelamar -> Express API"
      }
    ]
  },
  "systemArchitecture": {
    "summary": "A Vite-bundled React SPA communicates via Axios and Fetch with an Express 5 REST server. Controllers orchestrate Prisma ORM queries against SQLite while Multer writes uploaded documents and recruitment banners to disk under backend/uploads/ for static delivery.",
    "layers": [
      {
        "name": "Presentation & Client State",
        "role": "Renders responsive public, applicant, and admin views while persisting auth and form state.",
        "components": ["React", "React Router", "Redux Toolkit", "Redux Persist", "Tailwind CSS", "SheetJS"]
      },
      {
        "name": "API Gateway & Middleware",
        "role": "Routes REST endpoints, enables CORS, parses JSON/URL-encoded payloads, and handles file uploads.",
        "components": ["Express", "Multer", "CORS", "Static /uploads Middleware"]
      },
      {
        "name": "Controllers & Domain Logic",
        "role": "Processes NIK/NIP login, applicant registration, profile updates, dashboard aggregation, and banner upserts.",
        "components": ["authController", "internshipController", "bannerController", "userController"]
      },
      {
        "name": "Data & Media Persistence",
        "role": "Stores relational applicant records in SQLite and serves uploaded PDFs and images with sample fallbacks.",
        "components": ["Prisma Client", "SQLite (dev.db)", "Local Disk (backend/uploads/)"]
      }
    ]
  },
  "databaseDataFlow": {
    "type": "Database Schema / ERD",
    "summary": "Prisma models normalize applicant identity, academic metadata, and internship submissions into 1-to-1 relations anchored to User, complemented by standalone Admin and Banner tables.",
    "entitiesOrPipelines": [
      {
        "name": "User",
        "type": "Table",
        "fields": ["id", "name", "email", "password", "status", "createdAt", "updatedAt"]
      },
      {
        "name": "Profile",
        "type": "Table",
        "fields": ["id", "userId", "nik", "telp_user", "photo", "city_ktp", "city_domicile", "ipk", "semester", "name_supervisor"]
      },
      {
        "name": "University",
        "type": "Table",
        "fields": ["id", "userId", "nim", "univ_name", "major"]
      },
      {
        "name": "Regist",
        "type": "Table",
        "fields": ["id", "userId", "available_space", "recommend_letter", "cv", "portofolio", "score_list", "first_period", "last_period"]
      },
      {
        "name": "Admin",
        "type": "Table",
        "fields": ["id", "admin_name", "nip", "telp_admin", "email", "password", "createdAt"]
      },
      {
        "name": "Banner",
        "type": "Table",
        "fields": ["id", "name", "filename", "updatedAt"]
      }
    ]
  },
  "technicalImplementation": [
    {
      "category": "Orchestration & Seeding",
      "title": "Unified Zero-Config Runner & Seed Pipeline",
      "description": "Root runner.js detects missing backend/prisma/dev.db, runs prisma db push and seed.js to populate 26 applicants, 4 admins, and sample PDFs, and spawns both servers concurrently.",
      "badge": "DevOps"
    },
    {
      "category": "File Handling",
      "title": "Multer Disk Pipeline with Static Fallback",
      "description": "apiRoute.js stores multipart documents and banners with timestamped filenames in backend/uploads/, while Express middleware falls back to avatar_default.png or cv_sample.pdf when files are absent.",
      "badge": "Storage"
    },
    {
      "category": "Validation & UX",
      "title": "Two-Stage Form Validation & Duration Guard",
      "description": "FormPendaftaran1 and FormPendaftaran2 enforce placement consent, 5 MB file limits, and a 30-day minimum gap between first_period and last_period before dispatching FormData.",
      "badge": "Form Logic"
    },
    {
      "category": "Reporting & Outreach",
      "title": "Client-Side XLSX Generation & WhatsApp Links",
      "description": "DataPelamar.jsx and DataPengguna.jsx transform relational applicant records into downloadable Excel workbooks via SheetJS and format Indonesian 62-prefixed wa.me notification links.",
      "badge": "Automation"
    }
  ],
  "primaryTechSpecs": {
    "programmingLanguage": "JavaScript",
    "framework": "React & Express",
    "database": "SQLite"
  },
  "architectureQuality": {
    "badges": [
      "Modular REST API",
      "Persistent Client Store",
      "Multipart Upload Pipeline",
      "Relational Prisma Schema"
    ]
  }
}
```
