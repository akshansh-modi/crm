# Changes we made to upstream code

When you merge a newer upstream release, check whether each of these still applies or upstream fixed it.
Each changed spot is marked `crm-desk patch`.

| File | What | Why |
|---|---|---|
| `frontend/src/components/Customer360.vue` (new file) | Same file as the support-helpdesk copy (`desk/src/components/Customer360.vue`): change both together | Insurance 360 view in CRM. |
| `frontend/src/pages/Contact.vue` | Import + render `<Customer360>` under the contact header | 360 view on a CRM contact. |
| `frontend/src/pages/Deal.vue` | Import + render `<Customer360>` under the SLA block, for the deal's primary contact | 360 view on a CRM deal. |
