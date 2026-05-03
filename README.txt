# ForgeIntellAI Hub — How to Add New Clients

## Adding a new client room (drag and drop — no deleting needed)

When you get a new client, come back to this chat and say:
"Add a new client room — [Business Name], [industry], systems: [which ones]"

I will give you a new folder to drag into GitHub. You just:
1. Drag the new client folder into your GitHub repo under /rooms/
2. Update index.html with their room key
3. Done — their room is live

## File structure

forgeintellai-hub/
├── index.html          ← Key login page (update ROOMS object for new clients)
├── logo.png            ← ForgeIntellAI logo
├── admin/
│   └── index.html      ← Your personal admin panel
└── rooms/
    └── apex-roofing/   ← Each client gets their own folder here
        ├── dashboard.html   ← Client's private interface
        └── estimate.html    ← Public customer-facing estimate page

## Adding a new client key

In index.html, find the ROOMS object:

const ROOMS = {
  '$t0cks&G0lf':    'admin',
  'APEX-2025-K7X9': 'apex-roofing',
  'NEW-KEY-HERE':   'new-client-folder-name',   ← add new clients here
};

## Changing a room key

1. Go to your admin panel
2. Click "Change Key" on the client card
3. Fill out the form — it emails you the request
4. Update the ROOMS object in index.html with the new key
5. The old key instantly stops working

## Public estimate page URL format

Each client's estimate page is public — no key needed:
/rooms/apex-roofing/estimate.html

## Dashboard URL (private — requires room key)

/rooms/apex-roofing/dashboard.html
