<div align="center">

# Angelo Marzocchi

### Android Engineer · Full-Stack Developer

**Kotlin · Jetpack Compose · Spring Boot · Angular · Google Cloud**

I build and ship production software end to end — native Android apps on the Play Store
and a B2B SaaS that businesses pay for and use every day.
I care about architecture as much as I care about the last pixel of the UI.

[![Website](https://img.shields.io/badge/SafeTrack_AI-0B5FFF?style=flat-square&logo=googlechrome&logoColor=white)](https://safetrackai.it)
[![Google Play](https://img.shields.io/badge/Big_Goal_on_Play-3DDC84?style=flat-square&logo=googleplay&logoColor=white)](https://play.google.com/store/apps/details?id=com.biggoal)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/angelo-marzocchi-46563b182)
[![Email](https://img.shields.io/badge/Email-6D4AFF?style=flat-square&logo=protonmail&logoColor=white)](mailto:angelomarzocchi@proton.me)

</div>

---

## 🚀 Shipped and running

> These two are my main work. They are commercial products, so the repositories are private —
> the links go to the live product instead of the source.

<br>

### SafeTrack AI — AI-powered HACCP & food traceability platform

[![Live](https://img.shields.io/badge/live-safetrackai.it-0B5FFF?style=flat-square&logo=googlechrome&logoColor=white)](https://safetrackai.it)
![Status](https://img.shields.io/badge/commercial-in%20production-2ea44f?style=flat-square)
![Source](https://img.shields.io/badge/source-private-lightgrey?style=flat-square)

A SaaS that moves food-safety compliance from paper to the cloud: digital HACCP records,
automatic lot traceability and 24/7 fridge monitoring — so a health inspection becomes an
export, not a week of rebuilding binders.

**Designed and built end to end**, from the database migrations to the landing page.

- **AI document extraction** — delivery notes and lot labels are read from a photo by
  Gemini on Vertex AI, with a custom multi-model fallback chain, structured response
  schemas, retry-with-jitter and image preprocessing to keep token cost down.
- **IoT temperature monitoring** — wireless probes stream over MQTT into the backend, which
  deduplicates readings, detects sensors going silent and escalates an unacknowledged alarm
  from push to email.
- **Backend** — Spring Boot, feature-oriented modules, Spring Data JPA over Cloud SQL
  (PostgreSQL) with Flyway migrations, JWT + refresh tokens, TOTP 2FA with recovery codes
  and role/permission based access.
- **Frontend** — Angular 21 standalone components, lazy-loaded feature routes, i18n and SEO.
- **Platform** — Cloud Run, Cloud Storage with automatic tiering of cold documents,
  Cloud Scheduler for the cross-replica jobs, Web Push (VAPID) and FCM, subscription plans
  and quota enforcement.

<br>

### Big Goal — goal planning, live on Google Play

[![Google Play](https://img.shields.io/badge/Google_Play-com.biggoal-3DDC84?style=flat-square&logo=googleplay&logoColor=white)](https://play.google.com/store/apps/details?id=com.biggoal)
![Status](https://img.shields.io/badge/released-v1.5-2ea44f?style=flat-square)
![Source](https://img.shields.io/badge/source-private-lightgrey?style=flat-square)

An Android app that breaks a big objective into milestones and tasks — alone or together.
Shared goals are joined with a short invite code, and progress is rewarded with XP,
streaks, twelve levels and medals.

- **Kotlin Multiplatform** project structure with a **Jetpack Compose** UI and Material 3.
- **Firebase** backend — Firestore with hand-written security rules *and a test suite for
  them*, Cloud Functions in TypeScript for invite handling.
- **Verified Android App Links** with a static fallback page, so an invite still works when
  the app isn't installed — the code never leaves the browser.
- **CI/CD on GitHub Actions**: Android build, Functions and Firestore-rules pipelines,
  staging and production deploys.
- Localised in **5 languages** (EN · IT · DE · ES · FR), adaptive on foldables.

---

## 🧩 Open source

Public repositories, where the code — not the product — is the point.

| Project | What it is | Stack &amp; focus |
| :--- | :--- | :--- |
| **[Red Cable Club](https://github.com/angelomarzocchi/RedCableClub)** | A native rewrite of OnePlus' Red Cable Club, born as an answer to a sluggish web app — [featured on the OnePlus community](https://community.oneplus.com/thread/1952269719625007110) | Kotlin · Jetpack Compose · custom animations<br>**Focus:** proving a Material app can still have a personality of its own |
| **[Hacker News Client](https://github.com/angelomarzocchi/HackerNews)** | A fast, clean client for browsing Hacker News | Kotlin · Compose · Paging 3 · Retrofit · Coroutines &amp; Flow<br>**Focus:** MVVM, incremental loading, Material 3 and dynamic color |
| **[Sealed Train](https://github.com/angelomarzocchi/SealedTrain-Client)** | Encrypted QR train tickets — client, [server](https://github.com/angelomarzocchi/SealedTrain-Server) and a [write-up](https://angelomarzocchi.notion.site/QR-Codes-Encryption-to-protect-confidentiality-and-ensure-non-replicability-998258a8823d4be9a7d7dbd4de3c13e9) | Kotlin · Retrofit · cryptography<br>**Focus:** confidentiality and non-replicability of a physical token |
| **[Parallel Sorting](https://github.com/angelomarzocchi/parallelMergeSort)** | Parallel merge sort and bitonic sort for multi-core CPUs | C · OpenMP<br>**Focus:** workload partitioning, barrier synchronisation, benchmarking |

---

## 🛠 Tech stack

**Mobile**<br>
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white)
![Kotlin Multiplatform](https://img.shields.io/badge/Multiplatform-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![Material 3](https://img.shields.io/badge/Material%203-757575?style=flat-square&logo=materialdesign&logoColor=white)

**Backend &amp; Web**<br>
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-DD2C00?style=flat-square&logo=firebase&logoColor=white)

**Cloud &amp; Tooling**<br>
![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Vertex AI](https://img.shields.io/badge/Vertex%20AI%20%C2%B7%20Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

<div align="center">

### Open to interesting Android and full-stack work.

[![LinkedIn](https://img.shields.io/badge/Let's%20talk-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/angelo-marzocchi-46563b182)
[![Email](https://img.shields.io/badge/Write%20to%20me-6D4AFF?style=for-the-badge&logo=protonmail&logoColor=white)](mailto:angelomarzocchi@proton.me)

</div>
