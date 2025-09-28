# Certificate-Generator

This repo simply use a template certificate docx file and generates certificates in
both docx and pdf.

---

## Features

- Automatically generate certificates from a list of participants.
- Output certificates in both DOCX and PDF formats.
- Easy to customize with your event name, date, and text style.

---

##  For Windows and Mac users.


## Run these commands in your terminal

```
git clone https://github.com/amityadav-72/Certificate-Generator
cd Certificate-Generator
```

## Customization and Generation

### Step 1 : Adding list of participants


- Open the `participants.csv` file located in the project directory.  
- Replace the sample entries with the names of your attendees or beneficiaries.  
- Ensure that the header **"Name"** remains unchanged at the top of the file.  
- Insert participant names starting from the second row onward.
- Save the changes.

  

### Step 2 : Modifying your event details

<br>
<img width="1150" alt="Step 2" src="https://github.com/amityadav-72/Certificate-Generator/blob/main/assests/Event%20Name%26Date.png">


- Open the file `certificate_generator.py`
- Move to line 13 and Write name of the "Event" instead of "Your_Event_Name"
- Move to line 14 and Write "Event Date" instead of "Your_Event_Date"
- Move to line 16 and Write "Script Name" in which you want name should appear.
- Move to line 17 and Write size of the text.
- Save the changes.

### Step 3 : Open Terminal

### ```For Mac Users```

```
pip3 install -r requirements.txt
python3 main_certificate.py
```

### ```For Windows Users```

```
pip install -r requirements.txt
python certificate_generator.py
```

### Step 4 : Certificates

- Look for Certificates-PDF Folder in "Certificate-Generator" folder in your pc having the certificate in pdf format.
- Look for Certificates-DOCX Folder in "Certificate-Generator" folder in your pc having the certificate in docx format
- Extract the certificates and share with your participants


## Well Done!!! You Did It.
## Thank You
