# Awesome-Small-Business-Lending

## Top Small Business Lending Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Revenue-Based Financing, Embedded Lending & Loan Management Systems*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Small Business Lending**. These tools enable lenders, fintechs, and platforms to originate, underwrite, service, and collect small business loans—ranging from revenue-based financing and merchant cash advances to term loans and credit lines.



**Examples** include Shopify Capital, Stripe Capital, Square Loans, PayPal Working Capital, Clearco, Wayflyer, Parafin, Lendio, Funding Circle, and Fundbox (the category leaders).



**Open-source emphasis**: Small Business Lending is a domain where open-source tooling is **fragmented and largely immature for the core lending workflow**. The strongest active project is **Frappe Lending**, a production-proven loan management system built on ERPNext that handles the full lifecycle from origination to closure, with adopters managing 50,000+ active loans . Other projects are either early-stage loan management APIs (LaaS, LendFlow) or CRM tools for loan agents (local-loan-crm) . No open-source platform matches the embedded, revenue-based financing automation of Shopify Capital or Stripe Capital, which rely on proprietary platform data and underwriting models.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Shopify Capital](https://www.shopify.com/capital)**  

  Embedded lending for Shopify merchants, offering merchant cash advances and loans repaid automatically through daily sales; underwriting relies on Shopify's proprietary platform data.



- **[Stripe Capital](https://stripe.com/capital)**  

  Embedded financing for Stripe businesses, with automated repayment from daily card sales; eligibility and offers are based on Stripe's transaction data.



- **[Square Loans](https://squareup.com/us/en/loans)**  

  Small business loans for Square sellers, repaid automatically as a percentage of daily card sales; underwriting uses Square's payment processing history.



- **[PayPal Working Capital](https://www.paypal.com/us/business/working-capital)**  

  Business loans for PayPal merchants, repaid automatically from sales; amounts based on PayPal transaction history.



- **[Clearco](https://clear.co/)**  

  Revenue-based financing for ecommerce and SaaS businesses, with flexible repayment tied to revenue.



- **[Wayflyer](https://wayflyer.com/)**  

  Revenue-based financing for ecommerce brands, focused on inventory and marketing spend.



- **[Parafin](https://www.parafin.com/)**  

  Embedded capital infrastructure for platforms (marketplaces, payment processors) to offer financing to their small business users.



- **[Lendio](https://www.lendio.com/)**  

  Small business loan marketplace connecting borrowers with multiple lenders; includes a loan management platform for lenders.



- **[Funding Circle](https://www.fundingcircle.com/)**  

  Online small business lending platform (peer-to-peer origins, now institutional funding).



- **[Fundbox](https://fundbox.com/)**  

  Small business credit and invoice financing, with automated underwriting based on business data.



## Open-Source GitHub Projects



- **[Frappe Lending](https://github.com/frappe/lending)**  

  The most complete open-source loan management system available (GPL-3.0), built on the Frappe Framework and ERPNext . Covers the full loan lifecycle: loan product configuration (flat/reducing balance, processing fees), application and disbursement, automated repayment schedules, interest accrual, EMI allocation, overdue penalties, DPD tracking, NPA classification, provisioning, write-offs, and co-lending splits . **Production-proven at scale**: adopters manage 50,000+ active loans with 100,000+ daily accounting entries . Includes REST APIs, role-based access, audit logs, and credit bureau file generation. Available as a self-hosted production image via Microsoft Marketplace . **The clear starting point for any organization building a self-hosted lending operation.**



- **[LaaS (Loan-as-a-Service)](https://github.com/olukinni-029/LaaS)**  

  Open-source loan management API (MIT) built with Node.js, TypeScript, Express, and MongoDB . Features JWT authentication with access/refresh tokens, role-based access control (Admin, Customer, Lender, Agent), loan application/approval/rejection/tracking, repayment tracking with balance updates, and agent commission tracking . **Early-stage API-focused**—provides the backend primitives for a lending application but lacks the accounting integration, regulatory reporting, and scale-proven workflows of Frappe Lending.



- **[LendFlow](https://github.com/Hruthik2311/LendFlow)**  

  Open-source loan management and recovery system (Node.js/Express + React 19 + PostgreSQL) . Features multi-role system (Admin, Agent, Customer), loan applications with EMI calculations, payment tracking, recovery management with agent assignment, real-time notifications, and admin reporting . **Recovery-focused**—stronger on collections workflows than Frappe Lending, but earlier-stage and lacks the full accounting/ERP foundation.



- **[local-loan-crm](https://pypi.org/project/local-loan-crm/)**  

  Open-source CLI-based CRM for local loan agents and micro-lenders (Python package) . Features customer management with tags, communication logs (phone/WeChat/meeting), follow-up scheduling with overdue/today/upcoming views, and loan application tracking through stages (intent → documentation → review → approval → signing → disbursement) . **Agent-workflow focused**—not a lending engine, but useful for the sales/follow-up layer that precedes origination.



### Additional Strong Open-Source Options



- **Loan Origination System (alimarchal)** — Laravel-based LOS with borrower management, bank work, and PDF printing; last updated April 2025 . **Early-stage** with limited documentation; suitable as a reference for LOS structure but not production-ready.

- **Sahaay LOS** — Open-source Loan Origination System starter with React, FastAPI, AI-assisted underwriting, KYC, and PostgreSQL; updated August 2026 . **Starter-focused**—useful for building a custom LOS with AI components, but early-stage.



**Frameworks for building custom systems**: **Frappe Lending** is the only open-source project with production-scale proof for loan lifecycle management, accounting integration, and regulatory reporting . For teams building a lending product, it provides the servicing and accounting backbone. **LaaS** or **LendFlow** can serve as API/recovery layers for simpler deployments, and **local-loan-crm** addresses the agent follow-up workflow. No open-source platform replicates the embedded, data-driven underwriting of Shopify Capital or Stripe Capital—those require proprietary platform data and risk models.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Small business lending platforms must comply with applicable lending regulations (usury laws, disclosure requirements, fair lending, KYC/AML) and data privacy requirements; loan servicing and collections are subject to jurisdiction-specific rules.

- **Open-source small business lending is limited**—Frappe Lending provides a production-proven loan management system , but embedded lending platforms like Shopify Capital and Stripe Capital rely on proprietary data and underwriting that open-source cannot replicate. Organizations seeking to launch a lending operation should plan for significant compliance, underwriting, and capital infrastructure beyond software.

- Verify license terms for commercial use; Frappe Lending uses GPL-3.0 , LaaS uses MIT , and LendFlow is open-source.



---



**Made for fintech builders, lending operations teams, small business lenders, and embedded finance architects.**  

Let's make small business lending more open, but with clear eyes about the compliance and underwriting complexity that software alone cannot solve.
