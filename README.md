# Arvid Borglund

Software and AI engineer in Malmö, Sweden. I take problems all the way to running software: architecture, code, infrastructure and the operations around it.

## What I am building

Most of my current work lives in private repositories, which is why this profile looks quieter than it is. The main one is a procurement intelligence SaaS that I build and run on my own. It ingests public procurement notices from TED, the EU procurement database, processes them and makes them searchable and filterable.

- Backend in Java and Spring Boot, frontend in Angular and TypeScript, PostgreSQL with Flyway migrations, ShedLock for distributed jobs.
- Infrastructure as code with Terraform, three environments on two Linux servers, deploys with Kamal, CI/CD in GitHub Actions building multi-arch images, protected main with required checks, architecture decision records.
- Ingestion built for a source I do not control: rate limiting, retry strategies and archiving logic. The development environment holds thousands of real notices.
- Automation as a habit: when the cloud provider ran out of server capacity, a self-terminating GitHub Actions workflow polled the capacity API, provisioned the servers through Terraform the moment stock appeared, filed an issue with addresses and DNS records, and switched itself off.
- Next in the pipeline, work in progress: local AI inside the product. The first feature is a RAG chat over the tender database, served by open models running on an AI workstation I built myself: AMD Ryzen 7 9800X3D, 64 GB DDR5, NVIDIA GeForce RTX 5090 with 32 GB VRAM, 2 TB NVMe, mini-ITX on an ASRock B850I. Current model candidate is Qwen3.6-27B (dense, about 17 GB quantized, 256K context) via Ollama or llama.cpp, with Qwen3.8-27B queued for a local comparison, and the plan is to link the servers to the rig over a reverse SSH tunnel. The hardware is in place, the integration is in progress.

## How I work

I develop with AI agents as a daily practice, not as a demo. Claude Code is the primary tool. MCP servers are how the agents reach the tools around them, from debugging running code to driving a browser. A persistent knowledge vault means every session starts with context and leaves distilled knowledge behind instead of a chat history. Parallel sessions run in isolated git worktrees, nothing merges without review, and I can defend everything that ships.

## Background

AI engineer and developer at Sogeti, part of Capgemini, with client deliveries in AI, cloud and enterprise development: predictive maintenance with a digital twin for a global manufacturer, a translation platform on Azure neural machine translation for a travel operator, RAG-based compliance tooling for a pharmaceutical distributor, and enterprise development in a large public transport ticketing ecosystem. Runner-up in the Sogeti Global Agentic AI Ideathon 2025, entering solo against a hundred senior teams.

The public repositories here are university projects from my BSc in Information Systems at Lund University, kept as they were.

## Contact

[LinkedIn](https://www.linkedin.com/in/arvid-borglund-2a119b21b/) · arvid.borglund@gmail.com
