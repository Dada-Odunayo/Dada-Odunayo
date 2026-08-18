<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F766E,50:14B8A6,100:2DD4BF&height=200&section=header&text=Odunayo%20Dada&fontSize=48&fontColor=ffffff&fontAlignY=36&desc=Payments%20Mobile%20Engineer%20%C2%B7%20AI%20Agent%20Systems&descAlignY=58&descSize=18" width="100%" />

### 💳 I build the apps that move money — and the agents that decide whether they should

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/odunayo-dada-659941158/)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@dadaodunayo6)
[![Dev.to](https://img.shields.io/badge/dev.to-0A0A0A?style=for-the-badge&logo=devdotto&logoColor=white)](https://dev.to/odunayo_dada)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/DADA_ODUNAYO)
[![YouTube](https://img.shields.io/badge/OdunCodes-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/channel/UCtOQXJOpegh9ukuNcPdT1Ug)

</div>

---

I build the Android and React Native apps merchants use to take money, and the dashboards their operators use to find out why some of those payments didn't go through.

Lately I've been building AI agent systems for the same domain — merchant onboarding, compliance review, risk scoring. Payments work teaches you to distrust any decision you can't trace, so the agents I build come with approval gates and audit trails rather than confident answers.

---

## 🏧 &nbsp;What I Work On

<table>
<tr>
<td width="50%" valign="top">

### 📟 POS Terminal App
`Kotlin` · `Android` · `SmartPOS`

Card-insertion and EMV flows, PIN entry, authorization, response handling. Most of the job is closing the gap between *"this transaction should work"* and *"this transaction worked on this terminal, with this card, on this scheme"* — contactless taps failing while chip insertions succeed, PIN block errors, routing that dead-ends between terminal and issuer.

</td>
<td width="50%" valign="top">

### 📱 Merchant App
`React Native` · `TypeScript`

Transaction management, payment collection, and merchant dashboards. React Query and RTK Query over REST.

### ⚡ Real-Time Notifications
`WebSocket` · `OkHttp`

Merchants need to know a payment landed *now*, not in forty seconds. The first version used STOMP over WebSocket and dropped connections, so I rebuilt it on raw WebSocket with explicit connection management, retry, and reconnection.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔳 QR Payments
`Token generation` · `Validation`

Payment token generation through scan, validation, and completion — with attention to token expiry and what happens when the network isn't there.

</td>
<td width="50%" valign="top">

### 📊 Transaction Analytics
`Power BI` · `DAX`

Success rates, failure patterns, value and volume trends, merchant adoption, terminal utilization. Turning *"payments are failing"* into *"payments are failing on these terminals, at this hour, for this reason."*

</td>
</tr>
</table>

---

## 🤖 &nbsp;Agent Systems With Human Approval Gates

Two projects built with Qwen Cloud models, both in areas where an unexplained automated decision is a real problem.

<div align="center">

[![MerchantPilotAI](https://github-readme-stats.vercel.app/api/pin/?username=Dada-Odunayo&repo=MerchantPilotAI&theme=tokyonight&hide_border=true&border_radius=12)](https://github.com/Dada-Odunayo/MerchantPilotAI)
[![DevTeamAI](https://github-readme-stats.vercel.app/api/pin/?username=Dada-Odunayo&repo=DevTeamAI&theme=tokyonight&hide_border=true&border_radius=12)](https://github.com/Dada-Odunayo/DevTeamAI)

</div>

**🏦 MerchantPilotAI** — Merchant onboarding and compliance review. Agents handle intake, verification, risk scoring, and compliance mapping; a human approves, rejects, or asks for more. Model output is requested as strict JSON and validated with Pydantic before anything is persisted, with timeouts and retries around the call. Nigerian CAC documents are parsed locally with `pypdf` and the extracted business name fuzzy-matched against what the merchant submitted, producing a confidence score and reasons rather than a verdict. Every step writes to an audit trail.

**🧑‍💻 DevTeamAI** — A staged multi-agent pipeline that turns a product brief into a PRD, architecture plan, API spec, schema, and test plan. Each stage is gated on human approval and can be revised with feedback; conflicts between agents are surfaced and resolved rather than silently averaged out. It also runs the same brief through a single agent and scores the two against each other, because *"more agents"* is a claim that should have to prove itself.

> 🧪 Both were built for the Qwen Cloud hackathon — read them as design exercises rather than shipped products. CAC verification and object storage are deliberately stubbed behind adapters.

---

## 🛠️ &nbsp;Stack

<div align="center">

**Mobile**

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

**Backend & Data**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=for-the-badge&logo=nodedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

**Tools**

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

</div>

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Dada-Odunayo&layout=compact&theme=tokyonight&hide_border=true&border_radius=12&langs_count=8" height="165" />

<br/><br/>

**💬 Open to conversations about payments infrastructure, agent systems, or anything where a wrong decision needs to be traceable.**

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2DD4BF,50:14B8A6,100:0F766E&height=120&section=footer" width="100%" />

</div>
