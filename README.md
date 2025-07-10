## 🏡 ServiceNow Family Expenses Tracker

A custom ServiceNow application designed to help manage and track family expenses using native ServiceNow features such as tables, forms, business rules, and scheduled jobs.

---

### 📦 Project Contents

| Folder/File      | Description                                             |
| ---------------- | ------------------------------------------------------- |
| `update_sets/`   | Exported update sets (`.xml`) for import into instances |
| `scoped_app/`    | XML records from a scoped app (if used)                 |
| `scripts/`       | Custom scripts (for reference or reuse)                 |
| `documentation/` | Design and functional documentation                     |

---

### ✅ Features

* Custom table: `Family Expenses [x_family_expenses.expense]`
* UI Form for entering expenses
* Categories: Food, Utilities, Transport, etc.
* Scripted Business Rules to auto-tag and summarize
* Scheduled job for monthly summary email
* Reports and dashboards for visualization

---

### 📥 Getting Started

#### Option 1: Import via Update Set

1. Go to your ServiceNow instance
2. Navigate to **System Update Sets → Retrieved Update Sets**
3. Click **Import Update Set from XML**
4. Upload the file from `update_sets/family_expenses_v1.xml`
5. Preview and **Commit** the update set

#### Option 2: Import Scoped App (if applicable)

1. Go to **System Applications → Studio**
2. Click **Import from Source Control** (if linked to GitHub) or import via `sys_app` XML file
3. Browse and open the app to verify

---

### 🧰 Tables Used

| Table Name                       | Purpose                      |
| -------------------------------- | ---------------------------- |
| `x_family_expenses.expense`      | Stores each family expense   |
| `x_family_expenses.category`     | Lookup table for categories  |
| `sys_email` (ServiceNow default) | Used for scheduled summaries |

---

### 🚀 Scripts & Logic

* **Business Rules**: Auto-categorize based on keywords
* **Script Includes**: Shared utilities for formatting totals
* **Scheduled Jobs**: Monthly spending summaries emailed
* **Reports**: Expense trends by category and time

---

### 💡 Future Ideas

* Mobile-friendly interface via ServiceNow Mobile Studio
* Family user portal for submitting receipts
* AI-based auto-categorization
* Integration with Google Sheets or bank APIs

---

### 📄 License

MIT License – open for learning and non-commercial use.

---

### 🙋‍♀️ Contributions & Feedback

Feel free to fork, customize, or open issues if you're extending this for your own needs or team. This project is meant as a reference for learning ServiceNow app development.

