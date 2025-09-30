# Certificate-Generator

This repository provides a simple Python-based solution to generate certificates from a given **template DOCX file**.  
The template contains placeholders such as `{name}`, `{eventname}`, and `{date}`, which are replaced dynamically using participant data from a CSV file and event details provided in the script.  

Certificates are generated in both **DOCX** and **PDF** formats, and stored in separate folders for easy access.

---

## ✨ Features

- Automatically generate certificates for multiple participants from a CSV file.
- Generates certificates in **DOCX** and **PDF** formats.
- Uses a customizable DOCX template with placeholders:
  - `{name}` → Participant Name  
  - `{eventname}` → Event Name  
  - `{date}` → Event Date
- Font size and text style for **attendee names** are customizable.
- Works on **Windows**, **Mac**, and **Linux**.

---

## 📂 Project Structure

```
Certificate-Generator/
│
├── certificate_generator.py     # Main Python script
├── participants.csv             # List of participants (CSV input)
├── template
│     └── template.docx          # Certificate template with placeholders
├── requirements.txt             # Python dependencies
│
├── Certificates-DOCX/           # Generated certificates in DOCX format (Automatically )
├── Certificates-PDF/            # Generated certificates in PDF format (Automatically )
│
└── README.md                    # Project documentation
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/amityadav-72/Certificate-Generator
cd Certificate-Generator
```

### 2️⃣ Install Dependencies

- **For Windows:**
  ```bash
  pip install -r requirements.txt
  ```

- **For Mac/Linux:**
  ```bash
  pip3 install -r requirements.txt
  ```

---

## 📝 Customization and Certificate Generation

### Step 1: Add Participants
- Open **`participants.csv`** in the project directory.
- Replace the sample entries with the names of your attendees.
- Keep the header as:
  ```
  Name
  ```
- Enter participant names starting from the **second row**.
- Example:
  ```
  Name
  Amit Kumar
  Amit
  John Doe
  ```
- Save the file.

---

### Step 2: Modify Event Details


<br>
<img width="1150" alt="Step 2" src="https://github.com/amityadav-72/Certificate-Generator/blob/main/assests/Event%20Name%26Date.png">

</br>


- Open **`certificate_generator.py`** in a code editor.
- Update the following variables (line numbers are indicative, may vary depending on code):
  
  ```python
  EVENT_NAME = "Your_Event_Name"    # Replace with your event name
  EVENT_DATE = "Your_Event_Date"    # Replace with your event date
  FONT_NAME  = "Script MT Bold"     # Replace with the font name for attendee name
  FONT_SIZE  = 48                   # Adjust the font size
  ```
- Save the changes.

---

### Step 3: Run the Script

- **For Windows:**
  ```bash
  python certificate_generator.py
  ```

- **For Mac/Linux:**
  ```bash
  python3 certificate_generator.py
  ```

---

### Step 4: Get Certificates

After running the script:

- **DOCX Certificates:**  
  Located inside the folder:
  ```
  Certificates-DOCX/
  ```

- **PDF Certificates:**  
  Located inside the folder:
  ```
  Certificates-PDF/
  ```

Each file will be named after the participant, e.g.,  
```
Amit Kumar.docx  
Amit Kumar.pdf
```

---

## 📌 Notes

- Ensure that your **template.docx** contains placeholders exactly as:
  - `{name}` for participant name
  - `{eventname}` for the event name
  - `{date}` for the event date
- Text style (font and size) applies only to **participant names**, making it customizable.
- Make sure **Microsoft Word (or LibreOffice)** and **Python-docx** support the template format.

---

## 🎉 Example Workflow

1. Add participants in `participants.csv`.
2. Update event name and date in `certificate_generator.py`.
3. Place placeholders (`{name}`, `{eventname}`, `{date}`) in your template.docx.
4. Run the script.
5. Collect your certificates in **DOCX** and **PDF** folders.
6. Share with your participants!

---

## 🙌 Acknowledgments

Thanks for using **Certificate-Generator**!  
If you like this project, don’t forget to ⭐ star the repo.


## 🚀 Future Scope

- Support for **image-based certificates** as template input and output.
- Directly **send certificates to attendees via email** using their provided email addresses.
- Add more placeholders like `{college}`, `{rank}`, `{designation}`.
- Support for multiple template designs.
- Export all certificates as `.zip` for easy sharing.
- GUI / Web interface for non-technical users.

## 🧑‍💻 Creator

**Amit Kumar Yadav**  

- 🌐 [LinkedIn](https://www.linkedin.com/in/amityadav72)  
- 💻 [GitHub](https://github.com/amityadav-72)  

