# Portfolio Project Data — Prajagamer - Internship Registration

- **Category:** `web-development` (`Web Development`)
- **Accent Color:** `cyan`
- **Target Assets Folder:** `public/images/projects/prajagamer_internship_registration/`
- **Required Local Images:** `banner.webp`, `image01.webp` .. `image07.webp`

## TypeScript Data (`ProjectCaseStudy`)

```typescript
{
  "id": "prajagamer-internship-registration",
  "code": "PRO-20 // WEB-06",
  "title": "Prajagamer - Internship Registration",
  "category": "web-development",
  "categoryLabel": "Website",
  "year": "2023",
  "status": "Completed",
  "accentColor": "cyan",
  "repoUrl": "https://github.com/weztcy/Prajagamer-Internship-Registration",
  "license": "MIT License",
  "banner": "/images/projects/prajagamer_internship_registration/banner.webp",
  "summary": "Full-stack internship registration portal and admin verification suite built for Disdukcapil Semarang using React, Express.js, Prisma, and SQLite.",
  "projectDescription": "A full-stack internship portal for Disdukcapil Semarang digitizing university student applications. It pairs a React and Redux frontend with an Express.js and Prisma SQLite backend for NIK-based registration, PDF uploads, admin review, WhatsApp notifications, and Excel reporting.",
  "architectureSummary": "React + Vite SPA with Redux Persist communicates via REST/Multipart HTTP to an Express.js API, Multer disk storage, and Prisma SQLite database.",
  "techStack": [
    "JavaScript",
    "React",
    "Vite",
    "Tailwind CSS",
    "Redux Toolkit",
    "Redux Persist",
    "React Router",
    "Axios",
    "Node.js",
    "Express.js",
    "Prisma",
    "SQLite",
    "Multer",
    "SheetJS"
  ],
  "telemetryMatrix": {
    "projectType": "Full-Stack Web Application",
    "targetPlatform": "Responsive Web Browser",
    "primaryDomain": "Public Sector Internship Portal",
    "architecturePipeline": "React SPA -> Express REST API -> SQLite",
    "testingAndAudit": "Manual End-to-End Verified",
    "projectStatus": "Completed",
    "projectYear": "2023"
  },
  "projectInfo": {
    "projectType": "Full-Stack Web Application",
    "developmentStatus": "Completed",
    "developmentYear": "2023",
    "platform": "Web",
    "projectCategory": "Web Development"
  },
  "projectBackground": "Disdukcapil Semarang receives internship applications from university students across Central Java, previously managed through manual paperwork and fragmented document checks. Prajagamer centralizes registration, document verification, and recruitment announcements into a single web platform.",
  "problemStatements": [
    {
      "title": "Fragmented Manual Internship Submissions",
      "description": "Students previously submitted physical or ad-hoc files including CVs, academic transcripts, and recommendation letters, making applicant tracking and document retrieval slow for agency staff.",
      "issueCode": "ISSUE_01"
    },
    {
      "title": "Delayed Applicant Status Visibility",
      "description": "Applicants lacked a unified digital portal to verify registration completeness, review placement terms, and receive timely acceptance or rejection updates.",
      "issueCode": "ISSUE_02"
    },
    {
      "title": "Manual Administrative Reporting Overhead",
      "description": "HR and administrative officers had no centralized dashboard to filter applicants, preview uploaded PDFs, update recruitment banners, or export structured spreadsheets.",
      "issueCode": "ISSUE_03"
    }
  ],
  "projectObjectives": [
    {
      "title": "Digitize End-to-End Application Intake",
      "description": "Enable university applicants to register with validated 16-digit NIK identifiers, maintain academic profiles, and submit required PDF documents through a guided two-step workflow.",
      "targetTag": "TARGET_01"
    },
    {
      "title": "Streamline Admin Review & Notifications",
      "description": "Provide staff with real-time KPI counts, search/sort controls, one-click document previews, and automated WhatsApp notification links upon status changes.",
      "targetTag": "TARGET_02"
    },
    {
      "title": "Deliver Exportable Administrative Reporting",
      "description": "Support instant Excel (.xlsx) report generation for both registered users and internship applicants alongside dynamic recruitment banner publishing.",
      "targetTag": "TARGET_03"
    }
  ],
  "coreFeatures": [
    {
      "title": "NIK-Validated Registration & Document Upload",
      "description": "Validates 16-digit NIK, password strength, email format, and file constraints (JPG/PNG photos and PDF CVs/transcripts under 5 MB) before persisting multi-table records.",
      "badge": "Onboarding"
    },
    {
      "title": "Two-Step Internship Application Workflow",
      "description": "Captures branch placement willingness on Step 1 and enforces minimum 30-day internship periods, recommendation letters, CVs, optional portfolios, and terms consent on Step 2.",
      "badge": "Application Flow"
    },
    {
      "title": "Applicant Profile & Regional Lookup",
      "description": "Displays personal, academic, and faculty supervisor details with profile editing powered by Indonesian province and regency lookup and image cropper stylesheet support.",
      "badge": "User Profile"
    },
    {
      "title": "Admin KPI Dashboard & Status Workflow",
      "description": "Aggregates total, verifying, accepted, and rejected counts in real time and enables staff to approve or reject applicants while launching pre-filled WhatsApp notifications.",
      "badge": "Admin Console"
    },
    {
      "title": "Client-Side Excel Spreadsheet Export",
      "description": "Converts filtered user and applicant datasets—including document availability and internship dates—into downloadable .xlsx workbooks via SheetJS.",
      "badge": "Reporting"
    },
    {
      "title": "Recruitment Banner & Admin Account CMS",
      "description": "Lets administrators upload updated recruitment announcement banners served via /api/banner and manage staff accounts by NIP.",
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
    "summary": "Students register with their NIK and academic documents, sign in to complete their profile, and submit a two-step internship form with dates and PDF attachments. Admins log in via NIP to inspect submissions, export Excel sheets, update statuses, and notify applicants.",
    "steps": [
      {
        "step": "01",
        "title": "Explore Public Portal & Recruitment Info",
        "description": "Visitors browse the Disdukcapil Semarang landing page, partner universities, internship requirements, and dynamic recruitment banner fetched from /api/banner.",
        "actorOrNode": "Applicant / React Portal"
      },
      {
        "step": "02",
        "title": "Account Registration & Multipart Upload",
        "description": "Applicants submit personal, university, and NIK credentials alongside photo, CV, and transcript files to POST /api/user/register.",
        "actorOrNode": "Register Page / Multer API"
      },
      {
        "step": "03",
        "title": "NIK Authentication & Profile Completion",
        "description": "Applicants authenticate via POST /api/user/login, persist their token in Redux, and update domicile or supervisor details in ProfileUser and EditProfile.",
        "actorOrNode": "Redux Auth / Profile API"
      },
      {
        "step": "04",
        "title": "Two-Step Internship Application",
        "description": "Applicants confirm branch placement willingness in FormPendaftaran1, then upload recommendation letter, CV, optional portfolio, and >=30-day period dates in FormPendaftaran2.",
        "actorOrNode": "Application Wizard / POST /api/apply-internship"
      },
      {
        "step": "05",
        "title": "Admin Verification, Notification & Export",
        "description": "Administrators sign in via NIP, review KPIs and uploaded PDFs, update statuses via PUT /api/users/status2 to trigger WhatsApp notifications, or export tables to Excel.",
        "actorOrNode": "Admin Dashboard / SheetJS & WhatsApp"
      }
    ]
  },
  "systemArchitecture": {
    "summary": "A decoupled full-stack web architecture orchestrated by a Node.js runner script. The React + Vite SPA uses Redux Persist for client state and communicates over REST with an Express.js server that coordinates Multer disk uploads and Prisma ORM queries against SQLite.",
    "layers": [
      {
        "name": "Presentation & State Layer",
        "role": "Renders responsive public, applicant, and admin views while persisting authentication and form state",
        "components": ["React", "Vite", "Tailwind CSS", "React Router DOM", "Redux Toolkit", "Redux Persist"]
      },
      {
        "name": "API & File Middleware Layer",
        "role": "Exposes REST endpoints for auth, profiles, applications, banners, and static file fallback serving",
        "components": ["Node.js", "Express.js", "CORS", "Multer", "Auth & Internship Controllers"]
      },
      {
        "name": "Persistence & Storage Layer",
        "role": "Maintains relational user/application records and persists uploaded PDFs and images on disk",
        "components": ["Prisma ORM", "SQLite (dev.db)", "Local Uploads Directory"]
      },
      {
        "name": "External Integrations",
        "role": "Provides Indonesian regency data for address forms and deep-linked applicant status notifications",
        "components": ["Emsifa Wilayah API", "WhatsApp Web (wa.me)"]
      }
    ]
  },
  "databaseDataFlow": {
    "type": "Database Schema / ERD",
    "summary": "Prisma manages six relational SQLite models centered on User with one-to-one cascading relations to Profile, University, and Regist, plus standalone Admin and Banner tables.",
    "entitiesOrPipelines": [
      {
        "name": "User",
        "type": "Table",
        "fields": ["id", "name", "email", "password", "status", "createdAt", "updatedAt"]
      },
      {
        "name": "Profile",
        "type": "Table",
        "fields": ["id", "userId", "nik", "telp_user", "photo", "city_ktp", "address_domicile", "ipk", "semester", "name_supervisor"]
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
      "title": "Zero-Config Local Bootstrap Runner",
      "description": "Custom runner.js detects missing SQLite database files on startup, executes Prisma schema push and seed.js to generate 4 admin accounts, 26 realistic applicant records, and placeholder PDFs, then spawns backend and frontend dev servers concurrently.",
      "badge": "Automation"
    },
    {
      "category": "File Handling & Reliability",
      "title": "Multipart Upload Pipeline with Asset Fallbacks",
      "description": "Express configures Multer disk storage with timestamped unique filenames and wraps the /uploads static middleware with automatic fallbacks to avatar_default.png or cv_sample.pdf so seeded previews never break.",
      "badge": "Storage"
    },
    {
      "category": "Validation & UX",
      "title": "Client-Side Constraint Enforcement",
      "description": "Registration enforces 16-digit numeric NIKs, uppercase/digit password rules, and 5 MB MIME checks, while FormPendaftaran2 enforces a minimum 30-day gap between internship start and end dates.",
      "badge": "Validation"
    },
    {
      "category": "Reporting & Communication",
      "title": "Browser-Side XLSX Export & WhatsApp Deep Links",
      "description": "DataPelamar and DataPengguna map relational Prisma JSON payloads into formatted Excel workbooks via SheetJS and convert local 08xx phone numbers into international 62xx wa.me links upon status approval or rejection.",
      "badge": "Admin Tools"
    }
  ],
  "primaryTechSpecs": {
    "programmingLanguage": "JavaScript",
    "framework": "React and Express.js",
    "database": "SQLite"
  },
  "architectureQuality": {
    "badges": [
      "Full-Stack REST",
      "Relational ORM",
      "Multipart Uploads",
      "Excel Reporting"
    ]
  }
}
```
