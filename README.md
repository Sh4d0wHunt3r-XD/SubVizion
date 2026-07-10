# SubVizion

### Listing Title:
SubVizion: Ultra-Fast Next-Gen Attack Surface Mapping &
OSINT Engine (Single Binary with Embedded GUI)

### Product Description:
SubVizion is a high-performance, event-driven Attack Surface
Management (ASM) and subdomain enumeration tool designed
to outperform legacy tools like OWASP Amass. Built entirely in
Go, it features a concurrent 3-tier pipeline architecture that
simultaneously ingests passive OSINT data, actively resolves
DNS (with wildcard detection), and fingerprints web
technologies (HTTP/TLS/Ports) in a single pass.
Unlike competitors that require massive RAM overhead or
external databases, SubVizion streams results directly into an
embedded SQLite database using WAL mode for zero-lock
concurrency. Best of all, it ships as a self-contained 16MB single
binary. It can be run headlessly via CLI for automated pipelines,
or launched with a `--ui` flag to spin up an embedded,
Cyberpunk-themed interactive web dashboard (D3.js network
graphs, live polling, filterable data tables) with absolutely no
external dependencies.

### Key Features & Architecture:
#### • 3-Tier Event-Driven Pipeline: 
Passive ingestion (crt.sh, HackerTarget, URLScan, RapidDNS), Active DNS resolution
pool, and HTTP/TLS Profiling run concurrently via Go
channels.

#### • Ultra-Low Memory Footprint: 
Streams results directly to a local CGO-free SQLite database and JSON Lines output,
completely avoiding the RAM bloat associated with memoryheavy graph databases.

#### • Embedded Interactive GUI: 
A beautiful, Cyberpunk-styled HTML5/CSS3/JS dashboard compiled directly into the binary
using `//go:embed`. Features live D3.js force-directed network
graphs, tech-stack distribution charts, and a detailed asset
inventory.

#### • Single-Pass Profiling: 
Simultaneously discovers subdomains, resolves IPs, grabs TLS certificates, fingerprints
technologies (headers/body regex), and scans common ports.

#### • Smart Concurrency: 
Bulletproof architecture with dynamic port allocation, strict network timeouts, and thread-safe data
handling.

### Tech Stack:
#### • Backend: Go (Golang)

#### • Database: 
SQLite (pure-Go CGO-free implementation via modernc.org/sqlite)

#### • Frontend:
Vanilla HTML/CSS, JavaScript, D3.js (for network visualization)

#### • Delivery: 
Single executable binary (16.4 MB) for Windows, macOS, and Linux.

#### • One-Click Setup: 
Includes pre-configured .bat and .sh scripts for automated dependency installation and deployment. True plug-and-play architecture.


### Reason for Sale & Transfer Details:
I built this tool to solve the specific bottlenecks (speed, memory
usage, and lack of visual analytics) present in current opensource ASM tools. It is fully production-ready, highly optimized,
and has zero technical debt. I am selling the complete
intellectual property, source code, and full commercial rights
because my primary focus is transitioning to other projects, and I
want to pass this high-potential engine to someone who can
monetize it via enterprise licenses, a SaaS wrapper, or
integration into a larger cybersecurity suite.

The transfer includes the full GitHub repository, architecture
documentation, and a walkthrough of the codebase.
