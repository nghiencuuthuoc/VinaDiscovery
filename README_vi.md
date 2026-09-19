# VinaDiscovery

## Nền tảng AI cho Computer-Aided Drug Discovery

<p align="center">
  <img src="./images/VinaDiscovery_Brochure_Cover.png" alt="VinaDiscovery" width="100%">
</p>

<p align="center">
  <strong>Discover. Predict. Design. Prioritize.</strong>
</p>

<p align="center">
  <em>From Molecular Data to Drug Discovery Decisions.</em>
</p>

<p align="center">
  AI · Cheminformatics · Sinh học cấu trúc · Mô phỏng phân tử · ADME · An toàn · Thiết kế phân tử
</p>

<p align="center">

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](./LICENSE)
[![Repository](https://img.shields.io/badge/GitHub-VinaDiscovery-black?logo=github)](./)
[![Status](https://img.shields.io/badge/Status-Research%20%26%20Development-orange.svg)](./)

</p>

<p align="center">
  <a href="./images/">Visual Assets</a> ·
  <a href="./LICENSE">License</a> ·
  <a href="./issues">Issues</a> ·
  <a href="./pulls">Pull Requests</a> ·
  <a href="./releases">Releases</a>
</p>

---

## Tổng quan

VinaDiscovery là nền tảng scientific computing tích hợp dành cho nghiên cứu và phát triển thuốc hiện đại, kết hợp **cheminformatics, trí tuệ nhân tạo, sinh học cấu trúc, mô phỏng phân tử, ADME, an toàn, medicinal chemistry và lập kế hoạch tổng hợp** trong một môi trường nghiên cứu thống nhất.

VinaDiscovery được định hướng vượt ra ngoài mô hình các molecular calculator độc lập, hướng tới một workflow liên kết trong đó **molecule, model, simulation, evidence, uncertainty và project context** có thể được kết nối và truy vết xuyên suốt quá trình nghiên cứu.

> **From Molecular Data to Drug Discovery Decisions**

<p align="center">
  <img src="./images/a_wide_cinematic_high_quality_promotional_banner.png" alt="Nền tảng khoa học VinaDiscovery" width="100%">
</p>

---

# Vì sao VinaDiscovery?

Drug discovery hiện đại cần nhiều góc nhìn tính toán khác nhau.

Một molecule tiềm năng không thể được xác định chỉ bằng một score. Nhà nghiên cứu có thể cần đánh giá đồng thời:

- molecular identity và chemical representation
- chemical similarity và chemical space
- biological targets
- binding sites và molecular interactions
- docking và binding hypotheses
- molecular dynamics
- free-energy calculations
- physicochemical properties
- ADME và developability
- toxicity và safety
- potency và selectivity
- molecular optimization
- synthetic feasibility

VinaDiscovery kết nối các capability này thành một scientific workflow liên tục.

```text
Molecular Data
      │
      ▼
Molecular Preparation
      │
      ▼
Chemical Space & Similarity
      │
      ▼
Target Intelligence
      │
      ▼
Binding Site Intelligence
      │
      ▼
Molecular Binding
      │
      ▼
Interaction Analysis
      │
      ▼
Molecular Simulation
      │
      ▼
Free-Energy Analysis
      │
      ▼
ADME & Safety
      │
      ▼
Lead Optimization
      │
      ▼
Molecular Design
      │
      ▼
Synthesis Planning
```

<p align="center">
  <img src="./images/VinaDiscovery_Workflow_Infographic.png" alt="Workflow VinaDiscovery" width="100%">
</p>

---

# Kiến trúc khoa học

VinaDiscovery được tổ chức thành sáu scientific layers chính.

<p align="center">
  <img src="./images/a_wide_cinematic_clean_infographic_diagram_scene_batch_1.png" alt="Kiến trúc khoa học VinaDiscovery" width="100%">
</p>

```text
VinaDiscovery
│
├── Molecular Preparation & Chemical Space
│   ├── VinaMolPrep
│   ├── VinaSimilarity
│   └── VinaChemSpace
│
├── Medicinal Chemistry Intelligence
│   ├── VinaMMP
│   ├── VinaBioisostere
│   └── VinaPharmacophore
│
├── Target & Structural Intelligence
│   ├── VinaTarget
│   ├── VinaPocket
│   ├── VinaBind
│   └── VinaInteract
│
├── Molecular Simulation & Physics
│   ├── VinaParam
│   ├── VinaMD
│   └── VinaFEP
│
├── Predictive ADME & Safety Intelligence
│   ├── VinaQSAR
│   ├── VinaADME
│   └── VinaTox
│
└── AI Molecular Design
    ├── VinaLeadOpt
    ├── VinaDeNovo
    ├── VinaSynthesis
    └── VinaSidechain
```

Kiến trúc được thiết kế theo hướng module hóa nhưng vẫn duy trì interoperability giữa các thành phần khoa học.

---

# Các module cốt lõi

| Module | Vai trò khoa học |
|---|---|
| **VinaMolPrep** | Chuẩn hóa và chuẩn bị cấu trúc phân tử |
| **VinaSimilarity** | Molecular similarity và virtual screening |
| **VinaChemSpace** | Khám phá chemical space, clustering và diversity |
| **VinaMMP** | Matched molecular pair và chemical transformations |
| **VinaBioisostere** | Molecular replacement và lead optimization theo dữ liệu |
| **VinaPharmacophore** | Pharmacophore intelligence dựa trên ligand và structure |
| **VinaTarget** | AI target prediction và target fishing |
| **VinaPocket** | Binding-site và pocket intelligence |
| **VinaBind** | Molecular docking và binding-pose hypotheses |
| **VinaInteract** | Phân tích protein–ligand interactions |
| **VinaParam** | Molecular force-field parameterization |
| **VinaMD** | Molecular dynamics simulation |
| **VinaFEP** | Binding free-energy và relative free-energy workflows |
| **VinaQSAR** | Machine-learning molecular property modelling |
| **VinaADME** | ADME và drug-likeness intelligence |
| **VinaTox** | Toxicity và safety intelligence |
| **VinaLeadOpt** | Multi-parameter lead optimization |
| **VinaDeNovo** | Generative molecular design |
| **VinaSynthesis** | Retrosynthesis và synthetic route planning |
| **VinaSidechain** | Non-natural amino-acid và sidechain intelligence |

---

# Molecular Preparation

## VinaMolPrep

VinaMolPrep là cửa vào của computational molecular workflow.

Các bước chuẩn bị có thể bao gồm:

- kiểm tra cấu trúc
- normalization
- xử lý salt và fragment
- xử lý tautomer
- xác định protonation state
- kiểm tra stereochemistry
- tạo 3D conformer
- molecular representation
- chuẩn bị charge

Mục tiêu là tạo một molecular identity nhất quán có thể được sử dụng trong các workflow downstream.

<p align="center">
  <img src="./images/VinaDiscovery_Molecular_Preparation.png" alt="VinaDiscovery Molecular Preparation" width="100%">
</p>

---

# Chemical Intelligence

## VinaSimilarity

VinaSimilarity trả lời câu hỏi:

> **Những molecule nào giống query này nhất?**

Các ứng dụng có thể bao gồm:

- nearest-neighbor search
- tìm analog
- virtual screening
- scaffold exploration
- similarity-based filtering
- chemical library exploration

Hệ thống có thể hỗ trợ nhiều molecular representations thay vì phụ thuộc vào một representation duy nhất.

## VinaChemSpace

VinaChemSpace trả lời câu hỏi rộng hơn:

> **Một tập hợp hàng lớn molecule được tổ chức như thế nào?**

Các capability có thể bao gồm:

- clustering
- diversity analysis
- scaffold distribution
- nearest-neighbor networks
- activity landscapes
- property distributions
- dimensionality reduction
- chemical-space visualization

```text
VinaSimilarity
      =
Query & Search

VinaChemSpace
      =
Population-Level Chemical Intelligence
```

---

# Medicinal Chemistry Intelligence

## VinaMMP

VinaMMP tập trung vào **matched molecular pair transformations**.

```text
Compound A
     │
     └── structural transformation ──► Compound B
                                      │
                                      ▼
                              Property / Activity Δ
```

Các tín hiệu có thể bao gồm:

- ΔpIC50
- ΔKi
- ΔKd
- ΔlogP
- ΔlogD
- Δsolubility
- Δpermeability
- Δclearance

Điều này cho phép xây dựng transformation-level knowledge phục vụ medicinal chemistry.

## VinaBioisostere

VinaBioisostere dựa trên evidence về molecular transformation để khám phá các structural replacement thay thế.

Kết quả có thể bao gồm:

```text
Replacement
Activity Evidence
Property Effect
ADME Effect
Target Context
Frequency
Confidence
```

Mục tiêu là hỗ trợ medicinal chemist khi tìm kiếm các phương án cấu trúc mới trong quá trình lead optimization.

## VinaPharmacophore

VinaPharmacophore mô hình hóa các đặc trưng như:

- hydrogen-bond donors
- hydrogen-bond acceptors
- hydrophobic regions
- aromatic features
- ionizable features
- spatial constraints

Ứng dụng có thể gồm:

- ligand-based screening
- structure-based design
- scaffold exploration
- pharmacophore-driven virtual screening

---

# Target & Structural Intelligence

<p align="center">
  <img src="./images/VinaDiscovery_Binding_Intelligence.png" alt="VinaDiscovery Binding Intelligence" width="100%">
</p>

## VinaTarget

VinaTarget xây dựng target hypotheses từ chemical và biological evidence.

Các lớp evidence có thể bao gồm:

```text
Chemical Similarity
        +
Bioactivity Data
        +
Molecular Embeddings
        +
Protein Representations
        +
Knowledge Graph Evidence
        +
Structural Evidence
```

Mục tiêu là cung cấp ranked hypotheses cùng evidence và confidence thay vì coi computational prediction như một biological mechanism đã được xác nhận.

## VinaPocket

VinaPocket tập trung vào câu hỏi:

> **Binding có thể xảy ra ở đâu?**

Các output có thể gồm:

- pocket coordinates
- pocket volume
- residue composition
- physicochemical characteristics
- hotspot hypotheses
- ligandability/druggability indicators
- docking search regions

## VinaBind

VinaBind tập trung vào câu hỏi:

> **Ligand có thể gắn như thế nào?**

Platform layer được thiết kế theo hướng **engine-neutral**, cho phép tích hợp nhiều docking/scoring backend theo thời gian.

Các output có thể gồm:

```text
Binding Poses
Docking Scores
Pose Geometry
Search Metadata
Backend Information
```

Docking score được xem là computational ranking signal, không phải phép đo trực tiếp của experimental binding affinity.

## VinaInteract

VinaInteract chuyển structures và trajectories thành interaction information có thể diễn giải.

Các nhóm tương tác có thể gồm:

- hydrogen bonds
- hydrophobic contacts
- ionic interactions
- aromatic interactions
- cation–π interactions
- halogen interactions
- metal coordination
- residue contacts
- interaction fingerprints

Workflow cấu trúc:

```text
VinaPocket
    ↓
VinaBind
    ↓
VinaInteract
```

---

# Molecular Simulation & Physics

## VinaParam

VinaParam tập trung vào **molecular force-field parameterization**.

Output có thể gồm:

```text
Atom Types
Partial Charges
Bond Parameters
Angle Parameters
Torsions
Non-Bonded Parameters
Topology
```

Parameterization và simulation được thiết kế như hai trách nhiệm riêng biệt.

## VinaMD

VinaMD cung cấp molecular dynamics workflows để nghiên cứu:

- conformational behavior
- molecular stability
- interaction dynamics
- trajectory analysis
- solvent effects
- structural changes

```text
VinaParam
    ↓
Parameterized System
    ↓
VinaMD
    ↓
Trajectory
```

## VinaFEP

VinaFEP hướng tới các free-energy workflows ở cấp độ cao hơn, bao gồm:

- relative binding free energy
- alchemical transformations
- free-energy perturbation
- related free-energy analysis

Phân biệt khoa học cơ bản:

```text
Docking Score
      ≠
Binding Free Energy
      ≠
Experimental Measurement
```

---

# Predictive ADME & Safety Intelligence

<p align="center">
  <img src="./images/VinaDiscovery_ADME_Tox_Intelligence.png" alt="VinaDiscovery ADME và Toxicity Intelligence" width="100%">
</p>

## VinaQSAR

VinaQSAR là framework chung cho molecular property modelling.

Các model families có thể gồm:

- molecular descriptors
- molecular fingerprints
- tree-based models
- graph neural networks
- message-passing neural networks
- molecular transformers
- ensemble models

Framework được định hướng hỗ trợ:

- scaffold-aware splitting
- cluster splitting
- temporal validation
- external validation
- uncertainty estimation
- applicability-domain analysis
- explainability

## VinaADME

VinaADME tập trung vào early developability assessment.

Các nhóm chỉ tiêu có thể bao gồm:

- physicochemical properties
- lipophilicity
- aqueous solubility
- permeability
- intestinal absorption
- CNS/BBB-related properties
- transporter-related endpoints
- metabolic properties
- clearance-related endpoints
- drug-likeness
- medicinal-chemistry alerts

Prediction của VinaADME không nên được hiểu là experimental measurement.

Khi phù hợp, kết quả nên cung cấp:

```text
Prediction
Confidence
Uncertainty
Applicability Domain
Model Version
Dataset Version
Evidence
```

## VinaTox

VinaTox mở rộng predictive layer sang safety intelligence.

Các endpoint có thể gồm:

- mutagenicity
- cardiac safety-related endpoints
- liver toxicity
- cytotoxicity
- acute toxicity
- carcinogenicity
- skin sensitization
- endocrine-related endpoints

Safety prediction phục vụ early computational triage và hypothesis generation, không thay thế experimental toxicology.

---

# AI Molecular Design

<p align="center">
  <img src="./images/VinaDiscovery_AI_Design_Synthesis.png" alt="VinaDiscovery AI Design and Synthesis" width="100%">
</p>

## VinaLeadOpt

VinaLeadOpt được thiết kế cho **multi-parameter lead optimization**.

Một bài toán tối ưu thực tế có thể bao gồm:

```text
Maximize:
    Potency
    Selectivity
    Solubility

Minimize:
    Toxicity
    Metabolic Liability

Constraints:
    Molecular Weight
    Scaffold Retention
    Synthetic Feasibility
    Chemical Novelty
```

Các capability có thể gồm:

- multi-objective optimization
- Pareto-front analysis
- candidate ranking
- evidence aggregation
- trade-off analysis

## VinaDeNovo

VinaDeNovo tập trung vào generative molecular design.

Các cấu trúc được sinh ra nên tiếp tục đi qua downstream computational checks:

```text
Generate
   ↓
VinaMolPrep
   ↓
VinaSimilarity
   ↓
VinaADME / VinaTox
   ↓
VinaTarget / VinaBind
   ↓
VinaSynthesis
   ↓
VinaLeadOpt
```

Sinh ra một molecular structure mới chỉ là một giai đoạn trong discovery workflow.

## VinaSynthesis

VinaSynthesis kết nối computational molecular design với chemistry thực tế.

Output có thể gồm:

- retrosynthetic routes
- precursor candidates
- building blocks
- alternative routes
- synthetic feasibility evidence

```text
Computationally Designed Molecule
              ↓
       Synthetic Planning
              ↓
       Experimentally Testable
```

## VinaSidechain

VinaSidechain mở rộng platform sang peptide và protein-related molecular engineering.

Ứng dụng có thể gồm:

- non-natural amino acids
- sidechain libraries
- rotamer analysis
- peptide design
- protein engineering

---

# End-to-End Discovery Workflow

<p align="center">
  <img src="./images/wide_cinematic_conceptual_composite_image_of_drug_batch_2.png" alt="Khái niệm drug discovery của VinaDiscovery" width="100%">
</p>

Một workflow small-molecule có thể kết nối nhiều capability:

```text
SMILES / SDF
     │
     ▼
VinaMolPrep
     │
     ├──────────────► VinaSimilarity
     │
     ├──────────────► VinaChemSpace
     │
     └──────────────► VinaQSAR
                         │
                         ▼
                    VinaTarget
                         │
                         ▼
                    VinaPocket
                         │
                         ▼
                     VinaBind
                         │
                         ▼
                   VinaInteract
                         │
                         ▼
                      VinaMD
                         │
                         ▼
                     VinaFEP
                         │
                ┌────────┴────────┐
                ▼                 ▼
           VinaADME           VinaTox
                │                 │
                └────────┬────────┘
                         ▼
                    VinaLeadOpt
                         │
                         ▼
                    VinaDeNovo
                         │
                         ▼
                  VinaSynthesis
                         │
                         ▼
                 Experimental
                   Validation
```

---

# Scientific Result Contract

Computational result nên được xem là scientific record thay vì một con số đứng độc lập.

Ví dụ:

```json
{
  "value": 0.83,
  "unit": "probability",
  "method": "model",
  "model_version": "1.0.0",
  "dataset_version": "2026.09",
  "input_structure_id": "structure-id",
  "uncertainty": 0.07,
  "applicability_domain": "in-domain",
  "evidence_count": 124,
  "software_versions": {},
  "provenance": {},
  "warnings": []
}
```

Schema có thể tiếp tục thay đổi, nhưng nguyên tắc là:

> **Every scientific result should be traceable.**

---

# Molecular Knowledge Layer

VinaDiscovery được thiết kế dựa trên một shared scientific data model.

Các entity chính có thể gồm:

```text
Compound
Structure Variant
Target
Protein Structure
Assay
Activity
Prediction
Model Version
Simulation
Interaction
Transformation
Evidence
Artifact
Job
```

Một computational result nên truy vết được theo chuỗi:

```text
Input
  ↓
Preparation
  ↓
Dataset
  ↓
Model / Algorithm
  ↓
Parameters
  ↓
Execution
  ↓
Result
  ↓
Evidence
```

Kiến trúc này hỗ trợ:

- reproducibility
- auditability
- collaboration
- experiment tracking
- model lifecycle management
- computational provenance

---

# Uncertainty & Applicability Domain

VinaDiscovery coi uncertainty là một phần của scientific result.

Một prediction có thể đi kèm:

```text
Prediction
   +
Confidence
   +
Uncertainty
   +
Applicability Domain
   +
Evidence
```

Điều này giúp nhà nghiên cứu phân biệt giữa:

- prediction được hỗ trợ mạnh bởi các training examples liên quan
- prediction có evidence hạn chế
- prediction nằm ngoài applicability domain kỳ vọng
- computational hypothesis cần thêm experimental investigation

Mục tiêu không phải che giấu uncertainty mà là làm cho nó hiển thị rõ ràng.

---

# Scientific Integrity

VinaDiscovery phân biệt rõ các loại thông tin:

```text
Experimental
Calculated
Predicted
Inferred
Literature-Derived
```

Platform tránh các phép đồng nhất gây hiểu nhầm khoa học như:

```text
Docking score
    ≠
Experimental affinity

Prediction
    ≠
Experimental measurement

Target hypothesis
    ≠
Confirmed mechanism

Negative toxicity prediction
    ≠
Proof of safety
```

Computational results được dùng để hỗ trợ scientific reasoning và prioritization song song với experimental evidence.

---

# Validation Philosophy

Các scientific module khác nhau cần những chiến lược validation khác nhau.

| Nhóm module | Ví dụ validation |
|---|---|
| Similarity / Chemical Space | neighbour relevance, enrichment, scaffold recovery |
| Target Prediction | top-k recall, PR-AUC, temporal/external validation |
| Molecular Binding | pose RMSD, enrichment và benchmark evaluation |
| Interaction Analysis | recovery so với experimental structures |
| Parameterization | energies/geometries so với validated references |
| Molecular Dynamics | trajectory stability và experimental observables khi có |
| Free Energy | error so với experimental ΔG / ΔΔG |
| QSAR | scaffold, temporal và external validation |
| ADME | endpoint-specific predictive metrics và calibration |
| Toxicity | sensitivity, specificity, PR-AUC và external evaluation |
| Molecular Design | validity, novelty, uniqueness và property success |
| Synthesis Planning | route validity, feasibility và expert review |

Đối với molecular machine learning, random splitting đơn thuần có thể không đánh giá đầy đủ khả năng generalization trên chemical space. VinaDiscovery do đó hướng tới scaffold, cluster, temporal và external evaluation tùy intended use case.

---

# Data, AI & Physics

VinaDiscovery được thiết kế quanh ba phương thức scientific computing bổ trợ cho nhau:

```text
Data
 +
AI / ML
 +
Physics-Based Simulation
```

được kết nối bởi:

```text
Evidence
```

Tổng hợp:

```text
Data
  +
AI / ML
  +
Physics-Based Simulation
  +
Evidence
  =
Molecular Intelligence
```

<p align="center">
  <img src="./images/a_wide_cinematic_futuristic_infographic_style_il_batch_3.png" alt="Molecular intelligence của VinaDiscovery" width="100%">
</p>

---

# Platform Architecture

VinaDiscovery được định hướng như một extensible scientific platform thay vì một computational engine nguyên khối.

```text
Web Application
      │
      ▼
Scientific API
      │
      ▼
Workflow Orchestration
      │
      ├── Cheminformatics
      ├── AI / ML
      ├── Molecular Binding
      ├── Molecular Mechanics
      ├── Molecular Dynamics
      ├── Free Energy
      ├── ADME / Toxicology
      └── Synthesis Planning
      │
      ▼
Scientific Data Layer
      │
      ├── Molecular Data
      ├── Bioactivity
      ├── Models
      ├── Evidence
      ├── Simulations
      └── Artifacts
      │
      ▼
CPU / GPU / HPC / Cloud
```

Kiến trúc hướng tới cả interactive research và high-throughput computational campaigns.

---

# Design Principles

## 1. Scientific correctness over marketing claims

Thuật toán cần được mô tả đúng theo những gì nó thực sự tính toán.

## 2. Evidence-aware AI

Prediction nên đi kèm uncertainty, applicability context và provenance khi có thể.

## 3. Reproducibility by design

Molecular identity, dataset, model version, parameters và software versions cần có khả năng truy vết.

## 4. Modular scientific architecture

Các capability phải độc lập trong testing nhưng có khả năng interoperability thông qua shared scientific data contracts.

## 5. Engine-neutral infrastructure

Platform layer không nên bị phụ thuộc không cần thiết vào một computational backend duy nhất.

## 6. Human-led discovery

AI và automation phải hỗ trợ researcher thay vì che khuất scientific judgement.

## 7. Experimental validation remains essential

Computational prediction tạo hypothesis và hỗ trợ prioritization; không thay thế experimental evidence.

---

# Đối tượng sử dụng

VinaDiscovery hướng tới các nhóm nghiên cứu trong:

- Medicinal Chemistry
- Computational Chemistry
- Structural Biology
- Drug Discovery
- AI / ML for Chemistry
- Pharmaceutical R&D
- Biotechnology
- Academic Research
- Chemical Biology
- Molecular Design

---

# Cấu trúc repository

## Hiện tại

```text
VinaDiscovery/
├── images/
├── LICENSE
└── README.md
```

## Dự kiến

```text
VinaDiscovery/
├── images/
├── docs/
├── src/
├── tests/
├── examples/
├── benchmarks/
├── models/
├── workflows/
├── LICENSE
├── README.md
├── README_vi.md
├── CONTRIBUTING.md
└── CITATION.cff
```

---

# Resources

## Project

- **Repository:** [nghiencuuthuoc/VinaDiscovery](https://github.com/nghiencuuthuoc/VinaDiscovery)
- **Visual assets:** [`./images/`](./images/)
- **License:** [`Apache-2.0`](./LICENSE)
- **Issues:** [`GitHub Issues`](./issues)
- **Pull Requests:** [`GitHub Pull Requests`](./pulls)
- **Releases:** [`GitHub Releases`](./releases)

## Scientific Ecosystem

VinaDiscovery được thiết kế để tích hợp với các scientific software, molecular-data resources và computational frameworks phù hợp.

- **RDKit** — cheminformatics, molecular representations, descriptors, fingerprints, conformers và chemical structure processing.  
  https://www.rdkit.org/
- **Open Force Field Toolkit** — molecular mechanics, molecular topology và force-field workflows.  
  https://docs.openforcefield.org/
- **OpenMM** — molecular dynamics và molecular simulation infrastructure.  
  https://openmm.org/
- **OpenFE** — free-energy calculation workflows.  
  https://openfree.energy/
- **Chemprop** — message-passing neural networks cho molecular property prediction.  
  https://github.com/chemprop/chemprop
- **ProLIF** — protein–ligand interaction fingerprints và interaction analysis.  
  https://github.com/chemosim-lab/ProLIF
- **ChEMBL** — curated bioactivity và chemical data cho drug-discovery research.  
  https://www.ebi.ac.uk/chembl/

> Phần mềm, dataset, model và scientific resource của bên thứ ba giữ nguyên license và yêu cầu attribution riêng. Repository này không relicence các thành phần đó.

---

# Citation

VinaDiscovery là một research và software project đang phát triển.

Khi trích dẫn một implementation, benchmark, dataset, model hoặc scientific result cụ thể, vui lòng trích dẫn documentation của project tương ứng và các scientific resources upstream được sử dụng bởi component đó.

Một file `CITATION.cff` machine-readable được dự kiến bổ sung trong release tương lai.

---

# License

## Apache License 2.0

Phần mềm VinaDiscovery được phân phối theo **Apache License, Version 2.0**.

Xem [`LICENSE`](./LICENSE) để đọc toàn bộ license.

Apache License 2.0 cho phép sử dụng, sao chép, sửa đổi, phân phối, sublicense và commercial use theo các điều khoản của license, bao gồm việc giữ lại các copyright, attribution, patent và license notices tương ứng.

## Third-Party Components and Data

VinaDiscovery có thể tích hợp hoặc phụ thuộc vào phần mềm, dataset, model và service của bên thứ ba.

Các thành phần đó vẫn chịu sự điều chỉnh của license và terms riêng.

Ví dụ có thể gồm scientific libraries, molecular databases, machine-learning frameworks, simulation engines, pretrained models, external APIs và research datasets.

Apache-2.0 của VinaDiscovery **không thay thế và không relicence** material của bên thứ ba.

## Visual Assets

Nếu không có asset license riêng, visual materials trong [`./images/`](./images/) được xem là một phần của repository distribution.

Khi repository chuyển sang mô hình commercial/product, có thể bổ sung `ASSET-LICENSE.md` riêng nếu muốn phần software tiếp tục open source nhưng hạn chế reuse logo, branding, promotional artwork hoặc các visual assets khác.

---

# Roadmap

## Phase 1 — Molecular Foundation

- [ ] VinaMolPrep
- [ ] Molecular identity and standardization
- [ ] Shared molecular data model
- [ ] VinaSimilarity
- [ ] VinaChemSpace
- [ ] Scientific provenance

## Phase 2 — Discovery Intelligence

- [ ] VinaTarget
- [ ] VinaPocket
- [ ] VinaBind
- [ ] VinaInteract
- [ ] VinaPharmacophore
- [ ] VinaMMP
- [ ] VinaBioisostere

## Phase 3 — Simulation

- [ ] VinaParam
- [ ] VinaMD
- [ ] VinaFEP
- [ ] High-throughput computational workflows

## Phase 4 — Predictive Intelligence

- [ ] VinaQSAR
- [ ] VinaADME
- [ ] VinaTox
- [ ] Applicability-domain analysis
- [ ] Uncertainty estimation
- [ ] Model versioning and validation

## Phase 5 — Molecular Design

- [ ] VinaLeadOpt
- [ ] VinaDeNovo
- [ ] VinaSynthesis
- [ ] VinaSidechain
- [ ] Closed-loop molecular design workflows

---

# Trạng thái

> **Research & Development**

VinaDiscovery là một scientific platform đang phát triển.

Mỗi module có thể có mức độ maturity, validation và production readiness khác nhau.

Scientific claims, model performance và computational capabilities cần được đánh giá theo:

- module
- dataset
- model version
- computational method
- intended use

---

# Disclaimer

VinaDiscovery dành cho **research, computational analysis, hypothesis generation và decision support**.

Computational predictions không cấu thành experimental confirmation, clinical evidence, regulatory approval hay sự thay thế cho laboratory validation.

Người dùng chịu trách nhiệm diễn giải computational results trong scientific context phù hợp và thực hiện experimental validation đối với các phát hiện quan trọng.

---

# Contributing

Hoan nghênh đóng góp trong các lĩnh vực:

- cheminformatics
- molecular modelling
- machine learning
- structural biology
- molecular simulation
- ADME / toxicity modelling
- scientific software engineering
- data infrastructure
- workflow orchestration
- scientific visualization
- validation và benchmarking

Vui lòng mở issue hoặc pull request kèm mô tả rõ về thay đổi đề xuất, scientific rationale và validation strategy.

---

# VinaDiscovery by PharmApp

<p align="center">
  <img src="./images/VinaDiscovery_Brochure_Cover.png" alt="VinaDiscovery by PharmApp" width="720">
</p>

<p align="center">
  <strong>AI-Powered Computer-Aided Drug Discovery Platform</strong>
</p>

<p align="center">
  <strong>Discover. Predict. Design. Prioritize.</strong>
</p>

<p align="center">
  <em>From Molecular Data to Drug Discovery Decisions.</em>
</p>
