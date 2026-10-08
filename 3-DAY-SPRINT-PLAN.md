# AWS SAA — 3 Day Sprint Plan (Sec 4–20 + 27)

**Day 1:** Thu 08 Oct 2026 · **Day 2:** Fri 09 Oct · **Day 3:** Sat 10 Oct
**Course:** Udemy - Ultimate AWS SAA 2025 (2.2025), local copy
**Scope:** Section 04–20 + Section 27 (full)

## Real numbers (`.vtt` subtitle file theke exact duration)

| | Value |
|---|---|
| Total lectures | **252** |
| Total video | **18h 58m** (1139 min) |
| Minus skip-list | **18h 44m** |
| @ 1.5x speed | **12h 29m** |
| + note/pause overhead (~35%) | **~16h 50m** |
| + 6 checkpoint exams + 1 final mock | **~+3h 30m** |
| **Realistic total** | **~20h → 3 dine ~7h/din** |

> Eta ekta hard sprint. 7h/din na dile 3 dine hobe na. Kom time thakle Day 3 er Sec 18/19/20 ke Day 4 e thelo — kintu Day 1 ta **kokhonoi** kat'be na, oita puro base.

---

## Section-wise exact time

| Sec | Topic | Lec | Time |
|-----|-------|-----|------|
| 04 | IAM & AWS CLI | 18 | 55m |
| 05 | EC2 Fundamentals | 16 | 1h 45m |
| 06 | EC2 - SAA Level | 8 | 33m |
| 07 | EC2 Instance Storage | 14 | 59m |
| 08 | ELB & ASG | 17 | 1h 34m |
| 09 | RDS + Aurora + ElastiCache | 13 | 1h 09m |
| 10 | Route 53 | 19 | 1h 22m |
| 11 | Classic Solutions Architecture | 7 | 44m |
| 12 | Amazon S3 Introduction | 13 | 48m |
| 13 | Advanced Amazon S3 | 8 | 30m |
| 14 | Amazon S3 Security | 14 | 49m |
| 15 | CloudFront & Global Accelerator | 8 | 35m |
| 16 | AWS Storage Extras | 10 | 40m |
| 17 | SQS, SNS, Kinesis, MQ | 16 | 1h 21m |
| 18 | ECS, Fargate, ECR, EKS | 13 | 54m |
| 19 | Serverless Overviews | 17 | 1h 26m |
| 20 | Serverless Arch Discussions | 4 | 16m |
| **27** | **Networking - VPC** | **37** | **2h 37m** |

---

# DAY 1 — Identity → Compute → Network

**Sequence: 04 → 05 → 27 → 06 → 07** · Video 6h 50m · @1.5x ≈ 4h 24m · realistic ~7h

> **Keno 27 ke 6 ar 7 er agey?**
> Sec 06 er `ENI Overview`, `Private vs Public vs Elastic IP`, `Placement Groups` — tinta-i subnet/VPC er concept. Sec 07 er `Amazon EFS` e per-AZ mount target lage.
> VPC er jonno ja lage (EC2 launch, Security Group, SSH) — shob Sec 05 e peye jacho. Tai Sec 05 er thik por e VPC = perfect fit.

| Block | Time | Kaj |
|---|---|---|
| **1** | 09:00–09:40 | **Sec 04 — IAM & AWS CLI** (55m → 37m) |
| **2** | 09:40–10:50 | **Sec 05 — EC2 Fundamentals** (1h45 → 63m) |
| ☕ | 10:50–11:05 | Break |
| **3** | 11:05–12:00 | **Sec 27A — VPC Core** (L1–L19, 80m → 55m) |
| 🍽 | 12:00–13:00 | Lunch |
| **4** | 13:00–13:55 | **Sec 27B — VPC Advanced** (L20–L37, 78m → 52m) |
| 🧪 | 13:55–14:40 | **CHECKPOINT 1** — 20 questions |
| **5** | 14:40–15:05 | **Sec 06 — EC2 SAA Level** (33m → 22m) |
| **6** | 15:05–15:50 | **Sec 07 — EC2 Instance Storage** (59m → 39m) |
| 🧪 | 15:50–16:20 | **CHECKPOINT 2** — 15 questions |

### Sec 27 er split point
- **27A (Core):** `1. Section Introduction` → `19. VPC Peering Hands On` — **80 min**
- **27B (Advanced):** `20. VPC Endpoints` → `37. AWS Network Firewall` — **78 min**

### ⚠️ Day 1 er bhari lecture (eikhane slow koro, 1x e porba)
| Lecture | Time | Keno |
|---|---|---|
| `27 / 16. NACL & Security Groups` | **10.7m** | Exam er #1 networking topic. Stateful vs stateless, ephemeral port — mukhosto na, bujhte hobe |
| `27 / 23. VPC Flow Logs Hands On + Athena` | **10.2m** | Athena jana nai — syntax skip koro, Flow Log er **format** ta dekho |
| `27 / 36. Networking Costs in AWS` | **9.3m** | Cost-optimization question er sorashori source |
| `27 / 2. CIDR, Private vs Public IP` | **6.7m** | /16 /24 /28 hishab hatey kore dekho |
| `05 / 14. EC2 Purchasing Options` | **9.8m** | Spot/RI/Savings Plan — table banao |
| `05 / 16. Spot Instances & Spot Fleet` | **9.7m** | Same |

### ⏩ Day 1 er skip list (14 min bache)
```
04 / 8. AWS CLI Setup on Windows      1.7m   SKIP (tumi Linux)
04 / 9. AWS CLI Setup on Mac OS X     1.5m   SKIP
05 / 9. How to SSH using Windows      6.1m   SKIP
05 / 10. How to SSH using Windows 10  5.0m   SKIP
05 / 1. AWS Budget Setup              5.1m   OPTIONAL (budget already thakle skip)
```

### 🖐 Day 1 — nijer account e kora **BADDHOTAMULOK**
Ei 8 ta hands-on nijer hate korbe. Puro course e eitai single most important lab:
```
27 / 5. VPC Hands On
27 / 7. Subnet Hands On
27 / 9. Internet Gateways & Route Tables Hands On
27 / 11. Bastion Hosts Hands On
27 / 15. NAT Gateways Hands On
27 / 17. NACL & Security Groups Hands On
27 / 19. VPC Peering Hands On
27 / 21. VPC Endpoints Hands On
```
Baki Hands On (EC2 launch, SG, EBS, EFS, IAM) — **sudhu dekho, repeat koro na**. Tumi FOODI-PROD e eita roj korcho.

### 💸 Day 1 cost alert
- **NAT Gateway** — $0.045/hr + data. Lab sheshe **obosshoi delete**.
- **NAT Instance** — t2.micro free tier, kintu Elastic IP detach kore release koro.
- Din sheshe `27 / 34. Section Cleanup` dekhe cleanup koro, nahole mash sheshe bill ashbe.

---

# DAY 2 — HA → Database → DNS → Storage

**Sequence: 08 → 09 → 10 → 11 → 12 → 13 → 14** · Video 6h 56m · @1.5x ≈ 4h 37m

| Block | Time | Kaj |
|---|---|---|
| **1** | 09:00–10:05 | **Sec 08 — ELB & ASG** (1h34 → 63m) |
| **2** | 10:05–10:55 | **Sec 09 — RDS + Aurora + ElastiCache** (1h09 → 46m) |
| ☕ | 10:55–11:10 | Break |
| **3** | 11:10–12:05 | **Sec 10 — Route 53** (1h22 → 55m) |
| 🍽 | 12:05–13:00 | Lunch |
| **4** | 13:00–13:30 | **Sec 11 — Classic Solutions Architecture** (44m → 30m) ⚠️ **1x e dekho** |
| 🧪 | 13:30–14:20 | **CHECKPOINT 3** — 25 questions |
| **5** | 14:20–14:55 | **Sec 12 — S3 Introduction** (48m → 32m) |
| **6** | 14:55–15:15 | **Sec 13 — Advanced S3** (30m → 20m) |
| **7** | 15:15–15:50 | **Sec 14 — S3 Security** (49m → 33m) |
| 🧪 | 15:50–16:30 | **CHECKPOINT 4** — 20 questions |

### ⚠️ Day 2 er bhari lecture
| Lecture | Keno |
|---|---|
| `08 / 4. Application Load Balancer (ALB)` | Target group, path/host routing — exam e ghure firey ashe |
| `08 / 10–11. Sticky Sessions + Cross Zone LB` | Choto kintu exam favourite |
| `08 / 17. ASG Scaling Policies` | Target Tracking vs Step vs Scheduled vs Predictive — alada kore likhe rakho |
| `09 / 2. RDS Read Replicas vs Multi AZ` | **Exam er sob-cheye common confusion.** Read Replica = scaling, Multi-AZ = HA |
| `09 / 9. RDS Security` | Day 1 er SG chaining ekhane kaje lagbe |
| `10 / 7. CNAME vs Alias` | Zone apex e CNAME chole na — ei ekta point ei kom-e kom 1 ta question |
| `10 / 8–17. Routing Policies` (10 ta) | 7 ta policy. Ekta table banao: Simple / Weighted / Latency / Failover / Geolocation / Geoproximity / Multi-Value |
| **`11. puro section`** | **1x e dekho, speed up korba na.** Eitai tomar prothom architecture-thinking training |

### ⏩ Day 2 optional skip
```
10 / 3. Route 53 - Registering a domain   — domain kinte taka lage. Watch only.
09 / 6. Amazon Aurora - Hands On          — Aurora cluster costly. Watch only.
```

### 💸 Day 2 cost alert
- **RDS Multi-AZ / Aurora** — free tier er baire. Lab sheshe delete, **final snapshot off** kore.
- **ALB/NLB** — $0.0225/hr. Din sheshe delete.
- **ElastiCache** — delete.

---

# DAY 3 — Edge → Messaging → Containers → Serverless

**Sequence: 15 → 16 → 17 → 18 → 19 → 20** · Video 5h 12m · @1.5x ≈ 3h 28m

| Block | Time | Kaj |
|---|---|---|
| **1** | 09:00–09:25 | **Sec 15 — CloudFront & Global Accelerator** (35m → 23m) |
| **2** | 09:25–09:55 | **Sec 16 — AWS Storage Extras** (40m → 27m) |
| **3** | 09:55–10:50 | **Sec 17 — SQS, SNS, Kinesis, MQ** (1h21 → 54m) |
| ☕ | 10:50–11:05 | Break |
| **4** | 11:05–11:45 | **Sec 18 — ECS, Fargate, ECR, EKS** (54m → 36m) |
| 🧪 | 11:45–12:35 | **CHECKPOINT 5** — 25 questions |
| 🍽 | 12:35–13:30 | Lunch |
| **5** | 13:30–14:30 | **Sec 19 — Serverless Overviews** (1h26 → 57m) |
| **6** | 14:30–14:45 | **Sec 20 — Serverless Arch Discussions** (16m → 11m) ⚠️ **1x** |
| 🧪 | 14:45–15:15 | **CHECKPOINT 6** — 15 questions |
| ☕ | 15:15–15:45 | Break — weak topic note revise |
| 🎯 | 15:45–18:00 | **FINAL MOCK — 65 questions, 130 min, exam format** |
| 📊 | 18:00–18:45 | Review + weak topic list |

### ⚠️ Day 3 er bhari lecture
| Lecture | Keno |
|---|---|
| `17 / 4. SQS Message Visibility Timeout` | Duplicate processing scenario — classic question |
| `17 / 7. SQS + Auto Scaling Group` | Day 2 er ASG ekhane juktо hobe |
| `17 / 9. SNS and SQS - Fan Out Pattern` | Must know |
| `17 / 15. SQS vs SNS vs Kinesis` | **Ei ekta lecture 3-4 ta question er uttor** |
| `19 / 14. DynamoDB Advanced Features` | 8.6m — DAX, Streams, Global Table, TTL |
| `19 / 16. API Gateway Basics Hands-On` | 10.3m — hands-on, skim kora jay |
| `19 / 10. Lambda in VPC` | Day 1 er VPC ekhane kaje lagbe — ENI, cold start |
| `18 / 7. ECS - Solutions Architectures` | ALB + ECS dynamic port mapping |

### ⏩ Day 3 optional (time kom porle)
```
18 / 12–13. AWS App Runner + Hands On   — kom weight, 2x e dekho
18 / 14. AWS App2Container              — kom weight
16 / 7. Storage Gateway Hands On        — setup lomba, watch only
```

### 💸 Day 3 cost alert
- **EKS** — control plane $0.10/hr, **free tier nai**. Hands-on na korai bhalo, sudhu dekho.
- **Global Accelerator** — $0.025/hr fixed. Delete koro.
- **FSx / Storage Gateway** — costly. Watch only.
- **NAT Gateway** Day 1 er ta ekhono chalu ache ki na — check koro.

---

# 🧪 Self-Exam Checkpoints

Prottek checkpoint e amake bolba: **"CP-1 question dao"** — ami SAA exam format e scenario MCQ dibo, tumi answer dile grade + explanation dibo.

| CP | Kokhon | Coverage | Q | Time | Pass |
|----|--------|----------|---|------|------|
| **CP-1** | Day 1, Sec 27 sesh | IAM, EC2 Fundamentals, **VPC full** | 20 | 40m | 70% |
| **CP-2** | Day 1 sesh | EC2 SAA Level, EBS/EFS/AMI/Snapshot | 15 | 30m | 70% |
| **CP-3** | Day 2, Sec 11 sesh | ELB, ASG, RDS, Aurora, ElastiCache, Route 53, Architecture | 25 | 50m | 70% |
| **CP-4** | Day 2 sesh | S3 full (intro + advanced + security) | 20 | 40m | 70% |
| **CP-5** | Day 3, Sec 18 sesh | CloudFront, GA, Storage Extras, SQS/SNS/Kinesis, Containers | 25 | 50m | 70% |
| **CP-6** | Day 3, Sec 20 sesh | Lambda, DynamoDB, API GW, Cognito, Step Functions | 15 | 30m | 70% |
| **🎯 FINAL** | Day 3 raat | **Sec 4–20 + 27 cumulative, real exam format** | **65** | **130m** | **75%** |

### Rules
1. **Checkpoint skip korba na.** Section sesh kore sathe sathe test — 24 ghonta pore na. Recall freshness-i ei sprint er pura point.
2. **< 70% pele** — oi section er *non-hands-on* lecture gula 1.25x e re-watch koro, tarpor amake bolo "CP-X retake" — ami notun question dibo, purono gula na.
3. **Final mock e < 75%** — exam book korba na. Weak section gula 1 din niye re-do koro.
4. Checkpoint er por **weak topic gula `SAA-Progress-Tracker.md` er Notes section e likhe rakho**. Final revision oikhan theke hobe.

### CP-1 ebong CP-3 shob-cheye important
CP-1 (VPC + EC2) ar CP-3 (ELB/ASG/RDS/Route53) — SAA exam er **~45% question** ei dui block theke ashe. Ei dui tay 80%+ na pele samne agiye labh nai.

---

# 📝 Note-taking format (3 din e kaj korbe emon)

Lomba note likhte jeyo na, time nai. Prottek section sesh e sudhu **3 line**:

```
Sec 09 — RDS/Aurora/ElastiCache
WHEN: Read Replica = read scaling (async, eventual) | Multi-AZ = HA (sync, standby, no read)
TRAP: Multi-AZ theke read kora jay na. Read Replica cross-region kora jay, Multi-AZ ekta region e.
CMD/LIMIT: Aurora = 15 read replica, 6 copy / 3 AZ. RDS = 5 read replica.
```

Ei `WHEN / TRAP / CMD-LIMIT` format-ei exam er scenario question er uttor. 18 ta section = 18 ta block = 1 pata. Final mock er agey oi 1 pata porlei hobe.

---

# ✅ Pre-flight (shuru korar agey, 10 min)

- [ ] AWS account ready, **Billing Alert set** ($10 threshold)
- [ ] Browser e video player e **playback speed 1.5x** set
- [ ] `SAA-Progress-Tracker.md` khola — prottek section sesh e `[x]` mark
- [ ] Notes file khola — `WHEN / TRAP / LIMIT` format
- [ ] Phone silent / notification off
- [ ] Day 1 er lecture order: **04 → 05 → 27 → 06 → 07** (27 ta majhkhane, bhulba na)
