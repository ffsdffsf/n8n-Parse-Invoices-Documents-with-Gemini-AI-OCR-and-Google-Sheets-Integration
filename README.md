# n8n-Parse-Invoices-Documents-with-Gemini-AI-OCR-and-Google-Sheets-Integration

2. **Connect Integrations**:  
- Google Sheets (OAuth2)  
- Google Gemini (PaLM API Key) for parsing  
3. **Deploy Webhook** endpoint at: `/uploadDoc`  
4. **Test** with sample uploads (PDFs, images, CSVs).  
5. **Map Fields** → Ensure column mappings in the *Invoice Data* node.  

---

## ✅ Requirements

| Tool            | Purpose                          |
|-----------------|----------------------------------|
| **n8n**         | Workflow automation framework    |
| **Google Sheets** | Store structured output         |
| **Tesseract OCR** | Extract text from scanned images |
| **Google Gemini** | Natural language parsing & JSON output |

---

## 🎨 How to Customize
- Add extraction for **line items** using structured prompts.  
- Modify prompt for **sensor readings, log events, or custom keys**.  
- Extend support for **XLSX or DOCX files**.  
- Add **Slack/Email notifications** on success/failure.  
- Swap **Gemini** with **OpenAI or Hugging Face** models.  

---

## ➕ Add-ons
- Save uploaded files to **Google Drive or AWS S3**.  
- Add authentication for **secure uploads**.  
- Use **charting/dashboard nodes** to visualize extracted data.  
- Integrate with **billing/accounting software**.  

---

## 📌 Use Case Examples

| Scenario              | What Happens                                      |
|-----------------------|---------------------------------------------------|
| Invoice Upload (PDF)  | Extracts totals, customer, tax data into Sheets    |
| Scanned Receipt (Image) | OCR + LLM extracts structured values              |
| Log File (CSV)        | Parses and logs entries into Google Sheets         |

---

## 🛠️ Common Troubleshooting

| Issue                        | Possible Cause                | Solution                                    |
|------------------------------|-------------------------------|--------------------------------------------|
| Webhook not triggered        | Wrong URL or method           | Use correct `POST /uploadDoc` endpoint      |
| Text is blank                | OCR failed                    | Check image quality or Tesseract config     |
| Gemini not returning JSON    | Prompt formatting issue       | Ensure prompt ends with valid JSON schema   |
| Sheet not updated            | Wrong Sheet ID or tab name    | Double-check credentials & sheet details    |

---

## 🤝 Need Help?
Want to:  
- Fine-tune **Gemini prompts** for better accuracy?  
- Extract **full tables or multi-page invoices**?  
- Convert **PDFs to JSON lines** for advanced workflows?  

👉 The automation team at **WeblineIndia** can help you extend this into a **full document automation pipeline**.  

---

