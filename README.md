<p align="center">
  <a href="https://omeraltinova.com.tr">
    <img src="./assets/banner.svg" width="100%" alt="Ömer Faruk Altınova, Computer Engineering student at İstanbul Medeniyet University working on LLMs, AI agents and RAG" />
  </a>
</p>

<p align="center">
  <a href="https://omeraltinova.com.tr"><img src="https://img.shields.io/badge/Website-1f6feb?style=for-the-badge&logo=data:image%2Fsvg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjEwIi8%2BPHBhdGggZD0iTTEyIDJhMTQuNSAxNC41IDAgMCAwIDAgMjAgMTQuNSAxNC41IDAgMCAwIDAtMjAiLz48cGF0aCBkPSJNMiAxMmgyMCIvPjwvc3ZnPg%3D%3D" alt="Website" /></a>
  <a href="https://www.linkedin.com/in/omeraltinova/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:hello@f4r.uk"><img src="https://img.shields.io/badge/Email-8957e5?style=for-the-badge&logo=data:image%2Fsvg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxyZWN0IHdpZHRoPSIyMCIgaGVpZ2h0PSIxNiIgeD0iMiIgeT0iNCIgcng9IjIiLz48cGF0aCBkPSJtMjIgNy04Ljk3IDUuN2ExLjk0IDEuOTQgMCAwIDEtMi4wNiAwTDIgNyIvPjwvc3ZnPg%3D%3D" alt="Email" /></a>
  <a href="https://x.com/omeraltinova"><img src="https://img.shields.io/badge/X-353c45?style=for-the-badge&logo=x&logoColor=white" alt="X (Twitter)" /></a>
  <img src="https://img.shields.io/badge/Discord-omeraltinova-5865F2?style=for-the-badge&logo=discord&logoColor=white&labelColor=4752c4" alt="Discord: omeraltinova" />
</p>

### About me

I'm a fourth-year Computer Engineering student at İstanbul Medeniyet University, graduating in 2027. Most of what I build runs on large language models. I fine-tune them for narrow tasks, connect them to tools and documents, and then work on making them fast enough to serve. That last step is my favorite part, because it decides whether a model becomes a product or stays in a notebook. This summer I did exactly that as an AI Engineer intern at İMÜ BİLTAM, working on agent and RAG pipelines and serving them with vLLM.

### Milestones

- 🏆 **5th place at TEKNOFEST 2026, Trendyol E-Commerce Competition.** Our team DualCore finished 5th of 377 teams in the Kaggle round, then 5th again among the 10 finalists with the second-highest F1 score in the final. I fine-tuned Gemma-4-12B with LoRA, built the hard-negative training set with Gemma-4-31B as the teacher, and designed the vLLM and Docker inference pipeline that explains each prediction with SHAP. On query-disjoint cross-validation the system reached 0.9452 Macro-F1.
- 🤝 **CV Analiz for İMÜ Teknopark.** I built and delivered a recruitment platform where recruiters manage candidate pools and positions, search candidates by keyword or by meaning, and get an AI evaluation of each CV. No CV reaches an external LLM with personal data in it. The platform parses every file in isolation and redacts PII locally first.

### Focus areas

- 🧠 **Fine-tuning LLMs for one job.** I use LoRA and PEFT on models like Gemma-4, generate training data with a larger teacher model, and keep the same query out of both train and test splits. I also want to know why a model made a call, so I check its predictions with SHAP, field occlusion and attention.
- 🔎 **Agents and retrieval.** Prompts split into system, context and user layers, tool calls that run on the backend, fallback to another model when one fails, and routing each workload to the model that fits it. Retrieval mixes keyword and vector search over pgvector or FAISS.
- ⚙️ **Serving models.** vLLM behind OpenAI-compatible APIs, Docker pipelines that return the same output on every run, and FastAPI with PostgreSQL behind Next.js frontends.
- 🖥️ **C on Linux.** POSIX threads, TCP sockets, shared-memory IPC, and desktop interfaces in GTK4 and SDL2.
- 🔌 **Next up.** Embedded systems, Edge AI and robotics, on hardware like the Raspberry Pi.

### Selected projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/omeraltinova/CopyGuard">CopyGuard</a></h4>
      <p>Runs locally and finds plagiarism in Turkish student assignments. It scores document pairs with MinHash, TF-IDF, sentence embeddings and section overlap, and can ask an LLM for a second opinion. Reports export as HTML, CSV or images.</p>
      <p><code>FastAPI</code> <code>Next.js</code> <code>SQLite</code> <code>Sentence Transformers</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/omeraltinova/GameMasterAI_web">GameMaster AI</a></h4>
      <p>A digital game master for tabletop campaigns built on the 5e SRD. Each model request carries the current session, characters and world state. The model calls tools that the backend executes, falls back to another model when one fails, and stays inside token quotas and rate limits.</p>
      <p><code>TypeScript</code> <code>OpenRouter</code> <code>PostgreSQL</code> <code>Prisma</code></p>
    </td>
  </tr>
</table>

<details>
  <summary><b>More projects in C</b></summary>
  <br />
<table>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/omeraltinova/emergency-drone-coordination">Emergency Drone Coordination</a></h4>
      <p>A C client-server system that coordinates simulated rescue drones. Drones register, report status and receive missions as JSON over TCP. The server tracks heartbeats and handles reconnects and dropped clients across threads, and an SDL2 window shows drones and survivors live.</p>
      <p><code>C</code> <code>pthreads</code> <code>TCP sockets</code> <code>SDL2</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/omeraltinova/simple-shell">Simple-Shell</a></h4>
      <p>A multi-tab terminal emulator written in C and GTK4 with an MVC structure. It runs shell commands, manages processes, keeps command history, and passes messages between processes through POSIX shared memory.</p>
      <p><code>C</code> <code>GTK4</code> <code>POSIX IPC</code> <code>Linux</code></p>
    </td>
  </tr>
</table>
</details>

<details>
  <summary><h3>Toolbox</h3></summary>

<table>
  <tr>
    <td><b>Languages</b></td>
    <td><img src="https://cdn.simpleicons.org/python/3776AB" width="14" height="14" alt="" />&nbsp;Python &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/c/A8B9CC" width="14" height="14" alt="" />&nbsp;C &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/openjdk/ED8B00" width="14" height="14" alt="" />&nbsp;Java &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/typescript/3178C6" width="14" height="14" alt="" />&nbsp;TypeScript &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/javascript/F7DF1E" width="14" height="14" alt="" />&nbsp;JavaScript</td>
  </tr>
  <tr>
    <td><b>Machine learning</b></td>
    <td><img src="https://cdn.simpleicons.org/pytorch/EE4C2C" width="14" height="14" alt="" />&nbsp;PyTorch &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/huggingface/FFD21E" width="14" height="14" alt="" />&nbsp;Transformers &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/scikitlearn/F7931E" width="14" height="14" alt="" />&nbsp;scikit-learn &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/numpy/4DABCF" width="14" height="14" alt="" />&nbsp;NumPy &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/pandas/E70488" width="14" height="14" alt="" />&nbsp;Pandas</td>
  </tr>
  <tr>
    <td><b>LLM tooling</b></td>
    <td>PEFT / LoRA &nbsp;&nbsp; vLLM &nbsp;&nbsp; Sentence Transformers &nbsp;&nbsp; FAISS &nbsp;&nbsp; SHAP</td>
  </tr>
  <tr>
    <td><b>Backend &amp; data</b></td>
    <td><img src="https://cdn.simpleicons.org/fastapi/009688" width="14" height="14" alt="" />&nbsp;FastAPI &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/flask/8B949E" width="14" height="14" alt="" />&nbsp;Flask &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/postgresql/4169E1" width="14" height="14" alt="" />&nbsp;PostgreSQL + pgvector &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/sqlite/0F80CC" width="14" height="14" alt="" />&nbsp;SQLite &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/prisma/8B949E" width="14" height="14" alt="" />&nbsp;Prisma</td>
  </tr>
  <tr>
    <td><b>Web &amp; tools</b></td>
    <td><img src="https://cdn.simpleicons.org/nextdotjs/8B949E" width="14" height="14" alt="" />&nbsp;Next.js &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/react/61DAFB" width="14" height="14" alt="" />&nbsp;React &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/nodedotjs/5FA04E" width="14" height="14" alt="" />&nbsp;Node.js &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/docker/2496ED" width="14" height="14" alt="" />&nbsp;Docker &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/git/F05032" width="14" height="14" alt="" />&nbsp;Git &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/linux/FCC624" width="14" height="14" alt="" />&nbsp;Linux &nbsp;&nbsp; <img src="https://cdn.simpleicons.org/raspberrypi/A22846" width="14" height="14" alt="" />&nbsp;Raspberry Pi</td>
  </tr>
</table>
</details>

<br />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/omeraltinova/omeraltinova/output/snake.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/omeraltinova/omeraltinova/output/snake-light.svg" />
  <img src="https://raw.githubusercontent.com/omeraltinova/omeraltinova/output/snake.svg" width="100%" alt="Snake eating my contribution graph" />
</picture>

<details>
  <summary><b>GitHub stats &amp; what I'm listening to</b></summary>
  <br />
  <div align="center">
    <img src="https://github-readme-stats.vercel.app/api?username=omeraltinova&hide_title=false&hide_rank=false&show_icons=true&include_all_commits=true&count_private=true&disable_animations=false&theme=github_dark&locale=en&hide_border=true&order=1" height="150" alt="GitHub stats" />
    <img src="https://github-readme-stats.vercel.app/api/top-langs?username=omeraltinova&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=5&theme=github_dark&hide_border=true&order=2" height="150" alt="Top languages" />
    <img src="https://streak-stats.demolab.com?user=omeraltinova&locale=en&mode=daily&theme=github_dark&hide_border=true&border_radius=5&order=3" height="150" alt="GitHub streak" />
  </div>
  <br />
  <div align="center">
    <a href="https://open.spotify.com/user/21prwr3qlkrbm26rogjaycllq">
      <img src="https://spotify-recently-played-readme.vercel.app/api?user=21prwr3qlkrbm26rogjaycllq&count=5&unique=false" alt="Spotify recently played" />
    </a>
  </div>
</details>
