MERRY-GO-ROUND SCRATCH CARD — DEMO

Open index.html in a modern browser to try the visual prototype.

IMPORTANT LIMITATION
This is a local-only prototype. Each browser stores its own selections, so it does NOT coordinate picks among 12 people. Do not use it to allocate real payment turns. The random order is also generated in the browser and is not tamper-resistant.

To make it production-ready for a WhatsApp group, connect a shared backend (for example Supabase or Firebase) and implement server-side operations to:
1. Create one draw with exactly 12 unique turn numbers.
2. Register members and reserve one unused card per member atomically.
3. Keep turn assignments hidden until all 12 members have selected.
4. Reveal and publish a final immutable schedule to everyone.
5. Restrict organizer controls and prevent duplicate identities / picks.

No backend credentials are included in this prototype.
