# MCP-Server-for-One-Identity

## Kaj je MCP strežnik?
MCP strežnik (Model Context Protocol) je posrednik med AI asistentom in zunanjim sistemom. V tem primeru omogoča, da se Claude varno poveže z One Identity Manager (OIM) in kliče vnaprej določene API-je.

## Kako se MCP strežnik uporablja za povezavo Claude z OIM?
MCP strežnik sprejme zahtevo od Claude, jo pretvori v ustrezen OIM API klic, pošlje na OIM in vrne rezultat nazaj Claude. Tako Claude ne dostopa neposredno do OIM, ampak preko nadzorovanega vmesnika MCP strežnika.

## Ključne informacije, ki jih MCP strežnik potrebuje
- **Kje (WHERE):** naslov OIM API strežnika (base URL / endpointi).
- **Kdo (WHO):** namenski servisni račun v OIM, ki ga uporablja MCP strežnik za avtentikacijo in avtorizacijo.
- **Kaj (WHAT):** nabor API-jev, ki so vnaprej izbrani in dovoljeni za uporabo preko MCP strežnika.
