# CCNA-Routers
**CCNA Lab Practice: Step-by-Step Documentation**

---

### **Device: R1 (Cisco Router)**

#### **1. Enter Privileged EXEC Mode**
```
R1>enable
Password: (entered)
```

#### **2. Enter Global Configuration Mode**
```
R1#configure terminal
Enter configuration commands, one per line. End with CNTL/Z.
```

#### **3. Set Enable Password**
```
R1(config)#enable password ccna
```

#### **4. Configure Hostname**
```
R1(config)#hostname R1
```

#### **5. View Current Configuration (Attempted Incorrectly)**
```
R1(config)#sh run
% Invalid input detected at '^' marker.

R1(config)#sho run
% Invalid input detected at '^' marker.
```
**Fix:** Exit configuration mode before using `show run`:
```
R1(config)#end
R1#show run
```

#### **6. Attempt to Encrypt Passwords (Initially Mistyped)**
```
R1(config)#service pass
% Incomplete command

R1(config)#service password encryption
% Invalid input detected at '^' marker.
```
**Fix:** Ensure correct command spelling:
```
R1(config)#service password-encryption
```

#### **7. Verify Configuration**
```
R1#show run
```
This shows current configuration including version, hostname, services, and password settings.

#### **8. Save Configuration to NVRAM**
```
R1#write
Building configuration...
[OK]
```

---



