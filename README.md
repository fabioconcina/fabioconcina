### Fabio Concina

Head of AI & Analytics at [kwantis](https://kwantis.com/), based in Milan.

I lead an 8-person engineering team building AI and analytics for the energy sector. Our product is used in production by energy companies including Eni, Saipem, TotalEnergies, and KOC.

Background in statistics and mathematical engineering: MSc Statistics & Actuarial Science (Trieste, 2015), BSc Mathematical Engineering (Politecnico di Milano, 2012).

[fabioconcina.com](https://fabioconcina.com) · [LinkedIn](https://www.linkedin.com/in/fabioconcina) · [ORCID](https://orcid.org/0000-0002-9562-0426)

---

### Side projects

Small Go and Rust utilities, plus tooling around Claude Code.

### [claumon](https://github.com/fabioconcina/claumon)

<a href="https://github.com/fabioconcina/claumon"><img src="https://raw.githubusercontent.com/fabioconcina/claumon/main/assets/overview.png" height="170"></a>
<a href="https://github.com/fabioconcina/claumon"><img src="https://raw.githubusercontent.com/fabioconcina/claumon/main/assets/session-forecast.png" height="170"></a>

Claude Code dashboard. Rate-limit gauges with an embedded empirical-Bayes forecaster: projected utilization at reset with an 80% credible interval and ETA to threshold. The rate is estimated by conjugate update of an OLS slope against a Gaussian prior refit daily from past windows; path noise is Brownian and ETAs are Monte Carlo'd. Also per-session token breakdowns, cost estimates, historical trends, conversation history, and a memory browser with health scores and staleness alerts. Single binary, real-time SSE updates, SQLite-backed daily aggregates. Go, runs on macOS, Linux, Windows.

### [arpdvark](https://github.com/fabioconcina/arpdvark)

<a href="https://github.com/fabioconcina/arpdvark"><img src="https://raw.githubusercontent.com/fabioconcina/arpdvark/main/assets/banner.png" width="400"></a>

Terminal-based network inventory tool. Scans your local network using ARP, resolves hostnames through system DNS, gateway DNS, and mDNS, and identifies hardware vendors from the IEEE OUI database. Full-screen TUI with auto-refresh, persistent device labels, and rate-limited scanning. Go, single binary, Linux.

### [alertpaca](https://github.com/fabioconcina/alertpaca)

<a href="https://github.com/fabioconcina/alertpaca"><img src="https://raw.githubusercontent.com/fabioconcina/alertpaca/master/assets/banner.png" width="400"></a>

Server health checker. Monitors CPU, memory, disk usage with fill-time prediction, systemd units, Docker containers, backup freshness, TLS certificate expiry, and port drift. Runs as an interactive TUI, a JSON exporter, or an MCP server for AI agents. Rust, single binary, zero config.
