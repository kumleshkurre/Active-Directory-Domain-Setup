# Active Directory Domain Services (AD DS) Setup

## 📌 Objective
To configure Windows Server as a Domain Controller using Active Directory Domain Services (AD DS) and manage domain users and organizational units.

---

## 🛠 Tools & Technologies Used
- Windows Server
- Active Directory Domain Services (AD DS)
- Active Directory Users and Computers

## 🌐 Windows Server IP Address Configuration

### Objective
To configure a static IPv4 address on Windows Server before installing Active Directory Domain Services.

---

### Steps Performed
1. Open **Server Manager**
2. Click on **Local Server**
3. Click on **IPv4** (Network settings)
4. Right-click on the active **Network Adapter**
5. Select **Properties**
6. Choose **Internet Protocol Version 4 (TCP/IPv4)**
7. Click **Properties**
8. Assign a static IP address:
9. Click **OK** and **Close**

---

### Outcome
- Successfully configured a static IP address
- Ensured stable network connectivity for Domain Controller setup

---

### Note
Static IP configuration is required for proper Active Directory and DNS functionality.

---

## ⚙️ Configuration Details
- Domain Type: New Forest
- Root Domain Name: kurrecomputers.local
- Server Role: Domain Controller

---

## 🚀 Step-by-Step Implementation

### 1️⃣ Install Active Directory Domain Services
- Open **Server Manager**
- Click **Add Roles and Features**
- Select **Role-based or feature-based installation**
- Choose **Active Directory Domain Services**
- Add required features
- Click **Next** and **Install**
- Close after successful installation

---

### 2️⃣ Promote Server to Domain Controller
- Click the **Flag icon** in Server Manager
- Select **Promote this server to a domain controller**
- Choose **Add a new forest**
- Enter root domain name:

- Set DSRM password (hidden for security)
- Click **Next** (5 times)
- Click **Install**
- Server restarts automatically

---

### 3️⃣ Create Organizational Unit (OU)
- Open **Active Directory Users and Computers**
- Right-click on domain **kurrecomputers.local**
- Select **New → Organizational Unit**
- Name:


---

### 4️⃣ Create Domain User
- Go to **kurrecomputers.local**
- Right-click → **New → User**
- Enter user details
- Set password and permissions
- Finish

---

### 5️⃣ Move User to Organizational Unit
- Right-click on user (e.g., Kumlesh Kurre)
- Click **Move**
- Select **OU: Raipur**
- Click **OK**

---

## ✅ Outcome
- Successfully installed and configured Active Directory Domain Services
- Created a new domain and forest
- Managed domain users and organizational units
- Performed user movement between OUs

---

## 📚 Skills Gained
- Windows Server Administration
- Active Directory Domain Services
- User and OU Management
- Domain Controller Configuration

---

## 🔐 Security Note
Passwords and sensitive credentials are hidden to maintain security best practices.

---

## 📎 Author
**Kumlesh Kurre**  
Aspiring IT Support / Network Engineer
