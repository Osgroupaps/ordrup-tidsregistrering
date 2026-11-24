# Ordrup Consulting – Tidsregistrering

Selvstændig tidsregistrering for Ordrup Consulting på https://tid.ordrup.nu (GitHub Pages).
Samme funktioner som OS Groups tidsregistrering, men eget logo, egen database og egen Dinero-konto.

- Database og login: Supabase, organisationen "Ordrup Consulting", projektet "tidsregistrering" (asfpccdmvswuvfxnveqv, EU).
- Dinero (organisation 392234, Ordrup Consulting ApS): edge function `dinero` bruger secrets DINERO_CLIENT_ID, DINERO_CLIENT_SECRET, DINERO_API_KEY og DINERO_ORG_ID (Ordrups egen Dinero-organisation). Nøglerne ligger kun i Supabase.
- Invitation af medarbejdere: edge function `invite`.
- `config.js` indeholder kun den offentlige publishable key.
