# Awesome Virtual Telephony & Call Center

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Track Awesome List](https://www.trackawesomelist.com/badge.svg)](https://www.trackawesomelist.com/ishandutta2007/Awesome-Virtual-Telephony-Call-Center/)

> A curated list of top **Virtual Telephony**, **Cloud PBX**, **Contact Center as a Service (CCaaS)**, and **Call Center** platforms — covering enterprise SaaS hosted solutions and open-source alternatives for inbound ACD, predictive outbound dialing, WebRTC, SIP trunking, and AI-powered voice automation.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
- [Open-Source Software](#-open-source-software)
- [Feature Comparison Matrix](#-feature-comparison-matrix)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📈 Sector Overview & Market Dynamics

The global Cloud Telephony, Cloud PBX, and Contact Center as a Service (CCaaS) market is estimated at **$26.5B – $29.5B in 2025** and projected to exceed **$32B+ by 2026**, expanding at a 9%–11% CAGR for core voice/UCaaS and over 18%–22% CAGR for AI-integrated CCaaS workloads.

The sector is **moderately concentrated at the enterprise level**—dominated by top-tier incumbents like Zoom, RingCentral, 8x8, and Talkdesk—yet maintains a **heavily fragmented mid-market and long tail** composed of regional VoIP carriers, specialized CPaaS providers, and an active open-source ecosystem addressing local telecom compliance and self-hosted privacy requirements.

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Virtual Telephony and Call Center platforms. Sorted in descending order by company scale (market valuation / ARR).

| Platform | Valuation / Revenue | Starting Price | Free Tier / Trial Limits | Key Telephony & Call Center Capabilities |
|---|---|---|---|---|
| **[Zoom Phone](https://www.zoom.com/en/products/voip-phone/)** | ~$25.0B Market Cap (~$4.5B+ ARR) | $10.00 / user / month (US/Canada Metered) or $15.00 / user / month (Unlimited Regional) | No ongoing free trial for phone lines; live product demos available; 40-minute limit applies only to bundled basic Zoom Meetings | Cloud PBX integrated into the Zoom Workplace suite; native call routing, auto-attendant IVR, SMS/MMS, call recording, and optional CCaaS add-ons. |
| **[Talkdesk](https://www.talkdesk.com/)** | ~$10.0B Peak Valuation (~$300M+ ARR) | $25.00 / user / month (Talkdesk Express) or $85.00 / user / month (CX Cloud Digital Essentials) | 15-day free trial (Talkdesk Express) capped at 10 user seats with pre-loaded outbound communications credit | Enterprise-grade AI-native Contact Center as a Service (CCaaS); workforce engagement management (WEM), omnichannel routing, AI agent assistance, and deep CRM connectors. |
| **[RingCentral MVP](https://www.ringcentral.com/)** | ~$6.8B Market Cap (~$2.5B+ ARR) | $20.00 / user / month (Core tier, billed annually) | 14-day free trial limited to maximum 5 users, up to 2 desktop IP test phones, and excludes SMS functionality | Industry-leading unified communications (UCaaS) and cloud PBX platform; automated IVR, call recording, team messaging, video conferencing, and RingCX contact center integration. |
| **[Vonage Business Communications](https://www.vonage.com/unified-communications/)** | $6.2B Acquisition by Ericsson (~$1.3B+ ARR) | $19.99 / user / month (Mobile tier) or $29.99 / user / month (Premium tier) | No free trial offered; pay-from-day-one subscription with custom pilot demos upon request | Scalable cloud PBX backed by Ericsson's CPaaS API backbone; virtual receptionist, multi-level auto attendant, mobile/desktop softphones, and CRM integrations. |
| **[GoTo Connect](https://www.goto.com/connect)** | $4.3B Acquisition Valuation (~$1.0B+ ARR) | $26.00 / user / month (Phone System Basic tier, annual commitment) | 14-day free trial for software evaluation with rate-limited API access (~10 req/s) and capped test messaging credits | Unified cloud phone system and contact center suite; drag-and-drop dial plan visual editor, international calling to 50+ countries, custom IVR routing, and integrated GoTo meeting rooms. |
| **[Nextiva](https://www.nextiva.com/)** | ~$2.7B Valuation (~$400M+ ARR) | $18.95 / user / month (Essential plan, billed annually) | No direct free trial; backed by 30-day money-back guarantee with custom sales engineer pilot environments | Robust business VoIP and customer experience platform; unlimited voice/video calling within US/Canada, 1,500 toll-free minutes on base tier, conversational AI routing, and IVR. |
| **[Dialpad](https://www.dialpad.com/)** | ~$2.2B Valuation (~$300M+ ARR) | $15.00 / user / month (Standard plan, billed annually) | 14-day free trial for self-serve users; limited to single workspace testing with basic AI transcription credits and payment method required | AI-first business phone and contact center system; real-time voice transcription, live caller sentiment analysis, agent coaching suggestions, IVR routing, and omnichannel messaging. |
| **[8x8](https://www.8x8.com/)** | ~$310M Market Cap (~$740M+ ARR) | $24.00 / user / month (X2 plan, billed annually) | 30-day free trial available exclusively for 8x8 Express tier; includes unlimited US/Canada calling and basic phone features (enterprise tiers demo-only) | Global cloud phone system and unified contact center suite; integrated voice, video, team chat, omnichannel contact routing, and 30-day base reporting retention. |
| **[Ooma Office](https://www.ooma.com/small-business-phone-systems/)** | ~$530M Market Cap (~$275M+ ARR) | $19.95 / user / month (Essentials tier, contract-free) | No free trial; 30-day money-back guarantee with a fair-use cap of 5,000 pooled outbound minutes per seat and capped SMS blocks | SMB-oriented plug-and-play cloud PBX; virtual receptionist auto-attendant, extension dialing, ring groups, mobile softphone apps, and hardware IP phone compatibility. |

---

## 🟩 Open-Source Software

Self-hosted, community-driven Virtual Telephony, PBX, and Call Center platforms. Sorted in descending order by GitHub stargazer count.

### 1. [Fonoster](https://github.com/fonoster/fonoster)
[![Stars](https://img.shields.io/github/stars/fonoster/fonoster?style=social&color=white)](https://github.com/fonoster/fonoster/stargazers)  
**Stack:** Node.js / TypeScript | **License:** MIT  
An open-source programmable telecommunications stack designed as a modern alternative to Twilio. It provides a modular SDK to build custom voice applications using verbs like Answer, Play, Say, Gather, Dial, Record, and Stream. Features multi-tenant isolation, virtual PBX deployment capabilities, OAuth2/JWT authentication, RBAC, Amazon S3 media storage support, and direct Google Speech API integration.  
**Best for:** Developers looking to build custom VoIP workflows, IVR bots, and programmable telephony without commercial vendor lock-in.

### 2. [Call Center AI (Microsoft)](https://github.com/microsoft/call-center-ai)
[![Stars](https://img.shields.io/github/stars/microsoft/call-center-ai?style=social&color=white)](https://github.com/microsoft/call-center-ai/stargazers)  
**Stack:** Python / C# / Azure SDK | **License:** MIT  
Microsoft's open-source reference architecture and accelerator for building AI-driven call centers. It connects AI voice agents directly to incoming/outgoing phone calls via Azure Communication Services and OpenAI GPT models. Enables automated outbound dispatch, interactive voice bot conversations, real-time audio streaming, and seamless call transfer to human agents.  
**Best for:** Enterprise developers looking for a turnkey, AI-powered conversational voice agent connected to telecom networks.

### 3. [FreeSWITCH](https://github.com/signalwire/freeswitch)
[![Stars](https://img.shields.io/github/stars/signalwire/freeswitch?style=social&color=white)](https://github.com/signalwire/freeswitch/stargazers)  
**Stack:** C / C++ | **License:** MPL-2.0  
A carrier-grade, highly scalable software-defined telephony engine and multi-platform voice switch. FreeSWITCH forms the foundational bedrock of modern VoIP infrastructure, powering projects like FusionPBX, FS PBX, and countless commercial CPaaS providers. It natively supports SIP, WebRTC (via Verto), codec transcoding, secure RTP, and ultra-high concurrent call volumes.  
**Best for:** Platform architects and VoIP engineers seeking a rock-solid, scalable telephony routing switch to build custom PBX or call center solutions.

### 4. [Asterisk](https://github.com/asterisk/asterisk)
[![Stars](https://img.shields.io/github/stars/asterisk/asterisk?style=social&color=white)](https://github.com/asterisk/asterisk/stargazers)  
**Stack:** C | **License:** GPL-2.0  
The world's most widely deployed open-source telephony and PBX engine, created by Mark Spencer and maintained by Sangoma. Asterisk handles SIP trunking, call queues, interactive voice response (IVR), voicemail, conferencing, and WebRTC gateways via `chan_pjsip`. It powers major contact center platforms including VICIdial, FreePBX, and Wazo.  
**Best for:** Telephony engineers and system administrators constructing on-premise or cloud PBX setups with extensive hardware gateway compatibility.

### 5. [Kamailio](https://github.com/kamailio/kamailio)
[![Stars](https://img.shields.io/github/stars/kamailio/kamailio?style=social&color=white)](https://github.com/kamailio/kamailio/stargazers)  
**Stack:** C | **License:** GPL-2.0  
A battle-tested, carrier-grade SIP proxy and routing server capable of handling thousands of call setups per second. Often deployed alongside FreeSWITCH or Asterisk as an edge Session Border Controller (SBC), SIP load balancer, WebRTC gateway, and anti-fraud firewall. Features rich asynchronous routing scripts, RADIUS/Diameter accounting, and TLS/SRTP security.  
**Best for:** Large-scale telecom operators and enterprise contact centers requiring ultra-high throughput SIP trunk routing and load balancing.

### 6. [OpenSIPS](https://github.com/OpenSIPS/opensips)
[![Stars](https://img.shields.io/github/stars/OpenSIPS/opensips?style=social&color=white)](https://github.com/OpenSIPS/opensips/stargazers)  
**Stack:** C | **License:** GPL-2.0  
An open-source SIP implementation featuring ultra-fast call routing, high-throughput session management, and microservice clustering. OpenSIPS excels as a VoIP SIP proxy, registrar, redirect server, and call center dispatch front-end. It provides native clustering, dynamic routing, fraud detection engines, and call queuing distribution modules.  
**Best for:** Telephony carriers and high-volume call center networks requiring sophisticated SIP traffic distribution and carrier interconnection.

### 7. [FusionPBX](https://github.com/fusionpbx/fusionpbx)
[![Stars](https://img.shields.io/github/stars/fusionpbx/fusionpbx?style=social&color=white)](https://github.com/fusionpbx/fusionpbx/stargazers)  
**Stack:** PHP / FreeSWITCH / PostgreSQL | **License:** Open Source (MPL-1.1 / Per Project)  
A mature, full-featured multi-tenant PBX and voice switch graphical user interface built on FreeSWITCH. Delivers enterprise PBX features including domain-level tenancy, device auto-provisioning, voicemail-to-email, dynamic IVR menus, ring groups, call queues, call recording, fax server, and conference rooms. The installer sets up FreeSWITCH, NGINX, PHP-FPM, PostgreSQL, and Fail2ban out of the box.  
**Best for:** Service providers and SMBs needing a turnkey, multi-tenant cloud PBX with solid inbound call queue management.

### 8. [RustPBX](https://github.com/restsend/rustpbx)
[![Stars](https://img.shields.io/github/stars/restsend/rustpbx?style=social&color=white)](https://github.com/restsend/rustpbx/stargazers)  
**Stack:** Rust | **License:** Open Source  
A modern, memory-safe software-defined PBX engineered entirely in Rust. Call control is decoupled and accessible externally via HTTP, WebSockets, and Webhooks, enabling real-time programmability from any application stack. Features a dedicated Contact Center edition with agent skill groups, automatic call distribution (ACD), real-time wallboards, and instant Docker deployment.  
**Best for:** Teams seeking a lightweight, high-performance modern PBX with API-first call control and low resource footprint.

### 9. [InnovateAsterisk Browser Phone](https://github.com/InnovateAsterisk/Browser-Phone)
[![Stars](https://img.shields.io/github/stars/InnovateAsterisk/Browser-Phone?style=social&color=white)](https://github.com/InnovateAsterisk/Browser-Phone/stargazers)  
**Stack:** JavaScript / HTML5 / WebRTC | **License:** MIT  
A zero-install WebRTC SIP browser phone designed specifically for contact centers and remote call agents. Plugs directly into Asterisk, FreeSWITCH, or any SIP-compliant switch without browser plugins. Features call hold, transfer, 3-way conference calling, call recording, DTMF dial pad, audio visualizer, and customizable CRM screen-pop webhooks.  
**Best for:** Call center agent workstations requiring an embeddable, pure-browser WebRTC softphone interface.

### 10. [MikoPBX](https://github.com/mikopbx/Core)
[![Stars](https://img.shields.io/github/stars/mikopbx/Core?style=social&color=white)](https://github.com/mikopbx/Core/stargazers)  
**Stack:** PHP / Asterisk / Phalcon / Vue.js | **License:** GPL-3.0  
A modern, lightweight open-source IP PBX tailored for small-to-medium businesses. Powered by Asterisk 22 and Phalcon, it delivers an intuitive administrative web console, rapid ISO/Docker deployment, flexible routing rules, call recording, automated IVR, Telegram call notifications, and modular CRM integration plugins.  
**Best for:** Small businesses wanting a clean, user-friendly Asterisk-based phone system that deploys in minutes.

### 11. [AI Native Call Center](https://github.com/rasonyang/ai-native-callcenter)
[![Stars](https://img.shields.io/github/stars/rasonyang/ai-native-callcenter?style=social&color=white)](https://github.com/rasonyang/ai-native-callcenter/stargazers)  
**Stack:** Go / FreeSWITCH / PostgreSQL | **License:** Open Source  
An open-source call center where AI answers inbound calls by default using speech-to-speech LLMs (OpenAI Realtime, Grok, Qwen, Doubao). A programmable conversation flow handles customer queries and intelligently initiates human queue transfers when necessary. During transfer, the human agent's screen immediately pops with the complete AI bot transcript before pickup. Includes live wallboards and queue rosters.  
**Best for:** Teams wanting an AI-first automated call center with zero-drop handoff to human support representatives.

### 12. [FreePBX](https://github.com/FreePBX/sng_freepbx_debian_install)
[![Stars](https://img.shields.io/github/stars/FreePBX/sng_freepbx_debian_install?style=social&color=white)](https://github.com/FreePBX/sng_freepbx_debian_install/stargazers)  
**Stack:** PHP / Asterisk / MariaDB | **License:** GPL-2.0  
The most popular web GUI for configuring and maintaining Asterisk PBX systems, sponsored by Sangoma. It simplifies the setup of SIP extensions, IVR auto-attendants, ring groups, paging, voicemail, firewall rules, and inbound call queues. While primarily built for general business PBX needs rather than outbound telemarketing campaigns, commercial add-ons provide contact center reporting and queues.  
**Best for:** Organizations needing an Asterisk-based business phone system with a broad ecosystem of community modules and tutorials.

### 13. [FS PBX](https://github.com/nemerald-voip/fspbx)
[![Stars](https://img.shields.io/github/stars/nemerald-voip/fspbx?style=social&color=white)](https://github.com/nemerald-voip/fspbx/stargazers)  
**Stack:** Laravel / Vue.js / Tailwind CSS / FreeSWITCH | **License:** Apache-2.0  
A modern open-source PBX built on FreeSWITCH, forked from FusionPBX and redeveloped with modern Laravel and Vue.js frameworks. Offers multi-tenant extension management, CDR analytics, voicemail, ring groups, visual IVR configuration, firewall administration, and an optional Contact Center module featuring live supervisor wallboards and queue distribution.  
**Best for:** Teams looking for a FusionPBX alternative built on a modern, maintainable PHP/Vue codebase.

### 14. [FreeIPCC](https://github.com/lihaiya/freeipcc)
[![Stars](https://img.shields.io/github/stars/lihaiya/freeipcc?style=social&color=white)](https://github.com/lihaiya/freeipcc/stargazers)  
**Stack:** Go / FreeSWITCH / Vue.js | **License:** Open Source  
An open-source intelligent call center and customer service platform built on FreeSWITCH. Combines inbound call queue routing, outbound telemarketing dialing, work ticket management, and integration with large language models (LLMs) for smart auto-responses and voice agent bots.  
**Best for:** Customer service teams wanting an integrated open-source ticketing and call center suite with AI bot capabilities.

### 15. [VICIdial](https://github.com/inktel/Vicidial)
[![Stars](https://img.shields.io/github/stars/inktel/Vicidial?style=social&color=white)](https://github.com/inktel/Vicidial/stargazers)  
**Stack:** Perl / PHP / Asterisk / MariaDB | **License:** AGPL-2.0  
The undisputed open-source powerhouse for **high-volume outbound predictive dialing** and blended contact center operations. Active since 2003 with over 14,000 installations globally, VICIdial features predictive, progressive, and manual dial modes, skills-based inbound ACD, blended agent sessions, real-time whisper/barge monitoring, lead list management with Do-Not-Call (DNC) compliance scrubbing, and exhaustive regulatory reporting.  
**Best for:** Call centers requiring true algorithmic predictive dialing and blended inbound/outbound telemarketing at scale.

### 16. [Wazo Platform](https://github.com/wazo-platform/wazo-react-native-demo)
[![Stars](https://img.shields.io/github/stars/wazo-platform/wazo-react-native-demo?style=social&color=white)](https://github.com/wazo-platform/wazo-react-native-demo/stargazers)  
**Stack:** Python / C / Asterisk / Docker | **License:** GPL-3.0  
A microservices-based, API-first unified communications and IP PBX engine. Wazo breaks down telephony into discrete, programmable REST APIs and WebSockets, facilitating easy integration of voice calling, WebRTC softphones, mobile apps, and inbound queue agent distribution into existing enterprise software.  
**Best for:** Developers building white-label UCaaS products, telecom integrations, and mobile VoIP applications.

### 17. [Comcent CE](https://github.com/comcent-io/comcent-ce)
[![Stars](https://img.shields.io/github/stars/comcent-io/comcent-ce?style=social&color=white)](https://github.com/comcent-io/comcent-ce/stargazers)  
**Stack:** Docker Compose / FreeSWITCH / PostgreSQL | **License:** Open Source  
A modern Community Edition contact center platform packaged for rapid Docker deployment. Features an integrated agent web workspace, S3-compatible call audio storage, Twilio SIP trunk integration, and optional AI-assisted call transcription (Deepgram) and automated conversation summarization (OpenAI).  
**Best for:** Teams seeking a quick-to-deploy, containerized open-source contact center foundation with built-in AI hooks.

---

## 📊 Feature Comparison Matrix

| Software / Platform | Category | License | Outbound Predictive | Inbound ACD | WebRTC / Browser | Self-Hosted | Primary Use Case |
|---|---|---|---|---|---|---|---|
| **Zoom Phone** | Hosted SaaS | Commercial | Add-on | ✅ Advanced | ✅ Web/App | ❌ Cloud | Enterprise UCaaS & Phone |
| **Talkdesk** | Hosted SaaS | Commercial | Limited / Add-on | ✅ Advanced | ✅ Cloud | ❌ Cloud | High-Touch Omnichannel CCaaS |
| **RingCentral MVP** | Hosted SaaS | Commercial | Add-on (RingCX) | ✅ Advanced | ✅ Web/App | ❌ Cloud | Unified Business Telephony |
| **Vonage Business** | Hosted SaaS | Commercial | Add-on | ✅ Standard | ✅ Web/App | ❌ Cloud | Mid-Market Business PBX |
| **GoTo Connect** | Hosted SaaS | Commercial | Limited | ✅ Standard | ✅ Web/App | ❌ Cloud | All-in-One SMB Phone & Video |
| **Nextiva** | Hosted SaaS | Commercial | Limited | ✅ Standard | ✅ Web/App | ❌ Cloud | CX & Business VoIP |
| **Dialpad** | Hosted SaaS | Commercial | Add-on | ✅ AI Routing | ✅ Web/App | ❌ Cloud | AI-Powered Voice & Transcription |
| **8x8** | Hosted SaaS | Commercial | Add-on (X-Series) | ✅ Advanced | ✅ Web/App | ❌ Cloud | Global UC + Contact Center |
| **Ooma Office** | Hosted SaaS | Commercial | ❌ | ✅ Basic | ✅ Web/App | ❌ Cloud | Turnkey Small Business PBX |
| **Fonoster** | Open Source | MIT | ❌ | Programmable | ✅ SDK | ✅ | Programmable CPaaS (Twilio Alt) |
| **Call Center AI** | Open Source | MIT | ✅ Automated | ✅ AI Flow | ✅ | ✅ / Cloud | Conversational Voice AI Bot |
| **FreeSWITCH** | Open Source | MPL-2.0 | Framework | Framework | ✅ Verto | ✅ | Scalable Voice Engine Foundation |
| **Asterisk** | Open Source | GPL-2.0 | Framework | Framework | ✅ PJSIP | ✅ | PBX & Telephony Engine |
| **Kamailio** | Open Source | GPL-2.0 | Proxy | Proxy | ✅ Gateway | ✅ | High-Scale SIP Proxy & SBC |
| **OpenSIPS** | Open Source | GPL-2.0 | Proxy | Dispatch | ✅ Gateway | ✅ | SIP Server & Call Distribution |
| **FusionPBX** | Open Source | MPL-1.1 | ❌ | ✅ Queues | ✅ Add-on | ✅ | Multi-Tenant FreeSWITCH PBX |
| **RustPBX** | Open Source | Proprietary/OSS | CC Edition | ✅ CC Edition | ✅ WebSocket | ✅ | High-Performance Rust PBX |
| **Browser Phone** | Open Source | MIT | ❌ | Agent UI | ✅ Native | ✅ | Standalone WebRTC Agent Softphone |
| **MikoPBX** | Open Source | GPL-3.0 | ❌ | ✅ Queues | ✅ Softphone | ✅ | Simple Small Business Asterisk PBX |
| **AI Native CC** | Open Source | OSS | ❌ | ✅ AI First | ✅ Web | ✅ | AI Voice Bot + Agent Transfer |
| **FreePBX** | Open Source | GPL-2.0 | ❌ | ✅ Standard | Add-on | ✅ | Asterisk Web GUI Management |
| **FS PBX** | Open Source | Apache-2.0 | ❌ | ✅ CC Module | ✅ Softphone | ✅ | Modern Laravel/Vue FreeSWITCH PBX |
| **FreeIPCC** | Open Source | OSS | ✅ Auto-dial | ✅ Queues | ✅ | ✅ | Integrated CC + Work Order System |
| **VICIdial** | Open Source | AGPL-2.0 | ✅ Full Algorithmic | ✅ Blended | ✅ Web | ✅ | High-Volume Outbound Telemarketing |
| **Wazo Platform** | Open Source | GPL-3.0 | ❌ | ✅ Queues | ✅ WebRTC | ✅ | API-First Microservice PBX |
| **Comcent CE** | Open Source | OSS | ❌ | ✅ Queues | ✅ Web | ✅ | Containerized AI Contact Center |

---

## 🤝 Contributing

Contributions are welcome! If you know of an outstanding open-source Virtual Telephony, PBX, or Contact Center project that belongs here, please submit a pull request:

1. Fork this repository.
2. Create a feature branch: `git checkout -b feature/new-telephony-project`.
3. Add the project to the appropriate section following alphabetical or star ranking order.
4. Ensure the repository has a valid open-source license and recent commits within the past 12 months.
5. Commit and submit a PR!

---

## 📄 License

This curated list is licensed under the [Creative Commons Zero v1.0 Universal](LICENSE) (Public Domain Dedication). Software projects listed retain their respective individual licenses.

---

⭐ **Found this guide helpful? Please star this repository to support open-source telephony!** ⭐
