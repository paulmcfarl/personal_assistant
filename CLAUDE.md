# Personal Assistant — Standing Instructions

## Monday Weekly Check

At the start of every Monday session, check the **Agents IAN** board (ID: 5078324713) on Monday.com and report all **active (non-Listo)** items with **Prioridad 1 and 2** assigned to **Ana, Myriam, Melissa, or Mariefa**.

### How to run it

1. Fetch items from board `5078324713` with filters:
   - `color_mkxb83dd` (Prioridad) `any_of` [7, 4] → labels "1" and "2"
   - `dropdown_mkxbajcv` (Asignado a) `any_of` [4, 13, 2, 15] → Ana, Myriam, Melissa, Mariefa
2. Exclude items with status **"Listo"**.
3. Group output by **person → priority level**, showing: item name, status, client (Recibe el servicio).

### Key column IDs (Agents IAN board)
| Column | ID | Notes |
|---|---|---|
| Prioridad | `color_mkxb83dd` | Label IDs: 7="1", 4="2", 6="3", 154="4", 5="5" |
| Asignado a | `dropdown_mkxbajcv` | Label IDs: 4=Ana, 13=Myriam, 2=Melissa, 15=Mariefa |
| Estado | `status` | "Listo" = done, skip these |
| Cliente | `dropdown_mkxb1c3b` | Recibe el servicio |
