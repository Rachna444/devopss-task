# Task: Hub-and-Spoke VPC Architecture

## Objective
Design a Hub-and-Spoke VPC architecture where both Spoke VPCs can communicate with the Hub VPC but remain isolated from each other using route tables.

---

## Steps

### 1. Create VPCs
- Created 3 VPCs:
  - Hub VPC → `10.0.0.0/16`
  - Spoke1 VPC → `10.1.0.0/16`
  - Spoke2 VPC → `10.2.0.0/16`  
- Ensured CIDR ranges are non-overlapping  

---

### 2. Configure VPC Peering
- Created peering connections:
  - Hub ↔ Spoke1  
  - Hub ↔ Spoke2  
- Accepted peering requests  

---

### 3. Update Route Tables

#### Hub VPC
- Added routes:
  - `10.1.0.0/16` → Spoke1 peering  
  - `10.2.0.0/16` → Spoke2 peering  

#### Spoke1 VPC
- Added route:
  - `10.0.0.0/16` → Hub peering  

#### Spoke2 VPC
- Added route:
  - `10.0.0.0/16` → Hub peering  

---

### 4. Traffic Control
- No route added between Spoke1 and Spoke2  
- Ensured isolation using route tables  

---

## Output

- Hub VPC connected to both Spoke VPCs  
- Spoke1 → Hub communication successful  
- Spoke2 → Hub communication successful  
- Spoke1 and Spoke2 isolated (no direct communication)  
- Architecture successfully controlled via route tables  

---

## Screenshots

![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)