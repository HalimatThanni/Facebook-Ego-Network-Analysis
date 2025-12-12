# Facebook-Ego-Network-Analysis
This project is a full-scale graph intelligence analysis performed on the Facebook Ego Network (SNAP Dataset), containing 4,039 nodes and 88,234 edges.
This project demonstrates senior-level expertise in:
* Network Science
* Community Detection
* Centrality Analytics
* Structural Vulnerability Modeling
* Information Diffusion Simulation
* Core–Periphery Architecture
* Python (NetworkX)
* Data Storytelling & Business Mapping

This is arguably one of my most complex and technically rich analytical projects — and it shows my ability to think like a systems analyst, not just a data analyst.

## Project Highlights (What Makes This Work Stand Out)
 1. Full Graph Preprocessing & Verification
I validated and reconstructed the network using:
* Graph sanity checks
* Connected component extraction
* Adjacency matrix building
* Preprocessing for all downstream analysis

Result:
- Graph fully connected
- 4,039 nodes in the largest component
- Clean, stable structure for all analyses


2. Formulated 6 research questions and answered all below

### RQ1 — Community Structure & Role Analogy

Using Louvain Modularity, I discovered:
* 15 functional communities
* High modularity score: 0.8349 (indicates extremely strong natural clustering)
* Community sizes ranged from 19 → 548 nodes, showing both micro-groups and mega-clusters.

Interpretation:
These communities behave like natural "role groups", just like students, teachers, admins, parents inside a school platform.
The structure strongly supports circle-based communication.

<img width="407" height="350" alt="Louvain Community Structure" src="https://github.com/user-attachments/assets/6784dd52-0ca1-4984-a44b-99f8a9060af5" />

fig 1 - Louvain Community Structure



### RQ2 — Influence Dynamics & Brokerage

Using Degree, Betweenness, Articulation Points & Multi-community bridging, I identified:
* Node 107 as the global communication super-hub
  * Degree: 1,045
  * Betweenness: 0.48
  * Connected to 8 different communities
* Mid-level gatekeepers: 1684, 1912, 3437
  * These nodes bridge 5–6 communities
  * Act as communication “gateways”

Interpretation:
These nodes behave like cross-department communicators, e.g., school administrators connecting multiple role-groups.

<img width="522" height="358" alt="Visual Bridge Analysis Scatterplot" src="https://github.com/user-attachments/assets/97cd4356-7418-4659-8b7a-7430a2219e13" />

Fig 2: Degree vs. Betweenness with Broker Labels


### RQ3 — Hierarchical Core–Periphery Architecture
Using k-core decomposition, I uncovered:
* Maximum core index: 115
* 158 nodes in the top core
* These “inner-circle” users form the strategic communication spine
* Outer nodes become increasingly peripheral and less influential

Implication:
This network has a strong hierarchical organization, similar to how a digital school ecosystem has:
core admins → active teachers → students → occasional users.

<img width="404" height="368" alt="Core Periphery" src="https://github.com/user-attachments/assets/99d6d958-c2ee-48db-80f0-152daa6e9a51" />

Fig 3: K-core Shell Distribution Plot


### RQ4 — Network Resilience & Failure Simulation
I simulated a targeted attack, removing the top 200 most influential hubs.
Result after removal:
* Original LCC: 4,039 nodes
* After attack: 3,750 nodes
* Network stayed operational, but weaker
* Shows high resilience, thanks to redundant connections

Interpretation:
The network is robust, losing even the biggest influencers won’t break communication.
This is valuable for platform design and risk assessment.

<img width="272" height="281" alt="Network Resistance and Fragmentation Curve" src="https://github.com/user-attachments/assets/fb912d33-457b-47ac-82b4-4315185fa2d6" />

Fig 4: LCC Size vs. Removed Hubs & Number of Components vs. Removed Hubs


### RQ5 — Homophily, Clustering & Triadic Closure
Key findings:
* Global Clustering = 0.6055 → extremely high
* Local clustering peaks at 1.0
* Total triangles: 1,612,010
* Community assortativity = 0.9557 → exceptionally strong

Interpretation:
People cluster tightly.
Friends-of-friends become friends.
Communities remain closed and strongly bonded.
This is exactly how school groups, study teams, and parent circles behave.

### RQ6 — Information Diffusion Potential
Using BFS simulations & global distance metrics:
* Information from ego-node travels to entire network in 6 steps
* Average distance from ego-node: 2.83
* Global diameter: 8
* Global Efficiency = 0.3066
* Cascade simulation shows rapid first-wave spread (1,742 users at step 3)

Interpretation:
This network is excellent for fast broadcast.
Messages spread like wildfire — critical for school announcements, alerts, scheduling changes, etc.

<img width="578" height="356" alt="Information Cascade Spread" src="https://github.com/user-attachments/assets/154f3461-2aa9-47d4-b69a-8424e3a714ec" />

Fig 5: Cascade Simulation Chart


## Visual Artefacts Included

This repository includes all visualizations from the analysis:
* Louvain community structure plot (Fig 1)
* Top brokers & bridge-node visualization (Fig 2)
* k-core core-periphery radial graph (Fig 3)
* Resilience decline curve & Cascade diffusion histogram (Fig 4)
* All numerical data outputs: Cascade Simulation Chart (Fig 5)

## Tools & Technologies
* Python (NetworkX, Pandas, NumPy, Matplotlib)
* Louvain Community Detection
* Centrality Measures (degree, betweenness, articulation)
* Graph Simulations (BFS cascades, targeted attacks)
* k-core decomposition
* Statistic-based structural interpretation

## Business Relevance
This analysis mirrors real-world platform needs:
* Identifying core users who keep communication alive
* Discovering natural role groups for UI personalization
* Understanding spread of information for announcement planning
* Testing resilience for system reliability
* Understanding relationship patterns to improve engagement algorithms

This isn’t just graph science, this is how you design smarter digital platforms.

## Key Takeaways (What This Project Proves About My Skillset)

- I can run large-scale graph analysis — 4,039 nodes
- I can connect graph theory to real-world business meaning
- I can perform advanced structural modeling
- I understand information flow, hierarchy & resilience in complex systems
- I write clear, strong reports that non-technical people understand
- I operate at a senior data analyst / network analyst level

## Contact

If you want to collaborate or explore the analysis deeper, feel free to reach out.
