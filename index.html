import { useState, useEffect } from "react";

const C = {
  cream: "#FDFAF4", gold: "#B8960C", goldLight: "#F5E6C8", goldDim: "#8B6E0A",
  charcoal: "#1A1A1A", text: "#1A1A1A", textMid: "#4A4A4A", textLight: "#7A7A7A",
  error: "#8B1A1A", errorLight: "#FFF5F5",
  success: "#1A3A2A", successLight: "#E8F5EE",
  border: "#E8E0CC", white: "#FFFFFF",
};

const HOTEL = {
  name: "E-Phoenix Hotel & Tourism", branch: "Annex II",
  address: "No. 13 Reservation Road, Off Flower Garden, GRA, Ilorin",
  phone: "09039053579", email: "ephoenixhotel@gmail.com",
  checkin: "12:00 noon", checkout: "12:00 noon",
  wifi: "EPhoenix@2024", wifiName: "E-Phoenix_Guest",
  breakfast: "6:30am – 9:00am", pool: "7:00am – 9:00pm", gym: "6:00am – 10:00pm",
  googleMaps: "https://maps.google.com/?q=E-Phoenix+Hotel+Annex+II+Ilorin",
};

const HOTEL_INFO_CARDS = [
  { icon: "🌅", title: "BREAKFAST", desc: "Complimentary daily 6:30AM–9AM" },
  { icon: "🏊", title: "POOL & GYM", desc: "Free access for all in-house guests" },
  { icon: "🔒", title: "SECURITY", desc: "24hrs CCTV & security personnel" },
  { icon: "🅿️", title: "PARKING", desc: "Free on-site parking available" },
  { icon: "📶", title: "FREE WIFI", desc: `Network: ${HOTEL.wifiName}` },
  { icon: "🍳", title: "ROOM SERVICE", desc: "Available 24 hours daily" },
];

const SERVICES = [
  { icon: "🍽", title: "Restaurant", desc: "24hrs Kitchen & Dining", badge: "24hrs" },
  { icon: "🍺", title: "Bar & Lounge", desc: "Drinks & cocktails, 24hrs", badge: "24hrs" },
  { icon: "🛏", title: "Room Service", desc: "Food & requests to your room", badge: "24hrs" },
  { icon: "👕", title: "Laundry", desc: "24hrs wash, dry & iron", badge: "24hrs" },
  { icon: "💆", title: "Spa & Wellness", desc: "Massage, salon & treatments", badge: "Popular" },
  { icon: "🚗", title: "Transport", desc: "Airport shuttle & car hire", badge: "" },
];

const ADMIN_USERS = [
  { username: "admin", password: "ephoenix2024", role: "Owner", name: "Hotel Owner" },
  { username: "manager", password: "manager123", role: "Manager", name: "Fatima Abdullahi" },
  { username: "frontdesk", password: "desk123", role: "Front Desk", name: "Daniel Okafor" },
];

const MENU = {
  Food: [
    { id: 1, name: "Jollof Rice & Chicken", desc: "Party jollof with grilled chicken", price: 3500, emoji: "🍛" },
    { id: 2, name: "Pepper Soup (Catfish)", desc: "Spiced catfish pepper soup", price: 3200, emoji: "🐟" },
    { id: 3, name: "Fried Rice & Plantain", desc: "Nigerian fried rice with plantain", price: 3000, emoji: "🍚" },
    { id: 4, name: "Omelette & Toast", desc: "3-egg omelette with buttered toast", price: 2000, emoji: "🍳" },
    { id: 5, name: "Pounded Yam & Egusi", desc: "Smooth pounded yam, rich egusi soup", price: 3800, emoji: "🥣" },
    { id: 6, name: "Suya Platter", desc: "Spiced grilled beef suya", price: 2500, emoji: "🍢" },
  ],
  Drinks: [
    { id: 7, name: "Chapman", desc: "Chilled Nigerian Chapman cocktail", price: 1500, emoji: "🍹" },
    { id: 8, name: "Cold Heineken", desc: "Ice cold Heineken 600ml", price: 1200, emoji: "🍺" },
    { id: 9, name: "Maltina", desc: "Premium malt drink, chilled", price: 600, emoji: "🥤" },
    { id: 10, name: "Zobo Juice", desc: "Fresh hibiscus juice", price: 800, emoji: "🌺" },
    { id: 11, name: "Still Water 1.5L", desc: "Chilled bottled water", price: 400, emoji: "💧" },
  ],
  Extras: [
    { id: 12, name: "Extra Towels", desc: "Set of 2 fresh bath towels", price: 500, emoji: "🛁" },
    { id: 13, name: "Laundry Per Item", desc: "Same-day laundry and pressing", price: 800, emoji: "👕" },
    { id: 14, name: "Airport Pickup", desc: "Ilorin International Airport", price: 5000, emoji: "🚗" },
    { id: 15, name: "Complimentary Breakfast", desc: "Continental breakfast add-on", price: 0, emoji: "☕" },
  ],
};

const REQUEST_TYPES = [
  { icon: "🧹", label: "Housekeeping", sub: "Clean my room" },
  { icon: "🔧", label: "Maintenance", sub: "Fix something" },
  { icon: "🛁", label: "Extra Towels", sub: "Need more towels" },
  { icon: "❄️", label: "AC Issue", sub: "Too hot or cold" },
  { icon: "📺", label: "TV Problem", sub: "Remote or channels" },
  { icon: "💡", label: "Lighting", sub: "Bulb or switch" },
  { icon: "🔌", label: "Power Issue", sub: "Outlet not working" },
  { icon: "🚿", label: "Water Issue", sub: "Hot water / pressure" },
];

const INITIAL_ROOMS = Array.from({ length: 10 }, (_, i) => ({
  id: i + 1, number: String(i + 1).padStart(2, "0"),
  guest: "", email: "", phone: "", numGuests: 1,
  checkin: "", checkout: "", status: "vacant",
}));

const fmt = (n) => `₦${n.toLocaleString()}`;
const nowTime = () => new Date().toLocaleTimeString("en-NG", { hour: "2-digit", minute: "2-digit" });
const nowFull = () => new Date().toLocaleString("en-NG", { day: "numeric", month: "short", hour: "2-digit", minute: "2-digit" });

// ─── SHARED UI ────────────────────────────────────────────────────────────────
function BackBar({ title, subtitle, onBack, light, right }) {
  return (
    <div style={{ background: light ? C.white : C.charcoal, borderBottom: light ? `1px solid ${C.border}` : "none", padding: "16px 20px 18px", display: "flex", alignItems: "center", gap: 14 }}>
      <button onClick={onBack} style={{ background: light ? C.goldLight : `${C.gold}20`, border: `1px solid ${C.gold}40`, color: C.gold, borderRadius: 8, width: 34, height: 34, fontSize: 16, cursor: "pointer", display: "flex", alignItems: "center", justifyContent: "center", flexShrink: 0 }}>←</button>
      <div style={{ flex: 1 }}>
        <div style={{ fontSize: 17, fontFamily: "'Playfair Display', serif", fontWeight: 700, color: light ? C.charcoal : C.white }}>{title}</div>
        {subtitle && <div style={{ fontSize: 11, color: light ? C.textLight : "#888", marginTop: 2 }}>{subtitle}</div>}
      </div>
      {right}
    </div>
  );
}

function DeleteBtn({ onDelete, label = "Delete" }) {
  const [confirm, setConfirm] = useState(false);
  if (confirm) return (
    <div style={{ display: "flex", gap: 6 }}>
      <button onClick={onDelete} style={{ background: C.error, color: C.white, border: "none", borderRadius: 8, padding: "6px 12px", fontSize: 11, fontWeight: 700, cursor: "pointer" }}>Confirm</button>
      <button onClick={() => setConfirm(false)} style={{ background: C.white, color: C.textLight, border: `1px solid ${C.border}`, borderRadius: 8, padding: "6px 12px", fontSize: 11, cursor: "pointer" }}>Cancel</button>
    </div>
  );
  return <button onClick={() => setConfirm(true)} style={{ background: C.errorLight, color: C.error, border: `1px solid ${C.error}30`, borderRadius: 8, padding: "6px 12px", fontSize: 11, fontWeight: 600, cursor: "pointer" }}>🗑 {label}</button>;
}

// ─── ENTRY ────────────────────────────────────────────────────────────────────
function EntryScreen({ onGuest, onAdmin }) {
  return (
    <div style={{ minHeight: "100vh", background: C.cream, display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", padding: 28, fontFamily: "'DM Sans', sans-serif" }}>
      <div style={{ textAlign: "center", marginBottom: 48 }}>
        <div style={{ fontSize: 48, marginBottom: 12 }}>🦅</div>
        <div style={{ fontSize: 11, letterSpacing: 6, color: C.gold, textTransform: "uppercase", marginBottom: 10 }}>E-Phoenix Hotel</div>
        <div style={{ fontSize: 28, fontFamily: "'Playfair Display', serif", color: C.charcoal, fontWeight: 700 }}>Annex II — Ilorin</div>
        <div style={{ fontSize: 13, color: C.textLight, marginTop: 6 }}>Guest Portal</div>
      </div>
      <div style={{ width: "100%", display: "flex", flexDirection: "column", gap: 14 }}>
        <button onClick={onGuest} style={{ background: C.gold, color: C.white, border: "none", borderRadius: 14, padding: "20px 24px", fontSize: 16, fontWeight: 700, cursor: "pointer", display: "flex", justifyContent: "space-between", alignItems: "center" }}>
          <div style={{ textAlign: "left" }}>
            <div>🛎 Guest Portal</div>
            <div style={{ fontSize: 12, fontWeight: 400, opacity: 0.85, marginTop: 3 }}>Access hotel services during your stay</div>
          </div>
          <span style={{ fontSize: 20 }}>→</span>
        </button>
        <button onClick={onAdmin} style={{ background: C.white, color: C.charcoal, border: `1px solid ${C.border}`, borderRadius: 14, padding: "20px 24px", fontSize: 16, fontWeight: 700, cursor: "pointer", display: "flex", justifyContent: "space-between", alignItems: "center" }}>
          <div style={{ textAlign: "left" }}>
            <div>🔐 Staff Login</div>
            <div style={{ fontSize: 12, fontWeight: 400, color: C.textLight, marginTop: 3 }}>Manager, front desk & admin access</div>
          </div>
          <span style={{ fontSize: 20, color: C.textLight }}>→</span>
        </button>
      </div>
      <div style={{ marginTop: 40, fontSize: 10, color: C.textLight, letterSpacing: 2, textTransform: "uppercase" }}>Powered by Guestify</div>
    </div>
  );
}

// ─── GUEST LOGIN ──────────────────────────────────────────────────────────────
function GuestLogin({ onLogin, onBack }) {
  const [form, setForm] = useState({ name: "", room: "", email: "", numGuests: "1" });
  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);

  const set = (k, v) => setForm((f) => ({ ...f, [k]: v }));

  const handle = () => {
    if (!form.name.trim()) { setError("Please enter your full name"); return; }
    if (!form.room.trim()) { setError("Please enter your room number"); return; }
    setError(""); setLoading(true);
    setTimeout(() => { setLoading(false); onLogin({ name: form.name.trim(), room: form.room.trim(), email: form.email.trim(), numGuests: parseInt(form.numGuests) || 1 }); }, 1200);
  };

  return (
    <div style={{ minHeight: "100vh", background: C.cream, fontFamily: "'DM Sans', sans-serif" }}>
      <div style={{ padding: "20px" }}>
        <button onClick={onBack} style={{ background: "none", border: "none", color: C.textLight, fontSize: 14, cursor: "pointer" }}>← Back</button>
      </div>
      <div style={{ padding: "10px 28px 60px", display: "flex", flexDirection: "column", alignItems: "center" }}>
        <div style={{ fontSize: 40, marginBottom: 12 }}>🦅</div>
        <div style={{ fontSize: 11, letterSpacing: 5, color: C.gold, textTransform: "uppercase", marginBottom: 8 }}>E-Phoenix Hotel</div>
        <div style={{ fontSize: 26, fontFamily: "'Playfair Display', serif", color: C.charcoal, fontWeight: 700, textAlign: "center" }}>Annex II — Ilorin, Kwara State</div>
        <div style={{ fontSize: 13, color: C.textLight, marginTop: 4 }}>Guest Portal</div>

        <div style={{ width: "100%", marginTop: 32 }}>
          <div style={{ fontSize: 11, letterSpacing: 3, color: C.gold, textTransform: "uppercase", marginBottom: 20 }}>Welcome — Please Sign In</div>

          {[
            { label: "FULL NAME", key: "name", ph: "e.g. Amina Bello", type: "text" },
            { label: "ROOM NUMBER", key: "room", ph: "e.g. 204", type: "tel" },
            { label: "EMAIL ADDRESS", key: "email", ph: "your@email.com", type: "email" },
          ].map(({ label, key, ph, type }) => (
            <div key={key} style={{ marginBottom: 16 }}>
              <div style={{ fontSize: 11, letterSpacing: 2, color: C.textLight, marginBottom: 8, fontWeight: 600 }}>{label}</div>
              <input value={form[key]} onChange={(e) => set(key, e.target.value)} placeholder={ph} type={type}
                onKeyDown={(e) => e.key === "Enter" && handle()}
                style={{ width: "100%", padding: "14px 16px", borderRadius: 10, border: `1px solid ${C.border}`, background: C.white, color: C.charcoal, fontSize: 15, fontFamily: "'DM Sans', sans-serif", outline: "none", boxSizing: "border-box" }} />
            </div>
          ))}

          <div style={{ marginBottom: 24 }}>
            <div style={{ fontSize: 11, letterSpacing: 2, color: C.textLight, marginBottom: 8, fontWeight: 600 }}>NUMBER OF GUESTS</div>
            <select value={form.numGuests} onChange={(e) => set("numGuests", e.target.value)}
              style={{ width: "100%", padding: "14px 16px", borderRadius: 10, border: `1px solid ${C.border}`, background: C.white, color: C.charcoal, fontSize: 15, fontFamily: "'DM Sans', sans-serif", outline: "none", boxSizing: "border-box", appearance: "none", cursor: "pointer" }}>
              {[1, 2, 3, 4, 5].map((n) => <option key={n} value={n}>{n} Guest{n > 1 ? "s" : ""}</option>)}
            </select>
          </div>

          {error && <div style={{ color: C.error, fontSize: 13, marginBottom: 14, background: C.errorLight, padding: "10px 14px", borderRadius: 8 }}>{error}</div>}

          <button onClick={handle} style={{ width: "100%", background: loading ? C.goldDim : C.gold, color: C.white, border: "none", borderRadius: 10, padding: "16px", fontSize: 14, fontWeight: 700, cursor: "pointer", letterSpacing: 1 }}>
            {loading ? "Checking in..." : "ACCESS HOTEL SERVICES →"}
          </button>

          <div style={{ marginTop: 20, background: C.white, border: `1px solid ${C.border}`, borderRadius: 10, padding: "14px 16px", textAlign: "center", fontSize: 13 }}>
            <span style={{ color: C.textLight }}>WiFi: </span>
            <span style={{ color: C.gold, fontWeight: 700 }}>{HOTEL.wifiName}</span>
            {"  ·  "}
            <span style={{ color: C.textLight }}>Password: </span>
            <span style={{ color: C.gold, fontWeight: 700 }}>{HOTEL.wifi}</span>
          </div>
        </div>
      </div>
    </div>
  );
}

// ─── GUEST WELCOME ────────────────────────────────────────────────────────────
function GuestWelcome({ guest, onNav, pulseShown, announcements, onLogout }) {
  const first = guest.name.split(" ")[0];
  const h = new Date().getHours();
  const greet = h < 12 ? "Good morning" : h < 17 ? "Good afternoon" : "Good evening";
  const active = announcements.filter((a) => {
    if (!a.expires) return true;
    return new Date() < new Date(a.expires);
  });

  return (
    <div style={{ minHeight: "100vh", background: C.cream, fontFamily: "'DM Sans', sans-serif", paddingBottom: 80 }}>
      {/* Header */}
      <div style={{ background: C.cream, padding: "14px 20px 0", display: "flex", justifyContent: "space-between", alignItems: "center" }}>
        <div>
          <div style={{ fontSize: 13, fontWeight: 800, color: C.gold, letterSpacing: 2, textTransform: "uppercase" }}>E-Phoenix Hotel</div>
          <div style={{ fontSize: 11, color: C.textLight }}>Annex II, Ilorin</div>
        </div>
        <button onClick={onLogout} style={{ background: "none", border: `1px solid ${C.border}`, borderRadius: 8, padding: "6px 12px", fontSize: 11, color: C.textLight, cursor: "pointer" }}>Sign Out</button>
      </div>

      {/* Hero banner */}
      <div style={{ background: `linear-gradient(135deg, ${C.gold} 0%, ${C.goldDim} 100%)`, margin: "14px 16px", borderRadius: 16, padding: "24px 20px" }}>
        <div style={{ fontSize: 11, color: "rgba(255,255,255,0.7)", marginBottom: 4 }}>Room {guest.room}{guest.numGuests > 1 ? ` · ${guest.numGuests} Guests` : ""}</div>
        <div style={{ fontSize: 28, fontFamily: "'Playfair Display', serif", color: C.white, fontWeight: 700 }}>{greet}, {first}.</div>
        <div style={{ fontSize: 14, color: "rgba(255,255,255,0.85)", marginTop: 4 }}>Everything you need, right here.</div>
      </div>

      <div style={{ padding: "0 16px" }}>
        {/* Info cards strip */}
        <div style={{ display: "flex", gap: 10, overflowX: "auto", paddingBottom: 4, marginBottom: 20, scrollbarWidth: "none" }}>
          {HOTEL_INFO_CARDS.map((card) => (
            <div key={card.title} style={{ background: C.white, border: `1px solid ${C.border}`, borderRadius: 12, padding: "14px", minWidth: 140, flexShrink: 0 }}>
              <div style={{ fontSize: 20, marginBottom: 6 }}>{card.icon}</div>
              <div style={{ fontSize: 10, fontWeight: 700, color: C.gold, letterSpacing: 1, textTransform: "uppercase", marginBottom: 4 }}>{card.title}</div>
              <div style={{ fontSize: 11, color: C.textLight, lineHeight: 1.4 }}>{card.desc}</div>
            </div>
          ))}
        </div>

        {/* Emergency strip */}
        <div style={{ background: "#FFF5F5", border: `1px solid ${C.error}30`, borderRadius: 12, padding: "12px 16px", marginBottom: 20, display: "flex", alignItems: "center", gap: 10 }}>
          <span style={{ fontSize: 20 }}>🚨</span>
          <div style={{ fontSize: 12, color: C.error, lineHeight: 1.5 }}>
            Emergency? Dial <strong>500</strong> (Reception) or <strong>0</strong> from your room phone. Security available 24hrs.
          </div>
        </div>

        {/* Admin announcements */}
        {active.length > 0 && (
          <div style={{ marginBottom: 20 }}>
            {active.map((a) => (
              <div key={a.id} style={{ background: a.type === "urgent" ? C.errorLight : C.goldLight, border: `1px solid ${a.type === "urgent" ? C.error + "40" : C.gold + "40"}`, borderRadius: 12, padding: "14px 16px", marginBottom: 10 }}>
                <div style={{ display: "flex", alignItems: "center", gap: 8, marginBottom: 4 }}>
                  <span style={{ fontSize: 16 }}>{a.type === "urgent" ? "🚨" : a.type === "promo" ? "🎉" : "📢"}</span>
                  <span style={{ fontSize: 11, fontWeight: 700, color: a.type === "urgent" ? C.error : C.goldDim, textTransform: "uppercase", letterSpacing: 1 }}>{a.type === "urgent" ? "Urgent Notice" : a.type === "promo" ? "Special Offer" : "Hotel Notice"}</span>
                  {a.expires && <span style={{ fontSize: 10, color: C.textLight, marginLeft: "auto" }}>Expires: {new Date(a.expires).toLocaleTimeString("en-NG", { hour: "2-digit", minute: "2-digit" })}</span>}
                </div>
                <div style={{ fontSize: 14, fontWeight: 700, color: C.charcoal, marginBottom: 2 }}>{a.title}</div>
                <div style={{ fontSize: 13, color: C.textMid, lineHeight: 1.5 }}>{a.body}</div>
              </div>
            ))}
          </div>
        )}

        {/* Satisfaction pulse banner */}
        {!pulseShown && (
          <button onClick={() => onNav("pulse")} style={{ width: "100%", background: C.charcoal, border: "none", borderRadius: 14, padding: "16px 18px", display: "flex", alignItems: "center", gap: 14, cursor: "pointer", marginBottom: 20 }}>
            <span style={{ fontSize: 26 }}>😊</span>
            <div style={{ textAlign: "left" }}>
              <div style={{ fontSize: 14, fontWeight: 700, color: C.white }}>How is your stay so far?</div>
              <div style={{ fontSize: 11, color: "#888", marginTop: 2 }}>Tap to rate your experience</div>
            </div>
            <span style={{ marginLeft: "auto", color: C.gold, fontSize: 18 }}>→</span>
          </button>
        )}

        {/* Services grid */}
        <div style={{ fontSize: 11, letterSpacing: 2, color: C.textLight, textTransform: "uppercase", marginBottom: 14 }}>Our Services</div>
        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: 12, marginBottom: 20 }}>
          {SERVICES.map((s) => (
            <button key={s.title} onClick={() => s.title === "Restaurant" || s.title === "Room Service" ? onNav("menu") : s.title === "Laundry" ? onNav("requests") : null}
              style={{ background: C.white, border: `1px solid ${C.border}`, borderRadius: 14, padding: "18px 14px", textAlign: "left", cursor: "pointer", position: "relative" }}>
              {s.badge && <span style={{ position: "absolute", top: 10, right: 10, background: s.badge === "Popular" ? C.gold : C.charcoal, color: C.white, borderRadius: 6, padding: "2px 7px", fontSize: 9, fontWeight: 700 }}>{s.badge}</span>}
              <div style={{ fontSize: 28, marginBottom: 10 }}>{s.icon}</div>
              <div style={{ fontSize: 14, fontWeight: 700, color: C.charcoal }}>{s.title}</div>
              <div style={{ fontSize: 11, color: C.textLight, marginTop: 3 }}>{s.desc}</div>
            </button>
          ))}
        </div>
      </div>
    </div>
  );
}

// ─── GUEST MENU ───────────────────────────────────────────────────────────────
function GuestMenu({ guest, onNav, onOrder }) {
  const [tab, setTab] = useState("Food");
  const [cart, setCart] = useState({});
  const [note, setNote] = useState("");
  const [step, setStep] = useState("browse");
  const allItems = Object.values(MENU).flat();
  const cartTotal = Object.entries(cart).reduce((s, [id, q]) => { const i = allItems.find((x) => x.id === +id); return s + (i ? i.price * q : 0); }, 0);
  const cartCount = Object.values(cart).reduce((a, b) => a + b, 0);
  const add = (id) => setCart((c) => ({ ...c, [id]: (c[id] || 0) + 1 }));
  const rem = (id) => setCart((c) => { const n = { ...c }; n[id] > 1 ? n[id]-- : delete n[id]; return n; });

  const placeOrder = () => {
    const items = Object.entries(cart).map(([id, qty]) => { const item = allItems.find((i) => i.id === +id); return `${item.emoji} ${item.name} ×${qty}`; }).join(", ");
    onOrder({ id: Date.now(), room: guest.room, guest: guest.name, items, note, total: cartTotal, time: nowTime(), status: "pending" });
    setStep("done");
  };

  if (step === "done") return (
    <div style={{ minHeight: "100vh", background: C.cream, display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", padding: 28, fontFamily: "'DM Sans', sans-serif" }}>
      <div style={{ fontSize: 64, marginBottom: 16 }}>✅</div>
      <div style={{ fontSize: 24, fontFamily: "'Playfair Display', serif", fontWeight: 700, color: C.charcoal }}>Order Placed!</div>
      <div style={{ fontSize: 14, color: C.textMid, marginTop: 10, textAlign: "center", lineHeight: 1.6 }}>Delivery to Room {guest.room} in 20–30 minutes.</div>
      <div style={{ marginTop: 20, background: C.goldLight, border: `1px solid ${C.gold}40`, borderRadius: 14, padding: "14px 24px", textAlign: "center" }}>
        <div style={{ fontSize: 12, color: C.textLight }}>Total charged to room</div>
        <div style={{ fontSize: 22, fontWeight: 800, color: C.gold, marginTop: 4 }}>{fmt(cartTotal)}</div>
      </div>
      <button onClick={() => onNav("welcome")} style={{ marginTop: 28, background: C.charcoal, color: C.white, border: "none", borderRadius: 12, padding: "14px 36px", fontSize: 14, fontWeight: 700, cursor: "pointer" }}>← Back to Home</button>
    </div>
  );

  if (step === "confirm") return (
    <div style={{ minHeight: "100vh", background: C.cream, fontFamily: "'DM Sans', sans-serif" }}>
      <BackBar title="Confirm Order" subtitle={`Room ${guest.room}`} onBack={() => setStep("browse")} light />
      <div style={{ padding: "20px" }}>
        <div style={{ background: C.white, borderRadius: 14, border: `1px solid ${C.border}`, overflow: "hidden", marginBottom: 16 }}>
          <div style={{ background: C.goldLight, padding: "12px 16px", fontSize: 11, letterSpacing: 2, color: C.goldDim, textTransform: "uppercase", fontWeight: 700 }}>Your Order</div>
          {Object.entries(cart).map(([id, qty]) => { const item = allItems.find((i) => i.id === +id); if (!item) return null; return (
            <div key={id} style={{ display: "flex", justifyContent: "space-between", padding: "12px 16px", borderTop: `1px solid ${C.border}`, alignItems: "center" }}>
              <div><div style={{ fontSize: 14, color: C.charcoal, fontWeight: 600 }}>{item.emoji} {item.name}</div><div style={{ fontSize: 12, color: C.textLight, marginTop: 2 }}>×{qty} · {fmt(item.price)} each</div></div>
              <div style={{ fontSize: 14, fontWeight: 700, color: C.gold }}>{fmt(item.price * qty)}</div>
            </div>
          ); })}
          <div style={{ display: "flex", justifyContent: "space-between", padding: "14px 16px", borderTop: `2px solid ${C.gold}30`, background: C.goldLight }}>
            <span style={{ fontSize: 14, fontWeight: 700 }}>Total</span>
            <span style={{ fontSize: 18, fontWeight: 800, color: C.gold }}>{fmt(cartTotal)}</span>
          </div>
        </div>
        <textarea value={note} onChange={(e) => setNote(e.target.value)} placeholder="Special instructions (optional)..."
          style={{ width: "100%", padding: "12px 14px", borderRadius: 12, border: `1px solid ${C.border}`, fontSize: 14, fontFamily: "'DM Sans', sans-serif", minHeight: 80, resize: "none", outline: "none", boxSizing: "border-box", marginBottom: 16 }} />
        <button onClick={placeOrder} style={{ width: "100%", background: C.gold, color: C.white, border: "none", borderRadius: 14, padding: "16px", fontSize: 15, fontWeight: 700, cursor: "pointer" }}>Confirm & Send to Kitchen</button>
      </div>
    </div>
  );

  return (
    <div style={{ minHeight: "100vh", background: C.cream, fontFamily: "'DM Sans', sans-serif", paddingBottom: cartCount > 0 ? 100 : 20 }}>
      <BackBar title="Room Service" subtitle="Delivered to your door" onBack={() => onNav("welcome")} />
      <div style={{ background: C.charcoal, display: "flex" }}>
        {Object.keys(MENU).map((t) => (
          <button key={t} onClick={() => setTab(t)} style={{ flex: 1, background: "none", border: "none", borderBottom: tab === t ? `3px solid ${C.gold}` : "3px solid transparent", color: tab === t ? C.gold : "#888", padding: "13px 0", fontSize: 13, fontWeight: 600, cursor: "pointer" }}>{t}</button>
        ))}
      </div>
      <div style={{ padding: "16px 20px" }}>
        {MENU[tab].map((item) => (
          <div key={item.id} style={{ background: C.white, border: `1px solid ${C.border}`, borderRadius: 14, padding: "16px", marginBottom: 12, display: "flex", alignItems: "center", gap: 12 }}>
            <span style={{ fontSize: 36 }}>{item.emoji}</span>
            <div style={{ flex: 1 }}>
              <div style={{ fontSize: 14, fontWeight: 700, color: C.charcoal }}>{item.name}</div>
              <div style={{ fontSize: 12, color: C.textLight, marginTop: 2 }}>{item.desc}</div>
              <div style={{ fontSize: 16, fontWeight: 800, color: C.gold, marginTop: 6 }}>{item.price === 0 ? "Free" : fmt(item.price)}</div>
            </div>
            <div style={{ display: "flex", alignItems: "center", gap: 8, flexShrink: 0 }}>
              {cart[item.id] ? (
                <>
                  <button onClick={() => rem(item.id)} style={{ width: 32, height: 32, borderRadius: 8, background: C.goldLight, border: `1px solid ${C.gold}`, color: C.goldDim, fontSize: 20, fontWeight: 700, cursor: "pointer" }}>−</button>
                  <span style={{ fontWeight: 800, fontSize: 16, minWidth: 24, textAlign: "center" }}>{cart[item.id]}</span>
                  <button onClick={() => add(item.id)} style={{ width: 32, height: 32, borderRadius: 8, background: C.gold, border: "none", color: C.white, fontSize: 20, fontWeight: 700, cursor: "pointer" }}>+</button>
                </>
              ) : (
                <button onClick={() => add(item.id)} style={{ background: C.charcoal, color: C.white, border: "none", borderRadius: 10, padding: "9px 16px", fontSize: 13, fontWeight: 600, cursor: "pointer" }}>Add</button>
              )}
            </div>
          </div>
        ))}
      </div>
      {cartCount > 0 && (
        <div style={{ position: "fixed", bottom: 16, left: 16, right: 16, zIndex: 50 }}>
          <button onClick={() => setStep("confirm")} style={{ width: "100%", background: C.charcoal, color: C.white, border: `2px solid ${C.gold}`, borderRadius: 16, padding: "16px 20px", fontSize: 15, fontWeight: 700, cursor: "pointer", display: "flex", justifyContent: "space-between", alignItems: "center" }}>
            <span>🛒 {cartCount} item{cartCount > 1 ? "s" : ""}</span>
            <span>View Order · {fmt(cartTotal)}</span>
          </button>
        </div>
      )}
    </div>
  );
}

// ─── GUEST REQUESTS ───────────────────────────────────────────────────────────
function GuestRequests({ guest, onNav, onRequest }) {
  const [selected, setSelected] = useState(null);
  const [note, setNote] = useState("");
  const [sent, setSent] = useState(false);
  const send = () => { onRequest({ id: Date.now(), room: guest.room, guest: guest.name, type: selected, note, time: nowTime(), status: "open" }); setSent(true); };
  if (sent) return (
    <div style={{ minHeight: "100vh", background: C.cream, display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", padding: 28, fontFamily: "'DM Sans', sans-serif" }}>
      <div style={{ fontSize: 64, marginBottom: 16 }}>✅</div>
      <div style={{ fontSize: 22, fontFamily: "'Playfair Display', serif", fontWeight: 700, color: C.charcoal }}>{selected} Request Sent</div>
      <div style={{ fontSize: 14, color: C.textMid, marginTop: 10, textAlign: "center" }}>Our team will attend to Room {guest.room} shortly.</div>
      <button onClick={() => onNav("welcome")} style={{ marginTop: 28, background: C.charcoal, color: C.white, border: "none", borderRadius: 12, padding: "14px 36px", fontSize: 14, fontWeight: 700, cursor: "pointer" }}>← Back to Home</button>
    </div>
  );
  return (
    <div style={{ minHeight: "100vh", background: C.cream, fontFamily: "'DM Sans', sans-serif", paddingBottom: 20 }}>
      <BackBar title="My Requests" subtitle={`Room ${guest.room}`} onBack={() => onNav("welcome")} />
      <div style={{ padding: "20px" }}>
        <div style={{ fontSize: 12, color: C.textLight, marginBottom: 16 }}>What do you need help with?</div>
        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: 12, marginBottom: 20 }}>
          {REQUEST_TYPES.map((t) => (
            <button key={t.label} onClick={() => setSelected(selected === t.label ? null : t.label)}
              style={{ background: selected === t.label ? C.goldLight : C.white, border: `${selected === t.label ? "2px" : "1px"} solid ${selected === t.label ? C.gold : C.border}`, borderRadius: 14, padding: "18px 14px", textAlign: "center", cursor: "pointer" }}>
              <div style={{ fontSize: 26, marginBottom: 8 }}>{t.icon}</div>
              <div style={{ fontSize: 13, fontWeight: 700, color: C.charcoal }}>{t.label}</div>
              <div style={{ fontSize: 10, color: C.textLight, marginTop: 3 }}>{t.sub}</div>
            </button>
          ))}
        </div>
        {selected && (<>
          <textarea value={note} onChange={(e) => setNote(e.target.value)} placeholder="Additional details (optional)..."
            style={{ width: "100%", padding: "12px 14px", borderRadius: 12, border: `1px solid ${C.border}`, fontSize: 14, fontFamily: "'DM Sans', sans-serif", minHeight: 80, resize: "none", outline: "none", boxSizing: "border-box", marginBottom: 14 }} />
          <button onClick={send} style={{ width: "100%", background: C.gold, color: C.white, border: "none", borderRadius: 14, padding: "16px", fontSize: 15, fontWeight: 700, cursor: "pointer" }}>Send {selected} Request</button>
        </>)}
      </div>
    </div>
  );
}

// ─── GUEST INFO ───────────────────────────────────────────────────────────────
function GuestInfo({ onNav }) {
  const [open, setOpen] = useState(null);
  const sections = [
    { icon: "📍", title: "Location & Contact", items: [["Address", HOTEL.address], ["Phone", HOTEL.phone], ["Email", HOTEL.email]] },
    { icon: "⏰", title: "Check-in / Check-out", items: [["Check-in", HOTEL.checkin], ["Check-out", HOTEL.checkout], ["WiFi Name", HOTEL.wifiName], ["WiFi Password", HOTEL.wifi]] },
    { icon: "🏊", title: "Facilities & Hours", items: [["Breakfast", HOTEL.breakfast], ["Pool", HOTEL.pool], ["Gym", HOTEL.gym], ["Room Service", "24 hours"]] },
    { icon: "📍", title: "Nearby Attractions", items: [["Palms Mall", "~0.8 miles"], ["Viva Cinemas", "~2.4 miles"], ["Shoprite Ilorin", "Nearby"], ["Emir's Palace", "Nearby"]] },
    { icon: "🚨", title: "Emergency Contacts", items: [["Reception", "500 (room phone) / " + HOTEL.phone], ["Emergency", "112"], ["Police", "08039539280"], ["Hospital (UITH)", "~10 mins"]] },
  ];
  return (
    <div style={{ minHeight: "100vh", background: C.cream, fontFamily: "'DM Sans', sans-serif", paddingBottom: 20 }}>
      <BackBar title="Hotel Information" subtitle="E-Phoenix Annex II" onBack={() => onNav("welcome")} />
      <div style={{ padding: "20px" }}>
        {sections.map((s) => (
          <div key={s.title} style={{ background: C.white, border: `1px solid ${C.border}`, borderRadius: 14, marginBottom: 12, overflow: "hidden" }}>
            <button onClick={() => setOpen(open === s.title ? null : s.title)} style={{ width: "100%", background: "none", border: "none", padding: "14px 16px", display: "flex", alignItems: "center", justifyContent: "space-between", cursor: "pointer" }}>
              <div style={{ display: "flex", alignItems: "center", gap: 10 }}>
                <span style={{ fontSize: 20 }}>{s.icon}</span>
                <span style={{ fontSize: 14, fontWeight: 700, color: C.charcoal }}>{s.title}</span>
              </div>
              <span style={{ color: C.gold, fontSize: 18 }}>{open === s.title ? "−" : "+"}</span>
            </button>
            {open === s.title && s.items.map(([k, v]) => (
              <div key={k} style={{ display: "flex", justifyContent: "space-between", padding: "12px 16px", borderTop: `1px solid ${C.border}`, gap: 12 }}>
                <span style={{ fontSize: 13, color: C.textLight }}>{k}</span>
                <span style={{ fontSize: 13, color: C.charcoal, fontWeight: 600, textAlign: "right", maxWidth: "58%" }}>{v}</span>
              </div>
            ))}
          </div>
        ))}
      </div>
    </div>
  );
}

// ─── GUEST PULSE ──────────────────────────────────────────────────────────────
function GuestPulse({ guest, onNav, onDone, onComplaint }) {
  const [step, setStep] = useState("ask");
  const [msg, setMsg] = useState("");
  const first = guest.name.split(" ")[0];
  const sendComplaint = () => { if (!msg.trim()) return; onComplaint({ id: Date.now(), room: guest.room, guest: guest.name, message: msg, time: nowTime(), status: "open" }); setStep("sent"); };

  if (step === "happy") return (
    <div style={{ minHeight: "100vh", background: C.cream, display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", padding: 28, fontFamily: "'DM Sans', sans-serif" }}>
      <div style={{ fontSize: 64, marginBottom: 16 }}>🌟</div>
      <div style={{ fontSize: 24, fontFamily: "'Playfair Display', serif", fontWeight: 700, color: C.charcoal, textAlign: "center" }}>That's wonderful!</div>
      <div style={{ fontSize: 14, color: C.textMid, marginTop: 12, textAlign: "center", lineHeight: 1.7 }}>Would you mind sharing your experience? It helps other travellers find us.</div>
      <a href={HOTEL.googleMaps} target="_blank" rel="noreferrer" style={{ marginTop: 28, background: C.gold, color: C.white, textDecoration: "none", borderRadius: 14, padding: "16px 32px", fontSize: 15, fontWeight: 700, display: "block", textAlign: "center", width: "80%" }}>⭐ Leave a Google Review</a>
      <button onClick={() => { onDone(); onNav("welcome"); }} style={{ marginTop: 14, background: "none", border: "none", color: C.textLight, fontSize: 13, cursor: "pointer" }}>No thanks</button>
    </div>
  );
  if (step === "unhappy") return (
    <div style={{ minHeight: "100vh", background: C.cream, display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", padding: 28, fontFamily: "'DM Sans', sans-serif" }}>
      <div style={{ fontSize: 64, marginBottom: 16 }}>💌</div>
      <div style={{ fontSize: 22, fontFamily: "'Playfair Display', serif", fontWeight: 700, color: C.charcoal, textAlign: "center" }}>We're truly sorry.</div>
      <div style={{ fontSize: 14, color: C.textMid, marginTop: 10, textAlign: "center", lineHeight: 1.6 }}>Tell us what went wrong and we'll fix it immediately.</div>
      <textarea value={msg} onChange={(e) => setMsg(e.target.value)} placeholder="Describe the issue..."
        style={{ width: "100%", marginTop: 20, padding: "14px 16px", borderRadius: 12, border: `1px solid ${C.border}`, fontSize: 14, fontFamily: "'DM Sans', sans-serif", minHeight: 100, resize: "none", outline: "none", boxSizing: "border-box" }} />
      <button onClick={sendComplaint} style={{ marginTop: 16, width: "100%", background: C.error, color: C.white, border: "none", borderRadius: 14, padding: "16px", fontSize: 15, fontWeight: 700, cursor: "pointer", opacity: msg.trim() ? 1 : 0.5 }}>Send to Manager Now</button>
    </div>
  );
  if (step === "sent") return (
    <div style={{ minHeight: "100vh", background: C.cream, display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", padding: 28, fontFamily: "'DM Sans', sans-serif" }}>
      <div style={{ fontSize: 64, marginBottom: 16 }}>✅</div>
      <div style={{ fontSize: 22, fontFamily: "'Playfair Display', serif", fontWeight: 700, color: C.charcoal, textAlign: "center" }}>Message Sent</div>
      <div style={{ fontSize: 14, color: C.textMid, marginTop: 10, textAlign: "center", lineHeight: 1.6 }}>Our manager has been alerted and will resolve this within 15 minutes.</div>
      <button onClick={() => { onDone(); onNav("welcome"); }} style={{ marginTop: 28, background: C.charcoal, color: C.white, border: "none", borderRadius: 14, padding: "14px 32px", fontSize: 14, fontWeight: 700, cursor: "pointer" }}>Back to Home</button>
    </div>
  );
  return (
    <div style={{ minHeight: "100vh", background: C.cream, display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", padding: 28, fontFamily: "'DM Sans', sans-serif" }}>
      <div style={{ fontSize: 11, letterSpacing: 4, color: C.gold, textTransform: "uppercase", marginBottom: 20 }}>E-Phoenix Annex II</div>
      <div style={{ fontSize: 26, fontFamily: "'Playfair Display', serif", fontWeight: 700, color: C.charcoal, textAlign: "center" }}>Hi {first},</div>
      <div style={{ fontSize: 17, color: C.textMid, marginTop: 8, textAlign: "center" }}>How is your stay so far? 😊</div>
      <div style={{ width: "100%", marginTop: 36, display: "flex", flexDirection: "column", gap: 14 }}>
        {[
          { e: "😊", l: "Loving It!", sub: "Everything is great", a: () => setStep("happy"), bg: C.goldLight, bdr: C.gold, col: C.goldDim },
          { e: "😐", l: "It's Okay", sub: "Could be better", a: () => setStep("unhappy"), bg: C.white, bdr: C.border, col: C.textMid },
          { e: "😞", l: "Not Happy", sub: "Something went wrong", a: () => setStep("unhappy"), bg: "#FFF5F5", bdr: "#E0A0A0", col: C.error },
        ].map((btn) => (
          <button key={btn.l} onClick={btn.a} style={{ background: btn.bg, border: `2px solid ${btn.bdr}`, borderRadius: 16, padding: "18px 22px", display: "flex", alignItems: "center", gap: 16, cursor: "pointer", width: "100%" }}>
            <span style={{ fontSize: 36 }}>{btn.e}</span>
            <div style={{ textAlign: "left" }}>
              <div style={{ fontSize: 16, fontWeight: 700, color: btn.col }}>{btn.l}</div>
              <div style={{ fontSize: 12, color: C.textLight, marginTop: 2 }}>{btn.sub}</div>
            </div>
          </button>
        ))}
      </div>
    </div>
  );
}

// ─── GUEST NAV ────────────────────────────────────────────────────────────────
function GuestNav({ screen, onNav }) {
  return (
    <div style={{ position: "fixed", bottom: 0, left: 0, right: 0, background: C.white, borderTop: `1px solid ${C.border}`, display: "flex", maxWidth: 480, margin: "0 auto", zIndex: 100 }}>
      {[["🏠", "Home", "welcome"], ["🍽", "Order", "menu"], ["🛎", "Request", "requests"], ["⭐", "Rate", "pulse"], ["ℹ️", "Info", "info"]].map(([icon, label, s]) => (
        <button key={s} onClick={() => onNav(s)} style={{ flex: 1, background: "none", border: "none", padding: "10px 0 14px", cursor: "pointer", display: "flex", flexDirection: "column", alignItems: "center", gap: 3 }}>
          <span style={{ fontSize: 20 }}>{icon}</span>
          <span style={{ fontSize: 9, fontFamily: "'DM Sans', sans-serif", color: screen === s ? C.gold : C.textLight, fontWeight: screen === s ? 700 : 400 }}>{label}</span>
          {screen === s && <div style={{ width: 4, height: 4, borderRadius: "50%", background: C.gold }} />}
        </button>
      ))}
    </div>
  );
}

// ─── ADMIN LOGIN ──────────────────────────────────────────────────────────────
function AdminLogin({ onLogin, onBack }) {
  const [username, setUsername] = useState("");
  const [password, setPassword] = useState("");
  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);
  const handle = () => {
    const user = ADMIN_USERS.find((u) => u.username === username.trim().toLowerCase() && u.password === password);
    if (!user) { setError("Invalid username or password"); return; }
    setError(""); setLoading(true);
    setTimeout(() => { setLoading(false); onLogin(user); }, 1000);
  };
  return (
    <div style={{ minHeight: "100vh", background: "#0D0D0D", display: "flex", flexDirection: "column", fontFamily: "'DM Sans', sans-serif" }}>
      <div style={{ padding: "20px" }}><button onClick={onBack} style={{ background: "none", border: "none", color: "#666", fontSize: 14, cursor: "pointer" }}>← Back</button></div>
      <div style={{ flex: 1, display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", padding: "0 28px 60px" }}>
        <div style={{ width: 56, height: 56, background: `${C.gold}20`, border: `2px solid ${C.gold}40`, borderRadius: 16, display: "flex", alignItems: "center", justifyContent: "center", fontSize: 24, marginBottom: 20 }}>🔐</div>
        <div style={{ fontSize: 24, fontFamily: "'Playfair Display', serif", color: C.white, fontWeight: 700, textAlign: "center" }}>Staff Login</div>
        <div style={{ fontSize: 13, color: "#555", marginTop: 6, textAlign: "center" }}>E-Phoenix Annex II Management</div>
        <div style={{ width: "100%", marginTop: 36 }}>
          {[["Username", username, setUsername, "text"], ["Password", password, setPassword, "password"]].map(([ph, val, set, type]) => (
            <input key={ph} value={val} onChange={(e) => set(e.target.value)} placeholder={ph} type={type}
              onKeyDown={(e) => e.key === "Enter" && handle()}
              style={{ width: "100%", padding: "16px 18px", borderRadius: 12, border: "1px solid #222", background: "#1a1a1a", color: C.white, fontSize: 15, fontFamily: "'DM Sans', sans-serif", outline: "none", boxSizing: "border-box", marginBottom: 12 }} />
          ))}
          {error && <div style={{ color: "#ff8080", fontSize: 13, marginBottom: 12 }}>{error}</div>}
          <button onClick={handle} style={{ width: "100%", background: loading ? C.goldDim : C.gold, color: C.white, border: "none", borderRadius: 12, padding: "16px", fontSize: 15, fontWeight: 700, cursor: "pointer" }}>
            {loading ? "Verifying..." : "Sign In →"}
          </button>
          <div style={{ marginTop: 20, background: "#1a1a1a", border: "1px solid #2a2a2a", borderRadius: 10, padding: "12px 16px", fontSize: 12, color: "#555" }}>
            <div style={{ color: "#666", marginBottom: 4 }}>Demo credentials:</div>
            <div>admin / ephoenix2024 &nbsp;·&nbsp; manager / manager123 &nbsp;·&nbsp; frontdesk / desk123</div>
          </div>
        </div>
      </div>
    </div>
  );
}

// ─── ADMIN DASHBOARD ──────────────────────────────────────────────────────────
function AdminDashboard({ admin, rooms, setRooms, complaints, setComplaints, orders, setOrders, requests, setRequests, announcements, setAnnouncements, onLogout }) {
  const [screen, setScreen] = useState("overview");
  const openComplaints = complaints.filter((c) => c.status === "open");
  const pendingOrders = orders.filter((o) => o.status === "pending");

  const AdminTopBar = () => (
    <div style={{ background: C.charcoal, borderBottom: "1px solid #2a2a2a", padding: "14px 20px", display: "flex", justifyContent: "space-between", alignItems: "center" }}>
      <div>
        <div style={{ fontSize: 16, fontFamily: "'Playfair Display', serif", color: C.white, fontWeight: 700 }}>E-Phoenix Annex II</div>
        <div style={{ fontSize: 11, color: "#888" }}>{admin.role} · {admin.name}</div>
      </div>
      <div style={{ display: "flex", gap: 8 }}>
        {openComplaints.length > 0 && (
          <button onClick={() => setScreen("alerts")} style={{ background: C.error, color: C.white, border: "none", borderRadius: 8, padding: "6px 10px", fontSize: 11, fontWeight: 700, cursor: "pointer" }}>⚠️ {openComplaints.length}</button>
        )}
        <button onClick={onLogout} style={{ background: "none", border: "1px solid #444", color: "#888", borderRadius: 8, padding: "6px 10px", fontSize: 11, cursor: "pointer" }}>Sign Out</button>
      </div>
    </div>
  );

  const AdminNav = () => (
    <div style={{ position: "fixed", bottom: 0, left: 0, right: 0, background: C.charcoal, borderTop: "1px solid #2a2a2a", display: "flex", maxWidth: 480, margin: "0 auto", zIndex: 100 }}>
      {[
        ["📊", "Overview", "overview"],
        ["🏨", "Rooms", "rooms"],
        ["⚠️", openComplaints.length > 0 ? `Alerts(${openComplaints.length})` : "Alerts", "alerts"],
        ["🍽", pendingOrders.length > 0 ? `Orders(${pendingOrders.length})` : "Orders", "orders"],
        ["🛎", "Requests", "requests_admin"],
        ["📢", "Notice", "announce"],
        ["✅", "Check-in", "checkin"],
      ].map(([icon, label, s]) => (
        <button key={s} onClick={() => setScreen(s)} style={{ flex: 1, background: "none", border: "none", padding: "7px 0 11px", cursor: "pointer", display: "flex", flexDirection: "column", alignItems: "center", gap: 2 }}>
          <span style={{ fontSize: 15 }}>{icon}</span>
          <span style={{ fontSize: 7, fontFamily: "'DM Sans', sans-serif", color: screen === s ? C.gold : "#555", fontWeight: screen === s ? 700 : 400, textAlign: "center", maxWidth: 46, lineHeight: 1.2 }}>{label}</span>
          {screen === s && <div style={{ width: 3, height: 3, borderRadius: "50%", background: C.gold }} />}
        </button>
      ))}
    </div>
  );

  // ── OVERVIEW ──
  const Overview = () => {
    const totalRevenue = orders.reduce((s, o) => s + o.total, 0);
    const occupied = rooms.filter((r) => r.status !== "vacant").length;
    return (
      <div style={{ paddingBottom: 80 }}>
        <AdminTopBar />
        <div style={{ padding: "20px", background: "#F5F3EE" }}>
          <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: 12, marginBottom: 20 }}>
            {[
              { label: "Total Revenue", value: fmt(totalRevenue), sub: "From portal orders", color: C.gold },
              { label: "Open Complaints", value: String(openComplaints.length), sub: "Need attention", color: openComplaints.length > 0 ? C.error : "#22c55e" },
              { label: "Occupied Rooms", value: `${occupied}/${rooms.length}`, sub: "Right now", color: "#4C9AC9" },
              { label: "Pending Orders", value: String(pendingOrders.length), sub: "In kitchen queue", color: "#f59e0b" },
            ].map((kpi) => (
              <div key={kpi.label} style={{ background: C.white, border: `1px solid ${C.border}`, borderRadius: 14, padding: "16px" }}>
                <div style={{ fontSize: 22, fontWeight: 800, color: kpi.color }}>{kpi.value}</div>
                <div style={{ fontSize: 12, fontWeight: 600, color: C.charcoal, marginTop: 4 }}>{kpi.label}</div>
                <div style={{ fontSize: 11, color: C.textLight, marginTop: 2 }}>{kpi.sub}</div>
              </div>
            ))}
          </div>
          {orders.length > 0 ? (
            <div style={{ background: C.white, border: `1px solid ${C.border}`, borderRadius: 14, padding: "16px" }}>
              <div style={{ fontSize: 13, fontWeight: 700, color: C.charcoal, marginBottom: 12 }}>Recent Orders</div>
              {orders.slice(-4).reverse().map((o) => (
                <div key={o.id} style={{ display: "flex", justifyContent: "space-between", padding: "8px 0", borderBottom: `1px solid ${C.border}` }}>
                  <div>
                    <div style={{ fontSize: 13, color: C.charcoal, fontWeight: 600 }}>Room {o.room} · {o.guest.split(" ")[0]}</div>
                    <div style={{ fontSize: 11, color: C.textLight, marginTop: 2 }}>{o.time}</div>
                  </div>
                  <div style={{ fontSize: 14, fontWeight: 700, color: C.gold }}>{fmt(o.total)}</div>
                </div>
              ))}
            </div>
          ) : (
            <div style={{ background: C.white, border: `1px solid ${C.border}`, borderRadius: 14, padding: "32px", textAlign: "center" }}>
              <div style={{ fontSize: 32, marginBottom: 12 }}>🏨</div>
              <div style={{ fontSize: 14, fontWeight: 700, color: C.charcoal }}>Waiting for activity</div>
              <div style={{ fontSize: 12, color: C.textLight, marginTop: 6 }}>Guest orders, requests and complaints appear here in real time</div>
            </div>
          )}
        </div>
      </div>
    );
  };

  // ── ROOMS ──
  const Rooms = () => {
    const checkout = (id) => setRooms((r) => r.map((x) => x.id === id ? { ...x, guest: "", email: "", phone: "", numGuests: 1, checkin: "", checkout: "", status: "vacant" } : x));
    return (
      <div style={{ paddingBottom: 80 }}>
        <AdminTopBar />
        <div style={{ padding: "20px", background: "#F5F3EE" }}>
          <div style={{ fontSize: 11, letterSpacing: 2, color: C.textLight, textTransform: "uppercase", marginBottom: 14 }}>All Rooms</div>
          {rooms.map((r) => (
            <div key={r.id} style={{ background: C.white, border: `1.5px solid ${r.status === "complaint" ? C.error : C.border}`, borderRadius: 14, padding: "16px", marginBottom: 12 }}>
              <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start" }}>
                <div style={{ display: "flex", gap: 12, alignItems: "flex-start" }}>
                  <div style={{ fontSize: 20, fontWeight: 800, color: C.charcoal, minWidth: 44 }}>Rm {r.number}</div>
                  <div>
                    {r.guest ? (<>
                      <div style={{ fontSize: 14, fontWeight: 600, color: C.charcoal }}>{r.guest}</div>
                      {r.email && <div style={{ fontSize: 11, color: C.textLight }}>{r.email}</div>}
                      {r.phone && <div style={{ fontSize: 11, color: C.textLight }}>{r.phone}</div>}
                      {r.numGuests > 1 && <div style={{ fontSize: 11, color: C.textLight }}>{r.numGuests} guests</div>}
                      <div style={{ fontSize: 11, color: C.textLight }}>{r.checkin} → {r.checkout}</div>
                    </>) : <div style={{ fontSize: 13, color: C.textLight }}>Vacant</div>}
                  </div>
                </div>
                <span style={{ background: r.status === "vacant" ? "#F5F5F5" : r.status === "complaint" ? C.errorLight : C.successLight, color: r.status === "vacant" ? "#9ca3af" : r.status === "complaint" ? C.error : C.success, border: `1px solid ${r.status === "vacant" ? "#ddd" : r.status === "complaint" ? `${C.error}40` : `${C.success}40`}`, borderRadius: 6, padding: "3px 8px", fontSize: 10, fontWeight: 700, textTransform: "uppercase", flexShrink: 0 }}>
                  {r.status === "vacant" ? "Vacant" : r.status === "complaint" ? "Complaint" : r.status === "pending" ? "Request" : "Active"}
                </span>
              </div>
              {r.guest && (
                <div style={{ display: "flex", gap: 8, marginTop: 12 }}>
                  {r.status === "complaint" && <button onClick={() => setScreen("alerts")} style={{ background: C.errorLight, color: C.error, border: `1px solid ${C.error}30`, borderRadius: 8, padding: "6px 12px", fontSize: 11, fontWeight: 700, cursor: "pointer" }}>⚠️ View Alert</button>}
                  <DeleteBtn onDelete={() => checkout(r.id)} label="Check Out" />
                </div>
              )}
            </div>
          ))}
        </div>
      </div>
    );
  };

  // ── ALERTS ──
  const Alerts = () => {
    const [timer, setTimer] = useState(900);
    useEffect(() => { const t = setInterval(() => setTimer((v) => Math.max(0, v - 1)), 1000); return () => clearInterval(t); }, []);
    const mins = Math.floor(timer / 60).toString().padStart(2, "0");
    const secs = (timer % 60).toString().padStart(2, "0");
    const urgent = timer < 120;

    const resolve = (id) => {
      const comp = complaints.find((c) => c.id === id);
      setComplaints((c) => c.map((x) => x.id === id ? { ...x, status: "resolved" } : x));
      if (comp) setRooms((r) => r.map((x) => x.number === comp.room || x.number === comp.room.padStart(2, "0") ? { ...x, status: "active" } : x));
    };
    const clearAll = () => setComplaints([]);

    return (
      <div style={{ paddingBottom: 80 }}>
        <AdminTopBar />
        <div style={{ padding: "20px", background: "#F5F3EE" }}>
          <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: 14 }}>
            <div style={{ fontSize: 11, letterSpacing: 2, color: C.textLight, textTransform: "uppercase" }}>Complaint Alerts</div>
            {complaints.length > 0 && <DeleteBtn onDelete={clearAll} label="Clear All" />}
          </div>
          {complaints.length === 0 ? (
            <div style={{ background: C.white, borderRadius: 14, padding: "40px", textAlign: "center" }}>
              <div style={{ fontSize: 40, marginBottom: 12 }}>✅</div>
              <div style={{ fontSize: 15, fontWeight: 700, color: C.charcoal }}>No complaints</div>
              <div style={{ fontSize: 13, color: C.textLight, marginTop: 6 }}>All guests are happy right now</div>
            </div>
          ) : complaints.map((c) => (
            <div key={c.id} style={{ background: C.white, border: `1.5px solid ${c.status === "resolved" ? "#22c55e" : C.error}`, borderRadius: 16, overflow: "hidden", marginBottom: 16 }}>
              <div style={{ background: c.status === "resolved" ? C.successLight : C.errorLight, padding: "12px 16px", display: "flex", justifyContent: "space-between", alignItems: "center" }}>
                <div style={{ display: "flex", alignItems: "center", gap: 8 }}>
                  <span>{c.status === "resolved" ? "✅" : "⚠️"}</span>
                  <span style={{ fontSize: 14, fontWeight: 700, color: c.status === "resolved" ? C.success : C.error }}>Room {c.room} · {c.status === "resolved" ? "Resolved" : "Open"}</span>
                </div>
                <span style={{ fontSize: 11, color: C.textLight }}>{c.time}</span>
              </div>
              <div style={{ padding: "16px" }}>
                <div style={{ fontSize: 13, fontWeight: 700, color: C.charcoal, marginBottom: 4 }}>{c.guest}</div>
                <div style={{ fontSize: 13, color: C.textMid, fontStyle: "italic", lineHeight: 1.5, marginBottom: 14 }}>"{c.message}"</div>
                {c.status === "open" && (<>
                  <div style={{ background: urgent ? C.errorLight : C.goldLight, borderRadius: 10, padding: "10px", textAlign: "center", marginBottom: 14 }}>
                    <div style={{ fontSize: 9, color: C.textLight, letterSpacing: 2, textTransform: "uppercase" }}>Resolve Within</div>
                    <div style={{ fontSize: 26, fontWeight: 800, color: urgent ? C.error : C.gold, fontFamily: "monospace" }}>{mins}:{secs}</div>
                    {urgent && <div style={{ fontSize: 11, color: C.error, fontWeight: 700 }}>⚡ Act now!</div>}
                  </div>
                  <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: 10, marginBottom: 10 }}>
                    <button onClick={() => resolve(c.id)} style={{ background: C.gold, color: C.white, border: "none", borderRadius: 12, padding: "12px", fontSize: 12, fontWeight: 700, cursor: "pointer" }}>🔧 Assign Staff</button>
                    <button onClick={() => resolve(c.id)} style={{ background: C.white, color: C.charcoal, border: `1px solid ${C.border}`, borderRadius: 12, padding: "12px", fontSize: 12, fontWeight: 700, cursor: "pointer" }}>✋ Handle It</button>
                  </div>
                </>)}
                <div style={{ display: "flex", justifyContent: "flex-end" }}>
                  <DeleteBtn onDelete={() => setComplaints((x) => x.filter((y) => y.id !== c.id))} />
                </div>
              </div>
            </div>
          ))}
        </div>
      </div>
    );
  };

  // ── ORDERS ──
  const Orders = () => {
    const statusColor = { pending: "#f59e0b", preparing: C.gold, delivered: "#22c55e" };
    const clearAll = () => setOrders([]);
    return (
      <div style={{ paddingBottom: 80 }}>
        <AdminTopBar />
        <div style={{ padding: "20px", background: "#F5F3EE" }}>
          <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: 14 }}>
            <div style={{ fontSize: 11, letterSpacing: 2, color: C.textLight, textTransform: "uppercase" }}>Room Service Orders</div>
            {orders.length > 0 && <DeleteBtn onDelete={clearAll} label="Clear All" />}
          </div>
          {orders.length === 0 ? (
            <div style={{ background: C.white, borderRadius: 14, padding: "40px", textAlign: "center" }}>
              <div style={{ fontSize: 40, marginBottom: 12 }}>🍽</div>
              <div style={{ fontSize: 15, fontWeight: 700, color: C.charcoal }}>No orders yet</div>
              <div style={{ fontSize: 13, color: C.textLight, marginTop: 6 }}>Guest orders appear here in real time</div>
            </div>
          ) : orders.slice().reverse().map((o) => (
            <div key={o.id} style={{ background: C.white, border: `1px solid ${C.border}`, borderRadius: 14, padding: "16px", marginBottom: 12 }}>
              <div style={{ display: "flex", justifyContent: "space-between", marginBottom: 8 }}>
                <div style={{ fontSize: 14, fontWeight: 700, color: C.charcoal }}>Room {o.room}</div>
                <span style={{ background: `${statusColor[o.status]}20`, color: statusColor[o.status], border: `1px solid ${statusColor[o.status]}40`, borderRadius: 6, padding: "3px 10px", fontSize: 11, fontWeight: 700, textTransform: "uppercase" }}>{o.status}</span>
              </div>
              <div style={{ fontSize: 13, fontWeight: 600, color: C.charcoal, marginBottom: 4 }}>{o.guest}</div>
              <div style={{ fontSize: 12, color: C.textLight, marginBottom: 4 }}>{o.items}</div>
              {o.note && <div style={{ fontSize: 12, color: C.textMid, fontStyle: "italic", marginBottom: 8 }}>Note: {o.note}</div>}
              <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: 10 }}>
                <span style={{ fontSize: 11, color: C.textLight }}>{o.time}</span>
                <span style={{ fontSize: 16, fontWeight: 800, color: C.gold }}>{fmt(o.total)}</span>
              </div>
              <div style={{ display: "flex", gap: 8, flexWrap: "wrap" }}>
                {o.status === "pending" && <button onClick={() => setOrders((x) => x.map((y) => y.id === o.id ? { ...y, status: "preparing" } : y))} style={{ background: C.goldLight, color: C.goldDim, border: `1px solid ${C.gold}40`, borderRadius: 8, padding: "6px 12px", fontSize: 11, fontWeight: 700, cursor: "pointer" }}>Start Preparing</button>}
                {o.status === "preparing" && <button onClick={() => setOrders((x) => x.map((y) => y.id === o.id ? { ...y, status: "delivered" } : y))} style={{ background: C.successLight, color: C.success, border: `1px solid ${C.success}40`, borderRadius: 8, padding: "6px 12px", fontSize: 11, fontWeight: 700, cursor: "pointer" }}>Mark Delivered ✓</button>}
                <DeleteBtn onDelete={() => setOrders((x) => x.filter((y) => y.id !== o.id))} />
              </div>
            </div>
          ))}
        </div>
      </div>
    );
  };

  // ── REQUESTS ADMIN ──
  const RequestsAdmin = () => {
    const clearAll = () => setRequests([]);
    return (
      <div style={{ paddingBottom: 80 }}>
        <AdminTopBar />
        <div style={{ padding: "20px", background: "#F5F3EE" }}>
          <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: 14 }}>
            <div style={{ fontSize: 11, letterSpacing: 2, color: C.textLight, textTransform: "uppercase" }}>Guest Requests</div>
            {requests.length > 0 && <DeleteBtn onDelete={clearAll} label="Clear All" />}
          </div>
          {requests.length === 0 ? (
            <div style={{ background: C.white, borderRadius: 14, padding: "40px", textAlign: "center" }}>
              <div style={{ fontSize: 40, marginBottom: 12 }}>🛎</div>
              <div style={{ fontSize: 15, fontWeight: 700, color: C.charcoal }}>No requests yet</div>
              <div style={{ fontSize: 13, color: C.textLight, marginTop: 6 }}>Guest requests appear here in real time</div>
            </div>
          ) : requests.slice().reverse().map((r) => (
            <div key={r.id} style={{ background: C.white, border: `1.5px solid ${r.status === "resolved" ? "#22c55e40" : `${C.gold}40`}`, borderRadius: 14, padding: "16px", marginBottom: 12 }}>
              <div style={{ display: "flex", justifyContent: "space-between", marginBottom: 8 }}>
                <div style={{ fontSize: 14, fontWeight: 700, color: C.charcoal }}>Room {r.room} · {r.type}</div>
                <span style={{ background: r.status === "resolved" ? C.successLight : C.goldLight, color: r.status === "resolved" ? C.success : C.goldDim, borderRadius: 6, padding: "3px 8px", fontSize: 10, fontWeight: 700, textTransform: "uppercase" }}>{r.status}</span>
              </div>
              <div style={{ fontSize: 13, color: C.charcoal, marginBottom: 4 }}>{r.guest}</div>
              {r.note && <div style={{ fontSize: 12, color: C.textMid, fontStyle: "italic", marginBottom: 8 }}>"{r.note}"</div>}
              <div style={{ fontSize: 11, color: C.textLight, marginBottom: 10 }}>{r.time}</div>
              <div style={{ display: "flex", gap: 8 }}>
                {r.status === "open" && <button onClick={() => setRequests((x) => x.map((y) => y.id === r.id ? { ...y, status: "resolved" } : y))} style={{ background: C.goldLight, color: C.goldDim, border: `1px solid ${C.gold}40`, borderRadius: 8, padding: "6px 12px", fontSize: 11, fontWeight: 700, cursor: "pointer" }}>✓ Mark Resolved</button>}
                <DeleteBtn onDelete={() => setRequests((x) => x.filter((y) => y.id !== r.id))} />
              </div>
            </div>
          ))}
        </div>
      </div>
    );
  };

  // ── ANNOUNCEMENTS ──
  const Announce = () => {
    const [form, setForm] = useState({ title: "", body: "", type: "info", hours: "" });
    const set = (k, v) => setForm((f) => ({ ...f, [k]: v }));
    const [posting, setPosting] = useState(false);

    const post = () => {
      if (!form.title.trim() || !form.body.trim()) return;
      const expires = form.hours ? new Date(Date.now() + parseFloat(form.hours) * 3600000).toISOString() : null;
      setAnnouncements((a) => [...a, { id: Date.now(), title: form.title.trim(), body: form.body.trim(), type: form.type, expires, postedAt: nowFull() }]);
      setForm({ title: "", body: "", type: "info", hours: "" });
      setPosting(false);
    };

    const clearAll = () => setAnnouncements([]);

    return (
      <div style={{ paddingBottom: 80 }}>
        <AdminTopBar />
        <div style={{ padding: "20px", background: "#F5F3EE" }}>
          <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: 16 }}>
            <div style={{ fontSize: 11, letterSpacing: 2, color: C.textLight, textTransform: "uppercase" }}>Guest Notices</div>
            {announcements.length > 0 && <DeleteBtn onDelete={clearAll} label="Clear All" />}
          </div>

          {/* Post form */}
          <div style={{ background: C.white, border: `1px solid ${C.border}`, borderRadius: 14, padding: "18px", marginBottom: 20 }}>
            <div style={{ fontSize: 13, fontWeight: 700, color: C.charcoal, marginBottom: 14 }}>📢 Post New Notice to Guests</div>
            <div style={{ marginBottom: 12 }}>
              <div style={{ fontSize: 11, color: C.textLight, marginBottom: 6 }}>NOTICE TYPE</div>
              <div style={{ display: "flex", gap: 8 }}>
                {[["info", "📢 Info"], ["promo", "🎉 Promo"], ["urgent", "🚨 Urgent"]].map(([val, label]) => (
                  <button key={val} onClick={() => set("type", val)}
                    style={{ flex: 1, background: form.type === val ? C.gold : C.white, color: form.type === val ? C.white : C.textMid, border: `1px solid ${form.type === val ? C.gold : C.border}`, borderRadius: 8, padding: "8px 4px", fontSize: 11, fontWeight: 600, cursor: "pointer" }}>{label}</button>
                ))}
              </div>
            </div>
            <div style={{ marginBottom: 12 }}>
              <div style={{ fontSize: 11, color: C.textLight, marginBottom: 6 }}>TITLE</div>
              <input value={form.title} onChange={(e) => set("title", e.target.value)} placeholder="e.g. Pool closed for maintenance"
                style={{ width: "100%", padding: "12px 14px", borderRadius: 10, border: `1px solid ${C.border}`, fontSize: 14, fontFamily: "'DM Sans', sans-serif", outline: "none", boxSizing: "border-box" }} />
            </div>
            <div style={{ marginBottom: 12 }}>
              <div style={{ fontSize: 11, color: C.textLight, marginBottom: 6 }}>MESSAGE</div>
              <textarea value={form.body} onChange={(e) => set("body", e.target.value)} placeholder="Full announcement details..."
                style={{ width: "100%", padding: "12px 14px", borderRadius: 10, border: `1px solid ${C.border}`, fontSize: 14, fontFamily: "'DM Sans', sans-serif", minHeight: 80, resize: "none", outline: "none", boxSizing: "border-box" }} />
            </div>
            <div style={{ marginBottom: 16 }}>
              <div style={{ fontSize: 11, color: C.textLight, marginBottom: 6 }}>AUTO-EXPIRE AFTER (hours) — optional</div>
              <input value={form.hours} onChange={(e) => set("hours", e.target.value)} placeholder="e.g. 2 (leave blank = no expiry)" type="number"
                style={{ width: "100%", padding: "12px 14px", borderRadius: 10, border: `1px solid ${C.border}`, fontSize: 14, fontFamily: "'DM Sans', sans-serif", outline: "none", boxSizing: "border-box" }} />
            </div>
            <button onClick={post} style={{ width: "100%", background: form.title && form.body ? C.gold : "#ccc", color: C.white, border: "none", borderRadius: 12, padding: "14px", fontSize: 14, fontWeight: 700, cursor: form.title && form.body ? "pointer" : "not-allowed" }}>
              Post to All Guests Now
            </button>
          </div>

          {/* Live notices */}
          <div style={{ fontSize: 11, color: C.textLight, letterSpacing: 2, textTransform: "uppercase", marginBottom: 12 }}>Live Notices ({announcements.length})</div>
          {announcements.length === 0 ? (
            <div style={{ background: C.white, borderRadius: 14, padding: "30px", textAlign: "center" }}>
              <div style={{ fontSize: 13, color: C.textLight }}>No notices posted yet</div>
            </div>
          ) : announcements.slice().reverse().map((a) => {
            const expired = a.expires && new Date() > new Date(a.expires);
            return (
              <div key={a.id} style={{ background: C.white, border: `1px solid ${expired ? C.border : a.type === "urgent" ? `${C.error}40` : a.type === "promo" ? `${C.gold}40` : C.border}`, borderRadius: 14, padding: "16px", marginBottom: 12, opacity: expired ? 0.5 : 1 }}>
                <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start", marginBottom: 8 }}>
                  <div style={{ display: "flex", alignItems: "center", gap: 8 }}>
                    <span>{a.type === "urgent" ? "🚨" : a.type === "promo" ? "🎉" : "📢"}</span>
                    <span style={{ fontSize: 10, fontWeight: 700, color: a.type === "urgent" ? C.error : C.goldDim, textTransform: "uppercase", letterSpacing: 1 }}>{a.type}{expired ? " · EXPIRED" : ""}</span>
                  </div>
                  <DeleteBtn onDelete={() => setAnnouncements((x) => x.filter((y) => y.id !== a.id))} />
                </div>
                <div style={{ fontSize: 14, fontWeight: 700, color: C.charcoal, marginBottom: 4 }}>{a.title}</div>
                <div style={{ fontSize: 13, color: C.textMid, lineHeight: 1.5, marginBottom: 8 }}>{a.body}</div>
                <div style={{ fontSize: 11, color: C.textLight }}>
                  Posted: {a.postedAt}
                  {a.expires && ` · Expires: ${new Date(a.expires).toLocaleTimeString("en-NG", { hour: "2-digit", minute: "2-digit" })}`}
                </div>
              </div>
            );
          })}
        </div>
      </div>
    );
  };

  // ── CHECK-IN ──
  const CheckIn = () => {
    const [form, setForm] = useState({ name: "", room: "", email: "", phone: "", numGuests: "1", checkout: "" });
    const set = (k, v) => setForm((f) => ({ ...f, [k]: v }));
    const [done, setDone] = useState(false);

    const handle = () => {
      if (!form.name.trim() || !form.room.trim()) return;
      setRooms((r) => r.map((x) => x.number === form.room.padStart(2, "0") || x.number === form.room ? { ...x, guest: form.name, email: form.email, phone: form.phone, numGuests: parseInt(form.numGuests) || 1, status: "active", checkin: nowTime(), checkout: form.checkout || "Tomorrow 12:00" } : x));
      setDone(true);
    };

    if (done) return (
      <div style={{ paddingBottom: 80 }}>
        <AdminTopBar />
        <div style={{ display: "flex", flexDirection: "column", alignItems: "center", justifyContent: "center", padding: 40, minHeight: "60vh" }}>
          <div style={{ fontSize: 64, marginBottom: 16 }}>✅</div>
          <div style={{ fontSize: 20, fontFamily: "'Playfair Display', serif", fontWeight: 700, color: C.charcoal }}>{form.name} checked in</div>
          <div style={{ fontSize: 14, color: C.textLight, marginTop: 8 }}>Room {form.room} portal is now active</div>
          <button onClick={() => { setDone(false); setForm({ name: "", room: "", email: "", phone: "", numGuests: "1", checkout: "" }); }}
            style={{ marginTop: 24, background: C.gold, color: C.white, border: "none", borderRadius: 12, padding: "12px 28px", fontSize: 14, fontWeight: 700, cursor: "pointer" }}>Check In Another</button>
        </div>
      </div>
    );

    return (
      <div style={{ paddingBottom: 80 }}>
        <AdminTopBar />
        <div style={{ padding: "20px", background: "#F5F3EE" }}>
          <div style={{ fontSize: 11, letterSpacing: 2, color: C.textLight, textTransform: "uppercase", marginBottom: 14 }}>Check In New Guest</div>
          <div style={{ background: C.white, border: `1px solid ${C.border}`, borderRadius: 14, padding: "20px" }}>
            {[["Guest Full Name *", "name", "text", "e.g. Amina Bello"], ["Room Number *", "room", "tel", "e.g. 07"], ["Email Address", "email", "email", "guest@email.com"], ["Phone Number", "phone", "tel", "e.g. 08012345678"], ["Checkout Date & Time", "checkout", "text", "e.g. Friday 12:00"]].map(([label, key, type, ph]) => (
              <div key={key} style={{ marginBottom: 14 }}>
                <div style={{ fontSize: 12, color: C.textLight, marginBottom: 6 }}>{label}</div>
                <input value={form[key]} onChange={(e) => set(key, e.target.value)} placeholder={ph} type={type}
                  style={{ width: "100%", padding: "12px 14px", borderRadius: 10, border: `1px solid ${C.border}`, fontSize: 14, fontFamily: "'DM Sans', sans-serif", outline: "none", boxSizing: "border-box" }} />
              </div>
            ))}
            <div style={{ marginBottom: 16 }}>
              <div style={{ fontSize: 12, color: C.textLight, marginBottom: 6 }}>Number of Guests</div>
              <select value={form.numGuests} onChange={(e) => set("numGuests", e.target.value)}
                style={{ width: "100%", padding: "12px 14px", borderRadius: 10, border: `1px solid ${C.border}`, fontSize: 14, fontFamily: "'DM Sans', sans-serif", outline: "none", boxSizing: "border-box" }}>
                {[1, 2, 3, 4, 5].map((n) => <option key={n} value={n}>{n} Guest{n > 1 ? "s" : ""}</option>)}
              </select>
            </div>
            <button onClick={handle} style={{ width: "100%", background: form.name && form.room ? C.gold : "#ccc", color: C.white, border: "none", borderRadius: 12, padding: "14px", fontSize: 14, fontWeight: 700, cursor: form.name && form.room ? "pointer" : "not-allowed" }}>
              ✓ Activate Guest Portal
            </button>
          </div>
        </div>
      </div>
    );
  };

  return (
    <div>
      {screen === "overview" && <Overview />}
      {screen === "rooms" && <Rooms />}
      {screen === "alerts" && <Alerts />}
      {screen === "orders" && <Orders />}
      {screen === "requests_admin" && <RequestsAdmin />}
      {screen === "announce" && <Announce />}
      {screen === "checkin" && <CheckIn />}
      <AdminNav />
    </div>
  );
}

// ─── ROOT ─────────────────────────────────────────────────────────────────────
export default function GuestifyApp() {
  const [mode, setMode] = useState("entry");
  const [guest, setGuest] = useState(null);
  const [admin, setAdmin] = useState(null);
  const [guestScreen, setGuestScreen] = useState("welcome");
  const [pulseShown, setPulseShown] = useState(false);

  // Shared live state
  const [rooms, setRooms] = useState(INITIAL_ROOMS);
  const [complaints, setComplaints] = useState([]);
  const [orders, setOrders] = useState([]);
  const [requests, setRequests] = useState([]);
  const [announcements, setAnnouncements] = useState([]);

  const guestLogin = (data) => { setGuest(data); setMode("guest"); setGuestScreen("welcome"); };
  const adminLogin = (user) => { setAdmin(user); setMode("admin"); };
  const guestLogout = () => { setGuest(null); setMode("entry"); setGuestScreen("welcome"); setPulseShown(false); };
  const adminLogout = () => { setAdmin(null); setMode("entry"); };
  const nav = (s) => setGuestScreen(s);

  return (
    <div style={{ maxWidth: 480, margin: "0 auto", minHeight: "100vh", fontFamily: "'DM Sans', sans-serif" }}>
      {mode === "entry" && <EntryScreen onGuest={() => setMode("guestLogin")} onAdmin={() => setMode("adminLogin")} />}
      {mode === "guestLogin" && <GuestLogin onLogin={guestLogin} onBack={() => setMode("entry")} />}
      {mode === "adminLogin" && <AdminLogin onLogin={adminLogin} onBack={() => setMode("entry")} />}

      {mode === "guest" && (
        <div style={{ paddingBottom: 64 }}>
          {guestScreen === "welcome" && <GuestWelcome guest={guest} onNav={nav} pulseShown={pulseShown} announcements={announcements} onLogout={guestLogout} />}
          {guestScreen === "menu" && <GuestMenu guest={guest} onNav={nav} onOrder={(o) => setOrders((p) => [...p, o])} />}
          {guestScreen === "requests" && <GuestRequests guest={guest} onNav={nav} onRequest={(r) => setRequests((p) => [...p, r])} />}
          {guestScreen === "info" && <GuestInfo onNav={nav} />}
          {guestScreen === "pulse" && (
            <GuestPulse guest={guest} onNav={nav} onDone={() => setPulseShown(true)}
              onComplaint={(c) => {
                setComplaints((p) => [...p, c]);
                setRooms((r) => r.map((x) => x.number === guest.room || x.number === guest.room.padStart(2, "0") ? { ...x, status: "complaint" } : x));
              }} />
          )}
          <GuestNav screen={guestScreen} onNav={nav} />
        </div>
      )}

      {mode === "admin" && (
        <AdminDashboard
          admin={admin}
          rooms={rooms} setRooms={setRooms}
          complaints={complaints} setComplaints={setComplaints}
          orders={orders} setOrders={setOrders}
          requests={requests} setRequests={setRequests}
          announcements={announcements} setAnnouncements={setAnnouncements}
          onLogout={adminLogout}
        />
      )}
    </div>
  );
}
