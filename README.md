<img src="https://capsule-render.vercel.app/api?type=rect&color=0:12100e,100:1d1a16&height=150&text=Sebastian%20Chirinos&fontColor=f3efe4&fontSize=46&fontAlignY=42&desc=Software%20Engineer%20%C2%B7%20Arequipa,%20Peru&descAlignY=72&descSize=16&descColor=27f5a9" alt="Sebastian Chirinos — Software Engineer, Arequipa, Peru" width="100%"/>

<p align="center">
  <a href="https://sebastian-cn-portfolio.vercel.app"><img src="https://img.shields.io/badge/Portfolio-27f5a9?style=for-the-badge&logo=vercel&logoColor=14120f" alt="Portfolio"/></a>
  <a href="https://sebastian-cn-portfolio.vercel.app/cv/CV_Sebastian_Chirinos_FULLSTACK.pdf"><img src="https://img.shields.io/badge/CV-f3efe4?style=for-the-badge&logo=readme&logoColor=14120f" alt="CV"/></a>
  <a href="https://www.linkedin.com/in/sebastian-arley-chirinos-negr%C3%B3n-1762102a3/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:schirinosne@gmail.com"><img src="https://img.shields.io/badge/Email-12100e?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

I build software people use every day: a point of sale that keeps selling when the internet drops, calibration
certificates a technician opens by scanning the instrument, an Android app that screens for anemia without
sending a single photo off the phone.

Everyone has the same code generator now. What I bring is the decisions around the code: what belongs in the
system, what it costs, and where it breaks at ten times the size. I write those decisions down.

- 🎓 Systems Engineering, **Universidad Nacional de San Agustín** (UNSA), Arequipa
- 🚀 **7 systems in production**: web platforms, e-commerce, a POS, cloud infrastructure, on-device AI
- 🌎 Open to remote Software Engineering roles · UTC-5 · English C1

---

## 🏗️ In production

| | Project | What it is | The decision that shaped it | Links |
|---|---|---|---|---|
| 🎯 | **Lo Exacto** | Corporate platform built for search visibility and fast loads | Static generation for public pages, server rendering for the dashboard, one database | [site](https://www.lo-exacto.com/) |
| 📐 | **Calitop Services** | Service catalog and admin dashboard for a surveying company | Catalog reads are cached and may lag; every write goes through the transactional path | [site](https://www.calitop-services.com/) · [code](https://github.com/BastleyNait/CALITOP-WEB) |
| 🛰️ | **GEOTOP AQP** | Online store for surveying equipment (PrestaShop), plus a system serving 900+ calibration certificates from a QR printed on each instrument | Every change goes through a staging store with its own database; a deploy moves only theme files and backs up the live theme first | [site](https://geotop-aqp.com) · [code](https://github.com/BastleyNait/GEOTOP-WEB) · [certificates](https://sebastian-cn-portfolio.vercel.app/case-studies/geotop-certificates) |
| 🧾 | **Boom POS & CRM** | Point of sale and CRM for a real store, 100+ sales a day | The cart lives on the client; the server records each sale as one idempotent transaction | [site](https://boom-pos.vercel.app/) · [case study](https://sebastian-cn-portfolio.vercel.app/case-studies/boom-pos) |
| 💻 | **Revolt Laptops** | Store and admin panel for my own refurbished-laptop business | Stock is decremented inside the order transaction, so a unique unit cannot sell twice | [site](https://revolt-laptops.vercel.app/) · [code](https://github.com/BastleyNait/REVOLT-LAP) |
| 🩸 | **Anemivision** | Native Android app that screens for anemia from a photo of the eyelid | The model ships inside the app, so no patient image ever leaves the phone | [code](https://github.com/BastleyNait/ANEMIVISION) · [case study](https://sebastian-cn-portfolio.vercel.app/case-studies/anemivision) |

Case studies, architecture decision records and screenshots are on the **[portfolio →](https://sebastian-cn-portfolio.vercel.app)**

---

## 🔭 Other things I've built

<table>
<tr>
<td width="50%" valign="top">

### 🕵️ [Deal Hunter](https://github.com/BastleyNait/DEAL-HUNTER)
A bot that watches eBay for laptops worth refurbishing, scores every listing 0–100 and pings me on
Telegram when one is a real bargain. It runs as a Supabase Edge Function on `pg_cron`, and the search
criteria live in a database row, so I change what it hunts for without redeploying.
Paired with a **[Vue 3 dashboard](https://github.com/BastleyNait/DEAL-WEB)**.

`TypeScript` · `Deno` · `Supabase` · `PostgreSQL` · `Vue 3`

</td>
<td width="50%" valign="top">

### 🐶 [PERR-DIDOS](https://github.com/BastleyNait/PERRDIDOS)
A Unity game: fly a delivery drone to feed lost dogs before the battery runs out, while wind zones push
you back. Ten levels, each defined as data (`LevelData` assets) instead of hard-coded scenes.

`Unity` · `C#`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📨 [TelnetMail](https://github.com/BastleyNait/TelnetMail-Attachment)
Sends email with attachments by talking raw SMTP over a Telnet socket: the handshake, `AUTH`, and the
MIME multipart body with Base64 attachments, all written by hand. No `smtplib`.

`Python` · `SMTP` · `MIME`

</td>
<td width="50%" valign="top">

### 🧭 [Course recommender](https://github.com/BastleyNait/LAB01-04-TABD)
Semantic search over my school's course catalog: describe your interests and skills in plain words,
get the courses closest to them. Embeddings stored and queried in a vector database.

`Python` · `ChromaDB` · `Embeddings`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🗺️ [AQP Explorer](https://github.com/BastleyNait/AQP-EXPLORER)
Native Android tourism guide for Arequipa, built with a five-person team. MVVM with Jetpack Compose.

`Kotlin` · `Jetpack Compose` · `MVVM`

</td>
<td width="50%" valign="top">

### ♿ [MediNotis](https://github.com/BastleyNait/FomulaioMedicina)
Medication reminder prototype designed around accessibility: the whole UI rescales its text from
100% up to 180% at runtime, for people who cannot read small print.

`Kotlin` · `Jetpack Compose` · `Accessibility`

</td>
</tr>
</table>

> 📌 The **pinned repositories** above are the fundamentals: data structures, algorithms and operating systems,
> implemented from scratch.

---

## 🛠️ Stack

<table>
<tr>
<td width="150"><b>Languages</b></td>
<td><img src="https://skillicons.dev/icons?i=ts,js,py,kotlin,java,cs,php&theme=dark&perline=8" height="40" alt="TypeScript, JavaScript, Python, Kotlin, Java, C#, PHP"/></td>
</tr>
<tr>
<td width="150"><b>Frontend</b></td>
<td><img src="https://skillicons.dev/icons?i=react,nextjs,vue,astro,tailwind,bootstrap&theme=dark&perline=8" height="40" alt="React, Next.js, Vue, Astro, Tailwind CSS, Bootstrap"/></td>
</tr>
<tr>
<td width="150"><b>Backend</b></td>
<td><img src="https://skillicons.dev/icons?i=nodejs,fastapi,flask,django&theme=dark&perline=8" height="40" alt="Node.js, FastAPI, Flask, Django"/></td>
</tr>
<tr>
<td width="150"><b>Databases</b></td>
<td><img src="https://skillicons.dev/icons?i=postgres,supabase,mysql,mongodb,redis&theme=dark&perline=8" height="40" alt="PostgreSQL, Supabase, MySQL / MariaDB, MongoDB, Redis"/></td>
</tr>
<tr>
<td width="150"><b>Mobile & games</b></td>
<td><img src="https://skillicons.dev/icons?i=androidstudio,kotlin,unity&theme=dark&perline=8" height="40" alt="Android, Kotlin, Unity"/></td>
</tr>
<tr>
<td width="150"><b>AI / ML</b></td>
<td><img src="https://skillicons.dev/icons?i=tensorflow,pytorch&theme=dark&perline=8" height="40" alt="TensorFlow Lite, PyTorch"/></td>
</tr>
<tr>
<td width="150"><b>Cloud & DevOps</b></td>
<td><img src="https://skillicons.dev/icons?i=gcp,aws,vercel,docker,nginx,linux,git&theme=dark&perline=8" height="40" alt="Google Cloud, AWS, Vercel, Docker, Nginx, Linux, Git"/></td>
</tr>
</table>

---

## 📊 Activity

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=BastleyNait&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&bg_color=12100e&title_color=27f5a9&icon_color=27f5a9&text_color=f3efe4" alt="GitHub stats"/>
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=BastleyNait&layout=compact&hide_border=true&bg_color=12100e&title_color=27f5a9&text_color=f3efe4&langs_count=8" alt="Most used languages"/>
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=BastleyNait&hide_border=true&background=12100e&ring=27f5a9&fire=27f5a9&currStreakLabel=27f5a9&sideLabels=f3efe4&currStreakNum=f3efe4&sideNums=f3efe4&dates=a8a39a&stroke=3a3530" alt="GitHub streak"/>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=BastleyNait&style=flat-square&color=27f5a9&label=profile+views" alt="Profile views"/>
</p>
