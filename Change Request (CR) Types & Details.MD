# 🛠️ Change Request (CR) Types & Details

## 📌 Types of Changes (ITIL-based)

| Type             | Description                                      | Examples                                  |
|------------------|--------------------------------------------------|-------------------------------------------|
| **Standard**      | Low-risk, pre-approved, repeatable changes       | OS patches, printer installation          |
| **Normal**        | Risk-assessed and needs approval                 | Server upgrades, app deployment           |
| **Emergency**     | Urgent fixes, fast-tracked with minimal approval | Critical outage fix, zero-day patch       |

---

## 📝 Required Details in a Change Request

### ✅ Basic Info
- **Title**: Short and clear summary  
- **Requested By**: Name and contact  
- **Change ID**: Auto/manual ticket

---

### ✅ Description
- What is changing?
- Affected systems/services
- Type: Standard / Normal / Emergency

---

### ✅ Reason for Change
- Justification
- Compliance / performance / bug fix, etc.

---

### ✅ Impact Analysis
- Services/users affected  
- Expected downtime?  
- Business impact level  

---

### ✅ Risk Assessment
- Potential issues  
- Risk level (Low/Medium/High)  
- Mitigation plan  

---

### ✅ Implementation Plan
- Step-by-step actions  
- Responsible personnel/team  
- Scripts/tools to be used  

---

### ✅ Rollback Plan
- Revert strategy  
- Downtime for rollback  
- Tools to restore original state  

---

### ✅ Schedule
- Start date/time  
- End date/time  
- Estimated duration  

---

### ✅ Approvals
- Manager/CAB approval  
- Emergency contacts (if needed)  

---

### ✅ Post-Change Validation
- How success will be verified  
- Health checks  
- Sign-off owner  

---

### 📌 Example CR Summary

> **Title**: Apply Windows security patch  
> **Type**: Emergency  
> **Reason**: Microsoft zero-day exploit  
> **Impact**: 10 production servers, 10 min reboot  
> **Plan**: Patch via WSUS → reboot servers  
> **Rollback**: Uninstall + snapshot restore  
> **Validation**: Post-patch system health checks  
> **Approval**: IT Manager & Security Team  

---

> 🔗 *Maintained by [Manikanta Suru](https://github.com/manikanta-suru)*  
