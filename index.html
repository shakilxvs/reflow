import { useState, useEffect, useRef } from "react";

const ACCENT = "#F5A623";
const DARK = "#0D0D0D";
const CARD = "#161616";
const BORDER = "#2A2A2A";
const TEXT = "#E8E8E8";
const MUTED = "#888";

const styles = {
  root: {
    minHeight: "100vh",
    background: DARK,
    fontFamily: "'Georgia', 'Times New Roman', serif",
    color: TEXT,
    padding: "0",
    margin: "0",
  },
  header: {
    borderBottom: `1px solid ${BORDER}`,
    padding: "28px 40px 24px",
    display: "flex",
    alignItems: "center",
    gap: "16px",
    background: "#111",
  },
  logoMark: {
    width: 40,
    height: 40,
    background: ACCENT,
    borderRadius: 4,
    display: "flex",
    alignItems: "center",
    justifyContent: "center",
    fontSize: 20,
    flexShrink: 0,
  },
  headerTitle: {
    fontSize: 20,
    fontWeight: "bold",
    letterSpacing: "0.02em",
    color: "#fff",
    margin: 0,
  },
  headerSub: {
    fontSize: 13,
    color: MUTED,
    marginTop: 2,
    fontFamily: "system-ui, sans-serif",
  },
  main: {
    maxWidth: 780,
    margin: "0 auto",
    padding: "40px 24px",
  },
  sectionTitle: {
    fontFamily: "system-ui, sans-serif",
    fontSize: 11,
    fontWeight: 600,
    letterSpacing: "0.12em",
    textTransform: "uppercase",
    color: ACCENT,
    marginBottom: 16,
  },
  card: {
    background: CARD,
    border: `1px solid ${BORDER}`,
    borderRadius: 8,
    padding: "28px 28px",
    marginBottom: 20,
  },
  label: {
    display: "block",
    fontFamily: "system-ui, sans-serif",
    fontSize: 12,
    fontWeight: 600,
    letterSpacing: "0.08em",
    textTransform: "uppercase",
    color: MUTED,
    marginBottom: 8,
  },
  input: {
    width: "100%",
    background: "#1E1E1E",
    border: `1px solid ${BORDER}`,
    borderRadius: 6,
    color: TEXT,
    padding: "12px 14px",
    fontSize: 15,
    fontFamily: "'Georgia', serif",
    outline: "none",
    boxSizing: "border-box",
    transition: "border-color 0.2s",
  },
  textarea: {
    width: "100%",
    background: "#1E1E1E",
    border: `1px solid ${BORDER}`,
    borderRadius: 6,
    color: TEXT,
    padding: "12px 14px",
    fontSize: 15,
    fontFamily: "'Georgia', serif",
    outline: "none",
    boxSizing: "border-box",
    resize: "vertical",
    minHeight: 100,
    transition: "border-color 0.2s",
  },
  row: {
    display: "grid",
    gridTemplateColumns: "1fr 1fr",
    gap: 16,
    marginBottom: 18,
  },
  field: { marginBottom: 18 },
  select: {
    width: "100%",
    background: "#1E1E1E",
    border: `1px solid ${BORDER}`,
    borderRadius: 6,
    color: TEXT,
    padding: "12px 14px",
    fontSize: 14,
    fontFamily: "system-ui, sans-serif",
    outline: "none",
    boxSizing: "border-box",
    cursor: "pointer",
  },
  btn: {
    display: "flex",
    alignItems: "center",
    justifyContent: "center",
    gap: 10,
    width: "100%",
    padding: "16px",
    background: ACCENT,
    color: "#000",
    fontFamily: "system-ui, sans-serif",
    fontSize: 15,
    fontWeight: 700,
    letterSpacing: "0.04em",
    border: "none",
    borderRadius: 8,
    cursor: "pointer",
    transition: "opacity 0.2s, transform 0.1s",
    marginTop: 4,
  },
  btnDisabled: {
    opacity: 0.5,
    cursor: "not-allowed",
  },
  statusBox: {
    background: "#111",
    border: `1px solid ${BORDER}`,
    borderRadius: 8,
    padding: "20px 24px",
    marginTop: 20,
    fontFamily: "system-ui, sans-serif",
    fontSize: 14,
  },
  statusRow: {
    display: "flex",
    alignItems: "center",
    gap: 10,
    color: TEXT,
  },
  spinner: {
    width: 18,
    height: 18,
    border: `2px solid ${BORDER}`,
    borderTop: `2px solid ${ACCENT}`,
    borderRadius: "50%",
    animation: "spin 0.8s linear infinite",
    flexShrink: 0,
  },
  successIcon: {
    width: 20,
    height: 20,
    background: "#22C55E",
    borderRadius: "50%",
    display: "flex",
    alignItems: "center",
    justifyContent: "center",
    fontSize: 12,
    color: "#fff",
    flexShrink: 0,
  },
  errorIcon: {
    width: 20,
    height: 20,
    background: "#EF4444",
    borderRadius: "50%",
    display: "flex",
    alignItems: "center",
    justifyContent: "center",
    fontSize: 12,
    color: "#fff",
    flexShrink: 0,
  },
  downloadBtn: {
    display: "flex",
    alignItems: "center",
    gap: 8,
    padding: "12px 20px",
    background: "#22C55E",
    color: "#fff",
    fontFamily: "system-ui, sans-serif",
    fontSize: 14,
    fontWeight: 700,
    border: "none",
    borderRadius: 6,
    cursor: "pointer",
    marginTop: 14,
    transition: "opacity 0.2s",
  },
  previewBox: {
    background: "#1A1A1A",
    border: `1px solid ${BORDER}`,
    borderRadius: 8,
    padding: "24px",
    marginTop: 14,
    fontFamily: "system-ui, sans-serif",
    fontSize: 13,
    color: "#CCC",
    lineHeight: 1.7,
    maxHeight: 320,
    overflowY: "auto",
    whiteSpace: "pre-wrap",
  },
  chipRow: {
    display: "flex",
    flexWrap: "wrap",
    gap: 8,
    marginTop: 10,
  },
  chip: {
    padding: "6px 12px",
    borderRadius: 20,
    border: `1px solid ${BORDER}`,
    fontFamily: "system-ui, sans-serif",
    fontSize: 12,
    cursor: "pointer",
    transition: "all 0.15s",
    userSelect: "none",
  },
};

const TONES = ["Professional", "Friendly", "Formal", "Innovative", "Concise"];
const DOC_TYPES = [
  "Company Profile",
  "Product Brochure",
  "Service Proposal",
  "Annual Report Summary",
  "Business Plan",
  "Project Overview",
  "Marketing One-Pager",
];

function loadjsPDF() {
  return new Promise((resolve, reject) => {
    if (window.jspdf) return resolve(window.jspdf.jsPDF);
    const s = document.createElement("script");
    s.src = "https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js";
    s.onload = () => resolve(window.jspdf.jsPDF);
    s.onerror = reject;
    document.head.appendChild(s);
  });
}

function wrapText(text, maxWidth, fontSize) {
  // Approximate char width = fontSize * 0.5
  const charsPerLine = Math.floor(maxWidth / (fontSize * 0.52));
  const words = text.split(" ");
  const lines = [];
  let current = "";
  for (const word of words) {
    if ((current + " " + word).trim().length <= charsPerLine) {
      current = (current + " " + word).trim();
    } else {
      if (current) lines.push(current);
      current = word;
    }
  }
  if (current) lines.push(current);
  return lines;
}

async function generatePDF(data) {
  const jsPDF = await loadjsPDF();
  const doc = new jsPDF({ orientation: "portrait", unit: "mm", format: "a4" });
  const W = 210;
  const H = 297;
  const margin = 20;
  const contentW = W - margin * 2;

  // ── COVER PAGE ──────────────────────────────────────────
  doc.setFillColor(13, 13, 13);
  doc.rect(0, 0, W, H, "F");

  // Gold accent bar
  doc.setFillColor(245, 166, 35);
  doc.rect(0, 0, 6, H, "F");

  // Company name
  doc.setTextColor(245, 166, 35);
  doc.setFontSize(28);
  doc.setFont("helvetica", "bold");
  doc.text(data.companyName || "Your Company", margin + 8, 60);

  // Tagline
  if (data.tagline) {
    doc.setFontSize(12);
    doc.setTextColor(180, 180, 180);
    doc.setFont("helvetica", "italic");
    doc.text(data.tagline, margin + 8, 72);
  }

  // Document type badge
  doc.setFillColor(245, 166, 35);
  doc.setTextColor(0, 0, 0);
  doc.setFontSize(10);
  doc.setFont("helvetica", "bold");
  const badge = data.docType.toUpperCase();
  const badgeW = doc.getTextWidth(badge) + 16;
  doc.roundedRect(margin + 8, 82, badgeW, 10, 2, 2, "F");
  doc.text(badge, margin + 16, 89.5);

  // Divider
  doc.setDrawColor(245, 166, 35);
  doc.setLineWidth(0.3);
  doc.line(margin + 8, 100, W - margin, 100);

  // Topic
  doc.setFontSize(18);
  doc.setTextColor(232, 232, 232);
  doc.setFont("helvetica", "bold");
  const topicLines = doc.splitTextToSize(data.topic, contentW - 8);
  doc.text(topicLines, margin + 8, 114);

  // Date & website
  doc.setFontSize(10);
  doc.setTextColor(100, 100, 100);
  doc.setFont("helvetica", "normal");
  const dateStr = new Date().toLocaleDateString("en-US", { year: "numeric", month: "long", day: "numeric" });
  doc.text(dateStr, margin + 8, H - 30);
  if (data.website) doc.text(data.website, margin + 8, H - 24);
  if (data.email) doc.text(data.email, margin + 8, H - 18);

  // ── CONTENT PAGES ────────────────────────────────────────
  const sections = parseSections(data.generatedContent);

  for (const section of sections) {
    doc.addPage();
    doc.setFillColor(250, 250, 250);
    doc.rect(0, 0, W, H, "F");

    // Header stripe
    doc.setFillColor(13, 13, 13);
    doc.rect(0, 0, W, 18, "F");
    doc.setFillColor(245, 166, 35);
    doc.rect(0, 0, 6, 18, "F");

    doc.setFontSize(9);
    doc.setTextColor(200, 200, 200);
    doc.setFont("helvetica", "normal");
    doc.text((data.companyName || "").toUpperCase(), margin + 4, 11.5);
    doc.text(data.docType.toUpperCase(), W - margin, 11.5, { align: "right" });

    let y = 34;

    // Section heading
    doc.setFillColor(245, 166, 35);
    doc.rect(margin, y - 6, 3, 14, "F");
    doc.setFontSize(16);
    doc.setFont("helvetica", "bold");
    doc.setTextColor(20, 20, 20);
    doc.text(section.title, margin + 8, y + 3);
    y += 18;

    // Section body
    doc.setFontSize(11);
    doc.setFont("helvetica", "normal");
    doc.setTextColor(50, 50, 50);

    const bodyLines = doc.splitTextToSize(section.body, contentW);
    for (const line of bodyLines) {
      if (y > H - 26) {
        // Footer
        addFooter(doc, W, H, margin, data.companyName);
        doc.addPage();
        doc.setFillColor(250, 250, 250);
        doc.rect(0, 0, W, H, "F");
        y = 26;
        doc.setFontSize(11);
        doc.setFont("helvetica", "normal");
        doc.setTextColor(50, 50, 50);
      }
      doc.text(line, margin, y);
      y += 7;
    }

    addFooter(doc, W, H, margin, data.companyName);
  }

  // ── BACK COVER ───────────────────────────────────────────
  doc.addPage();
  doc.setFillColor(13, 13, 13);
  doc.rect(0, 0, W, H, "F");
  doc.setFillColor(245, 166, 35);
  doc.rect(0, 0, 6, H, "F");

  doc.setFontSize(22);
  doc.setFont("helvetica", "bold");
  doc.setTextColor(232, 232, 232);
  doc.text("Thank You", margin + 8, H / 2 - 10);

  doc.setFontSize(12);
  doc.setFont("helvetica", "normal");
  doc.setTextColor(136, 136, 136);
  doc.text(data.companyName || "", margin + 8, H / 2 + 4);
  if (data.email) doc.text(data.email, margin + 8, H / 2 + 14);
  if (data.website) doc.text(data.website, margin + 8, H / 2 + 22);

  const fname = `${(data.companyName || "document").replace(/\s+/g, "_")}_${data.docType.replace(/\s+/g, "_")}.pdf`;
  doc.save(fname);
}

function addFooter(doc, W, H, margin, companyName) {
  doc.setDrawColor(210, 210, 210);
  doc.setLineWidth(0.3);
  doc.line(margin, H - 16, W - margin, H - 16);
  doc.setFontSize(8);
  doc.setTextColor(160, 160, 160);
  doc.setFont("helvetica", "normal");
  doc.text(companyName || "", margin, H - 10);
  doc.text("Confidential", W - margin, H - 10, { align: "right" });
}

function parseSections(content) {
  if (!content) return [];
  const lines = content.split("\n");
  const sections = [];
  let current = null;
  for (const line of lines) {
    const trimmed = line.trim();
    if (!trimmed) continue;
    if (/^#{1,3}\s/.test(trimmed) || /^\d+\.\s+[A-Z]/.test(trimmed) || /^[A-Z][A-Z\s]{4,}$/.test(trimmed)) {
      if (current) sections.push(current);
      current = { title: trimmed.replace(/^#+\s*/, "").replace(/^\d+\.\s*/, ""), body: "" };
    } else {
      if (!current) current = { title: "Overview", body: "" };
      current.body += (current.body ? "\n" : "") + trimmed;
    }
  }
  if (current) sections.push(current);
  return sections.filter((s) => s.body.length > 10);
}

export default function App() {
  const [form, setForm] = useState({
    companyName: "",
    tagline: "",
    email: "",
    website: "",
    topic: "",
    details: "",
    docType: "Company Profile",
    tone: "Professional",
    pages: "3-4",
  });
  const [status, setStatus] = useState("idle"); // idle | loading | done | error
  const [statusMsg, setStatusMsg] = useState("");
  const [generatedContent, setGeneratedContent] = useState("");
  const [selectedTone, setSelectedTone] = useState("Professional");

  const set = (k) => (e) => setForm((f) => ({ ...f, [k]: e.target.value }));

  async function handleGenerate() {
    if (!form.companyName || !form.topic) {
      setStatus("error");
      setStatusMsg("Please fill in Company Name and Topic at minimum.");
      return;
    }
    setStatus("loading");
    setStatusMsg("Generating content with AI...");
    setGeneratedContent("");

    try {
      const prompt = `You are a professional business document writer. 
Create a detailed ${form.docType} document for the following company and topic.

Company: ${form.companyName}
${form.tagline ? `Tagline: ${form.tagline}` : ""}
Topic: ${form.topic}
Tone: ${selectedTone}
${form.details ? `Additional Details: ${form.details}` : ""}
Target length: ${form.pages} pages when formatted as a PDF

Write the full document content with clear section headings (use ## for headings).
Each section should have substantial, informative paragraphs.
Make it professional, compelling, and ready to present to clients or stakeholders.
Include 4-6 well-developed sections.
Do NOT include any meta-commentary, just write the document content directly.`;

      const response = await fetch("https://api.anthropic.com/v1/messages", {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({
          model: "claude-sonnet-4-20250514",
          max_tokens: 1800,
          messages: [{ role: "user", content: prompt }],
        }),
      });

      const data = await response.json();
      if (!response.ok) throw new Error(data.error?.message || "API error");

      const content = data.content?.[0]?.text || "";
      setGeneratedContent(content);
      setStatus("done");
      setStatusMsg("Content generated! Ready to download your PDF.");
    } catch (err) {
      setStatus("error");
      setStatusMsg("Error: " + (err.message || "Something went wrong."));
    }
  }

  async function handleDownload() {
    setStatusMsg("Building your PDF...");
    try {
      await generatePDF({ ...form, tone: selectedTone, generatedContent });
      setStatusMsg("PDF downloaded successfully! ✓");
    } catch (err) {
      setStatusMsg("PDF error: " + err.message);
    }
  }

  const inputFocus = (e) => (e.target.style.borderColor = ACCENT);
  const inputBlur = (e) => (e.target.style.borderColor = BORDER);

  return (
    <div style={styles.root}>
      <style>{`
        @keyframes spin { to { transform: rotate(360deg); } }
        input::placeholder, textarea::placeholder { color: #444; }
        * { box-sizing: border-box; }
        ::-webkit-scrollbar { width: 6px; }
        ::-webkit-scrollbar-track { background: #111; }
        ::-webkit-scrollbar-thumb { background: #333; border-radius: 3px; }
      `}</style>

      <div style={styles.header}>
        <div style={styles.logoMark}>📄</div>
        <div>
          <div style={styles.headerTitle}>Smart PDF Generator</div>
          <div style={styles.headerSub}>AI-powered professional documents for your business</div>
        </div>
      </div>

      <div style={styles.main}>
        {/* Company Details */}
        <div style={styles.sectionTitle}>Company Details</div>
        <div style={styles.card}>
          <div style={styles.row}>
            <div style={styles.field}>
              <label style={styles.label}>Company Name *</label>
              <input style={styles.input} value={form.companyName} onChange={set("companyName")}
                placeholder="Acme Corporation" onFocus={inputFocus} onBlur={inputBlur} />
            </div>
            <div style={styles.field}>
              <label style={styles.label}>Tagline / Slogan</label>
              <input style={styles.input} value={form.tagline} onChange={set("tagline")}
                placeholder="Innovation at its finest" onFocus={inputFocus} onBlur={inputBlur} />
            </div>
          </div>
          <div style={styles.row}>
            <div style={styles.field}>
              <label style={styles.label}>Email</label>
              <input style={styles.input} value={form.email} onChange={set("email")}
                placeholder="hello@company.com" onFocus={inputFocus} onBlur={inputBlur} />
            </div>
            <div style={styles.field}>
              <label style={styles.label}>Website</label>
              <input style={styles.input} value={form.website} onChange={set("website")}
                placeholder="www.company.com" onFocus={inputFocus} onBlur={inputBlur} />
            </div>
          </div>
        </div>

        {/* Document Settings */}
        <div style={styles.sectionTitle}>Document Settings</div>
        <div style={styles.card}>
          <div style={styles.row}>
            <div style={styles.field}>
              <label style={styles.label}>Document Type</label>
              <select style={styles.select} value={form.docType} onChange={set("docType")}>
                {DOC_TYPES.map((t) => <option key={t}>{t}</option>)}
              </select>
            </div>
            <div style={styles.field}>
              <label style={styles.label}>Page Length</label>
              <select style={styles.select} value={form.pages} onChange={set("pages")}>
                <option>2-3</option>
                <option>3-4</option>
                <option>4-6</option>
                <option>6-8</option>
              </select>
            </div>
          </div>

          <div style={styles.field}>
            <label style={styles.label}>Topic / Main Subject *</label>
            <input style={styles.input} value={form.topic} onChange={set("topic")}
              placeholder="e.g. Our new AI-powered logistics solution for e-commerce"
              onFocus={inputFocus} onBlur={inputBlur} />
          </div>

          <div style={styles.field}>
            <label style={styles.label}>Additional Details</label>
            <textarea style={styles.textarea} value={form.details} onChange={set("details")}
              placeholder="Add any specific points, data, or sections you'd like included..."
              onFocus={inputFocus} onBlur={inputBlur} />
          </div>

          <div style={styles.field}>
            <label style={styles.label}>Tone</label>
            <div style={styles.chipRow}>
              {TONES.map((t) => (
                <div key={t} style={{
                  ...styles.chip,
                  background: selectedTone === t ? ACCENT : "transparent",
                  color: selectedTone === t ? "#000" : TEXT,
                  borderColor: selectedTone === t ? ACCENT : BORDER,
                  fontFamily: "system-ui, sans-serif",
                  fontWeight: selectedTone === t ? 700 : 400,
                }} onClick={() => setSelectedTone(t)}>{t}</div>
              ))}
            </div>
          </div>
        </div>

        {/* Generate Button */}
        <button style={{ ...styles.btn, ...(status === "loading" ? styles.btnDisabled : {}) }}
          onClick={handleGenerate} disabled={status === "loading"}>
          {status === "loading" ? (
            <><span style={styles.spinner} /> Generating with AI...</>
          ) : (
            <><span>✦</span> Generate Smart PDF</>
          )}
        </button>

        {/* Status */}
        {status !== "idle" && (
          <div style={styles.statusBox}>
            <div style={styles.statusRow}>
              {status === "loading" && <span style={styles.spinner} />}
              {status === "done" && <span style={styles.successIcon}>✓</span>}
              {status === "error" && <span style={styles.errorIcon}>✕</span>}
              <span style={{ fontFamily: "system-ui, sans-serif" }}>{statusMsg}</span>
            </div>

            {status === "done" && generatedContent && (
              <>
                <div style={styles.previewBox}>{generatedContent}</div>
                <button style={styles.downloadBtn} onClick={handleDownload}>
                  ⬇ Download PDF
                </button>
              </>
            )}
          </div>
        )}
      </div>
    </div>
  );
}
