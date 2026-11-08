# Awesome-Virtual-Telephony-Call-Center

# Awesome Virtual Telephony & Call Center

> A curated list of top Virtual Telephony and Call Center platforms — both SaaS/Hosted commercial solutions and open-source alternatives for cloud PBX, inbound ACD, outbound dialing, and contact center operations.  
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [RingCentral MVP](#ringcentral-mvp)
  - [Nextiva](#nextiva)
  - [Dialpad](#dialpad)
  - [8x8](#8x8)
  - [Vonage Business Communications](#vonage-business-communications)
  - [Zoom Phone](#zoom-phone)
  - [Talkdesk](#talkdesk)
  - [GoTo Connect](#goto-connect)
  - [Ooma Office](#ooma-office)
- [Open-Source Software](#-open-source-software)
  - [VICIdial](#vicidial)
  - [FusionPBX](#fusionpbx)
  - [FS PBX](#fs-pbx)
  - [FreeSWITCH](#freeswitch)
  - [Asterisk](#asterisk)
  - [FreePBX](#freepbx)
  - [Wazo](#wazo)
  - [Comcent CE](#comcent-ce)
  - [AI Native Call Center](#ai-native-call-center)
  - [Fonoster](#fonoster)
  - [RustPBX](#rustpbx)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Virtual Telephony and Call Center platforms. These are not open-source but are included as reference points for feature comparison.

### RingCentral MVP
**Type:** Unified communications and contact center  
RingCentral is a leading cloud communications provider offering voice, video, team messaging, and contact center capabilities in a unified platform. Its MVP (Message, Video, Phone) suite is widely adopted for business telephony, with contact center add-ons for advanced routing and analytics.

### Nextiva
**Type:** Business communications and customer experience  
Nextiva provides cloud PBX, contact center, and customer experience management. Known for reliability and a strong focus on customer support, with AI-powered features for conversation analytics and workflow automation.

### Dialpad
**Type:** AI-powered cloud telephony and contact center  
Dialpad differentiates with native AI capabilities built on its own voice infrastructure, offering real-time transcription, sentiment analysis, and coaching. Its contact center solution includes skills-based routing, workforce management, and quality assurance.

### 8x8
**Type:** Integrated cloud communications and contact center  
8x8 offers unified communications, contact center, and CPaaS capabilities on a single platform. Suited for mid-market and enterprise organizations needing integrated voice, video, chat, and contact center in one vendor.

### Vonage Business Communications
**Type:** Cloud PBX and contact center (Ericsson)  
Vonage provides business cloud PBX with contact center add-ons, backed by its programmable communications APIs (now part of Ericsson). Offers flexible plans for small businesses through to enterprise deployments.

### Zoom Phone
**Type:** Cloud phone system within Zoom ecosystem  
Zoom Phone extends Zoom's meeting platform into cloud telephony, offering calling, SMS, and contact center capabilities. Best suited for organizations already standardized on Zoom for meetings and collaboration.

### Talkdesk
**Type:** Cloud contact center platform  
Talkdesk is purpose-built for contact centers, with AI-powered agent assistance, workforce engagement management, and industry-specific solutions. Positioned for customer experience teams needing deep contact center functionality rather than basic PBX.

### GoTo Connect
**Type:** Unified communications and contact center  
GoTo Connect (formerly GoToMeeting/GoToWebinar) provides cloud PBX and contact center with integrated meetings and webinars. Suited for small to mid-sized businesses wanting an all-in-one communications suite.

### Ooma Office
**Type:** Cloud phone system for small businesses  
Ooma Office targets small businesses with a straightforward cloud PBX offering, including virtual receptionist, ring groups, and mobile app support. A budget-friendly option for basic business telephony.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Virtual Telephony and Call Center tools. All listed projects offer source code you can deploy on your own infrastructure.

### VICIdial
**Stack:** PHP / Asterisk / MySQL | **License:** AGPLv2  
The dominant open-source contact center platform, purpose-built for **high-volume outbound operations**. Features include predictive dialing (monitors agent answer rates to maximize talk time with minimal dropped calls), progressive/ratio/preview/manual dialing modes, inbound ACD with skills-based routing, **blended campaigns** (agents handle both inbound and outbound in the same session), call recording, real-time monitoring with whisper/barge, lead list management with DNC scrubbing, and extensive reporting . Over 14,000 installations worldwide, with active development on SVN trunk (version 2.14b0.5 as of early 2026) . **Trade-off:** Web UI is functional but dated; you manage your own infrastructure.  
**Best for:** Organizations needing genuine predictive dialing and blended inbound/outbound contact center operations at scale, with tolerance for self-managed infrastructure.

### FusionPBX
**Stack:** PHP / FreeSWITCH / PostgreSQL | **License:** Open Source (per project)  
A full-featured domain-based multi-tenant PBX and voice switch built on FreeSWITCH. Provides carrier-grade switching with a web GUI covering extensions, device provisioning, voicemail-to-email, IVR menus, ring groups, call center queues, call recording, conference, fax server, and multi-tenancy . The official install script sets up FreeSWITCH, NGINX, PHP-FPM, PostgreSQL, iptables, and Fail2ban on Debian/Ubuntu/FreeBSD/CentOS . **Important:** FusionPBX handles **inbound queue-based call center** functionality well, but it is **not** a viable option for outbound predictive dialing at meaningful scale — no campaign management, lead list handling, or predictive algorithms .  
**Best for:** Organizations needing a multi-tenant PBX with solid inbound ACD/queues, rather than high-volume outbound dialing.

### FS PBX
**Stack:** Laravel / Vue / FreeSWITCH / PostgreSQL | **License:** Apache 2.0  
A modern open-source PBX built on FreeSWITCH with a redesigned Laravel/Vue/Tailwind stack, forked from FusionPBX but extensively redeveloped. Includes extensions, CDR, voicemail, ring groups, IVRs, time-based routing, **contact center functionality**, fax, firewall management, and device provisioning . A **premium Contact Center module** adds live visibility and queue-management workflows. Requires Debian 12/13, 4 GB RAM, 30 GB disk. Install via a single script .  
**Best for:** Teams wanting FusionPBX-style multi-tenant PBX functionality with a modern, maintainable codebase and an optional contact center module.

### FreeSWITCH
**Stack:** C | **License:** MPL-2.0  
The highly scalable, multi-platform voice switch that powers FusionPBX, FS PBX, and many commercial platforms. FreeSWITCH is a **telephony framework**, not a turnkey call center — it handles SIP connectivity, call routing, codec transcoding, and VoIP protocol management, but **does not** include campaigns, lead lists, agent states, or predictive dialing . You build call center functionality on top of it (or use a GUI like FusionPBX/FS PBX).  
**Best for:** Developers and platform builders wanting a rock-solid, scalable telephony engine as the foundation for a custom PBX or contact center.

### Asterisk
**Stack:** C | **License:** GPL-2.0  
The other major open-source telephony engine, and the foundation for VICIdial, FreePBX, Issabel, and Wazo. Like FreeSWITCH, Asterisk is a **PBX framework** — it provides SIP connectivity, routing, and codec handling, but not contact center workflow. Building a call center on bare Asterisk requires substantial engineering .  
**Best for:** Organizations building custom telephony solutions or running platforms (VICIdial, FreePBX) that depend on Asterisk.

### FreePBX
**Stack:** PHP / Asterisk / MySQL | **License:** GPL-2.0  
A web-based GUI for managing Asterisk, now owned by Sangoma. Excellent for extensions, ring groups, IVRs, voicemail, and inbound call routing . **Important distinction:** FreePBX is a **business phone system, not a contact center platform** — it does not handle outbound dialing campaigns, predictive dialing, lead list management, or real-time agent performance monitoring . Sangoma offers commercial contact center add-ons, but those are proprietary.  
**Best for:** Small to mid-sized businesses needing a straightforward Asterisk-based PBX, not high-volume contact center operations.

### Wazo
**Stack:** Python / Asterisk | **License:** GPL-3.0  
A modern Asterisk-based platform with a microservices architecture and modern APIs. Wazo has a contact center module handling **inbound queues and basic agent management**, but its call center functionality is limited to inbound queue distribution — no predictive dialing or outbound campaign management .  
**Best for:** Organizations wanting a modern, API-first PBX with basic inbound ACD, not outbound dialing.

### Comcent CE
**Stack:** Docker / FreeSWITCH / PostgreSQL | **License:** Open Source (Community Edition)  
An open-source contact center platform with a modern installer. Features include a built-in agent desktop, S3-compatible storage for recordings, optional AI transcription (Deepgram) and summaries (OpenAI), and Twilio SIP trunk integration. Deploys via Docker Compose with an installer script that handles secrets generation and configuration .  
**Best for:** Teams wanting a modern, Docker-deployed contact center foundation with optional AI features.

### AI Native Call Center
**Stack:** Go / FreeSWITCH / PostgreSQL | **License:** Open Source (per GitHub)  
An open-source call center where **AI answers calls by default** via speech-to-speech models (OpenAI, Grok, Qwen, Doubao). A flow steers the conversation and decides when to transfer to a human queue. When transferred, the agent's screen pops with the bot-phase transcript before the phone rings. One Go binary + PostgreSQL + FreeSWITCH. Includes a live wallboard, queue view, and roster for supervisors .  
**Best for:** Teams wanting AI-first call handling with seamless human handover, particularly for high-volume inbound scenarios.

### Fonoster
**Stack:** Node.js / TypeScript | **License:** MIT  
An open-source programmable telecommunications stack positioned as a Twilio alternative. Provides a Node.js SDK for building voice applications with verbs like Answer, Play, Say, Gather, Dial, Record, and Stream . Features include multitenancy, PBX deployment, OAuth2/JWT authentication, RBAC, S3 storage support, and Google Speech API integration . API-first design where everything is programmable.  
**Best for:** Developers wanting to build custom voice applications and programmable telephony without Twilio's pricing.

### RustPBX
**Stack:** Rust | **License:** Open Source (per project)  
A high-performance software-defined PBX built in Rust, with all call control externalized via HTTP/WebSocket/Webhook for programmability in any language . Ships in four editions: Community (core PBX + queue/archive/transcript), Commerce, Wholesale, and **Contact Center** (agents, skill groups, ACD, wallboards). Commercial editions run in trial mode out of the box. Deploys via Docker or builds from source.  
**Best for:** Teams wanting a modern, Rust-based PBX with a dedicated Contact Center edition and API-driven call control.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Outbound Predictive | Inbound ACD | Multi-Tenant | Self-Hosted | Best For |
|----------|---------|-------|---------------------|-------------|--------------|-------------|----------|
| **RingCentral** | Proprietary | Cloud | (add-on) | ✅ | ❌ | ❌ | Unified UC + CC |
| **Dialpad** | Proprietary | Cloud | Limited | ✅ | ❌ | ❌ | AI-native contact center |
| **Talkdesk** | Proprietary | Cloud | Limited | ✅ | ❌ | ❌ | Purpose-built CC |
| **VICIdial** | AGPLv2 | PHP/Asterisk | ✅ Full | ✅ | ✅ | ✅ | High-volume outbound + blended |
| **FusionPBX** | Open Source | PHP/FreeSWITCH | ❌ | ✅ Queues | ✅ | ✅ | Multi-tenant PBX + inbound ACD |
| **FS PBX** | Apache 2.0 | Laravel/FreeSWITCH | ❌ | ✅ (Premium) | ✅ | ✅ | Modern PBX + optional CC |
| **FreeSWITCH** | MPL-2.0 | C | ❌ (framework) | ❌ (framework) | ✅ (via GUI) | ✅ | Telephony engine foundation |
| **Asterisk** | GPL-2.0 | C | ❌ (framework) | ❌ (framework) | (via GUI) | ✅ | Telephony engine foundation |
| **FreePBX** | GPL-2.0 | PHP/Asterisk | ❌ | ✅ Basic | Limited | ✅ | Business PBX, not CC |
| **Wazo** | GPL-3.0 | Python/Asterisk | ❌ | ✅ Basic | (Check) | ✅ | Modern API-first PBX |
| **Comcent CE** | Open Source | Docker/FreeSWITCH | (Check) | (Check) | (Check) | ✅ | Modern CC with AI |
| **AI Native CC** | Open Source | Go/FreeSWITCH | ❌ | ✅ (AI-first) | ❌ | ✅ | AI answer + human handover |
| **Fonoster** | MIT | Node.js | ❌ | (Programmable) | ✅ | ✅ | Twilio alternative (CPaaS) |
| **RustPBX** | Open Source | Rust | (Contact Center ed.) | ✅ (CC edition) | (Check) | ✅ | Rust-based PBX + CC edition |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Virtual Telephony or Call Center platform that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source. Note that the open-source ecosystem splits sharply between **PBX platforms** (FusionPBX, FreePBX, FS PBX) and **contact center platforms** (VICIdial); few tools excel at both. Predictive dialing in particular is almost exclusively the domain of VICIdial among open-source options.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
