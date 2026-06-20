# Claude Cowork Business Canvas

เว็บแอปหน้าเดียวสำหรับออกแบบ workflow ของ Claude Cowork/Claude ด้วย node แบบลากวาง โดยชุด business pack อ้างอิงจาก interface จริงของ Claude:

- `+` หรือ `/` ใน chat -> `Connectors` สำหรับเปิดใช้ connector ต่อ conversation
- `+` หรือ `/` ใน chat -> `Connectors` -> `Tool access` สำหรับเลือก Auto หรือ On demand
- `Customize > Connectors` สำหรับ browse, connect, disconnect, modify settings และ review permissions
- `Connectors Directory` สำหรับดูหมวดหมู่, complete list, use cases, read/write capabilities และ availability
- `Organization settings > Connectors` สำหรับ Team/Enterprise owner เพิ่ม connector ให้ทีม
- `Tool permissions` แยกเป็น Always allow, Needs approval หรือ Blocked ตามระดับความเสี่ยง
- Custom connector ใช้ remote MCP server ที่ Claude เข้าถึงผ่าน public URL
- Desktop extension เหมาะกับ local files, localhost, desktop apps และ OS-level access
- Plugin สามารถ bundle remote MCP หรือ local MCP เพื่อใช้เป็น business capability เฉพาะงาน
- Interactive connectors สามารถแสดง inline card หรือ fullscreen UI ในบทสนทนา

## Business Nodes Added

- Interface controls: Connectors Directory, Manage Connectors, Per-chat Connector Toggle, Tool Access Auto, Tool Access On demand, Search and Tools Menu, Tool Approval Request, Interactive Inline Card, Interactive Fullscreen
- Connectors / business candidates: Google Drive, Google Sheets, Gmail, Google Calendar, Microsoft 365, Slack, Linear, Asana, Jira, Notion, Confluence, GitHub, Salesforce, HubSpot, QuickBooks, PayPal, DocuSign, Canva, Figma, Zendesk, Intercom, ServiceNow, Zapier, Stripe, Custom Business SaaS Connector
- MCP Servers: Remote MCP Web, Desktop Extension, Internal Knowledge MCP, Data Warehouse MCP, CRM MCP, ERP MCP, HRIS MCP, Support MCP, BI Dashboard MCP, Browser Automation MCP, Audit Log MCP
- Permissions & governance: Organization Settings > Connectors, Enterprise-managed Auth, Verified-domain Restriction, Private Project Boundary, Always allow, Needs approval, Blocked, Read-only Scope, Write/Delete Scope, OAuth Consent Review, Prompt Injection Review
- Plugins: Finance, Sales Ops, HR, Legal, Design, Engineering, Operations
- Skills: Finance Analyst, Sales Brief, HR Policy, Legal Review, Marketing Campaign, Support QA, Meeting Brief, Executive Summary, Procurement, Risk & Compliance, plus DOCX/PPTX/XLSX/CSV/PDF/Learn skills

## Business Use Templates

Click `Claude Pack` to load a workflow that mirrors how a business user would operate Claude:

1. Start in Claude Chat with `+` / `Connectors`.
2. Browse or manage connectors from the directory/settings surface.
3. Enable only the connectors needed for the conversation.
4. Use On demand tool access when many connectors are active.
5. Route sensitive write actions through `Needs approval` and record them in `Audit Log MCP`.
6. Combine business context from Drive, Gmail, Slack, CRM, and Data Warehouse nodes.
7. Generate executive summary, finance analysis, sales brief, risk review, saved files, and notifications.

## Source Notes

This workshop intentionally includes two kinds of nodes:

- Real Claude interface concepts from Claude Help Center / MCP docs: connectors, custom remote MCP, desktop extensions, per-chat toggles, Tool access modes, Tool permissions, Team/Enterprise org settings, interactive connectors, OAuth and approval review.
- Business-use connector candidates that should be checked against the live `Connectors Directory` in the user's Claude account because availability can vary by plan, region, organization policy, and directory updates.

Open `index.html` in a browser, join in demo mode, then click `Claude Pack` to load a ready-made business workflow blueprint.
