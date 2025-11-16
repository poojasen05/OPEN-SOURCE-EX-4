# OPEN-SOURCE-EX-4

## NAME: POOJA S
## REGNO: 212223040146
## DEPT: CSE

## AIM:
To create a shared directory for the admin group, set proper ownership and permissions, and verify group access in RHEL.

## PROCEDURE:

### **STEP 1:**  
Create a shared directory  
```bash
sudo mkdir -p /common/admin
```

### **STEP 2:**  
Change ownership to root and admin group  
```bash
sudo chown root:admin /common/admin
```

### **STEP 3:**  
Set group ID and permissions  
```bash
sudo chmod 2770 /common/admin
```

### **STEP 4:**  
Verify directory permissions  
```bash
ls -ld /common/admin
```

### **STEP 5:**  
Expected permission output  
```bash
drwxrws--- 2 root admin ... /common/admin
```

### **STEP 6:**  
Check user group membership  
```bash
groups harry
```

## OUTPUT:
![Screenshot](https://github.com/user-attachments/assets/bfe57e75-6a45-49c3-a248-d5283391f22b)

---


## RESULT:
The shared admin directory was successfully created with correct ownership and permissions, and group access was verified in the Red Hat Lab environment.
