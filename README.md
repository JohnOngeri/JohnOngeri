# John Ongeri Ouma

Software engineer working on applied AI systems, privacy-preserving ML, and
offline-first software for low-connectivity environments.
B.Sc. Software Engineering, African Leadership University - First Class Honours.
Nairobi, Kenya.

Most of my work sits in the gap between a model that behaves in a notebook and a
system that behaves in a clinic with 2G. I care about evaluation you can rerun and
failure modes you've actually measured.

---

## Selected work

**[Referral Pack Checker](https://github.com/JohnOngeri/referral-pack-checker)** - LLM extraction with deterministic checks and a human checkpoint

A woman referred for a planned caesarean arrives at the district hospital with her
blood group missing from the paperwork. No clinical decision was wrong; the delay was
documentation. This tool reads a referral pack, checks it against the receiving
facility's requirements, and flags what's missing, expired, or self-contradictory. It
makes no clinical judgment, and that boundary is written down and enforced.

The interesting part is the evaluation. An agent workflow caught 10 of 10 seeded
defects with 0 false flags; a single end-to-end prompt caught 9 and raised 34 findings
against packs that were fine. Every request and response is committed, so the run
replays offline without touching the API.

*TypeScript, LLM tool orchestration, deterministic validators, reproducible evals*

**[SOMO](https://github.com/JohnOngeri/SOMO-AI)** - Offline-first AI teaching coach

An AI coach for teachers that works across the whole connectivity ladder: Wi-Fi, 2G,
SMS/USSD, down to a button phone. Institutions license seats per term, each gated by a
one-time authorization PIN and a hard monthly quota, so LLM spend is predictable to the
call rather than open-ended. Fail-closed cost gates, a k-anonymity privacy wall on the
analytics mart, and nine ADRs documenting why.

*TypeScript, Node, Postgres, Redis, monorepo, architecture decision records*

**[PrivFed](https://github.com/JohnOngeri/PriFed)** - Federated learning for cross-bank fraud detection

Fraud patterns that no single bank can see, without any bank sharing raw transactions.
FedAvg for collaborative training, DP-SGD to bound what model updates leak under
membership-inference and model-inversion attacks, built against non-IID data where every
institution's distribution differs. Deployed as microservices on Render with an Android
client.

*Dart, Flutter, Python, Docker, PostgreSQL*

**[Federated Intelligence](https://github.com/JohnOngeri/Federated-Intelligence)** - RL agents for federated fraud screening

DQN, PPO, A2C, and REINFORCE compared on a multi-bank transaction-screening environment,
with agents trading off fraud caught against privacy budget and manual-review capacity.
Ten-plus tuning runs per algorithm with significance testing across seeds.

*Python, Gymnasium, Stable-Baselines3*

**[Sentiment Analysis: four-architecture benchmark](https://github.com/JohnOngeri/Sentiment-Analysis)**

50k IMDB reviews across TF-IDF with Logistic Regression, Word2Vec with BiLSTM, and two
variants. The tuned Logistic Regression reached 88% F1 at roughly a tenth of the
BiLSTM's training cost. The write-up covers where the extra capacity earned its keep and
where it didn't.

*Python, scikit-learn, TensorFlow*

**[Finance Chatbot](https://github.com/JohnOngeri/finance-chatbot)** - Fine-tuned T5 with an explicit out-of-domain policy

Domain-specific financial literacy Q&A: synthetic data generation, T5-small fine-tuning
with hyperparameter sweeps, evaluation, and a Gradio interface. Declines medical, legal,
and political questions by design rather than by accident.

*Python, TensorFlow, Transformers, Gradio*

Also here: [Deep Q-Learning on Atari](https://github.com/JohnOngeri/Deep-Q-Learning),
[Hidden Markov Models](https://github.com/JohnOngeri/Hidden-Markov-Models),
[time-series forecasting](https://github.com/JohnOngeri/Time-Series-Forecasting),
[an ML pipeline with a live prediction API](https://github.com/JohnOngeri/flutter-pregnancy-app),
and [241 commits of fundamentals](https://github.com/JohnOngeri/alu-higher_level_programming):
Python OOP, SQL schema design, SQLAlchemy, networking, scripting.

---

## Stack

**Languages** TypeScript, Python, Dart, JavaScript, SQL, Shell
**AI and ML** LLM orchestration and evals, TensorFlow, Keras, scikit-learn, Stable-Baselines3, federated learning, differential privacy, NumPy, pandas
**Backend** Node, FastAPI, REST, PostgreSQL, Redis, Docker
**Mobile** Flutter, offline-first, low-bandwidth, production deployments
**Tools** Git, Linux, pnpm monorepos, CI

---

## Currently

- Agent workflows I can actually measure: seeded-defect suites, false-flag budgets, committed traces so a run is reproducible six months later
- Differential privacy in practice: epsilon budgets, gradient clipping, FedAvg implemented rather than imported
- Cost control as an architectural constraint, not a dashboard: hard quotas, fail-closed gates
- Building for the bottom of the connectivity ladder, where the constraints make the system leaner

---

## Contact

Open to software engineering, ML engineering, and research engineering roles.

[LinkedIn](https://www.linkedin.com/in/john-ouma-b72365281) - johnongeriouma@gmail.com

![contribution snake](https://raw.githubusercontent.com/JohnOngeri/JohnOngeri/output/github-snake-dark.svg)
