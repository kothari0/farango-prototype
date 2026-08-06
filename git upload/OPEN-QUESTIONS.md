# Farango — Open Questions for Client

These are gaps or ambiguities found while building the wireframes/prototypes against the discovery doc (V2.4). None of these block using the prototypes — they're flagged so the client can confirm direction before development starts.

---

## 1. Can Creators browse other Creators' content?

The discovery doc gives Players (and Guests) an **Explore Creators** page (Feature 6, Player section), but the **Creator Dashboard sidebar** (Feature 3, Creator section) has no equivalent — it lists only Dashboard, Content Management, Subscribers, Followers, Livestreams, Add-On Services, Marketplace, Earnings & Settlements, Messages, Analytics, Settings, Logout. As written, a Creator has no way to browse another creator's profile or feed from their own account.

**Options, roughly by build effort:**

| Option | Description | Matches doc as-is? |
|---|---|---|
| A — Separate account | Creator uses a separate Player login to browse as a fan | ✅ Yes (current prototype behaviour) |
| E — Own-community feed | Extend Feature 6 (Followers & Community) into a feed of the creator's own subscribers'/followers' activity, not a full directory | ⚠️ Partial — smallest true extension |
| C — Free-content Discover | Read-only browse of other creators' *free* posts only — no subscribe/tip commerce inside the Creator account | ❌ No — needs sign-off, medium build |
| B — Full Player-style Explore | Give Creators the same Explore Creators access as Players, including subscribe/tip | ❌ No — needs sign-off, larger build |
| D — Dual-role toggle | One login carries both Creator and Player identity with a switcher (like Twitch "watch as viewer") | ❌ No — schema-level change, not just UI; the Role table treats each role as separate/single-value |

**Recommendation:** confirm with client which of A/C/E/B/D they want before the Creator prototype is finalized. Current prototype ships with **A** (no browse access) since that's the literal doc scope.

---

## 2. Admin wireframes — not in the official Wireframe Page List

The doc's Wireframe Page List (used as the Phase-1 UI/UX deliverable checklist) only itemizes **Guest Home, Player, Coach (Creator), and Brand** screens. Admin is not listed there, even though Admin has 22 full feature sections written up elsewhere in the doc.

The Admin prototype (19 screens) was built anyway since "all user types" was requested, but it covers the highest-priority modules only:
- Covered: Login/Forgot Password, Dashboard, User Management, Creator & Brand Verification, Content Moderation, Golf Ball Economy, Transactions & Revenue, Payouts & Settlements, Marketplace/Disputes overview, Notification broadcast, Sub-Admin Management, Admin Settings.
- Not yet built: Subscription Management (admin view), full Livestream Management (admin), Community Management (admin), Analytics & Reporting, CMS & Platform Settings, Brand Management (separate from verification), Help & Support Management.

**Confirm with client:** is a full 22-feature Admin panel in scope for the wireframe deliverable, or is the current core set sufficient for Phase-1?

---

## 3. Enumerated screen variants condensed

The Wireframe Page List calls out some screens with a range, e.g. "Subscriber Management (2–3)", "Product Management (4–5)", "Profile Management (3–4)". The prototypes represent these with their most essential 1–2 screens (e.g. list + detail) rather than every literal variant, to keep things navigable rather than repetitive.

**Confirm with client:** which specific sub-screens they expect broken out individually (e.g. is "Product Management" expected to include separate screens for inventory alerts, bulk upload, and archived products, or is list + add/edit sufficient)?

---

*Prepared alongside the Farango clickable prototypes, Draft v1. Update this file as questions are resolved.*
