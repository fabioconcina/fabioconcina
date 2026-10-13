### Fabio Concina

Head of AI & Analytics at [kwantis](https://kwantis.com/), based in Milan.

I lead an 8-person engineering team building AI and analytics for the energy sector. Our product is used in production by energy companies including Eni, Saipem, TotalEnergies, and Weatherford.

Background in statistics and mathematical engineering: MSc Statistics & Actuarial Science (Trieste, 2015), BSc Mathematical Engineering (Politecnico di Milano, 2012).

[fabioconcina.com](https://fabioconcina.com) · [LinkedIn](https://www.linkedin.com/in/fabioconcina) · [ORCID](https://orcid.org/0000-0002-9562-0426)

---

### Side projects

Small Go and Rust utilities, plus tooling around Claude Code.

### [claumon](https://github.com/fabioconcina/claumon)

<a href="https://github.com/fabioconcina/claumon"><img src="https://raw.githubusercontent.com/fabioconcina/claumon/main/assets/logo.png" alt="claumon" height="170"></a>
<a href="https://github.com/fabioconcina/claumon"><img src="https://raw.githubusercontent.com/fabioconcina/claumon/main/assets/overview.png" height="170"></a>
<a href="https://github.com/fabioconcina/claumon"><img src="https://raw.githubusercontent.com/fabioconcina/claumon/main/assets/session-forecast.png" height="170"></a>

Claude Code dashboard that shows where your rate limits are headed before you hit them. Live session, weekly, and per-model gauges with an embedded empirical-Bayes forecaster: projected utilization at reset with an 80% credible interval and ETA to threshold. The rate is a conjugate update of an OLS slope against a Gaussian prior refit daily from past windows; usage paths are simulated as a monotone Gamma process, and the interval and ETAs come from the same Monte Carlo. The model has a [published spec](https://github.com/fabioconcina/claumon/blob/main/internal/forecast/MODEL.pdf) and is benchmarked out-of-sample with proper scoring rules (CRPS, pinball loss, interval coverage). Also per-session token and cost breakdowns, 7 to 90 day trends, running-process control, and a memory browser with health scores, staleness alerts, and recoverable deletion. Single binary, real-time SSE updates, SQLite-backed history. Go, runs on macOS, Linux, Windows.

Mentioned in [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code). Available on Homebrew, plus a companion VS Code extension that puts live usage and the forecast in the status bar. Site: [claumon.fabioconcina.com](https://claumon.fabioconcina.com).

### [arpdvark](https://github.com/fabioconcina/arpdvark)

<a href="https://github.com/fabioconcina/arpdvark"><img src="https://raw.githubusercontent.com/fabioconcina/arpdvark/main/assets/banner.png" width="400"></a>

Terminal-based network inventory tool. Scans your local network using ARP, resolves hostnames through system DNS, gateway DNS, and mDNS, and identifies hardware vendors from the IEEE OUI database. Full-screen TUI with auto-refresh, persistent device labels, and rate-limited scanning. Go, single binary, Linux.

### [alertpaca](https://github.com/fabioconcina/alertpaca)

<a href="https://github.com/fabioconcina/alertpaca"><img src="https://raw.githubusercontent.com/fabioconcina/alertpaca/master/assets/banner.png" width="400"></a>

Server health checker. Monitors CPU, memory, disk usage with fill-time prediction, systemd units, Docker containers, backup freshness, TLS certificate expiry, and port drift. Runs as an interactive TUI, a JSON exporter, or an MCP server for AI agents. Rust, single binary, zero config.
