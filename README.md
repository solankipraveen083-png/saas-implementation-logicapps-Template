# ⚡ Enterprise Automation — Azure Logic Apps Template Library

> A practical, open-source library of Microsoft Azure Logic Apps workflow templates for SaaS implementation consultants, enterprise architects, and operations teams — covering field operations, finance, supply chain, and workforce management.

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Azure Logic Apps](https://img.shields.io/badge/Azure-Logic%20Apps-0078D4?logo=microsoft-azure)
![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)
![Templates](https://img.shields.io/badge/templates-20%2B-blue)
![Industries](https://img.shields.io/badge/industries-healthcare%20%7C%20utilities%20%7C%20services-lightgrey)

---

## 📌 What is this?

Enterprise software delivers on its promise only when the manual, repetitive workflows connecting systems, teams, and data are automated. Without automation, even the most capable SaaS platform still depends on human effort to move information, trigger actions, and keep processes running on time.

This library exists to close that gap.

It is a growing collection of **production-ready Azure Logic Apps workflow templates** built from real enterprise implementation experience — covering operational workflows across field operations, finance and billing, supply chain, and workforce management.

Each template is designed to be **deployed quickly, adapted easily, and understood clearly** — whether you are a consultant implementing a platform for a client, an IT administrator maintaining an existing integration, or an operations team looking to remove manual steps from your daily processes.

---

## 👥 Who is this for?

- **SaaS implementation consultants** who need automation templates they can adapt across client deployments
- **Enterprise architects** designing integration layers between business systems
- **Operations and IT teams** looking to automate repeatable, rule-based workflows
- **Developers** building on top of Logic Apps for the first time and looking for real-world reference implementations

---

## 📁 Repository Structure

```
enterprise-automation-logicapps-templates/
│
├── 01-operational-workflows/
│   ├── job-assigned-notification.json
│   ├── job-completed-notification.json
│   ├── job-delayed-escalation.json
│   ├── engineer-arrival-customer-alert.json
│   ├── appointment-reminder.json
│   └── README.md
│
├── 02-finance-and-billing/
│   ├── automated-billing-trigger.json
│   ├── overdue-invoice-escalation.json
│   ├── payment-received-confirmation.json
│   └── README.md
│
├── 03-supply-chain-and-operations/
│   ├── purchase-order-creation-trigger.json
│   ├── purchase-order-approval-workflow.json
│   └── README.md
│
├── 04-workforce-and-hr/
│   ├── contract-renewal-notification.json
│   ├── absence-leave-notification.json
│   └── README.md
│
├── 05-reporting-and-data-sync/
│   ├── daily-operations-summary-report.json
│   ├── weekly-performance-report-distribution.json
│   ├── cross-system-data-sync.json
│   ├── customer-record-sync.json
│   └── README.md
│
└── docs/
    ├── deployment-guide.md
    ├── prerequisites.md
    └── customisation-guide.md
```

---

## 📦 Template Categories

### 1. 🔔 Operational Workflows
Automate real-time communication and status management across customer-facing and internal operations — removing manual coordination and reducing response lag.

| Template | Trigger | Action | Use Case |
|---|---|---|---|
| `job-assigned-notification` | Job assigned in platform | Notification to assigned operative | Instant dispatch confirmation without manual contact |
| `job-completed-notification` | Job marked complete | Email to coordinator + client | Trigger downstream steps on completion |
| `job-delayed-escalation` | Job exceeds SLA threshold | Alert to operations manager | Proactive escalation before breach becomes visible to client |
| `engineer-arrival-customer-alert` | Operative checks in near location | SMS or email to customer | Reduce missed appointments and no-shows |
| `appointment-reminder` | 24 hours before scheduled visit | Automated customer reminder | Lower wasted visit rate from unattended appointments |

**Why it matters:** Missed appointments and manual status coordination are among the highest-cost inefficiencies in service operations. Industry estimates put the cost of a single wasted site visit at £150–£300 when factoring travel, labour, and rebooking. These templates eliminate the communication gaps that cause them.

---

### 2. 💰 Finance and Billing
Automate the handoffs between operational activity and financial processing — reducing invoice delays, payment lag, and manual finance administration.

| Template | Trigger | Action | Use Case |
|---|---|---|---|
| `automated-billing-trigger` | Service or job signed off | Trigger invoice creation in finance system | Remove manual invoice initiation step after service delivery |
| `overdue-invoice-escalation` | Invoice unpaid past due date | Escalation alert to finance team + automated client reminder | Reduce debtor days without manual chasing |
| `payment-received-confirmation` | Payment recorded in system | Confirmation to client + internal notification | Close the loop on payment and trigger any post-payment workflows |

**Why it matters:** Manual billing processes are a persistent source of revenue leakage in service organisations. Automating the trigger points between service delivery and financial processing accelerates cash flow and removes the administrative burden from operations teams who should not be managing billing follow-up.

---

### 3. 📦 Supply Chain and Operations
Automate procurement and approval workflows — reducing the delay and manual effort involved in purchase order management across teams and departments.

| Template | Trigger | Action | Use Case |
|---|---|---|---|
| `purchase-order-creation-trigger` | Stock threshold reached or request submitted | Auto-generate draft purchase order and notify procurement | Eliminate manual PO initiation step |
| `purchase-order-approval-workflow` | PO submitted for approval | Route to approver with deadline alert; escalate if no response | Enforce approval SLAs without manual chasing |

**Why it matters:** Purchase order delays slow operations and create knock-on effects across fulfilment, engineering, and finance. Automating the creation and approval routing steps removes the most predictable bottlenecks in the procurement cycle without requiring changes to the underlying system.

---

### 4. 👥 Workforce and HR
Automate the administrative notifications that keep workforce management running smoothly — from contract lifecycle to daily absence handling.

| Template | Trigger | Action | Use Case |
|---|---|---|---|
| `contract-renewal-notification` | Contract expiry date approaching (60, 30, 7 days) | Staged alerts to HR and line manager | Prevent contract lapses through proactive, automated reminders |
| `absence-leave-notification` | Absence submitted or approved | Notification to line manager, team, and scheduling system | Keep operational planning updated without manual communication |

**Why it matters:** Contract lapses and unmanaged absences are disproportionately disruptive in organisations with large field workforces. These templates create structured, automated notification chains that ensure the right people are informed at the right time — without relying on someone remembering to tell them.

---

### 5. 📊 Reporting and Data Sync
Automate report generation, distribution, and cross-system data synchronisation — ensuring teams have the information they need without manual extraction.

| Template | Trigger | Action | Use Case |
|---|---|---|---|
| `daily-operations-summary-report` | Scheduled (daily, 07:00) | Generate and distribute operations summary | Start-of-day visibility without manual data pull |
| `weekly-performance-report-distribution` | Scheduled (Monday, 08:00) | Generate and email performance report to management | Weekly review data delivered automatically |
| `cross-system-data-sync` | Record created or updated in source system | Sync to target system via API | Keep data consistent across platforms without duplication |
| `customer-record-sync` | Customer updated in CRM | Push update to operational platform | Ensure field teams always have current client information |

**Why it matters:** Management teams in enterprise organisations routinely spend 2–4 hours per week manually compiling operational reports. Automated report distribution eliminates this entirely while improving consistency and timeliness of the data being reviewed.

---

## 🚀 How to Use These Templates

### Prerequisites
- Active **Microsoft Azure subscription**
- Access to **Azure Logic Apps** (Consumption or Standard tier)
- Relevant **connectors configured** (Office 365, SQL, HTTP, your platform's REST API)
- Basic familiarity with the Azure Portal

Full prerequisites: [`docs/prerequisites.md`](docs/prerequisites.md)

### Deployment in 5 steps

**Step 1 — Clone the repository**
```bash
git clone https://github.com/praveensolanki/enterprise-automation-logicapps-templates.git
```

**Step 2 — Choose your template**
Navigate to the relevant category folder and open the `.json` file for the workflow you want to deploy.

**Step 3 — Customise**
Find all `[CONFIGURE]` tags in the JSON — these mark every value specific to your environment: connection strings, email addresses, API endpoints, table and field names.

Full customisation guide: [`docs/customisation-guide.md`](docs/customisation-guide.md)

**Step 4 — Deploy via Azure Portal**
1. Go to **Logic Apps** → **Add** → **Consumption**
2. Once created, open **Logic App Code View**
3. Paste your customised JSON and save
4. Enable the workflow

**Step 5 — Test before enabling for production**
Use **Run Trigger** in the Azure Portal to validate the workflow against real data before going live.

Full deployment guide: [`docs/deployment-guide.md`](docs/deployment-guide.md)

---

## 🌍 Sectors These Templates Have Been Applied In

| Sector | Application |
|---|---|
| Healthcare | Community care scheduling, patient visit coordination, equipment maintenance |
| Utilities | Engineer dispatch, infrastructure maintenance, compliance workflows |
| Facilities Management | Reactive and planned maintenance, contract SLA tracking |
| Professional Services | Client onboarding, billing automation, contract lifecycle |
| National Services | Multi-site workforce coordination, operational reporting |

---

## 🛠 Design Principles

Every template in this library is built around three principles:

**Platform-agnostic where possible** — HTTP connector templates work with any system that exposes a REST API. SQL templates clearly mark table and field names for replacement.

**Documented for the person deploying it, not the person who built it** — each template folder includes a plain-language explanation of what the workflow does, why it exists, and what to configure.

**Built for real operational environments** — these are not toy examples. They reflect the edge cases, error handling, and practical constraints of enterprise deployments.

---

## 🤝 Contributing

This library grows through contributions from the implementation and automation community. If you have built a Logic Apps workflow that solves a real enterprise problem and is not covered here, a pull request is welcome.

**To contribute:**
- Include the JSON export from Azure Logic Apps
- Add a `README.md` in your template folder with use case, trigger, action, and configuration notes
- Mark all environment-specific values with `[CONFIGURE]`
- Test before submitting

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for full guidelines.

---

## 📄 License

MIT License — free to use, adapt, and deploy in your own client or internal implementations. See [`LICENSE`](LICENSE).

---

## 👤 About

This library is maintained by **Praveen Solanki**, a SaaS Implementation and Automation Consultant with experience designing and delivering enterprise workflow automation across healthcare, utilities, and national services organisations. His work sits at the intersection of cloud automation, operational efficiency, and enterprise digital transformation — helping organisations extract the full value from the software platforms they have already invested in.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Praveen%20Solanki-0077B5?logo=linkedin)](https://linkedin.com/in/praveensolanki)

---

*If this library saved you time on a deployment, consider giving it a ⭐ — it helps others in the enterprise software community find it.*
