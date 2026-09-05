# KENDALIKU

Mobile-first business control center for WhatsApp AI sales, products, payment approval, finance, and n8n automation.

## Current foundation

- Dark-first responsive dashboard with light theme toggle.
- Product catalog controls for data consumed by AI.
- Inbox and customer conversation history.
- Payment proof review and owner approval before digital delivery.
- Bot behavior and response template controls.
- n8n workflow control panel, webhook copy action, and execution log.
- Five Gemini API key slots with priority/failover UI.
- Gemini Flash / Flash-Lite routing rules.
- Vercel health and n8n webhook endpoints.

The dedicated Supabase project is `jhlgihzrtutsctzwcdqt` in `ap-southeast-1`; it is separate from Kepsek AI and Disiplin Pro.

## Integration contract

`POST /api/n8n-webhook` accepts events such as:

- `whatsapp.message.received`
- `payment.proof.received`
- `payment.verified`
- `order.approved`
- `followup.due`

For production, API keys must be stored and used server-side through encrypted storage. The browser UI only keeps a masked last-four hint in the demo layer until the dedicated KENDALIKU Supabase project and server secret are connected.
