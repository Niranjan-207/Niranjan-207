<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&duration=2800&pause=900&color=58A6FF&center=true&vCenter=true&width=650&lines=AI%2FML+Systems+Engineer;LeetCode+Knight+(2062+Peak);LoRA+%26+RAG+Architect;B.Tech+IT+%2727" alt="Typing SVG" />

<br/>

[![LeetCode Knight](https://img.shields.io/badge/LeetCode-Knight%20|%202062%20Peak-FFA116?style=for-the-badge&logo=leetcode&logoColor=black&labelColor=1a1a2e)](https://leetcode.com/niranjan0207)
[![Amazon ML Summer School](https://img.shields.io/badge/Amazon%20ML%20Summer%20School-Top%202.3%25%20%7C%20%2726-FF9900?style=for-the-badge&logo=amazon&logoColor=white&labelColor=1a1a2e)](https://www.linkedin.com/in/niranjan-reddy)
[![HACKaSTONE Finalist](https://img.shields.io/badge/HACKaSTONE%202026-Global%20Finalist-8A2BE2?style=for-the-badge&logo=vercel&logoColor=white&labelColor=1a1a2e)](https://www.linkedin.com/in/niranjan-reddy)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=1a1a2e)](https://www.linkedin.com/in/niranjan-reddy)
[![Email](https://img.shields.io/badge/Email-Reach%20Out-D14836?style=for-the-badge&logo=gmail&logoColor=white&labelColor=1a1a2e)](mailto:kvniranjanreddy01@gmail.com)

</div>

<br/>

```bash
niranjan@dev:~$ whoami --profile
> B.Tech IT '27 @ BVRIT (CGPA 9.24/10.0) | AI/ML Systems Engineer

niranjan@dev:~$ cat cp_profile.log
[LeetCode]         Knight | Peak Rating: 2062 (Top ~2% Global)
[CodeChef]         Peak Rating: 1647
[USACO]            Silver Division
[Smart Interviews] Global Rank: 167 / 57,528
[Total Solved]     800+ problems across platforms

niranjan@dev:~$ cat achievements.log
[Amazon ML Summer School '26]  Selected -- Top 2.3% of 130,000+ applicants
[HACKaSTONE 2026]              Global Grand Finalist @ VU Amsterdam
[Smart India Hackathon]        Top 5 / 250+ teams

niranjan@dev:~$ echo $CURRENT_FOCUS
Multi-Adapter LoRA Inference Engines & Contradiction-Aware RAG Pipelines

niranjan@dev:~$ _
```

<br/>

## 🧮 Coding Profiles & Live Problem Solving Stats

<div align="center">

[![LeetCode](https://img.shields.io/badge/LeetCode-Knight%20|%202062%20Peak-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/niranjan0207)
[![CodeChef](https://img.shields.io/badge/CodeChef-Peak%201647-5B4638?style=for-the-badge&logo=codechef&logoColor=white)](https://www.codechef.com/users/niranjan07)
[![Smart Interviews](https://img.shields.io/badge/Smart%20Interviews-Rank%20167%2F57%2C528-1E90FF?style=for-the-badge&logoColor=white)](https://smartinterviews.in/certificate/0af7a54c)
[![USACO](https://img.shields.io/badge/USACO-Silver%20Division-4CAF50?style=for-the-badge&logo=codeforces&logoColor=white)](http://www.usaco.org/)

<br/>

<a href="https://leetcode.com/niranjan0207">
  <img src="https://leetcode-stats.vercel.app/api?username=niranjan0207&theme=Dark" width="48%" alt="LeetCode Stats" />
</a>
<a href="https://leetcode.com/niranjan0207">
  <img src="https://leetcode-badge-showcase.vercel.app/api?username=niranjan0207&theme=tokyonight" width="48%" alt="LeetCode Badge Showcase" />
</a>

<!-- If the above is slow to load, fallback: -->
<!-- <img src="https://leetcode-stats-showcase.vercel.app/api?username=niranjan0207&theme=tokyonight" width="100%" alt="LeetCode Stats Showcase" /> -->

</div>

<br/>

**Key CP Highlights**

- 🥇 **LeetCode:** Knight Badge · Peak Rating **2062** (Top ~2% globally) — live solved count above
- 🍫 **CodeChef:** Peak Rating **1647**
- 🌽 **USACO:** Silver Division
- 🧮 **Smart Interviews:** Global Rank **167 / 57,528** · Diamond Certificate in DSA

<br/>

## 🛠️ Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 🔀 RouterNet
**Multi-Domain LoRA Adapter Routing Engine**

Hot-swappable multi-adapter inference engine on **Qwen3-4B**, routing queries via a SentenceTransformer + Logistic Regression classifier.

```
  User Query
      │
      ▼
┌──────────────┐
│ Sentence-Tfmr│
│   Encoder    │
└──────┬───────┘
       ▼
┌──────────────────┐
│ Logistic Reg.     │
│ Domain Router      │
│ (96.8–98.4% acc)  │
└─────────┬──────────┘
          │  <0.02s · O(1)
   ┌──────┼──────┬──────┐
   ▼      ▼      ▼      ▼
 LoRA-A LoRA-B LoRA-C LoRA-N
   └──────┴──────┴──────┘
          ▼
   Qwen3-4B Base
          ▼
       Response
```

- ⚡ **O(1) adapter switching**, `<0.02s` latency
- 📈 Proof completion **40% → 80%+** on a single T4 (~8.2GB VRAM)
- 🎯 **100%** ground-truth math accuracy maintained
- 🧩 Domain-isolated LoRA (r = 16–32) — zero cross-task weight pollution

**Tech:** `Python` `PyTorch` `🤗 Transformers/PEFT` `Sentence-Transformers` `scikit-learn`

</td>
<td width="50%" valign="top">

### ⚖️ Nyaya-Verify
**Contradiction-Aware Legal RAG Pipeline**

Verification-first RAG for Indian legal statutes — audits retrieved context for contradictions **before** generation.

```
 Legal Query
      │
      ▼
┌───────────────┐
│   ChromaDB     │
│  BGE-Small     │
│ (dynamic K)    │
└───────┬────────┘
        ▼
┌────────────────────┐
│ DeBERTa-v3 NLI       │
│ Cross-Encoder Audit  │
│ (filters repealed /  │
│  conflicting clauses)│
└──────────┬───────────┘
           ▼
┌────────────────────┐
│ Llama 3.1 (8B)       │
│ 4-bit Quant · RTX4050│
└──────────┬───────────┘
           ▼
    Verified Answer
```

- 🛡️ **DeBERTa-v3 NLI** cross-encoder audit layer catches old IPC vs. new BNS conflicts
- 🔍 Dynamic **K-scaling retrieval** over ChromaDB + BGE-Small embeddings
- 💾 **4-bit quantization** co-runs Llama 3.1 (8B) + cross-encoder on 6GB VRAM

**Tech:** `Python` `LangChain` `ChromaDB` `DeBERTa-v3` `PyTorch` `Ollama`

</td>
</tr>
</table>

<br/>

## 📂 Deep Dives

<details>
<summary><b>🏆 Competitions & Achievements</b></summary>
<br/>

| Achievement | Detail |
|---|---|
| 🥇 **LeetCode Knight** | Peak Rating **2062** — Top ~2% globally |
| 🍫 **CodeChef** | Peak Rating **1647** |
| 🌽 **USACO** | Silver Division |
| 🧮 **Smart Interviews** | Global Rank **167 / 57,528** |
| 📦 **Amazon ML Summer School 2026** | Selected — Top **2.3%** of 130,000+ applicants |
| 🌍 **HACKaSTONE 2026 Global Grand Finalist** | Team project *"EcoLearn: A Socio-Cognitive AI Agent"* — international grand final in Agentic AI for Education @ Vrije Universiteit Amsterdam |
| 🇮🇳 **Smart India Hackathon (SIH)** | Top 5 / 250+ teams |
| 🎤 **Promethean 2025** | Technical Coordinator — organized a 150+ participant CP contest |

</details>

<details>
<summary><b>📜 Research & Certifications</b></summary>
<br/>

| Credential | Detail |
|---|---|
| 🎓 **B.Tech, Information Technology** | B V Raju Institute of Technology, 2023–2027 — CGPA **9.24 / 10.0** |
| 📘 **SWAYAM-NPTEL** | Domain Certification in Programming — **93%**, Top **1%** Nationally |
| 💎 **Smart Interviews** | Diamond Certificate in DSA |
| 🔬 **Focus Areas** | LoRA/QLoRA fine-tuning · RAG pipelines · NLI-based contradiction detection |

</details>

<br/>

## 💻 Tech Stack

**Languages**

<p>
<img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" alt="C++"/>
<img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white" alt="C"/>
<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL"/>
</p>

**AI/ML & GenAI Frameworks**

<p>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/>
<img src="https://img.shields.io/badge/🤗%20Hugging%20Face-FFD21E?style=for-the-badge&logoColor=black" alt="Hugging Face"/>
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV"/>
</p>

**Databases & Cloud Infrastructure**

<p>
<img src="https://img.shields.io/badge/ChromaDB-FF6B6B?style=for-the-badge&logoColor=white" alt="ChromaDB"/>
<img src="https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" alt="Azure"/>
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git"/>
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
</p>

<br/>

## 📊 Dynamic Dashboard

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Niranjan-207&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats"/>
<img height="165" src="https://github-readme-streak-stats.herokuapp.com/?user=Niranjan-207&theme=tokyonight&hide_border=true" alt="GitHub Streak"/>

<br/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Niranjan-207&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages"/>

<br/>

<img src="https://github-profile-trophy.vercel.app/?username=Niranjan-207&theme=tokyonight&no-frame=true&row=1&column=7" alt="GitHub Trophies"/>

</div>

<br/>

<div align="center">

### 🤝 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/niranjan-reddy)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kvniranjanreddy01@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Niranjan-207)

<i>⭐️ Thanks for stopping by — always open to collaborating on AI/ML and competitive programming projects!</i>

</div>
